# Comparing `tmp/mahdix-0.1.1.tar.gz` & `tmp/mahdix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahdix-0.1.1.tar", last modified: Mon May 22 08:13:53 2023, max compression
+gzip compressed data, was "mahdix-0.1.2.tar", last modified: Mon May 22 12:27:08 2023, max compression
```

## Comparing `mahdix-0.1.1.tar` & `mahdix-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:53.419073 mahdix-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 08:13:53.419073 mahdix-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:53.419073 mahdix-0.1.1/mahdix/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-22 08:13:32.000000 mahdix-0.1.1/mahdix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:53.419073 mahdix-0.1.1/mahdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 08:13:53.000000 mahdix-0.1.1/mahdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:13:53.000000 mahdix-0.1.1/mahdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:13:53.000000 mahdix-0.1.1/mahdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 08:13:53.000000 mahdix-0.1.1/mahdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:13:53.419073 mahdix-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 08:13:32.000000 mahdix-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:27:08.932955 mahdix-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 12:27:08.932955 mahdix-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:27:08.932955 mahdix-0.1.2/mahdix/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-22 12:26:55.000000 mahdix-0.1.2/mahdix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:27:08.932955 mahdix-0.1.2/mahdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 12:27:08.000000 mahdix-0.1.2/mahdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 12:27:08.000000 mahdix-0.1.2/mahdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:27:08.000000 mahdix-0.1.2/mahdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 12:27:08.000000 mahdix-0.1.2/mahdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:27:08.932955 mahdix-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 12:26:55.000000 mahdix-0.1.2/setup.py
```

