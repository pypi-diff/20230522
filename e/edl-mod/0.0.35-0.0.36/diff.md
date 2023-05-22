# Comparing `tmp/edl-mod-0.0.35.tar.gz` & `tmp/edl-mod-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpypxr1mwf/edl-mod-0.0.35.tar", last modified: Sat May 20 03:47:41 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpxdj_r_r7/edl-mod-0.0.36.tar", last modified: Mon May 22 14:13:31 2023, max compression
```

## Comparing `edl-mod-0.0.35.tar` & `edl-mod-0.0.36.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:47:41.000000 edl-mod-0.0.35/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.35/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46639 2023-05-20 03:46:26.000000 edl-mod-0.0.35/edl.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-20 03:47:41.000000 edl-mod-0.0.35/edl_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.35/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.35/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.35/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-20 03:47:41.000000 edl-mod-0.0.35/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-20 03:47:41.000000 edl-mod-0.0.35/setup.cfg
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:13:31.000000 edl-mod-0.0.36/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.36/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    47219 2023-05-22 14:12:21.000000 edl-mod-0.0.36/edl.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:13:31.000000 edl-mod-0.0.36/edl_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.36/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.36/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.36/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-22 14:13:31.000000 edl-mod-0.0.36/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-22 14:13:31.000000 edl-mod-0.0.36/setup.cfg
```

### Comparing `edl-mod-0.0.35/edl.py` & `edl-mod-0.0.36/edl.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 # Explicit No Prompt
 NoPrompt=False
 
 # Autosave EDLFIle
 AutoSave=False
 
 # Version
-VERSION=(0,0,35)
+VERSION=(0,0,36)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
 # Config File
 __Config__ = "/etc/edl/config"
@@ -995,15 +995,15 @@
 # Append TO EDL
 def AppendToEDL(entry,masterfile=None,edlfile=None):
 	"""
 	Append new entry to the EDL
 	"""
 	global EDLMaster, Columns, AutoSave, NoIPv6, AuditFile
 
-	DbgMsg("Entering AppendToEDL")
+	DbgMsg("Entering edl::AppendToEDL",dbglabel="edl")
 
 	if masterfile == None: masterfile = EDLMaster
 
 	success = True
 
 	if type(entry) is EDLEntry:
 		pass
@@ -1028,20 +1028,24 @@
 		if AuditFile: Audit("Appended {} to edl master".format(entry.GetRow()))
 
 		if AutoSave: Save(edlfile,masterfile)
 	else:
 		DbgMsg(f"Rejected {ip}, NoIPv6 = {NoIPv6}")
 		success = False
 
+	DbgMsg("Exiting edl::AppendToEDL",dbglabel="edl")
+
 	return success
 
 # Add EntryEntry
 def AddEDLEntry(entry,masterfile=None,edlfile=None):
 	"""Add Filled In EDLEntry To EDL"""
 
+	DbgMsg("Entering edl::AddEDLEntry",dbglabel="edl")
+
 	existing = False
 	excluded = False
 	success = True
 
 	if entry != None:
 		if not Excluded(entry.IP()):
 			found = FindEntry(entry.IP(),masterfile)
@@ -1055,22 +1059,26 @@
 				existing = True
 		else:
 			exclude = True
 			success = False
 	else:
 		success = False
 
+	DbgMsg("Exiting edl::AddEDLEntry",dbglabel="edl")
+
 	return (success,excluded,existing)
 
 # Add IP (or list of IPs, or DNS Names) To EDL Master
 def Add(host,user=None,timestamp=None,owner=None,abuse=None,comment=None,protect=False,nosleep=False,masterfile=None,edlfile=None):
 	"""Add Host/List of Hosts/Subnets/List of subnets/DNS names to EDL Master"""
 
 	global LastAdd, Responses, EDLRowTemplate
 
+	DbgMsg("Entering edl::Add",dbglabel="edl")
+
 	if user == None:
 		user = getpass.getuser()
 
 	if timestamp == None:
 		timestamp = datetime.now()
 	elif type(timestamp) == str:
 		old_timestamp,timestamp = Timestamp(timestamp)
@@ -1118,14 +1126,17 @@
 			"exists" : False,
 			"entry" : None,
 			"excluded" : False,
 			"edl_entry" : None
 			}
 
 		if not Excluded(host):
+			DbgMsg(f"edl::Add - {host} is not excluded",dbglabel="edl")
+			if ph.IsDebugEnabled("edl-breakpoint"): breakpoint()
+
 			found = FindEntry(host)
 
 			if found == None:
 				if owner == None or abuse == None:
 					entry.GetWhois()
 
 				AppendToEDL(entry,masterfile=masterfile,edlfile=edlfile)
@@ -1136,20 +1147,26 @@
 				# Exists
 				result["exists"] = True
 				result["entry"] = found.GetRow()
 				result["edl_entry"] = found
 				results.append(tuple(result.values()))
 		else:
 			# Excluded
+
+			DbgMsg(f"edl::Add - {host} excluded",dbglabel="edl")
+			if ph.IsDebugEnabled("edl-breakpoint"): breakpoint()
+
 			results["excluded"] = True
 			results.append(tuple(entry.values()))
 
 		if len(hosts) > 1 and not nosleep:
 			time.sleep(4)
 
+	DbgMsg("Exiting edl::Add",dbglabel="edl")
+
 	return results
 
 # Bulk Add
 def BulkAdd(fname,user=None,timestamp=None,owner=None,abuse=None,comment=None,protect=False,masterfile=None,edlfile=None):
 	"""
 	Bulk add file of IP address to EDL. The file should be on IP per line.
 	"""
@@ -1391,14 +1408,15 @@
 	return success
 
 # Remove Excluded IP/Range
 def RemoveExclude(item,exclude_file=None):
 	"""
 	Remove the given IP or subnet from the excludes list
 	"""
+
 	global Excludes
 
 	if exclude_file == None: exclude_file = Excludes
 
 	success = False
 
 	tmp = TmpFilename()
@@ -1743,14 +1761,16 @@
 	if args == None:
 		# Parse 'dem args my brother
 		if arguments != None:
 			args,unknowns = ParseArgs(arguments)
 		else:
 			args,unknowns = ParseArgs()
 
+	DbgMsg("Entering run",dbglabel="edl")
+
 	#
 	# Now Check for actions
 	#
 
 	results = None
 	success = True
 
@@ -1872,14 +1892,16 @@
 		Dump(Excludes)
 	elif op in [ "checkexcludes", "chex", "checkex", "checkx" ]:
 		if SearchExclude(args.exclude):
 			Msg("Is in exclude list")
 		else:
 			Msg("Not in exclude list")
 
+	DbgMsg("Exiting run",dbglabel="edl")
+
 	return results
 
 #
 # Initialization
 #
 
 # Initialize Module
```

### Comparing `edl-mod-0.0.35/edl_mod.egg-info/PKG-INFO` & `edl-mod-0.0.36/edl_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.35
+Version: 0.0.36
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.35/LICENSE` & `edl-mod-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `edl-mod-0.0.35/PKG-INFO` & `edl-mod-0.0.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.35
+Version: 0.0.36
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.35/setup.cfg` & `edl-mod-0.0.36/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = edl-mod
-version = 0.0.35
+version = 0.0.36
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Module for editting and searching external dynamic lists (EDLs)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/edl
 project_urls =
```

