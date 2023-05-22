# Comparing `tmp/boneflet-0.1.0.dev1.tar.gz` & `tmp/boneflet-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneflet-0.1.0.dev1.tar", last modified: Mon Apr 10 13:01:18 2023, max compression
+gzip compressed data, was "boneflet-0.1.0.dev2.tar", last modified: Mon May 22 13:52:25 2023, max compression
```

## Comparing `boneflet-0.1.0.dev1.tar` & `boneflet-0.1.0.dev2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       31 2023-04-10 12:59:29.626977 boneflet-0.1.0.dev1/README.md
--rw-r--r--   0        0        0      330 2023-04-10 13:01:18.554715 boneflet-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      212 1970-01-01 00:00:00.000000 boneflet-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-04-10 12:59:29.626977 boneflet-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0      354 2023-05-22 13:52:25.736531 boneflet-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      243 1970-01-01 00:00:00.000000 boneflet-0.1.0.dev2/PKG-INFO
```

