# Comparing `tmp/carchive-0.0.58.tar.gz` & `tmp/carchive-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.58.tar", last modified: Tue May  9 03:16:52 2023, max compression
+gzip compressed data, was "carchive-0.0.59.tar", last modified: Mon May 22 11:57:32 2023, max compression
```

## Comparing `carchive-0.0.58.tar` & `carchive-0.0.59.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.044066 carchive-0.0.58/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-09 03:16:45.000000 carchive-0.0.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 03:16:52.044066 carchive-0.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 03:16:45.000000 carchive-0.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.040065 carchive-0.0.58/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10290 2023-05-09 03:16:45.000000 carchive-0.0.58/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.044066 carchive-0.0.58/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:16:52.044066 carchive-0.0.58/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-09 03:16:45.000000 carchive-0.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 11:57:25.000000 carchive-0.0.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 11:57:32.196610 carchive-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 11:57:25.000000 carchive-0.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10290 2023-05-22 11:57:25.000000 carchive-0.0.59/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:57:32.196610 carchive-0.0.59/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 11:57:32.000000 carchive-0.0.59/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:57:32.196610 carchive-0.0.59/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3358 2023-05-22 11:57:25.000000 carchive-0.0.59/setup.py
```

### Comparing `carchive-0.0.58/LICENSE` & `carchive-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.58/carchive/__init__.py` & `carchive-0.0.59/carchive/__init__.py`

 * *Files identical despite different names*

### Comparing `carchive-0.0.58/setup.py` & `carchive-0.0.59/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.58"
+VERSION = "0.0.59"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -103,15 +103,15 @@
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
 		"PyGithub", 
 		#"git2net @ git+ssh://git@github.com/franceme/git2net/tarball/master@0ca0ce7db9c3a616096a250c9412a8780dd30768",
-		"git2net@git+http://github.com/franceme/git2net",
+		"git4net",
 		"splittr",
 		"waybackpy",
 		"mystring",
 		"pygit2",
 		"pause",
 	],
 	include_package_data=True,
```

