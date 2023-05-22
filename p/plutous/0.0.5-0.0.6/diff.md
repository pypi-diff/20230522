# Comparing `tmp/plutous-0.0.5.tar.gz` & `tmp/plutous-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.5.tar", max compression
+gzip compressed data, was "plutous-0.0.6.tar", max compression
```

## Comparing `plutous-0.0.5.tar` & `plutous-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.5/LICENSE
--rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.5/README.md
--rw-r--r--   0        0        0       87 2023-05-10 18:54:52.571344 plutous-0.0.5/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.5/plutous/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.5/plutous/cli/main.py
--rw-r--r--   0        0        0      728 2023-05-10 18:50:45.463672 plutous-0.0.5/plutous/config.py
--rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.5/plutous/database.py
--rw-r--r--   0        0        0      668 2023-05-10 18:54:57.059701 plutous-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 plutous-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.6/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-16 15:20:39.229066 plutous-0.0.6/README.md
+-rw-r--r--   0        0        0       87 2023-05-22 19:30:14.563811 plutous-0.0.6/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:50:41.766051 plutous-0.0.6/plutous/app/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-22 10:47:17.974453 plutous-0.0.6/plutous/app/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:16:48.809093 plutous-0.0.6/plutous/app/utils/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-16 16:17:49.462926 plutous-0.0.6/plutous/app/utils/session.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.6/plutous/cli/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-22 13:46:32.044605 plutous-0.0.6/plutous/cli/main.py
+-rw-r--r--   0        0        0      756 2023-05-22 11:46:04.769603 plutous-0.0.6/plutous/config.py
+-rw-r--r--   0        0        0     2415 2023-05-22 19:03:40.598523 plutous-0.0.6/plutous/database.py
+-rw-r--r--   0        0        0       30 2023-05-22 15:46:16.955532 plutous-0.0.6/plutous/enums/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-16 18:27:41.692272 plutous-0.0.6/plutous/enums/exchange.py
+-rw-r--r--   0        0        0       27 2023-05-16 12:50:11.352964 plutous-0.0.6/plutous/models/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-22 15:47:35.887122 plutous-0.0.6/plutous/models/base.py
+-rw-r--r--   0        0        0      813 2023-05-22 19:30:19.196256 plutous-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 plutous-0.0.6/PKG-INFO
```

### Comparing `plutous-0.0.5/LICENSE` & `plutous-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.5/plutous/config.py` & `plutous-0.0.6/plutous/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,18 @@
                 data = data.get(key, {})
         return cls(**data)
 
 
 class Db(BaseModel):
     host: str
     port: int
-    user: str
+    username: str
     password: str
     database: str
 
 
 class Config(BaseConfig):
     db: Db
+    encryption_key: str
 
 
 config = Config.from_file()
```

### Comparing `plutous-0.0.5/pyproject.toml` & `plutous-0.0.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous"
-version = "0.0.5"
+version = "0.0.6"
 description = "Plutous Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
@@ -12,17 +12,24 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 SQLAlchemy = ">=2.0.12"
+sqlalchemy_utils=">=0.41.1"
 typer = ">=0.9.0"
 alembic = ">=1.10.4"
 pydantic = ">=1.10.7"
+fastapi = ">=0.95.1"
+psycopg2 = ">=2.9.6"
+loguru = ">=0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+plutous = "plutous.cli.main:app"
```

