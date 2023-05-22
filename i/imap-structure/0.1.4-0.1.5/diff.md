# Comparing `tmp/imap_structure-0.1.4.tar.gz` & `tmp/imap_structure-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_structure-0.1.4.tar", max compression
+gzip compressed data, was "imap_structure-0.1.5.tar", max compression
```

## Comparing `imap_structure-0.1.4.tar` & `imap_structure-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.4/imap_structure/__init__.py
--rw-r--r--   0        0        0    10793 2023-05-18 04:21:04.349483 imap_structure-0.1.4/imap_structure/body_structure.py
--rw-r--r--   0        0        0     5032 2023-05-18 05:31:45.507524 imap_structure-0.1.4/imap_structure/metadata.py
--rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.4/imap_structure/parser.py
--rw-r--r--   0        0        0      540 2023-05-18 05:32:14.067512 imap_structure-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.4/setup.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.5/imap_structure/__init__.py
+-rw-r--r--   0        0        0    10965 2023-05-22 07:56:02.884600 imap_structure-0.1.5/imap_structure/body_structure.py
+-rw-r--r--   0        0        0     5084 2023-05-18 08:39:35.872324 imap_structure-0.1.5/imap_structure/metadata.py
+-rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.5/imap_structure/parser.py
+-rw-r--r--   0        0        0      540 2023-05-22 07:56:19.594593 imap_structure-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.5/setup.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.5/PKG-INFO
```

### Comparing `imap_structure-0.1.4/imap_structure/body_structure.py` & `imap_structure-0.1.5/imap_structure/body_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from email import _header_value_parser as parser
 from functools import cached_property
 from typing import NamedTuple, Optional
 
 from pyparsing import (
     Literal,
     ParseResults,
     Word,
@@ -112,15 +113,16 @@
             disposition = part.body_disposition.as_list()
             if "attachment" not in disposition:
                 continue
             if len(disposition) > 1 and isinstance(disposition[1], list):
                 filename_idx = disposition[1].index("filename")
                 if len(disposition[1]) > filename_idx + 1:
                     filename = disposition[1][filename_idx + 1]
-                    yield filename
+                    # Should be parse_content_disposition_header but we use get_unstructured
+                    yield str(parser.get_unstructured(filename))
 
     @cached_property
     def has_attachment(self) -> bool:
         return any(
             isinstance(part, BodyPartNonMultipart)
             and part.body_disposition is not None
             and "attachment" in part.body_disposition.as_list()
```

### Comparing `imap_structure-0.1.4/imap_structure/metadata.py` & `imap_structure-0.1.5/imap_structure/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     # https://datatracker.ietf.org/doc/html/rfc9051#IMAP-ABNF
     if isinstance(uid_set, int) or isinstance(uid_set, str):
         uid_set = f"({uid_set})"
     elif isinstance(uid_set, collections.abc.Sequence):
         assert not isinstance(
             uid_set, str
         )  # We don't want to get a string like "(1,2,3)"
+        if len(uid_set) == 0:
+            return []
         message_set_inner = ",".join(str(x) for x in uid_set)
         uid_set = f"({message_set_inner})"
 
     result, response = mail.uid("fetch", uid_set, METADATA_MESSAGE_PARTS)
     if result != "OK":
         logger.error(response)
         raise mail.error("Failed to fetch metadata")
```

### Comparing `imap_structure-0.1.4/imap_structure/parser.py` & `imap_structure-0.1.5/imap_structure/parser.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.4/pyproject.toml` & `imap_structure-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imap-structure"
-version = "0.1.4"
+version = "0.1.5"
 description = "IMAP BODYSTRUCTURE parser"
 authors = ["Kiruya Momochi <65301509+kiruyamomochi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "imap_structure" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `imap_structure-0.1.4/setup.py` & `imap_structure-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyparsing>=3.0.9,<4.0.0']
 
 setup_kwargs = {
     'name': 'imap-structure',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'IMAP BODYSTRUCTURE parser',
     'long_description': '# imap-structure\n\nIMAP BODYSTRUCTURE parser\n',
     'author': 'Kiruya Momochi',
     'author_email': '65301509+kiruyamomochi@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

