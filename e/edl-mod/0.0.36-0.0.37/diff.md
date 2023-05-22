# Comparing `tmp/edl-mod-0.0.36.tar.gz` & `tmp/edl-mod-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpxdj_r_r7/edl-mod-0.0.36.tar", last modified: Mon May 22 14:13:31 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpt6szdi4v/edl-mod-0.0.37.tar", last modified: Mon May 22 14:24:07 2023, max compression
```

## Comparing `edl-mod-0.0.36.tar` & `edl-mod-0.0.37.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:13:31.000000 edl-mod-0.0.36/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.36/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    47219 2023-05-22 14:12:21.000000 edl-mod-0.0.36/edl.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.36/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.36/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.36/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:13:31.000000 edl-mod-0.0.36/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-22 14:13:31.000000 edl-mod-0.0.36/setup.cfg
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:24:07.000000 edl-mod-0.0.37/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.37/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46984 2023-05-22 14:22:57.000000 edl-mod-0.0.37/edl.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:24:07.000000 edl-mod-0.0.37/edl_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.37/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.37/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.37/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:24:07.000000 edl-mod-0.0.37/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-22 14:24:07.000000 edl-mod-0.0.37/setup.cfg
```

### Comparing `edl-mod-0.0.36/edl.py` & `edl-mod-0.0.37/edl.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 # Explicit No Prompt
 NoPrompt=False
 
 # Autosave EDLFIle
 AutoSave=False
 
 # Version
-VERSION=(0,0,36)
+VERSION=(0,0,37)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
 # Config File
 __Config__ = "/etc/edl/config"
@@ -1126,17 +1126,14 @@
 			"exists" : False,
 			"entry" : None,
 			"excluded" : False,
 			"edl_entry" : None
 			}
 
 		if not Excluded(host):
-			DbgMsg(f"edl::Add - {host} is not excluded",dbglabel="edl")
-			if ph.IsDebugEnabled("edl-breakpoint"): breakpoint()
-
 			found = FindEntry(host)
 
 			if found == None:
 				if owner == None or abuse == None:
 					entry.GetWhois()
 
 				AppendToEDL(entry,masterfile=masterfile,edlfile=edlfile)
@@ -1147,19 +1144,15 @@
 				# Exists
 				result["exists"] = True
 				result["entry"] = found.GetRow()
 				result["edl_entry"] = found
 				results.append(tuple(result.values()))
 		else:
 			# Excluded
-
-			DbgMsg(f"edl::Add - {host} excluded",dbglabel="edl")
-			if ph.IsDebugEnabled("edl-breakpoint"): breakpoint()
-
-			results["excluded"] = True
+			result["excluded"] = True
 			results.append(tuple(entry.values()))
 
 		if len(hosts) > 1 and not nosleep:
 			time.sleep(4)
 
 	DbgMsg("Exiting edl::Add",dbglabel="edl")
```

### Comparing `edl-mod-0.0.36/edl_mod.egg-info/PKG-INFO` & `edl-mod-0.0.37/edl_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.36
+Version: 0.0.37
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.36/LICENSE` & `edl-mod-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `edl-mod-0.0.36/PKG-INFO` & `edl-mod-0.0.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.36
+Version: 0.0.37
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.36/setup.cfg` & `edl-mod-0.0.37/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = edl-mod
-version = 0.0.36
+version = 0.0.37
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Module for editting and searching external dynamic lists (EDLs)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/edl
 project_urls =
```

