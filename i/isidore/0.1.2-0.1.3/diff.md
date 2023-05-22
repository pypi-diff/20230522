# Comparing `tmp/isidore-0.1.2.tar.gz` & `tmp/isidore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-n02w3bb_/isidore-0.1.2.tar", last modified: Fri May 12 16:01:36 2023, max compression
+gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-gjmd_icc/isidore-0.1.3.tar", last modified: Mon May 22 18:47:57 2023, max compression
```

## Comparing `isidore-0.1.2.tar` & `isidore-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-12 16:01:36.000000 isidore-0.1.2/
--rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.2/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1001 2023-05-12 16:01:36.000000 isidore-0.1.2/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      244 2023-05-12 12:18:21.000000 isidore-0.1.2/README.md
--rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-12 15:59:07.000000 isidore-0.1.2/pyproject.toml
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-12 16:01:36.000000 isidore-0.1.2/setup.cfg
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-12 16:01:36.000000 isidore-0.1.2/src/
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore/
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.2/src/isidore/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)    29490 2023-05-12 15:59:07.000000 isidore-0.1.2/src/isidore/libIsidore.py
--rw-r--r--   0 scott     (1000) scott     (1000)    33265 2023-05-12 15:59:07.000000 isidore-0.1.2/src/isidore/libIsidoreCmdline.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1001 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/requires.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-12 16:01:36.000000 isidore-0.1.2/src/isidore.egg-info/top_level.txt
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.3/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-22 18:47:57.000000 isidore-0.1.3/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      245 2023-05-12 17:10:25.000000 isidore-0.1.3/README.md
+-rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-22 18:47:38.000000 isidore-0.1.3/pyproject.toml
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-22 18:47:57.000000 isidore-0.1.3/setup.cfg
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore/
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.3/src/isidore/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    32541 2023-05-22 18:47:38.000000 isidore-0.1.3/src/isidore/libIsidore.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    37498 2023-05-22 18:47:38.000000 isidore-0.1.3/src/isidore/libIsidoreCmdline.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/requires.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/top_level.txt
```

### Comparing `isidore-0.1.2/LICENSE` & `isidore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isidore-0.1.2/PKG-INFO` & `isidore-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.2
+Version: 0.1.3
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
@@ -16,11 +16,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Isidore
 =======
 
 Isidore is a database, API, and CLI for managing Ansible inventories. It allows
-for a flexible tag base classification approach to group management.
+for a flexible tag based classification approach to group management.
 
 Website: [https://github.com/Z5T1/isidore](https://github.com/Z5T1/isidore)
```

### Comparing `isidore-0.1.2/pyproject.toml` & `isidore-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "isidore"
-version = "0.1.2"
+version = "0.1.3"
 keywords = [ "ansible", "inventory", "database", "isidore" ]
 authors = [
   { name="Scott Court", email="Z5T1@Z5T1.com" },
 ]
 description = "database, API, and CLI suite for managing Ansible inventories"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `isidore-0.1.2/src/isidore/libIsidore.py` & `isidore-0.1.3/src/isidore/libIsidore.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import yaml
 import json
 
 # Represents an Isidore database instance
 class Isidore:
 
     _conn = None
-    _version = '0.1.2'
+    _version = '0.1.3'
 
     # Connects to a MySQL database and creates a new Isidore object to interact
     # with it.
     # @param user       The MySQL username
     # @param password   The password for the MySQL user
     # @param host       The MySQL server to connect to
     # @param database   The name of the database to use
@@ -448,14 +448,42 @@
     def addTag(self, tag):
         cursor = self._isidore._conn.cursor()
         stmt = "INSERT INTO HostHasTag (HostID, TagID) VALUES (%s, %s)"
         cursor.execute(stmt, [ self._hostId, tag.getTagId() ])
         self._isidore._conn.commit()
         cursor.close()
 
+    # Appends an item to a list variable
+    # @param path       The path of the list to append to.
+    # @param value      The value to append to the list. This can
+    #                   be of any type that is JSON serializable.
+    def appendVar(self, path, value):
+        # Ensure the path starts with $
+        if path[0] != '$':
+            path = '$.' + path
+
+        # Set the variable
+        stmt = '''
+            UPDATE Host
+            SET Variables =
+                JSON_ARRAY_APPEND(
+                    (SELECT Variables FROM Host WHERE HostId = %s),
+                    %s,
+                    JSON_EXTRACT(%s, '$')
+                )
+            WHERE HostID = %s'''
+        cursor = self._isidore._conn.cursor()
+        cursor.execute(stmt, [
+            self._hostId,
+            path,
+            json.dumps(value),
+            self._hostId])
+        self._isidore._conn.commit()
+        cursor.close()
+
     # Deletes this host from the database. The host object should
     # not be referenced after this method is called.
     def delete(self):
         # Delete the host
         cursor = self._isidore._conn.cursor()
         stmt = "DELETE FROM Host WHERE HostID = %s"
         cursor.execute(stmt, [ self._hostId ])
@@ -665,14 +693,35 @@
                 )
             WHERE HostID = %s'''
         cursor = self._isidore._conn.cursor()
         cursor.execute(stmt, [path, json.dumps(value), self._hostId])
         self._isidore._conn.commit()
         cursor.close()
 
+    # Unsets a variable.
+    # @param path       The path of the variable to unset.
+    def unsetVar(self, path):
+        # Ensure the path starts with $
+        if path[0] != '$':
+            path = '$.' + path
+
+        # Set the variable
+        stmt = '''
+            UPDATE Host
+            SET Variables =
+                JSON_REMOVE(
+                    Variables,
+                    %s
+                )
+            WHERE HostID = %s'''
+        cursor = self._isidore._conn.cursor()
+        cursor.execute(stmt, [path, self._hostId])
+        self._isidore._conn.commit()
+        cursor.close()
+
 # An individual tag
 class Tag:
     
     _tagId = None
     _name = None
     _group = None
     _description = None
@@ -688,14 +737,42 @@
             isidore=None):
         self._tagId = tagId
         self._name = name
         self._group = group
         self._description = description
         self._isidore = isidore
 
+    # Appends an item to a list variable
+    # @param path       The path of the list to append to.
+    # @param value      The value to append to the list. This can
+    #                   be of any type that is JSON serializable.
+    def appendVar(self, path, value):
+        # Ensure the path starts with $
+        if path[0] != '$':
+            path = '$.' + path
+
+        # Set the variable
+        stmt = '''
+            UPDATE Tag
+            SET Variables =
+                JSON_ARRAY_APPEND(
+                    (SELECT Variables FROM Tag WHERE TagID = %s),
+                    %s,
+                    JSON_EXTRACT(%s, '$')
+                )
+            WHERE TagID = %s'''
+        cursor = self._isidore._conn.cursor()
+        cursor.execute(stmt, [
+            self._tagId,
+            path,
+            json.dumps(value),
+            self._tagId])
+        self._isidore._conn.commit()
+        cursor.close()
+
     # Deletes this tag from the database. The tag object should
     # not be referenced after this method is called.
     def delete(self):
         # Delete the tag
         cursor = self._isidore._conn.cursor()
         stmt = "DELETE FROM Tag WHERE TagID = %s"
         cursor.execute(stmt, [ self._tagId ])
@@ -863,7 +940,28 @@
                 )
             WHERE TagID = %s'''
         cursor = self._isidore._conn.cursor()
         cursor.execute(stmt, [path, json.dumps(value), self._tagId])
         self._isidore._conn.commit()
         cursor.close()
 
+    # Unsets a variable.
+    # @param path       The path of the variable to unset.
+    def unsetVar(self, path):
+        # Ensure the path starts with $
+        if path[0] != '$':
+            path = '$.' + path
+
+        # Set the variable
+        stmt = '''
+            UPDATE Tag
+            SET Variables =
+                JSON_REMOVE(
+                    Variables,
+                    %s
+                )
+            WHERE TagID = %s'''
+        cursor = self._isidore._conn.cursor()
+        cursor.execute(stmt, [path, self._tagId])
+        self._isidore._conn.commit()
+        cursor.close()
+
```

### Comparing `isidore-0.1.2/src/isidore/libIsidoreCmdline.py` & `isidore-0.1.3/src/isidore/libIsidoreCmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from isidore.libIsidore import *
 
 # The Isidore command prompt
 class IsidoreCmdline:
 
     _isidore = None
-    _version = '0.1.2'
+    _version = '0.1.3'
 
     # Creates a new Isidore command prompt
     # @param isidore    The underlying Isidore instance for the command prompt
     #                   to connect to.
     def __init__(self, isidore):
         self._isidore = isidore
 
@@ -196,22 +196,25 @@
             print("host "+name+" var set $ '"+\
                     json.dumps(host.getVar()).replace("'", "'\"'\"'")+"'")
         print()
 
         # Create Tags
         for tag in tags:
             name = "'"+tag.getName().replace("'", "'\"'\"'")+"'"
-            print("create tag "+name)
-            print("tag "+name+" set group '"+\
-                    str(tag.getGroup())+"'")
-            if tag.getDescription() == None:
-                print("tag "+name+" set description none")
-            else:
-                print("tag "+name+" set description '"+\
-                        str(tag.getDescription()).replace("'", "'\"'\"'")+"'")
+            group = tag.getGroup()
+            description = tag.getDescription()
+            print("create tag %s" % (name))
+            print("tag %s set group '%s'" %
+                    (name,
+                    'none' if group == None
+                        else group.replace("'", "'\"'\"'")))
+            print("tag %s set description '%s'" % 
+                    (name,
+                    'none' if description == None
+                        else description.replace("'", "'\"'\"'")))
             print("tag "+name+" var set $ '"+\
                     json.dumps(tag.getVar()).replace("'", "'\"'\"'")+"'")
         print()
 
         # Assign Tags to Hosts
         for host in hosts:
             hostname = "'"+host.getHostname().replace("'", "'\"'\"'")+"'"
@@ -296,14 +299,17 @@
         elif args[2] == '?':
             print('''\
 ?           print this help message
 <hostname>  the hostname for the new host to create''')
         else:
             try:
                 self._isidore.createHost(args[2])
+            except mysql.connector.errors.IntegrityError as e:
+                print('Host %s already exists' % args[2],
+                        file=sys.stderr)
             except:
                 print('Failed to create host '+args[2],
                         file=sys.stderr)
                 print(traceback.format_exc(),
                         file=sys.stderr)
 
     # > create tag
@@ -313,14 +319,17 @@
         elif args[2] == '?':
             print('''\
 ?           print this help message
 <name>      the name of the new tag to create''')
         else:
             try:
                 self._isidore.createTag(args[2])
+            except mysql.connector.errors.IntegrityError as e:
+                print('Tag %s already exists' % args[2],
+                        file=sys.stderr)
             except:
                 print('Failed to create tag '+args[2],
                         file=sys.stderr)
                 print(traceback.format_exc(),
                         file=sys.stderr)
 
     # > delete
@@ -490,14 +499,16 @@
         elif args[3] == 'commissioned':
             self.host_set_commissioned(args)
         elif args[3] == 'decommissioned':
             self.host_set_decommissioned(args)
         elif args[3] == 'description':
             if len(args) == 4:
                 print("<description>   the description")
+            elif args[4] == 'none':
+                host.setDescription(None)
             else:
                 host.setDescription(args[4])
         else:
             print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
     # > host <hostname> set commissioned
     def host_set_commissioned(self, args):
@@ -575,16 +586,21 @@
     def host_var(self, args):
         host = self._isidore.getHost(args[1])
         if len(args) == 3:
             self.subprompt(args, self.host_var)
         elif args[3] == '?':
             print('''\
 ?           print this help message
+append      append a value to a list variable
 print       print a variable
-set         set a variable''')
+set         set a variable
+unset       unset (delete) a variable''')
+
+        elif args[3] == 'append':
+            self.host_var_append(args)
 
         elif args[3] == 'print':
             if len(args) == 4:
                 print(yaml.dump(
                     host.getVar(),
                     default_flow_style=False,
                     sort_keys=False))
@@ -598,17 +614,59 @@
                     host.getVar(args[4]),
                     default_flow_style=False,
                     sort_keys=False))
 
         elif args[3] == 'set':
             self.host_var_set(args)
 
+        elif args[3] == 'unset':
+            self.host_var_unset(args)
+
         else:
             print('Invalid command '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
+    # > host <hostname> var append
+    def host_var_append(self, args):
+        host = self._isidore.getHost(args[1])
+        if len(args) == 4:
+            self.subprompt(args, self.host_var_append)
+        elif args[4] == '?':
+            print('''\
+?           print this help message
+<variable>  name of the list variable to append to''')
+
+        elif len(args) == 5:
+            self.subprompt(args, self.host_var_append)
+
+        elif args[5] == '?':
+            print('''\
+?           print this help message
+<json>      the JSON value to append to the list''')
+
+        else:
+            try:
+                host.appendVar(args[4], json.loads(args[5]))
+            except json.decoder.JSONDecodeError:
+                print(args[5] + '''
+^-- this is not valid JSON
+
+Strings must be double quoted. It will be necessary to either nest double
+quotes inside single quotes or escape the double quotes like so:
+
+   > host myhost var set foo '"bar"'
+
+or
+
+   > host myhost var set foo \\"bar\\"
+
+''')
+            except:
+                print(\
+'Failed to append to list variable. Is %s a valid list path?' % args[4])
+
     # > host <hostname> var set
     def host_var_set(self, args):
         host = self._isidore.getHost(args[1])
         if len(args) == 4:
             self.subprompt(args, self.host_var_set)
         elif args[4] == '?':
             print('''\
@@ -638,14 +696,29 @@
 
 or
 
    > host myhost var set foo \\"bar\\"
 
 ''')
 
+    # > host <hostname> var unset
+    def host_var_unset(self, args):
+        host = self._isidore.getHost(args[1])
+        if len(args) == 4:
+            self.subprompt(args, self.host_var_set)
+        elif args[4] == '?':
+            print('''\
+?           print this help message
+<variable>  name of the variable to unset''')
+        else:
+            try:
+                host.unsetVar(args[4])
+            except:
+                print("Failed to unset variable %s" % args[4])
+
     # > host <hostname> tag add
     def host_tag_add(self, args):
         host = self._isidore.getHost(args[1])
         if len(args) == 4:
             self.subprompt(args, self.host)
             return
         elif args[4] == '?':
@@ -915,14 +988,16 @@
 description     set the tag's description
 group           set the tag's group''')
         elif args[3] == 'group':
             self.tag_set_group(args)
         elif args[3] == 'description':
             if len(args) == 4:
                 print("<description>   the description")
+            elif args[4] == 'none':
+                tag.setDescription(None)
             else:
                 tag.setDescription(args[4])
         else:
             print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
     # > tag <tagname> set group
     def tag_set_group(self, args):
@@ -945,16 +1020,21 @@
     def tag_var(self, args):
         tag = self._isidore.getTag(args[1])
         if len(args) == 3:
             self.subprompt(args, self.tag_var)
         elif args[3] == '?':
             print('''\
 ?           print this help message
+append      append a value to a list variable
 print       print a variable
-set         set a variable''')
+set         set a variable
+unset       unset (delete) a variable''')
+
+        elif args[3] == 'append':
+            self.tag_var_append(args)
 
         elif args[3] == 'print':
             if len(args) == 4:
                 print(yaml.dump(
                     tag.getVar(),
                     default_flow_style=False,
                     sort_keys=False))
@@ -968,18 +1048,60 @@
                     tag.getVar(args[4]),
                     default_flow_style=False,
                     sort_keys=False))
 
         elif args[3] == 'set':
             self.tag_var_set(args)
 
+        elif args[3] == 'unset':
+            self.tag_var_unset(args)
+
         else:
             print('Invalid command '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
-    # > tag <hostname> var set
+    # > tag <tagname> var append
+    def tag_var_append(self, args):
+        tag = self._isidore.getTag(args[1])
+        if len(args) == 4:
+            self.subprompt(args, self.tag_var_append)
+        elif args[4] == '?':
+            print('''\
+?           print this help message
+<variable>  name of the list variable to append to''')
+
+        elif len(args) == 5:
+            self.subprompt(args, self.tag_var_append)
+
+        elif args[5] == '?':
+            print('''\
+?           print this help message
+<json>      the JSON value to append to the list''')
+
+        else:
+            try:
+                tag.appendVar(args[4], json.loads(args[5]))
+            except json.decoder.JSONDecodeError:
+                print(args[5] + '''
+^-- this is not valid JSON
+
+Strings must be double quoted. It will be necessary to either nest double
+quotes inside single quotes or escape the double quotes like so:
+
+   > tag mytag var set foo '"bar"'
+
+or
+
+   > tag mytag var set foo \\"bar\\"
+
+''')
+            except:
+                print(\
+'Failed to append to list variable. Is %s a valid list path?' % args[4])
+
+    # > tag <tagname> var set
     def tag_var_set(self, args):
         tag = self._isidore.getTag(args[1])
         if len(args) == 4:
             self.subprompt(args, self.tag_var_set)
         elif args[4] == '?':
             print('''\
 ?           print this help message
@@ -1008,13 +1130,28 @@
 
 or
 
    > tag mytag var set foo \\"bar\\"
 
 ''')
 
+    # > tag <tagname> var unset
+    def tag_var_unset(self, args):
+        tag = self._isidore.getTag(args[1])
+        if len(args) == 4:
+            self.subprompt(args, self.tag_var_set)
+        elif args[4] == '?':
+            print('''\
+?           print this help message
+<variable>  name of the variable to unset''')
+        else:
+            try:
+                tag.unsetVar(args[4])
+            except:
+                print("Failed to unset variable %s" % args[4])
+
     # > version
     def version(self, args):
             print('Isidore Command Prompt version: '+self.getVersion())
             print('libIsidore version: '+self._isidore.getVersion())
             print('Isidore database version: '+self._isidore.getDatabaseVersion())
```

### Comparing `isidore-0.1.2/src/isidore.egg-info/PKG-INFO` & `isidore-0.1.3/src/isidore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.2
+Version: 0.1.3
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
@@ -16,11 +16,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Isidore
 =======
 
 Isidore is a database, API, and CLI for managing Ansible inventories. It allows
-for a flexible tag base classification approach to group management.
+for a flexible tag based classification approach to group management.
 
 Website: [https://github.com/Z5T1/isidore](https://github.com/Z5T1/isidore)
```

