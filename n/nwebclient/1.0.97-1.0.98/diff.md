# Comparing `tmp/nwebclient-1.0.97.tar.gz` & `tmp/nwebclient-1.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.97.tar", last modified: Fri May 19 11:43:04 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.98.tar", last modified: Mon May 22 12:51:56 2023, max compression
```

## Comparing `nwebclient-1.0.97.tar` & `nwebclient-1.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:43:04.294831 nwebclient-1.0.97/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.97/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:43:04.294831 nwebclient-1.0.97/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.97/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:43:04.294831 nwebclient-1.0.97/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.97/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.97/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.97/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.97/nwebclient/nlp.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13678 2023-05-19 11:42:51.000000 nwebclient-1.0.97/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.97/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.97/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:43:04.294831 nwebclient-1.0.97/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:43:04.000000 nwebclient-1.0.97/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:43:04.294831 nwebclient-1.0.97/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:43:01.000000 nwebclient-1.0.97/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.98/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 12:51:56.373321 nwebclient-1.0.98/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.98/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.98/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.98/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.98/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.98/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13678 2023-05-19 11:42:51.000000 nwebclient-1.0.98/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7104 2023-05-22 12:51:19.000000 nwebclient-1.0.98/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.98/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-22 12:51:56.373321 nwebclient-1.0.98/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-22 12:51:51.000000 nwebclient-1.0.98/setup.py
```

### Comparing `nwebclient-1.0.97/LICENSE` & `nwebclient-1.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/PKG-INFO` & `nwebclient-1.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.97
+Version: 1.0.98
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.97/README.md` & `nwebclient-1.0.98/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/__init__.py` & `nwebclient-1.0.98/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/__main__.py` & `nwebclient-1.0.98/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/crypt.py` & `nwebclient-1.0.98/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/nlp.py` & `nwebclient-1.0.98/nwebclient/nlp.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/sd.py` & `nwebclient-1.0.98/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient/sdb.py` & `nwebclient-1.0.98/nwebclient/sdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -150,14 +150,43 @@
         cursor.execute(sql)
         cursor.close()
     except sqlite3.Error as error:
         print("Failed to read data from sqlite table", error)
     finally:
         if sqliteConnection:
             sqliteConnection.close()
+            
+def sortin(dbfile='data.db'):
+    try:
+        sqliteConnection = sqlite3.connect(dbfile)
+        cursor = sqliteConnection.cursor()
+        sql_fetch_blob_query = """SELECT id, name, data from nxfiles"""
+        cursor.execute(sql_fetch_blob_query)
+        record = cursor.fetchall()
+        for row in record:
+            print("Id = ", row[0], "Name = ", row[1])
+            name = row[1]
+            id = row[0]
+            data = row[2]
+            i = 0
+            os.mkdir(name)
+            filename = name+"/"+str(id)+".jpg"
+            while os.path.isfile(file):
+                i = i+1
+                filename = name+"/"+str(id+i)+".jpg"
+            print("Write File: " + filename)
+            writeTofile(data, filename)
+
+        cursor.close()
+
+    except sqlite3.Error as error:
+        print("Failed to read blob data from sqlite table", error)
+    finally:
+        if sqliteConnection:
+            sqliteConnection.close()
         
         
 def main():
     print("SDB")
     print("Usage nx-sdb (show|extract|from|count|clear)")
     #print(str(sys.argv)) # 0-path
     if len(sys.argv)>1:
@@ -166,14 +195,16 @@
             count()
         elif op=='extract':
             sdb_extract()
         elif op=='inc':
             inc()
         elif op =='from':
             print("Extract from id:"+str(sys.argv[2]))
+        elif op =='sortin':
+            sortin()
         else:
             print("Error: Unknown Operation")
     else:
         show()
    
 if __name__ == '__main__': # nx-sdb vom python-package bereitgestellt
     main()
```

### Comparing `nwebclient-1.0.97/nwebclient/ticker.py` & `nwebclient-1.0.98/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.97/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.98/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.97
+Version: 1.0.98
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.97/setup.py` & `nwebclient-1.0.98/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.97",
+    version="1.0.98",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

