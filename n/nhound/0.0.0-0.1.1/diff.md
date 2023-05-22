# Comparing `tmp/nhound-0.0.0.tar.gz` & `tmp/nhound-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhound-0.0.0.tar", max compression
+gzip compressed data, was "nhound-0.1.1.tar", max compression
```

## Comparing `nhound-0.0.0.tar` & `nhound-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-05-22 13:46:14.119618 nhound-0.0.0/LICENSE
--rw-r--r--   0        0        0     2864 2023-05-22 13:46:14.119618 nhound-0.0.0/README.md
--rw-r--r--   0        0        0    25790 2023-05-22 13:46:14.119618 nhound-0.0.0/docs/assets/logo.png
--rw-r--r--   0        0        0      352 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/__init__.py
--rw-r--r--   0        0        0     3419 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/cohort.py
--rw-r--r--   0        0        0    11235 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/console.py
--rw-r--r--   0        0        0     1344 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/dehumanize.py
--rw-r--r--   0        0        0     2239 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/email.py
--rw-r--r--   0        0        0     7863 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/inotion.py
--rw-r--r--   0        0        0     1154 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/user.py
--rw-r--r--   0        0        0     2928 2023-05-22 13:46:14.119618 nhound-0.0.0/nhound/utils.py
--rw-r--r--   0        0        0     5701 2023-05-22 13:46:14.123618 nhound-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 nhound-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-22 15:39:43.795055 nhound-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2864 2023-05-22 15:39:43.795055 nhound-0.1.1/README.md
+-rw-r--r--   0        0        0    25790 2023-05-22 15:39:43.795055 nhound-0.1.1/docs/assets/logo.png
+-rw-r--r--   0        0        0      352 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/__init__.py
+-rw-r--r--   0        0        0     3419 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/cohort.py
+-rw-r--r--   0        0        0    11235 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/console.py
+-rw-r--r--   0        0        0     1344 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/dehumanize.py
+-rw-r--r--   0        0        0     2239 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/email.py
+-rw-r--r--   0        0        0     8030 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/inotion.py
+-rw-r--r--   0        0        0     1154 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/user.py
+-rw-r--r--   0        0        0     2928 2023-05-22 15:39:43.795055 nhound-0.1.1/nhound/utils.py
+-rw-r--r--   0        0        0     5701 2023-05-22 15:40:21.299547 nhound-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 nhound-0.1.1/PKG-INFO
```

### Comparing `nhound-0.0.0/LICENSE` & `nhound-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/README.md` & `nhound-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/docs/assets/logo.png` & `nhound-0.1.1/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/cohort.py` & `nhound-0.1.1/nhound/cohort.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/console.py` & `nhound-0.1.1/nhound/console.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/dehumanize.py` & `nhound-0.1.1/nhound/dehumanize.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/email.py` & `nhound-0.1.1/nhound/email.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/inotion.py` & `nhound-0.1.1/nhound/inotion.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         """Analyse any callout block."""
         users: list[User] = []
         threashold = NOW.subtract(weeks=self._nhound_default_threashold)
         for block in blocks:
             if block["type"] == "callout":
                 for item in block["callout"]["rich_text"]:
                     if item["type"] == "mention":
+                        if "user" not in item["mention"]:
+                            rlog.debug("No user in callout", item=item)
+                            continue
                         usr = self._cohort.get_by_uuid(item["mention"]["user"]["id"])
                         if usr is not None:
                             users.append(usr)
                         rlog.debug("Found callout user", user=usr)
                     if item["type"] == "text":
                         try:
                             # This will overwirght the standard threashold.
```

### Comparing `nhound-0.0.0/nhound/user.py` & `nhound-0.1.1/nhound/user.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/nhound/utils.py` & `nhound-0.1.1/nhound/utils.py`

 * *Files identical despite different names*

### Comparing `nhound-0.0.0/pyproject.toml` & `nhound-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhound"
-version = "0.0.0"
+version = "0.1.1"
 description = "Notion hound, as in nagging you to keep content up to date."
 authors = ["Dr Yann Golanski <ygg@worldr.com>"]
 keywords = ["worldr"]
 license = "MIT"
 homepage = "https://github.com/worldr/nhound"
 repository = "https://github.com/worldr/nhound"
 readme = "README.md"
```

### Comparing `nhound-0.0.0/PKG-INFO` & `nhound-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhound
-Version: 0.0.0
+Version: 0.1.1
 Summary: Notion hound, as in nagging you to keep content up to date.
 Home-page: https://github.com/worldr/nhound
 License: MIT
 Keywords: worldr
 Author: Dr Yann Golanski
 Author-email: ygg@worldr.com
 Requires-Python: >=3.9,<3.12
```

