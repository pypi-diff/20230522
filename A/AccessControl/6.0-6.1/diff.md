# Comparing `tmp/AccessControl-6.0.tar.gz` & `tmp/AccessControl-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AccessControl-6.0.tar", last modified: Thu Jan 12 14:26:47 2023, max compression
+gzip compressed data, was "AccessControl-6.1.tar", last modified: Mon May 22 11:34:00 2023, max compression
```

## Comparing `AccessControl-6.0.tar` & `AccessControl-6.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.914275 AccessControl-6.0/
--rw-r--r--   0 jens       (501) staff       (20)      587 2023-01-03 12:47:17.000000 AccessControl-6.0/.coveragerc
--rwxr-xr-x   0 jens       (501) staff       (20)     1918 2023-01-03 12:47:17.000000 AccessControl-6.0/.manylinux-install.sh
--rwxr-xr-x   0 jens       (501) staff       (20)      509 2023-01-03 12:47:17.000000 AccessControl-6.0/.manylinux.sh
--rw-r--r--   0 jens       (501) staff       (20)     6717 2023-01-12 14:02:23.000000 AccessControl-6.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      799 2023-01-03 12:47:17.000000 AccessControl-6.0/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:50:53.000000 AccessControl-6.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     1849 2021-11-02 08:50:53.000000 AccessControl-6.0/HISTORY.rst
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:50:53.000000 AccessControl-6.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      359 2023-01-03 12:47:17.000000 AccessControl-6.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)     8667 2023-01-12 14:26:47.914369 AccessControl-6.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      768 2022-03-26 10:28:34.000000 AccessControl-6.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)     1782 2023-01-03 12:47:17.000000 AccessControl-6.0/appveyor.yml
--rw-r--r--   0 jens       (501) staff       (20)      439 2023-01-11 16:46:17.000000 AccessControl-6.0/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.904504 AccessControl-6.0/docs/
--rw-r--r--   0 jens       (501) staff       (20)     6187 2021-11-02 08:50:53.000000 AccessControl-6.0/docs/AccessControl.rst
--rw-r--r--   0 jens       (501) staff       (20)     1090 2021-11-02 08:50:53.000000 AccessControl-6.0/docs/requestmethod.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.901298 AccessControl-6.0/include/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.904632 AccessControl-6.0/include/Acquisition/
--rw-r--r--   0 jens       (501) staff       (20)     2451 2021-11-02 08:50:53.000000 AccessControl-6.0/include/Acquisition/Acquisition.h
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.904855 AccessControl-6.0/include/ExtensionClass/
--rw-r--r--   0 jens       (501) staff       (20)     9572 2021-11-02 08:50:53.000000 AccessControl-6.0/include/ExtensionClass/ExtensionClass.h
--rw-r--r--   0 jens       (501) staff       (20)     1719 2021-11-02 08:50:53.000000 AccessControl-6.0/include/ExtensionClass/_compat.h
--rw-r--r--   0 jens       (501) staff       (20)      582 2023-01-12 14:26:47.914775 AccessControl-6.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     3561 2023-01-12 14:02:31.000000 AccessControl-6.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.901469 AccessControl-6.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.909918 AccessControl-6.0/src/AccessControl/
--rw-r--r--   0 jens       (501) staff       (20)     2211 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/AuthEncoding.py
--rw-r--r--   0 jens       (501) staff       (20)     1732 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/ImplC.py
--rw-r--r--   0 jens       (501) staff       (20)    32088 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/ImplPython.py
--rw-r--r--   0 jens       (501) staff       (20)     3805 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/Implementation.py
--rw-r--r--   0 jens       (501) staff       (20)     1237 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/Owned.py
--rw-r--r--   0 jens       (501) staff       (20)     5312 2022-03-26 10:28:34.000000 AccessControl-6.0/src/AccessControl/Permission.py
--rw-r--r--   0 jens       (501) staff       (20)     5202 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/PermissionMapping.py
--rw-r--r--   0 jens       (501) staff       (20)      826 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/PermissionRole.py
--rw-r--r--   0 jens       (501) staff       (20)     2876 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/Permissions.py
--rw-r--r--   0 jens       (501) staff       (20)     1563 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/Role.py
--rw-r--r--   0 jens       (501) staff       (20)    13880 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/SecurityInfo.py
--rw-r--r--   0 jens       (501) staff       (20)     2463 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/SecurityManagement.py
--rw-r--r--   0 jens       (501) staff       (20)     1097 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/SecurityManager.py
--rw-r--r--   0 jens       (501) staff       (20)     4882 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/SimpleObjectPolicies.py
--rw-r--r--   0 jens       (501) staff       (20)      912 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/SpecialUsers.py
--rw-r--r--   0 jens       (501) staff       (20)     2328 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/User.py
--rw-r--r--   0 jens       (501) staff       (20)    17536 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/ZopeGuards.py
--rw-r--r--   0 jens       (501) staff       (20)     1951 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/ZopeSecurityPolicy.py
--rw-r--r--   0 jens       (501) staff       (20)     2271 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      736 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/_compat.h
--rw-r--r--   0 jens       (501) staff       (20)    62941 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/cAccessControl.c
--rw-r--r--   0 jens       (501) staff       (20)     3817 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/class_init.py
--rw-r--r--   0 jens       (501) staff       (20)      104 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)    11074 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)      214 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/logger_wrapper.py
--rw-r--r--   0 jens       (501) staff       (20)     1443 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/meta.zcml
--rw-r--r--   0 jens       (501) staff       (20)     2095 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/metaconfigure.py
--rw-r--r--   0 jens       (501) staff       (20)     8617 2022-03-26 10:28:34.000000 AccessControl-6.0/src/AccessControl/owner.py
--rw-r--r--   0 jens       (501) staff       (20)     1691 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/permissions.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3344 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/requestmethod.py
--rw-r--r--   0 jens       (501) staff       (20)    16013 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/rolemanager.py
--rw-r--r--   0 jens       (501) staff       (20)     2123 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/safe_formatter.py
--rw-r--r--   0 jens       (501) staff       (20)     7349 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/security.py
--rw-r--r--   0 jens       (501) staff       (20)     5518 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tainted.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913338 AccessControl-6.0/src/AccessControl/tests/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     5168 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/actual_python.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913485 AccessControl-6.0/src/AccessControl/tests/mixed_module/
--rw-r--r--   0 jens       (501) staff       (20)       78 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/mixed_module/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913605 AccessControl-6.0/src/AccessControl/tests/mixed_module/submodule/
--rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/mixed_module/submodule/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913729 AccessControl-6.0/src/AccessControl/tests/private_module/
--rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/private_module/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913854 AccessControl-6.0/src/AccessControl/tests/private_module/submodule/
--rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/private_module/submodule/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.913979 AccessControl-6.0/src/AccessControl/tests/public_module/
--rw-r--r--   0 jens       (501) staff       (20)      125 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/public_module/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.914127 AccessControl-6.0/src/AccessControl/tests/public_module/submodule/
--rw-r--r--   0 jens       (501) staff       (20)       44 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/public_module/submodule/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     6618 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/testClassSecurityInfo.py
--rw-r--r--   0 jens       (501) staff       (20)     2449 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/testImplementation.py
--rw-r--r--   0 jens       (501) staff       (20)     4805 2022-05-03 09:03:15.000000 AccessControl-6.0/src/AccessControl/tests/testModuleSecurity.py
--rw-r--r--   0 jens       (501) staff       (20)      343 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/testPermissionMapping.py
--rw-r--r--   0 jens       (501) staff       (20)     4110 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/testPermissionRole.py
--rw-r--r--   0 jens       (501) staff       (20)     9361 2022-03-26 10:28:34.000000 AccessControl-6.0/src/AccessControl/tests/testSecurityManager.py
--rw-r--r--   0 jens       (501) staff       (20)    15171 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/testZCML.py
--rw-r--r--   0 jens       (501) staff       (20)    33544 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/testZopeGuards.py
--rw-r--r--   0 jens       (501) staff       (20)    25448 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/testZopeSecurityPolicy.py
--rw-r--r--   0 jens       (501) staff       (20)     9056 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/test_owner.py
--rw-r--r--   0 jens       (501) staff       (20)     5411 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/test_requestmethod.py
--rw-r--r--   0 jens       (501) staff       (20)     4708 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/test_rolemanager.py
--rw-r--r--   0 jens       (501) staff       (20)     8726 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/test_safe_formatter.py
--rw-r--r--   0 jens       (501) staff       (20)     2138 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/test_safeiter.py
--rw-r--r--   0 jens       (501) staff       (20)    12667 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/test_tainted.py
--rw-r--r--   0 jens       (501) staff       (20)     6446 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/tests/test_userfolder.py
--rw-r--r--   0 jens       (501) staff       (20)    22853 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/tests/test_users.py
--rw-r--r--   0 jens       (501) staff       (20)     1224 2021-11-02 08:50:53.000000 AccessControl-6.0/src/AccessControl/unauthorized.py
--rw-r--r--   0 jens       (501) staff       (20)    17049 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/userfolder.py
--rw-r--r--   0 jens       (501) staff       (20)    15399 2023-01-03 12:38:42.000000 AccessControl-6.0/src/AccessControl/users.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-12 14:26:47.910872 AccessControl-6.0/src/AccessControl.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)     8667 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     2999 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)       67 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-03-26 10:31:42.000000 AccessControl-6.0/src/AccessControl.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      311 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)       14 2023-01-12 14:26:47.000000 AccessControl-6.0/src/AccessControl.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1173 2023-01-03 12:47:17.000000 AccessControl-6.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.238470 AccessControl-6.1/
+-rw-r--r--   0 jens       (501) staff       (20)      587 2023-04-18 09:35:29.000000 AccessControl-6.1/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2182 2023-04-18 09:35:29.000000 AccessControl-6.1/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2023-04-18 09:35:29.000000 AccessControl-6.1/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)     6982 2023-05-22 11:19:12.000000 AccessControl-6.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2023-04-18 09:35:29.000000 AccessControl-6.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:50:53.000000 AccessControl-6.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1849 2021-11-02 08:50:53.000000 AccessControl-6.1/HISTORY.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:50:53.000000 AccessControl-6.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      359 2023-04-18 09:35:29.000000 AccessControl-6.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)     8932 2023-05-22 11:34:00.238541 AccessControl-6.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      768 2022-03-26 10:28:34.000000 AccessControl-6.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1948 2023-04-18 09:35:29.000000 AccessControl-6.1/appveyor.yml
+-rw-r--r--   0 jens       (501) staff       (20)      439 2023-01-11 16:46:17.000000 AccessControl-6.1/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.230450 AccessControl-6.1/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     6187 2021-11-02 08:50:53.000000 AccessControl-6.1/docs/AccessControl.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1090 2021-11-02 08:50:53.000000 AccessControl-6.1/docs/requestmethod.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.227910 AccessControl-6.1/include/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.230559 AccessControl-6.1/include/Acquisition/
+-rw-r--r--   0 jens       (501) staff       (20)     2451 2023-04-18 09:21:36.000000 AccessControl-6.1/include/Acquisition/Acquisition.h
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.230768 AccessControl-6.1/include/ExtensionClass/
+-rw-r--r--   0 jens       (501) staff       (20)     9572 2023-04-18 09:22:22.000000 AccessControl-6.1/include/ExtensionClass/ExtensionClass.h
+-rw-r--r--   0 jens       (501) staff       (20)     1964 2023-04-19 05:40:53.000000 AccessControl-6.1/include/ExtensionClass/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)      583 2023-05-22 11:34:00.238966 AccessControl-6.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3561 2023-05-22 11:19:23.000000 AccessControl-6.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.228094 AccessControl-6.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.234726 AccessControl-6.1/src/AccessControl/
+-rw-r--r--   0 jens       (501) staff       (20)     2211 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/AuthEncoding.py
+-rw-r--r--   0 jens       (501) staff       (20)     1732 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/ImplC.py
+-rw-r--r--   0 jens       (501) staff       (20)    32088 2023-04-18 09:53:10.000000 AccessControl-6.1/src/AccessControl/ImplPython.py
+-rw-r--r--   0 jens       (501) staff       (20)     3805 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/Implementation.py
+-rw-r--r--   0 jens       (501) staff       (20)     1237 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/Owned.py
+-rw-r--r--   0 jens       (501) staff       (20)     5312 2022-03-26 10:28:34.000000 AccessControl-6.1/src/AccessControl/Permission.py
+-rw-r--r--   0 jens       (501) staff       (20)     5202 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/PermissionMapping.py
+-rw-r--r--   0 jens       (501) staff       (20)      826 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/PermissionRole.py
+-rw-r--r--   0 jens       (501) staff       (20)     2876 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/Permissions.py
+-rw-r--r--   0 jens       (501) staff       (20)     1563 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/Role.py
+-rw-r--r--   0 jens       (501) staff       (20)    13880 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/SecurityInfo.py
+-rw-r--r--   0 jens       (501) staff       (20)     2463 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/SecurityManagement.py
+-rw-r--r--   0 jens       (501) staff       (20)     1097 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/SecurityManager.py
+-rw-r--r--   0 jens       (501) staff       (20)     4882 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/SimpleObjectPolicies.py
+-rw-r--r--   0 jens       (501) staff       (20)      912 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/SpecialUsers.py
+-rw-r--r--   0 jens       (501) staff       (20)     2328 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/User.py
+-rw-r--r--   0 jens       (501) staff       (20)    17536 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/ZopeGuards.py
+-rw-r--r--   0 jens       (501) staff       (20)     1951 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/ZopeSecurityPolicy.py
+-rw-r--r--   0 jens       (501) staff       (20)     2271 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      738 2023-04-17 06:50:46.000000 AccessControl-6.1/src/AccessControl/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)    62941 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/cAccessControl.c
+-rw-r--r--   0 jens       (501) staff       (20)     3889 2023-04-17 06:50:46.000000 AccessControl-6.1/src/AccessControl/class_init.py
+-rw-r--r--   0 jens       (501) staff       (20)      104 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)    11074 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)      214 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/logger_wrapper.py
+-rw-r--r--   0 jens       (501) staff       (20)     1443 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/meta.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     2095 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/metaconfigure.py
+-rw-r--r--   0 jens       (501) staff       (20)     8617 2022-03-26 10:28:34.000000 AccessControl-6.1/src/AccessControl/owner.py
+-rw-r--r--   0 jens       (501) staff       (20)     1691 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/permissions.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3344 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/requestmethod.py
+-rw-r--r--   0 jens       (501) staff       (20)    16013 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/rolemanager.py
+-rw-r--r--   0 jens       (501) staff       (20)     2123 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/safe_formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)     7349 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/security.py
+-rw-r--r--   0 jens       (501) staff       (20)     5518 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tainted.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.237636 AccessControl-6.1/src/AccessControl/tests/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     5168 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/actual_python.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.237765 AccessControl-6.1/src/AccessControl/tests/mixed_module/
+-rw-r--r--   0 jens       (501) staff       (20)       78 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/mixed_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.237897 AccessControl-6.1/src/AccessControl/tests/mixed_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/mixed_module/submodule/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.238006 AccessControl-6.1/src/AccessControl/tests/private_module/
+-rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/private_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.238115 AccessControl-6.1/src/AccessControl/tests/private_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/private_module/submodule/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.238227 AccessControl-6.1/src/AccessControl/tests/public_module/
+-rw-r--r--   0 jens       (501) staff       (20)      125 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/public_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.238338 AccessControl-6.1/src/AccessControl/tests/public_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       44 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/public_module/submodule/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     6618 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/testClassSecurityInfo.py
+-rw-r--r--   0 jens       (501) staff       (20)     2449 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/testImplementation.py
+-rw-r--r--   0 jens       (501) staff       (20)     4805 2022-05-03 09:03:15.000000 AccessControl-6.1/src/AccessControl/tests/testModuleSecurity.py
+-rw-r--r--   0 jens       (501) staff       (20)      343 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/testPermissionMapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     4110 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/testPermissionRole.py
+-rw-r--r--   0 jens       (501) staff       (20)     9361 2022-03-26 10:28:34.000000 AccessControl-6.1/src/AccessControl/tests/testSecurityManager.py
+-rw-r--r--   0 jens       (501) staff       (20)    15171 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/testZCML.py
+-rw-r--r--   0 jens       (501) staff       (20)    33544 2023-04-19 05:40:53.000000 AccessControl-6.1/src/AccessControl/tests/testZopeGuards.py
+-rw-r--r--   0 jens       (501) staff       (20)    25448 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/testZopeSecurityPolicy.py
+-rw-r--r--   0 jens       (501) staff       (20)     9056 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/test_owner.py
+-rw-r--r--   0 jens       (501) staff       (20)     5411 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/test_requestmethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     4708 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/test_rolemanager.py
+-rw-r--r--   0 jens       (501) staff       (20)     8726 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/test_safe_formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)     2138 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/test_safeiter.py
+-rw-r--r--   0 jens       (501) staff       (20)    12667 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/test_tainted.py
+-rw-r--r--   0 jens       (501) staff       (20)     6446 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/tests/test_userfolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    22853 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/tests/test_users.py
+-rw-r--r--   0 jens       (501) staff       (20)     1224 2021-11-02 08:50:53.000000 AccessControl-6.1/src/AccessControl/unauthorized.py
+-rw-r--r--   0 jens       (501) staff       (20)    17049 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/userfolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    15399 2023-01-03 12:38:42.000000 AccessControl-6.1/src/AccessControl/users.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-22 11:34:00.235430 AccessControl-6.1/src/AccessControl.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)     8932 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     2999 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       67 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-03-26 10:31:42.000000 AccessControl-6.1/src/AccessControl.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      311 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)       14 2023-05-22 11:34:00.000000 AccessControl-6.1/src/AccessControl.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1215 2023-04-18 09:35:29.000000 AccessControl-6.1/tox.ini
```

### Comparing `AccessControl-6.0/.coveragerc` & `AccessControl-6.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/.manylinux-install.sh` & `AccessControl-6.1/.manylinux-install.sh`

 * *Files 10% similar despite different names*

```diff
@@ -24,33 +24,40 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
+        *"cp312"*) echo 'py312';;
         *"cp37"*) echo 'py37';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
+       [[ "${PYBIN}" == *"cp312"* ]] || \
        [[ "${PYBIN}" == *"cp311"* ]] || \
        [[ "${PYBIN}" == *"cp37"* ]] || \
        [[ "${PYBIN}" == *"cp38"* ]] || \
        [[ "${PYBIN}" == *"cp39"* ]] || \
        [[ "${PYBIN}" == *"cp310"* ]] ; then
-        "${PYBIN}/pip" install -e /io/
-        "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        if [[ "${PYBIN}" == *"cp312"* ]] ; then
+            "${PYBIN}/pip" install --pre -e /io/
+            "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
+        else
+            "${PYBIN}/pip" install -e /io/
+            "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        fi
         if [ `uname -m` == 'aarch64' ]; then
           cd /io/
           ${PYBIN}/pip install tox
           TOXENV=$(tox_env_map "${PYBIN}")
           ${PYBIN}/tox -e ${TOXENV}
           cd ..
         fi
```

### Comparing `AccessControl-6.0/CHANGES.rst` & `AccessControl-6.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+6.1 (2023-05-22)
+----------------
+- Update C header files for ``ExtensionClass`` and ``Acquisition``
+  from the original packages where needed.
+  (`#140 <https://github.com/zopefoundation/AccessControl/issues/140>`_)
+
+- Add preliminary support for Python 3.12a5.
+
+
 6.0 (2023-01-12)
 ----------------
 
 - Build Linux binary wheels for Python 3.11
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `AccessControl-6.0/CONTRIBUTING.md` & `AccessControl-6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/HISTORY.rst` & `AccessControl-6.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/LICENSE.txt` & `AccessControl-6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/PKG-INFO` & `AccessControl-6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AccessControl
-Version: 6.0
+Version: 6.1
 Summary: Security framework for Zope.
 Home-page: https://github.com/zopefoundation/AccessControl
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/AccessControl/issues
 Project-URL: Sources, https://github.com/zopefoundation/AccessControl
@@ -49,14 +49,23 @@
 
 
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+6.1 (2023-05-22)
+----------------
+- Update C header files for ``ExtensionClass`` and ``Acquisition``
+  from the original packages where needed.
+  (`#140 <https://github.com/zopefoundation/AccessControl/issues/140>`_)
+
+- Add preliminary support for Python 3.12a5.
+
+
 6.0 (2023-01-12)
 ----------------
 
 - Build Linux binary wheels for Python 3.11
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `AccessControl-6.0/README.rst` & `AccessControl-6.1/README.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/appveyor.yml` & `AccessControl-6.1/appveyor.yml`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
   matrix:
     - python: 37-x64
     - python: 38-x64
     - python: 39-x64
     - python: 310-x64
     - python: 311-x64
+    # `multibuild` cannot install non-final versions as they are not on
+    # ftp.python.org, so we skip Python 3.11 until its final release:
+    # - python: 312-x64
 
 install:
   - "SET PYTHONVERSION=%PYTHON%"
   - "SET PATH=C:\\Python%PYTHON%;c:\\Python%PYTHON%\\scripts;%PATH%"
   - ps: |
       $env:PYTHON = "C:\\Python${env:PYTHON}"
       if (-not (Test-Path $env:PYTHON)) {
```

### Comparing `AccessControl-6.0/docs/AccessControl.rst` & `AccessControl-6.1/docs/AccessControl.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/docs/requestmethod.rst` & `AccessControl-6.1/docs/requestmethod.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/include/Acquisition/Acquisition.h` & `AccessControl-6.1/include/Acquisition/Acquisition.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/include/ExtensionClass/ExtensionClass.h` & `AccessControl-6.1/include/ExtensionClass/ExtensionClass.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/include/ExtensionClass/_compat.h` & `AccessControl-6.1/include/ExtensionClass/_compat.h`

 * *Files 27% similar despite different names*

```diff
@@ -13,41 +13,50 @@
  ****************************************************************************/
 
 #ifndef PERSISTENT__COMPAT_H
 #define PERSISTENT__COMPAT_H
 
 #include "Python.h"
 
-#if PY_MAJOR_VERSION >= 3
-#define PY3K
-#endif
-
-#ifdef PY3K
 #define INTERN PyUnicode_InternFromString
 #define INTERN_INPLACE PyUnicode_InternInPlace
 #define NATIVE_CHECK PyUnicode_Check
 #define NATIVE_CHECK_EXACT PyUnicode_CheckExact
 #define NATIVE_FROM_STRING PyUnicode_FromString
 #define NATIVE_FROM_STRING_AND_SIZE PyUnicode_FromStringAndSize
 
 #define INT_FROM_LONG(x) PyLong_FromLong(x)
 #define INT_CHECK(x) PyLong_Check(x)
 #define INT_AS_LONG(x) PyLong_AS_LONG(x)
 
 #define HAS_TP_DESCR_GET(ob) 1
 
-#else
-#define INTERN PyString_InternFromString
-#define INTERN_INPLACE PyString_InternInPlace
-#define NATIVE_CHECK PyString_Check
-#define NATIVE_CHECK_EXACT PyString_CheckExact
-#define NATIVE_FROM_STRING PyString_FromString
-#define NATIVE_FROM_STRING_AND_SIZE PyString_FromStringAndSize
-
-#define INT_FROM_LONG(x) PyInt_FromLong(x)
-#define INT_CHECK(x) PyInt_Check(x)
-#define INT_AS_LONG(x) PyInt_AS_LONG(x)
+#endif
+
+/* Python compatibility shims */
+
+// Compatibility with Visual Studio 2013 and older which don't support
+// the inline keyword in C (only in C++): use __inline instead.
+#if (defined(_MSC_VER) && _MSC_VER < 1900 \
+     && !defined(__cplusplus) && !defined(inline))
+#  define inline __inline
+#  define PYTHONCAPI_COMPAT_MSC_INLINE
+   // These two macros are undefined at the end of this file
+#endif
+
+#ifndef _PyObject_CAST
+#  define _PyObject_CAST(op) ((PyObject*)(op))
+#endif
 
-#define HAS_TP_DESCR_GET(ob) PyType_HasFeature(Py_TYPE(ob), Py_TPFLAGS_HAVE_CLASS)
+#if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_TYPE)
+static inline void
+_Py_SET_TYPE(PyObject *ob, PyTypeObject *type)
+{
+    ob->ob_type = type;
+}
+#define Py_SET_TYPE(ob, type) _Py_SET_TYPE(_PyObject_CAST(ob), type)
 #endif
 
+#ifdef PYTHONCAPI_COMPAT_MSC_INLINE
+#  undef inline
+#  undef PYTHONCAPI_COMPAT_MSC_INLINE
 #endif
```

### Comparing `AccessControl-6.0/setup.cfg` & `AccessControl-6.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	.editorconfig
 	.meta.toml
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
-known_third_party = six, docutils, pkg_resources
+known_third_party = docutils, pkg_resources, pytz
 known_zope = 
 known_first_party = 
 default_section = ZOPE
 line_length = 79
 lines_after_imports = 2
 
 [egg_info]
```

### Comparing `AccessControl-6.0/setup.py` & `AccessControl-6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         include_dirs=['include', 'src'],
         sources=[join('src', 'AccessControl', 'cAccessControl.c')],
         depends=[join('include', 'ExtensionClass', 'ExtensionClass.h'),
                  join('include', 'ExtensionClass', '_compat.h'),
                  join('include', 'Acquisition', 'Acquisition.h')]),
 ]
 
-version = '6.0'
+version = '6.1'
 
 
 setup(name='AccessControl',
       version=version,
       url='https://github.com/zopefoundation/AccessControl',
       project_urls={
           'Issue Tracker': ('https://github.com/zopefoundation'
```

### Comparing `AccessControl-6.0/src/AccessControl/AuthEncoding.py` & `AccessControl-6.1/src/AccessControl/AuthEncoding.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/ImplC.py` & `AccessControl-6.1/src/AccessControl/ImplC.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/ImplPython.py` & `AccessControl-6.1/src/AccessControl/ImplPython.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/Implementation.py` & `AccessControl-6.1/src/AccessControl/Implementation.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/Owned.py` & `AccessControl-6.1/src/AccessControl/Owned.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/Permission.py` & `AccessControl-6.1/src/AccessControl/Permission.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/PermissionMapping.py` & `AccessControl-6.1/src/AccessControl/PermissionMapping.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/PermissionRole.py` & `AccessControl-6.1/src/AccessControl/PermissionRole.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/Permissions.py` & `AccessControl-6.1/src/AccessControl/Permissions.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/Role.py` & `AccessControl-6.1/src/AccessControl/Role.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/SecurityInfo.py` & `AccessControl-6.1/src/AccessControl/SecurityInfo.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/SecurityManagement.py` & `AccessControl-6.1/src/AccessControl/SecurityManagement.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/SecurityManager.py` & `AccessControl-6.1/src/AccessControl/SecurityManager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/SimpleObjectPolicies.py` & `AccessControl-6.1/src/AccessControl/SimpleObjectPolicies.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/SpecialUsers.py` & `AccessControl-6.1/src/AccessControl/SpecialUsers.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/User.py` & `AccessControl-6.1/src/AccessControl/User.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/ZopeGuards.py` & `AccessControl-6.1/src/AccessControl/ZopeGuards.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/ZopeSecurityPolicy.py` & `AccessControl-6.1/src/AccessControl/ZopeSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/__init__.py` & `AccessControl-6.1/src/AccessControl/__init__.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/_compat.h` & `AccessControl-6.1/src/AccessControl/_compat.h`

 * *Files 19% similar despite different names*

```diff
@@ -11,8 +11,8 @@
   FOR A PARTICULAR PURPOSE
 
  ****************************************************************************/
 
 #include "Python.h"
 
 #define NATIVE_FORMAT PyUnicode_Format
-#define NATIVE_GET_SIZE PyUnicode_GET_SIZE
+#define NATIVE_GET_SIZE PyUnicode_GET_LENGTH
```

### Comparing `AccessControl-6.0/src/AccessControl/cAccessControl.c` & `AccessControl-6.1/src/AccessControl/cAccessControl.c`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/class_init.py` & `AccessControl-6.1/src/AccessControl/class_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 def InitializeClass(self):
     from AccessControl.Permission import registerPermissions
     from AccessControl.PermissionRole import PermissionRole
 
     dict = self.__dict__
     have = dict.__contains__
     ft = type(InitializeClass)
+    # Prevent `RuntimeError: dictionary changed size during iteration`:
     dict_items = list(dict.items())
 
     for name, v in dict_items:
         if getattr(v, '_need__name__', 0):
             d = v.__dict__
             oldname = d.get('__name__', '')
             if d.get('_implicit__name__', 0):
```

### Comparing `AccessControl-6.0/src/AccessControl/interfaces.py` & `AccessControl-6.1/src/AccessControl/interfaces.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/meta.zcml` & `AccessControl-6.1/src/AccessControl/meta.zcml`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/metaconfigure.py` & `AccessControl-6.1/src/AccessControl/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/owner.py` & `AccessControl-6.1/src/AccessControl/owner.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/permissions.zcml` & `AccessControl-6.1/src/AccessControl/permissions.zcml`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/requestmethod.py` & `AccessControl-6.1/src/AccessControl/requestmethod.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/rolemanager.py` & `AccessControl-6.1/src/AccessControl/rolemanager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/safe_formatter.py` & `AccessControl-6.1/src/AccessControl/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/security.py` & `AccessControl-6.1/src/AccessControl/security.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tainted.py` & `AccessControl-6.1/src/AccessControl/tainted.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/actual_python.py` & `AccessControl-6.1/src/AccessControl/tests/actual_python.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testClassSecurityInfo.py` & `AccessControl-6.1/src/AccessControl/tests/testClassSecurityInfo.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testImplementation.py` & `AccessControl-6.1/src/AccessControl/tests/testImplementation.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testModuleSecurity.py` & `AccessControl-6.1/src/AccessControl/tests/testModuleSecurity.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testPermissionRole.py` & `AccessControl-6.1/src/AccessControl/tests/testPermissionRole.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testSecurityManager.py` & `AccessControl-6.1/src/AccessControl/tests/testSecurityManager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testZCML.py` & `AccessControl-6.1/src/AccessControl/tests/testZCML.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/testZopeGuards.py` & `AccessControl-6.1/src/AccessControl/tests/testZopeGuards.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         from AccessControl.ZopeGuards import guarded_getattr
         obj, name = object(), 'nonesuch'
         self.assertRaises(AttributeError, guarded_getattr, obj, name)
         self.assertEqual(len(self.__sm.calls), 0)
 
     def test_unhashable_key(self):
         from AccessControl.ZopeGuards import guarded_getattr
-        obj, name = object(), {}
+        obj, name = object(), []
         self.assertRaises(TypeError, guarded_getattr, obj, name)
         self.assertEqual(len(self.__sm.calls), 0)
 
     def test_unauthorized(self):
         from AccessControl import Unauthorized
         from AccessControl.ZopeGuards import guarded_getattr
         obj, name = Method(), 'args'
@@ -176,15 +176,15 @@
         obj, name = object(), 'nonesuch'
         self.assertFalse(guarded_hasattr(obj, name))
         self.assertEqual(len(self.__sm.calls), 0)
         del self.__sm.calls[:]
 
     def test_unhashable_key(self):
         from AccessControl.ZopeGuards import guarded_hasattr
-        obj, name = object(), {}
+        obj, name = object(), []
         self.assertFalse(guarded_hasattr(obj, name))
         self.assertEqual(len(self.__sm.calls), 0)
 
     def test_unauthorized(self):
         from AccessControl.ZopeGuards import guarded_hasattr
         obj, name = Method(), 'args'
         value = getattr(obj, name)
```

### Comparing `AccessControl-6.0/src/AccessControl/tests/testZopeSecurityPolicy.py` & `AccessControl-6.1/src/AccessControl/tests/testZopeSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_owner.py` & `AccessControl-6.1/src/AccessControl/tests/test_owner.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_requestmethod.py` & `AccessControl-6.1/src/AccessControl/tests/test_requestmethod.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_rolemanager.py` & `AccessControl-6.1/src/AccessControl/tests/test_rolemanager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_safe_formatter.py` & `AccessControl-6.1/src/AccessControl/tests/test_safe_formatter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_safeiter.py` & `AccessControl-6.1/src/AccessControl/tests/test_safeiter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_tainted.py` & `AccessControl-6.1/src/AccessControl/tests/test_tainted.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_userfolder.py` & `AccessControl-6.1/src/AccessControl/tests/test_userfolder.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/tests/test_users.py` & `AccessControl-6.1/src/AccessControl/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/unauthorized.py` & `AccessControl-6.1/src/AccessControl/unauthorized.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/userfolder.py` & `AccessControl-6.1/src/AccessControl/userfolder.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl/users.py` & `AccessControl-6.1/src/AccessControl/users.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/src/AccessControl.egg-info/PKG-INFO` & `AccessControl-6.1/src/AccessControl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AccessControl
-Version: 6.0
+Version: 6.1
 Summary: Security framework for Zope.
 Home-page: https://github.com/zopefoundation/AccessControl
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/AccessControl/issues
 Project-URL: Sources, https://github.com/zopefoundation/AccessControl
@@ -49,14 +49,23 @@
 
 
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+6.1 (2023-05-22)
+----------------
+- Update C header files for ``ExtensionClass`` and ``Acquisition``
+  from the original packages where needed.
+  (`#140 <https://github.com/zopefoundation/AccessControl/issues/140>`_)
+
+- Add preliminary support for Python 3.12a5.
+
+
 6.0 (2023-01-12)
 ----------------
 
 - Build Linux binary wheels for Python 3.11
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `AccessControl-6.0/src/AccessControl.egg-info/SOURCES.txt` & `AccessControl-6.1/src/AccessControl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AccessControl-6.0/tox.ini` & `AccessControl-6.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 [tox]
-minversion = 3.18
+minversion = 4.0
 envlist =
     lint
     py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
+    py312,py312-pure
     coverage
 
 [testenv]
 usedevelop = true
+pip_pre = py312: true
 deps =
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
```

