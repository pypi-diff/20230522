# Comparing `tmp/iparapheur-utils.beta-0.0.1.post94307.tar.gz` & `tmp/iparapheur-utils.beta-0.0.1.post94309.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iparapheur-utils.beta-0.0.1.post94307.tar", last modified: Mon Oct  7 15:51:32 2019, max compression
+gzip compressed data, was "dist/iparapheur-utils.beta-0.0.1.post94309.tar", last modified: Mon Oct  7 15:52:20 2019, max compression
```

## Comparing `iparapheur-utils.beta-0.0.1.post94307.tar` & `iparapheur-utils.beta-0.0.1.post94309.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/
--rwxrwxrwx   0 root         (0) root         (0)     3513 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/JSONHelper.py
--rwxrwxrwx   0 root         (0) root         (0)     3624 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12644 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/Client.py
--rwxrwxrwx   0 root         (0) root         (0)     8364 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/Webservice.py
--rwxrwxrwx   0 root         (0) root         (0)     3319 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/pprint.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2019-10-07 15:51:31.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/files/
--rw-rw-rw-   0 root         (0) root         (0)     1675 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/files/private.pem
--rw-rw-rw-   0 root         (0) root         (0)     2520 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/files/public.pem
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/
--rw-rw-rw-   0 root         (0) root         (0)      281 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/recuparchives.cfg
--rw-rw-rw-   0 root         (0) root         (0)      206 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/import.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/reset_admin_password.cfg
--rw-rw-rw-   0 root         (0) root         (0)      173 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/pushdoc.cfg
--rwxrwxrwx   0 root         (0) root         (0)       82 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/script.cfg
--rw-rw-rw-   0 root         (0) root         (0)      155 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/ldapsearch.cfg
--rw-rw-rw-   0 root         (0) root         (0)      344 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/export.cfg
--rw-rw-rw-   0 root         (0) root         (0)       74 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/configs/patch.cfg
--rwxrwxrwx   0 root         (0) root         (0)    13745 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/core.py
--rwxrwxrwx   0 root         (0) root         (0)       82 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/script.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    20022 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/import_data.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11785 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/export_data.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/ipclean.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/change_name.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/pushdoc.py
--rw-rw-rw-   0 root         (0) root         (0)    12064 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/recupArchives.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/
--rw-rw-rw-   0 root         (0) root         (0)     5256 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/count_files.sh
--rwxrwxrwx   0 root         (0) root         (0)     2553 2019-10-07 15:49:45.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/patch.sh
--rw-rw-rw-   0 root         (0) root         (0)     4203 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/ipclean.sh
--rw-rw-rw-   0 root         (0) root         (0)    40906 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/checkInstallationIP.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/javascript/
--rw-rw-rw-   0 root         (0) root         (0)       98 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/javascript/removeNode.js
--rw-rw-rw-   0 root         (0) root         (0)     1495 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/reset_admin_password.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/ldapsearch.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/remove_ldap.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/count_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17068 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1431 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      622 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1589 2019-10-07 15:51:31.000000 iparapheur-utils.beta-0.0.1.post94307/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    17068 2019-10-07 15:51:32.000000 iparapheur-utils.beta-0.0.1.post94307/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       68 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    13382 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/README.md
--rw-rw-rw-   0 root         (0) root         (0)     5683 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94307/CHANGELOG.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/
+-rwxrwxrwx   0 root         (0) root         (0)     3513 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/JSONHelper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3624 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12644 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/Client.py
+-rwxrwxrwx   0 root         (0) root         (0)     8364 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/Webservice.py
+-rwxrwxrwx   0 root         (0) root         (0)     3319 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/pprint.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/files/
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/files/private.pem
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/files/public.pem
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      281 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/recuparchives.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      206 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/import.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/reset_admin_password.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      173 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/pushdoc.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       82 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/script.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      155 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/ldapsearch.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      344 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/export.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       74 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/configs/patch.cfg
+-rwxrwxrwx   0 root         (0) root         (0)    13745 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       82 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/script.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    20022 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/import_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11785 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/export_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/ipclean.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/change_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/pushdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    12064 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/recupArchives.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/count_files.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2553 2019-10-07 15:49:45.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/patch.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/ipclean.sh
+-rw-rw-rw-   0 root         (0) root         (0)    40906 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/checkInstallationIP.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/javascript/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/javascript/removeNode.js
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/reset_admin_password.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/ldapsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)      946 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/remove_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/count_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17068 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1431 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      622 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    17068 2019-10-07 15:52:20.000000 iparapheur-utils.beta-0.0.1.post94309/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       68 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    13382 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2019-10-07 09:53:27.000000 iparapheur-utils.beta-0.0.1.post94309/CHANGELOG.md
```

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/JSONHelper.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/JSONHelper.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/__init__.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/Client.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/Client.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/Webservice.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/Webservice.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/parapheur/pprint.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/parapheur/pprint.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/files/private.pem` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/files/private.pem`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/files/public.pem` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/files/public.pem`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/core.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/core.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/import_data.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/import_data.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/__init__.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/export_data.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/change_name.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/change_name.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/pushdoc.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/pushdoc.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/recupArchives.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/recupArchives.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/count_files.sh` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/count_files.sh`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/patch.sh` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/patch.sh`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/script/ipclean.sh` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/script/ipclean.sh`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/checkInstallationIP.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/checkInstallationIP.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/reset_admin_password.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/reset_admin_password.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/ldapsearch.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/ldapsearch.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/parapheur/scripts/remove_ldap.py` & `iparapheur-utils.beta-0.0.1.post94309/parapheur/scripts/remove_ldap.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/PKG-INFO` & `iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-utils.beta
-Version: 0.0.1.post94307
+Version: 0.0.1.post94309
 Summary: Client python pour i-Parapheur
 Home-page: https://gitlab.libriciel.fr/i-parapheur/client-python
 Author: Lukas Hameury
 Author-email: lukas.hameury@libriciel.fr
 License: CeCILL v2
 Description: # Introduction
```

### Comparing `iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/SOURCES.txt` & `iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/iparapheur_utils.beta.egg-info/entry_points.txt` & `iparapheur-utils.beta-0.0.1.post94309/iparapheur_utils.beta.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/setup.py` & `iparapheur-utils.beta-0.0.1.post94309/setup.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/PKG-INFO` & `iparapheur-utils.beta-0.0.1.post94309/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-utils.beta
-Version: 0.0.1.post94307
+Version: 0.0.1.post94309
 Summary: Client python pour i-Parapheur
 Home-page: https://gitlab.libriciel.fr/i-parapheur/client-python
 Author: Lukas Hameury
 Author-email: lukas.hameury@libriciel.fr
 License: CeCILL v2
 Description: # Introduction
```

### Comparing `iparapheur-utils.beta-0.0.1.post94307/README.md` & `iparapheur-utils.beta-0.0.1.post94309/README.md`

 * *Files identical despite different names*

### Comparing `iparapheur-utils.beta-0.0.1.post94307/CHANGELOG.md` & `iparapheur-utils.beta-0.0.1.post94309/CHANGELOG.md`

 * *Files identical despite different names*

