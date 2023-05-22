# Comparing `tmp/kolombos-1.5.3.tar.gz` & `tmp/kolombos-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolombos-1.5.3.tar", last modified: Mon May 22 01:12:43 2023, max compression
+gzip compressed data, was "kolombos-1.5.4.tar", last modified: Mon May 22 01:18:24 2023, max compression
```

## Comparing `kolombos-1.5.3.tar` & `kolombos-1.5.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.078410 kolombos-1.5.3/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1076 2022-05-09 22:55:55.000000 kolombos-1.5.3/LICENSE
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14085 2023-05-22 01:12:43.078410 kolombos-1.5.3/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13513 2023-05-01 10:08:20.000000 kolombos-1.5.3/README.md
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      391 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      366 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      995 2023-02-07 05:02:28.000000 kolombos-1.5.3/kolombos/app.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    12687 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/arghelp.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/byteio/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      644 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      317 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2090 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/const.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/byteio/formatter/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      425 2022-06-26 06:50:16.000000 kolombos-1.5.3/kolombos/byteio/formatter/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2131 2022-09-12 06:34:27.000000 kolombos-1.5.3/kolombos/byteio/formatter/_abstract.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4448 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/formatter/binary.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2022-05-10 09:36:33.000000 kolombos-1.5.3/kolombos/byteio/formatter/factory.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2161 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/formatter/text.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/byteio/parser/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      336 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/parser/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1749 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/parser/buffer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8385 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/parser/parser.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1688 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/partial_override.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3928 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/reader.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/byteio/segment/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      500 2022-05-10 09:36:33.000000 kolombos-1.5.3/kolombos/byteio/segment/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8327 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/segment/buffer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      540 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/segment/chainable.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      824 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/segment/printer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2298 2022-05-10 09:36:33.000000 kolombos-1.5.3/kolombos/byteio/segment/segment.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1056 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/byteio/segment/sequence_ref.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/byteio/template/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      665 2022-05-10 09:36:33.000000 kolombos-1.5.3/kolombos/byteio/template/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3257 2023-04-27 19:42:47.000000 kolombos-1.5.3/kolombos/byteio/template/registry.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4346 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/template/template.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2955 2022-07-01 12:01:40.000000 kolombos-1.5.3/kolombos/byteio/template/template_control.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2678 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/byteio/template/template_escape.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3593 2023-05-19 03:17:59.000000 kolombos-1.5.3/kolombos/byteio/template/template_escape_sgr.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1011 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/template/template_newline.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      779 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/template/template_printable.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1262 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/byteio/template/template_utf8.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      685 2023-02-07 05:22:33.000000 kolombos-1.5.3/kolombos/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10579 2023-02-07 05:22:33.000000 kolombos-1.5.3/kolombos/console.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      640 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/demo.bin
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24074 2023-05-22 01:12:38.000000 kolombos-1.5.3/kolombos/legend.ansi
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos/runner/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      481 2023-02-07 05:22:33.000000 kolombos-1.5.3/kolombos/runner/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      411 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/runner/_abstract.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2346 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/runner/byteio.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1050 2023-05-20 13:23:26.000000 kolombos-1.5.3/kolombos/runner/demo.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      790 2023-02-07 05:22:33.000000 kolombos-1.5.3/kolombos/runner/factory.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      664 2022-05-10 09:36:32.000000 kolombos-1.5.3/kolombos/runner/legend.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      635 2023-01-11 01:46:13.000000 kolombos-1.5.3/kolombos/runner/version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4130 2023-04-01 18:06:55.000000 kolombos-1.5.3/kolombos/settings.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       22 2023-05-20 13:19:11.000000 kolombos-1.5.3/kolombos/version.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.074410 kolombos-1.5.3/kolombos.egg-info/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14085 2023-05-22 01:12:43.000000 kolombos-1.5.3/kolombos.egg-info/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1922 2023-05-22 01:12:43.000000 kolombos-1.5.3/kolombos.egg-info/SOURCES.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-05-22 01:12:43.000000 kolombos-1.5.3/kolombos.egg-info/dependency_links.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       52 2023-05-22 01:12:43.000000 kolombos-1.5.3/kolombos.egg-info/entry_points.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       18 2023-05-22 01:12:43.000000 kolombos-1.5.3/kolombos.egg-info/top_level.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-05-09 22:55:55.000000 kolombos-1.5.3/pyproject.toml
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.078410 kolombos-1.5.3/pytermor/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      642 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      262 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      290 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/_version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    25301 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/ansi.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27939 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/color.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1871 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27766 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/render.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:12:43.078410 kolombos-1.5.3/pytermor/util/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1160 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5402 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/auto_float.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     7188 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/prefixed_unit.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1931 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/stdlib_ext.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3996 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/string_filter.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10092 2023-01-11 01:46:13.000000 kolombos-1.5.3/pytermor/util/time_delta.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      798 2023-05-22 01:12:43.078410 kolombos-1.5.3/setup.cfg
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.836495 kolombos-1.5.4/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1076 2022-05-09 22:55:55.000000 kolombos-1.5.4/LICENSE
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14216 2023-05-22 01:18:24.836495 kolombos-1.5.4/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13644 2023-05-22 01:18:09.000000 kolombos-1.5.4/README.md
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.828496 kolombos-1.5.4/kolombos/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      391 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      366 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      995 2023-02-07 05:02:28.000000 kolombos-1.5.4/kolombos/app.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    12687 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/arghelp.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/byteio/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      644 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      317 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2090 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/const.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/byteio/formatter/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      425 2022-06-26 06:50:16.000000 kolombos-1.5.4/kolombos/byteio/formatter/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2131 2022-09-12 06:34:27.000000 kolombos-1.5.4/kolombos/byteio/formatter/_abstract.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4448 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/formatter/binary.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2022-05-10 09:36:33.000000 kolombos-1.5.4/kolombos/byteio/formatter/factory.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2161 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/formatter/text.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/byteio/parser/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      336 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/parser/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1749 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/parser/buffer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8385 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/parser/parser.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1688 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/partial_override.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3928 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/reader.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/byteio/segment/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      500 2022-05-10 09:36:33.000000 kolombos-1.5.4/kolombos/byteio/segment/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8327 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/segment/buffer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      540 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/segment/chainable.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      824 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/segment/printer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2298 2022-05-10 09:36:33.000000 kolombos-1.5.4/kolombos/byteio/segment/segment.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1056 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/byteio/segment/sequence_ref.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/byteio/template/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      665 2022-05-10 09:36:33.000000 kolombos-1.5.4/kolombos/byteio/template/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3257 2023-04-27 19:42:47.000000 kolombos-1.5.4/kolombos/byteio/template/registry.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4346 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/template/template.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2955 2022-07-01 12:01:40.000000 kolombos-1.5.4/kolombos/byteio/template/template_control.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2678 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/byteio/template/template_escape.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3593 2023-05-19 03:17:59.000000 kolombos-1.5.4/kolombos/byteio/template/template_escape_sgr.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1011 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/template/template_newline.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      779 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/template/template_printable.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1262 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/byteio/template/template_utf8.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      685 2023-02-07 05:22:33.000000 kolombos-1.5.4/kolombos/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10579 2023-02-07 05:22:33.000000 kolombos-1.5.4/kolombos/console.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      640 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/demo.bin
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24074 2023-05-22 01:18:20.000000 kolombos-1.5.4/kolombos/legend.ansi
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/kolombos/runner/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      481 2023-02-07 05:22:33.000000 kolombos-1.5.4/kolombos/runner/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      411 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/runner/_abstract.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2346 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/runner/byteio.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1074 2023-05-22 01:15:48.000000 kolombos-1.5.4/kolombos/runner/demo.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      790 2023-02-07 05:22:33.000000 kolombos-1.5.4/kolombos/runner/factory.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      664 2022-05-10 09:36:32.000000 kolombos-1.5.4/kolombos/runner/legend.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      635 2023-01-11 01:46:13.000000 kolombos-1.5.4/kolombos/runner/version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4130 2023-04-01 18:06:55.000000 kolombos-1.5.4/kolombos/settings.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       22 2023-05-22 01:15:56.000000 kolombos-1.5.4/kolombos/version.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.828496 kolombos-1.5.4/kolombos.egg-info/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14216 2023-05-22 01:18:24.000000 kolombos-1.5.4/kolombos.egg-info/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1922 2023-05-22 01:18:24.000000 kolombos-1.5.4/kolombos.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-05-22 01:18:24.000000 kolombos-1.5.4/kolombos.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       52 2023-05-22 01:18:24.000000 kolombos-1.5.4/kolombos.egg-info/entry_points.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       18 2023-05-22 01:18:24.000000 kolombos-1.5.4/kolombos.egg-info/top_level.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-05-09 22:55:55.000000 kolombos-1.5.4/pyproject.toml
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.832496 kolombos-1.5.4/pytermor/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      642 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      262 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      290 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/_version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    25301 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/ansi.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27939 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/color.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1871 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27766 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/render.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-05-22 01:18:24.836495 kolombos-1.5.4/pytermor/util/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1160 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5402 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/auto_float.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     7188 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/prefixed_unit.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1931 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/stdlib_ext.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3996 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/string_filter.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10092 2023-01-11 01:46:13.000000 kolombos-1.5.4/pytermor/util/time_delta.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      798 2023-05-22 01:18:24.836495 kolombos-1.5.4/setup.cfg
```

### Comparing `kolombos-1.5.3/LICENSE` & `kolombos-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/PKG-INFO` & `kolombos-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolombos
-Version: 1.5.3
+Version: 1.5.4
 Summary: CLI control characters and escape sequences viewer/visualizer
 Home-page: https://github.com/es7s/kolombos
 Author: Aleksandr Shavykin
 Author-email: 0.delameter@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -216,63 +216,57 @@
 
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
+### v1.5.4
+- FIX: reverted default column amount in `--demo` mode
 
-### v1.5.2
+### v1.5.3
+- FIX: errors while processing SGR with subparams (e.g. `4:3;`)
 
+### v1.5.2
 - UPDATE: icon redraw
 
-
 ### v1.5.1
-
 - FIX: packaging assets
 
-
 ### v1.5
 - NEW: `--demo` mode
 
-
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
 
 ### v1.4
 - REFACTOR: base colors
 - REFACTOR: extended legend 
 - DOCS:  update README and screenshots 
 
-
 ### v1.3
 - Swap -D and -d (debug/decode)
 - Make '--marker 0' default (was 1)
 - Update legend
 - Upgrade `pytermor` to 2.1
 
 ### v1.2.1
-
 - Minor update.
 
 ### v1.2
-
 - Separators additional styling.
 - Separators auto-hide from `-m0`.
 - `--no-sep[arators]` launch option.
 - `run` dev script for quick launch of repo versions.
 - Updated output format of SGR color prefixes.
 - SGR labels are now getting colored instead of marker details (if `-m0` is set).
 - Updated legend.
 
 ### v1.1
-
 - Additional separators around escape seqs (in text mode) for better readability.
 
 ### v1.0.2
-
 - Added logos.
 - Fixed pipy README images.
 
 ### v1.0.1
-
 - First public version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolombos Version: 1.5.3 Summary: CLI control
+Metadata-Version: 2.1 Name: kolombos Version: 1.5.4 Summary: CLI control
 characters and escape sequences viewer/visualizer Home-page: https://
 github.com/es7s/kolombos Author: Aleksandr Shavykin Author-email:
 0.delameter@gmail.com Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Terminals Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -157,19 +157,21 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
-### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
-### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
-README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
-marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
-v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
-auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
-for quick launch of repo versions. - Updated output format of SGR color
-prefixes. - SGR labels are now getting colored instead of marker details (if `-
-m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
-seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
-pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.4 - FIX: reverted default column amount in `--demo` mode ###
+v1.5.3 - FIX: errors while processing SGR with subparams (e.g. `4:3;`) ###
+v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets ### v1.5 - NEW:
+`--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1 ### v1.4 -
+REFACTOR: base colors - REFACTOR: extended legend - DOCS: update README and
+screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--marker 0'
+default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ### v1.2.1 - Minor
+update. ### v1.2 - Separators additional styling. - Separators auto-hide from
+`-m0`. - `--no-sep[arators]` launch option. - `run` dev script for quick launch
+of repo versions. - Updated output format of SGR color prefixes. - SGR labels
+are now getting colored instead of marker details (if `-m0` is set). - Updated
+legend. ### v1.1 - Additional separators around escape seqs (in text mode) for
+better readability. ### v1.0.2 - Added logos. - Fixed pipy README images. ###
+v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.3/README.md` & `kolombos-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,63 +199,57 @@
 
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
+### v1.5.4
+- FIX: reverted default column amount in `--demo` mode
 
-### v1.5.2
+### v1.5.3
+- FIX: errors while processing SGR with subparams (e.g. `4:3;`)
 
+### v1.5.2
 - UPDATE: icon redraw
 
-
 ### v1.5.1
-
 - FIX: packaging assets
 
-
 ### v1.5
 - NEW: `--demo` mode
 
-
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
 
 ### v1.4
 - REFACTOR: base colors
 - REFACTOR: extended legend 
 - DOCS:  update README and screenshots 
 
-
 ### v1.3
 - Swap -D and -d (debug/decode)
 - Make '--marker 0' default (was 1)
 - Update legend
 - Upgrade `pytermor` to 2.1
 
 ### v1.2.1
-
 - Minor update.
 
 ### v1.2
-
 - Separators additional styling.
 - Separators auto-hide from `-m0`.
 - `--no-sep[arators]` launch option.
 - `run` dev script for quick launch of repo versions.
 - Updated output format of SGR color prefixes.
 - SGR labels are now getting colored instead of marker details (if `-m0` is set).
 - Updated legend.
 
 ### v1.1
-
 - Additional separators around escape seqs (in text mode) for better readability.
 
 ### v1.0.2
-
 - Added logos.
 - Fixed pipy README images.
 
 ### v1.0.1
-
 - First public version.
```

#### html2text {}

```diff
@@ -149,19 +149,21 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
-### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
-### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
-README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
-marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
-v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
-auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
-for quick launch of repo versions. - Updated output format of SGR color
-prefixes. - SGR labels are now getting colored instead of marker details (if `-
-m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
-seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
-pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.4 - FIX: reverted default column amount in `--demo` mode ###
+v1.5.3 - FIX: errors while processing SGR with subparams (e.g. `4:3;`) ###
+v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets ### v1.5 - NEW:
+`--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1 ### v1.4 -
+REFACTOR: base colors - REFACTOR: extended legend - DOCS: update README and
+screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--marker 0'
+default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ### v1.2.1 - Minor
+update. ### v1.2 - Separators additional styling. - Separators auto-hide from
+`-m0`. - `--no-sep[arators]` launch option. - `run` dev script for quick launch
+of repo versions. - Updated output format of SGR color prefixes. - SGR labels
+are now getting colored instead of marker details (if `-m0` is set). - Updated
+legend. ### v1.1 - Additional separators around escape seqs (in text mode) for
+better readability. ### v1.0.2 - Added logos. - Fixed pipy README images. ###
+v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.3/kolombos/app.py` & `kolombos-1.5.4/kolombos/app.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/arghelp.py` & `kolombos-1.5.4/kolombos/arghelp.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/__init__.py` & `kolombos-1.5.4/kolombos/byteio/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/const.py` & `kolombos-1.5.4/kolombos/byteio/const.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/formatter/_abstract.py` & `kolombos-1.5.4/kolombos/byteio/formatter/_abstract.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/formatter/binary.py` & `kolombos-1.5.4/kolombos/byteio/formatter/binary.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/formatter/factory.py` & `kolombos-1.5.4/kolombos/byteio/formatter/factory.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/formatter/text.py` & `kolombos-1.5.4/kolombos/byteio/formatter/text.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/parser/buffer.py` & `kolombos-1.5.4/kolombos/byteio/parser/buffer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/parser/parser.py` & `kolombos-1.5.4/kolombos/byteio/parser/parser.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/partial_override.py` & `kolombos-1.5.4/kolombos/byteio/partial_override.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/reader.py` & `kolombos-1.5.4/kolombos/byteio/reader.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/segment/buffer.py` & `kolombos-1.5.4/kolombos/byteio/segment/buffer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/segment/chainable.py` & `kolombos-1.5.4/kolombos/byteio/segment/chainable.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/segment/printer.py` & `kolombos-1.5.4/kolombos/byteio/segment/printer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/segment/segment.py` & `kolombos-1.5.4/kolombos/byteio/segment/segment.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/segment/sequence_ref.py` & `kolombos-1.5.4/kolombos/byteio/segment/sequence_ref.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/__init__.py` & `kolombos-1.5.4/kolombos/byteio/template/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/registry.py` & `kolombos-1.5.4/kolombos/byteio/template/registry.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template.py` & `kolombos-1.5.4/kolombos/byteio/template/template.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_control.py` & `kolombos-1.5.4/kolombos/byteio/template/template_control.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_escape.py` & `kolombos-1.5.4/kolombos/byteio/template/template_escape.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_escape_sgr.py` & `kolombos-1.5.4/kolombos/byteio/template/template_escape_sgr.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_newline.py` & `kolombos-1.5.4/kolombos/byteio/template/template_newline.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_printable.py` & `kolombos-1.5.4/kolombos/byteio/template/template_printable.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/byteio/template/template_utf8.py` & `kolombos-1.5.4/kolombos/byteio/template/template_utf8.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/common.py` & `kolombos-1.5.4/kolombos/common.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/console.py` & `kolombos-1.5.4/kolombos/console.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/demo.bin` & `kolombos-1.5.4/kolombos/demo.bin`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/legend.ansi` & `kolombos-1.5.4/kolombos/legend.ansi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [1;92m    __         [34m__                __[m
 [1;92m   / /[92m__[94m____  / /___  ____ ___  / /_  ____ [93m _____[m
 [1;32m  / //_/[36m __ \/ / __ \[35m/ __ '__ \/ __ \/ __ \[33m/ ___/[m
 [1;94m / ,< [36m/ /_/ / / /_/ [35m/ / / / / / /_/ / /_/ [33m(__  )[m
 [1;34m/_/|_|[34m\____/_/\____/_/ /_/ /_/\.___/\____[33m/____/[m
-                                            [93mv1.5.3[m
+                                            [93mv1.5.4[m
 
 [97;1mCHARACTER CLASSES[m
   [90m<[m[1mS[m[90m>[m   ASCII whitespace chars   09-0d, 20      [90;1m-s -S[m
   [90m<[m[1mC[m[90m>[m   ASCII control chars      01-08, 0e-1f   [90;1m-c -C[m
   [90m<[m[1mP[m[90m>[m   ASCII printable chars    21-7e          [90;1m-p -P[m
   [90m<[m[1mI[m[90m>[m   binary data              80-ff          [90;1m-i -I[m
   [90m<[m[1mU[m[90m>[m   UTF-8 sequences          various        [90;1m-u -U[m
@@ -62,8 +62,8 @@
  [38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m
 
 [90mFor the best view your terminal should be [1m88[22m chars wide (or wider)[m
 
 [90mIs a part of [1;37mes7s[90m pack[m
 [90m(c) 2022—2023 A. Shavykin[m
 [90m<[94m0[90m.delameter@gmail.com>[m
-# Generated at 22-May-23 04:12
+# Generated at 22-May-23 04:18
```

### Comparing `kolombos-1.5.3/kolombos/runner/byteio.py` & `kolombos-1.5.4/kolombos/runner/byteio.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/runner/demo.py` & `kolombos-1.5.4/kolombos/runner/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         with resources.path('kolombos', self.DEMO_FILENAME) as path:
             aps = SettingsManager.app_settings
             aps.filename = path
             aps.set_default_read_mode(ReadMode.BINARY)
             if aps.decode is None:
                 aps.decode = True
             if aps.columns is None:
-                aps.columns = 32
+                aps.columns = 16  # @TODO auto-detection
             ByteIoRunner().run()
         Console.info("\nRun the app with '"+Spans.BOLD('--legend')+"' option to learn how to read the output")
```

### Comparing `kolombos-1.5.3/kolombos/runner/factory.py` & `kolombos-1.5.4/kolombos/runner/factory.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/runner/legend.py` & `kolombos-1.5.4/kolombos/runner/legend.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/runner/version.py` & `kolombos-1.5.4/kolombos/runner/version.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos/settings.py` & `kolombos-1.5.4/kolombos/settings.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/kolombos.egg-info/PKG-INFO` & `kolombos-1.5.4/kolombos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolombos
-Version: 1.5.3
+Version: 1.5.4
 Summary: CLI control characters and escape sequences viewer/visualizer
 Home-page: https://github.com/es7s/kolombos
 Author: Aleksandr Shavykin
 Author-email: 0.delameter@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -216,63 +216,57 @@
 
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
+### v1.5.4
+- FIX: reverted default column amount in `--demo` mode
 
-### v1.5.2
+### v1.5.3
+- FIX: errors while processing SGR with subparams (e.g. `4:3;`)
 
+### v1.5.2
 - UPDATE: icon redraw
 
-
 ### v1.5.1
-
 - FIX: packaging assets
 
-
 ### v1.5
 - NEW: `--demo` mode
 
-
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
 
 ### v1.4
 - REFACTOR: base colors
 - REFACTOR: extended legend 
 - DOCS:  update README and screenshots 
 
-
 ### v1.3
 - Swap -D and -d (debug/decode)
 - Make '--marker 0' default (was 1)
 - Update legend
 - Upgrade `pytermor` to 2.1
 
 ### v1.2.1
-
 - Minor update.
 
 ### v1.2
-
 - Separators additional styling.
 - Separators auto-hide from `-m0`.
 - `--no-sep[arators]` launch option.
 - `run` dev script for quick launch of repo versions.
 - Updated output format of SGR color prefixes.
 - SGR labels are now getting colored instead of marker details (if `-m0` is set).
 - Updated legend.
 
 ### v1.1
-
 - Additional separators around escape seqs (in text mode) for better readability.
 
 ### v1.0.2
-
 - Added logos.
 - Fixed pipy README images.
 
 ### v1.0.1
-
 - First public version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolombos Version: 1.5.3 Summary: CLI control
+Metadata-Version: 2.1 Name: kolombos Version: 1.5.4 Summary: CLI control
 characters and escape sequences viewer/visualizer Home-page: https://
 github.com/es7s/kolombos Author: Aleksandr Shavykin Author-email:
 0.delameter@gmail.com Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Terminals Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -157,19 +157,21 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
-### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
-### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
-README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
-marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
-v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
-auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
-for quick launch of repo versions. - Updated output format of SGR color
-prefixes. - SGR labels are now getting colored instead of marker details (if `-
-m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
-seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
-pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.4 - FIX: reverted default column amount in `--demo` mode ###
+v1.5.3 - FIX: errors while processing SGR with subparams (e.g. `4:3;`) ###
+v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets ### v1.5 - NEW:
+`--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1 ### v1.4 -
+REFACTOR: base colors - REFACTOR: extended legend - DOCS: update README and
+screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--marker 0'
+default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ### v1.2.1 - Minor
+update. ### v1.2 - Separators additional styling. - Separators auto-hide from
+`-m0`. - `--no-sep[arators]` launch option. - `run` dev script for quick launch
+of repo versions. - Updated output format of SGR color prefixes. - SGR labels
+are now getting colored instead of marker details (if `-m0` is set). - Updated
+legend. ### v1.1 - Additional separators around escape seqs (in text mode) for
+better readability. ### v1.0.2 - Added logos. - Fixed pipy README images. ###
+v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.3/kolombos.egg-info/SOURCES.txt` & `kolombos-1.5.4/kolombos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/__init__.py` & `kolombos-1.5.4/pytermor/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/ansi.py` & `kolombos-1.5.4/pytermor/ansi.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/color.py` & `kolombos-1.5.4/pytermor/color.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/common.py` & `kolombos-1.5.4/pytermor/common.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/render.py` & `kolombos-1.5.4/pytermor/render.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/__init__.py` & `kolombos-1.5.4/pytermor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/auto_float.py` & `kolombos-1.5.4/pytermor/util/auto_float.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/prefixed_unit.py` & `kolombos-1.5.4/pytermor/util/prefixed_unit.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/stdlib_ext.py` & `kolombos-1.5.4/pytermor/util/stdlib_ext.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/string_filter.py` & `kolombos-1.5.4/pytermor/util/string_filter.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/pytermor/util/time_delta.py` & `kolombos-1.5.4/pytermor/util/time_delta.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.3/setup.cfg` & `kolombos-1.5.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kolombos
-version = 1.5.3
+version = 1.5.4
 author = Aleksandr Shavykin
 author_email = 0.delameter@gmail.com
 description = CLI control characters and escape sequences viewer/visualizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/es7s/kolombos
 project_urls =
```

