# Comparing `tmp/serenity-module-root-cause-finder-0.0.0.tar.gz` & `tmp/serenity-module-root-cause-finder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serenity-module-root-cause-finder-0.0.0.tar", last modified: Wed Feb  1 20:17:15 2023, max compression
+gzip compressed data, was "serenity-module-root-cause-finder-0.1.3.tar", last modified: Mon May 22 10:07:21 2023, max compression
```

## Comparing `serenity-module-root-cause-finder-0.0.0.tar` & `serenity-module-root-cause-finder-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 20:17:15.213432 serenity-module-root-cause-finder-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      207 2023-02-01 20:17:15.213432 serenity-module-root-cause-finder-0.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 20:17:15.209432 serenity-module-root-cause-finder-0.0.0/serenity_module_root_cause_finder.egg-info/
--rw-r--r--   0 root         (0) root         (0)      207 2023-02-01 20:17:15.000000 serenity-module-root-cause-finder-0.0.0/serenity_module_root_cause_finder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      236 2023-02-01 20:17:15.000000 serenity-module-root-cause-finder-0.0.0/serenity_module_root_cause_finder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 20:17:15.000000 serenity-module-root-cause-finder-0.0.0/serenity_module_root_cause_finder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 20:17:15.000000 serenity-module-root-cause-finder-0.0.0/serenity_module_root_cause_finder.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-01 20:17:15.213432 serenity-module-root-cause-finder-0.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      134 2023-02-01 20:16:53.000000 serenity-module-root-cause-finder-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:07:21.454744 serenity-module-root-cause-finder-0.1.3/
+-rw-rw-rw-   0        0        0       80 2023-05-22 10:07:21.455743 serenity-module-root-cause-finder-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 10:07:21.452747 serenity-module-root-cause-finder-0.1.3/serenity_module_root_cause_finder.egg-info/
+-rw-rw-rw-   0        0        0       80 2023-05-22 10:07:21.000000 serenity-module-root-cause-finder-0.1.3/serenity_module_root_cause_finder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-22 10:07:21.000000 serenity-module-root-cause-finder-0.1.3/serenity_module_root_cause_finder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:07:21.000000 serenity-module-root-cause-finder-0.1.3/serenity_module_root_cause_finder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:07:21.000000 serenity-module-root-cause-finder-0.1.3/serenity_module_root_cause_finder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:07:21.458744 serenity-module-root-cause-finder-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      125 2023-05-22 10:07:01.000000 serenity-module-root-cause-finder-0.1.3/setup.py
```

