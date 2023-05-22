# Comparing `tmp/AmiAutomation-0.1.4.2.tar.gz` & `tmp/AmiAutomation-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AmiAutomation-0.1.4.2.tar", last modified: Tue Feb  7 18:53:34 2023, max compression
+gzip compressed data, was "dist\AmiAutomation-0.1.4.3.tar", last modified: Mon May 22 20:02:21 2023, max compression
```

## Comparing `AmiAutomation-0.1.4.2.tar` & `AmiAutomation-0.1.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 18:53:34.295984 AmiAutomation-0.1.4.2/
-drwxrwxrwx   0        0        0        0 2023-02-07 18:53:34.280358 AmiAutomation-0.1.4.2/AmiAutomation/
--rw-rw-rw-   0        0        0    28001 2023-02-07 18:53:29.000000 AmiAutomation-0.1.4.2/AmiAutomation/LogData.py
--rw-rw-rw-   0        0        0     3448 2021-08-11 22:52:50.000000 AmiAutomation-0.1.4.2/AmiAutomation/PX3_Bin.py
--rw-rw-rw-   0        0        0     3994 2023-02-07 18:53:29.000000 AmiAutomation-0.1.4.2/AmiAutomation/RphData.py
--rw-rw-rw-   0        0        0        0 2021-08-11 22:52:50.000000 AmiAutomation-0.1.4.2/AmiAutomation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 18:53:34.295984 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/
--rw-rw-rw-   0        0        0     6695 2023-02-07 18:53:33.000000 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-02-07 18:53:33.000000 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 18:53:33.000000 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-07 18:53:33.000000 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-07 18:53:33.000000 AmiAutomation-0.1.4.2/AmiAutomation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27648 2021-08-11 22:52:54.000000 AmiAutomation-0.1.4.2/DigitArcPX3.Tools.DataToPython.dll
--rw-rw-rw-   0        0        0   126976 2021-08-11 22:52:54.000000 AmiAutomation-0.1.4.2/ICSharpCode.SharpZipLib.dll
--rw-rw-rw-   0        0        0   131072 2021-08-11 22:52:54.000000 AmiAutomation-0.1.4.2/Kernel.Message.dll
--rw-rw-rw-   0        0        0     1090 2021-08-11 22:52:54.000000 AmiAutomation-0.1.4.2/LICENSE
--rw-rw-rw-   0        0        0     6695 2023-02-07 18:53:34.295984 AmiAutomation-0.1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4980 2023-02-07 18:53:29.000000 AmiAutomation-0.1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-07 18:53:34.295984 AmiAutomation-0.1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1009 2023-02-07 18:53:29.000000 AmiAutomation-0.1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 20:02:21.796657 AmiAutomation-0.1.4.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 20:02:21.779899 AmiAutomation-0.1.4.3/AmiAutomation/
+-rw-rw-rw-   0        0        0    28341 2023-05-22 19:51:17.000000 AmiAutomation-0.1.4.3/AmiAutomation/LogData.py
+-rw-rw-rw-   0        0        0     3448 2021-02-22 19:37:41.000000 AmiAutomation-0.1.4.3/AmiAutomation/PX3_Bin.py
+-rw-rw-rw-   0        0        0     3994 2022-05-18 18:14:45.000000 AmiAutomation-0.1.4.3/AmiAutomation/RphData.py
+-rw-rw-rw-   0        0        0        0 2020-10-06 22:23:36.000000 AmiAutomation-0.1.4.3/AmiAutomation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 20:02:21.793653 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/
+-rw-rw-rw-   0        0        0     8975 2023-05-22 20:02:21.000000 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-05-22 20:02:21.000000 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 20:02:21.000000 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 20:02:21.000000 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 20:02:21.000000 AmiAutomation-0.1.4.3/AmiAutomation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27648 2021-02-22 19:37:45.000000 AmiAutomation-0.1.4.3/DigitArcPX3.Tools.DataToPython.dll
+-rw-rw-rw-   0        0        0   126976 2020-10-06 22:23:43.000000 AmiAutomation-0.1.4.3/ICSharpCode.SharpZipLib.dll
+-rw-rw-rw-   0        0        0   131072 2020-10-06 22:25:56.000000 AmiAutomation-0.1.4.3/Kernel.Message.dll
+-rw-rw-rw-   0        0        0     1090 2020-10-06 22:25:49.000000 AmiAutomation-0.1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     8975 2023-05-22 20:02:21.795654 AmiAutomation-0.1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8470 2023-05-22 19:51:03.000000 AmiAutomation-0.1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 20:02:21.797652 AmiAutomation-0.1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2023-05-22 20:02:07.000000 AmiAutomation-0.1.4.3/setup.py
```

### Comparing `AmiAutomation-0.1.4.2/AmiAutomation/LogData.py` & `AmiAutomation-0.1.4.3/AmiAutomation/LogData.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self._hash = dict()
         self._properties = dict()
         
     def Unserialize(self,bytesStream, oldSerialize=True):
         if not oldSerialize:
             self._header.Unserialize(bytesStream)
             if self._header._version != 0:
-                raise Exception ("Error unserializing properties, version " , str.from_bytes(self._header._version) , " is not supported")
+                raise Exception (f"Error unserializing properties, version {self._header._version}, is not supported")
         
         #Properties  
         self._properties = Properties.Unserialize(bytesStream)
         #Inner
         count = struct.unpack("h", bytesStream.read(2))[0]      
         #Unserialize inner 
         for element in range(count):
@@ -565,37 +565,46 @@
     logData._data = arraySamples
     logData._mainTrendsNames = trendsNames
     logData._mainDivisors = divisors
     logData.properties = composite._properties
     
     return logData
 
-def binStreamToDF(file, logData=LogData(), null_promoting={}):
+def binStreamToDF(file, extension = 'bin', null_promoting={}):
     """
     Unpacks binary file stream into LogData
     
     Parameters
     ----------
     file : stream
         stream of binary file
        
-    bin_file : bool
-        whether source file is .bin extension
+    extension : str, optional
+        read file extention, value must be "bin", "cpst" or "hist"
+        default: bin
         
     null_promoting : dict
         A dictionary with a .NET Source Type key and a value of either one of 
-        the following (default, object, float, Int64, string, error).\n
+        the following (default, object, float, Int64, string, error).
 
     Returns
     -------
     LogData
         Structure containing most file data
 
     """  
+
+    # Validate extension
+    accepted_extensions = ['bin','cpst','rph','hist']
+    if extension not in accepted_extensions:
+        raise Exception(f"Given extension \"{extension}\" is not a compatible extension")
     
+    logData = LogData()
+    logData._fileType = extension
+
     #header
     TAGS = file.read(4)
     if TAGS != b'TAGS':
         print("Error with Tags header")
     versionHeader = file.read(1)
     if versionHeader == b'\xFF':
         print("Corrupt header, version can never reach 255")
@@ -742,16 +751,18 @@
     Unpacks binary file into LogData
     
     Parameters
     ----------
     path : str
         Complete file path
         
-    extension : str
-        Assume given file extension. ex: 'bin'
+    extension : str, optional
+        Read file extention, value must be "bin", "cpst" or "hist".
+        If no value is given, it will be infered from the file name
+        default: bin
         
     null_promoting : dict
         A dictionary with a .NET Source Type key and a value of either one of 
         the following (default, object, float, Int64, string, error).\n
         
         The possible dictionary keys are the .NET simple types:
             * SByte
@@ -781,29 +792,24 @@
             
     Returns
     -------
     LogData
         Structure containing most file data
 
     """
-        
-    file = open(path, "rb")
-
     _, file_extension = os.path.splitext(path)
-      
-    logData = LogData()
-    logData._fileName = os.path.basename(path)
-    
+        
     if extension == None:
         if '.' not in file_extension:
             print("Warning, unidentified file extension, assuming .bin")
             file_extension = '.bin'
-            
-        logData._fileType = file_extension.strip('.')
-        
-    else:
-        logData._fileType = extension
-    
-    logData = binStreamToDF(file, logData, null_promoting)
+                
+        extension = file_extension.strip('.')
+
+    file = open(path, "rb")
+      
+    logData = binStreamToDF(file, extension, null_promoting)
+
+    logData._fileName = os.path.basename(path)
     
     file.close()
-    return logData    
+    return logData
```

### Comparing `AmiAutomation-0.1.4.2/AmiAutomation/PX3_Bin.py` & `AmiAutomation-0.1.4.3/AmiAutomation/PX3_Bin.py`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/AmiAutomation/RphData.py` & `AmiAutomation-0.1.4.3/AmiAutomation/RphData.py`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/DigitArcPX3.Tools.DataToPython.dll` & `AmiAutomation-0.1.4.3/DigitArcPX3.Tools.DataToPython.dll`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/ICSharpCode.SharpZipLib.dll` & `AmiAutomation-0.1.4.3/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/Kernel.Message.dll` & `AmiAutomation-0.1.4.3/Kernel.Message.dll`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/LICENSE` & `AmiAutomation-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AmiAutomation-0.1.4.2/setup.py` & `AmiAutomation-0.1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AmiAutomation", 
-    version="0.1.4.2", ### Change before commit
+    version="0.1.4.3", ### Change before commit
     author="AMI",
     author_email="luis.castro@amiautomation.com",
     description="Package to extract binary files into pandas dataframes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

