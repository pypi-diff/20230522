# Comparing `tmp/ansar-encode-0.1.76.tar.gz` & `tmp/ansar-encode-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.76.tar", last modified: Mon May 22 05:15:35 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.77.tar", last modified: Mon May 22 09:53:30 2023, max compression
```

## Comparing `ansar-encode-0.1.76.tar` & `ansar-encode-0.1.77.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4857 2023-05-22 05:15:32.000000 ansar-encode-0.1.76/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8167 2023-05-22 05:12:17.000000 ansar-encode-0.1.76/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    17364 2023-05-22 01:27:37.000000 ansar-encode-0.1.76/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.76/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4931 2023-05-22 09:53:27.000000 ansar-encode-0.1.77/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11271 2023-05-22 09:25:36.000000 ansar-encode-0.1.77/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19680 2023-05-22 09:46:06.000000 ansar-encode-0.1.77/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.77/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.76/LICENSE` & `ansar-encode-0.1.77/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/PKG-INFO` & `ansar-encode-0.1.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.76
+Version: 0.1.77
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.76/README.md` & `ansar-encode-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/setup.py` & `ansar-encode-0.1.77/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/command/show_release.py` & `ansar-encode-0.1.77/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/__init__.py` & `ansar-encode-0.1.77/src/ansar/encode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: e5cbed66e67b6cf75319557b0f9decb59fc222a5
-Version: 0.1.75 (2023-05-22@17:15:32+NZST)
+Commit: e9552778e711a638a9c22dd7006f8ee06fd28ca6
+Version: 0.1.76 (2023-05-22@21:53:27+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
@@ -92,15 +92,15 @@
 from .codec import CodecError, CodecUsage, CodecFailed, EnumerationFailed
 from .codec import python_to_word, word_to_python
 from .codec import Codec
 
 from .json import word_to_json, json_to_word, CodecJson
 from .xml import word_to_xml, xml_to_word, CodecXml
 
-from .file import FileFailure, FileEncoding
+from .file import FileFailure, FileOpenFailure, FileNotFound, FileNoAccess, FileNotAFile, FileIOFailure, FileEncoding
 from .file import File
 from .file import read_from_file, write_to_file
 
 from .folder import Folder, remove_contents, remove_folder, shape_of_folder
 
 from .version import migrate, cannot_upgrade
```

### Comparing `ansar-encode-0.1.76/src/ansar/encode/codec.py` & `ansar-encode-0.1.77/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/convert.py` & `ansar-encode-0.1.77/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/file.py` & `ansar-encode-0.1.77/src/ansar/encode/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,28 +34,34 @@
    :member-order: bysource
 """
 
 __docformat__ = 'restructuredtext'
 
 __all__ = [
     'FileFailure',
+	'FileOpenFailure',
+    'FileNotFound',
+    'FileNoAccess',
+    'FileNotAFile',
+    'FileIOFailure',
     'FileEncoding',
     'File',
     'read_from_file',
     'write_to_file',
 ]
 
 import os
 import errno
 
 from .portable import *
 from .message import *
 from .codec import *
 from .json import *
 
+
 # Exceptions.
 class FileFailure(Exception):
     """Base exception for all file exceptions.
 
     :param what: the failed operation
     :type what: str
     :param name: the name of the file
@@ -71,26 +77,68 @@
         self.what = what
         self.name = name
         self.note = note
         self.code = code
 
     def __str__(self):
         """Auto-convert to string representation."""
-        if self.code == 0:
+        if self.code is None:
             s = 'cannot %s "%s", %s' % (self.what, self.name, self.note)
         else:
             s = 'cannot %s "%s", %s (%s)' % (self.what, self.name, self.note, self.code)
         return s
 
-class FileEncoding(FileFailure):
+class FileOpenFailure(FileFailure):
+    """The named file did not exist."""
+
+    def __init__(self, what, name, note):
+        """Construct an instance of FileNotFound."""
+        FileFailure.__init__(self, what, name, note, None)
+
+class FileNotFound(FileOpenFailure):
+    """The named file did not exist."""
+
+    def __init__(self, what, name, note):
+        """Construct an instance of FileNotFound."""
+        FileOpenFailure.__init__(self, what, name, note)
+
+class FileNoAccess(FileOpenFailure):
+    """No access or a permissions problem."""
+
+    def __init__(self, what, name, note):
+        """Construct an instance of FileNoAccess."""
+        FileOpenFailure.__init__(self, what, name, note)
+
+class FileNotAFile(FileOpenFailure):
+    """Refers to a folder or the path includes a non-folder."""
+
+    def __init__(self, what, name, note):
+        """Construct an instance of FileNotAFile."""
+        FileOpenFailure.__init__(self, what, name, note)
+
+class FileAlreadyExists(FileOpenFailure):
+    """The named file already exists."""
+
+    def __init__(self, what, name, note):
+        """Construct an instance of FileAlreadyExists."""
+        FileOpenFailure.__init__(self, what, name, note)
+
+class FileIOFailure(FileFailure):
+    """A device I/O operation failed."""
+
+    def __init__(self, what, name, note, code):
+        """Construct an instance of FileIOFailure."""
+        FileFailure.__init__(self, what, name, note, code)
+
+class FileEncoding(FileIOFailure):
     """File or object content problem, encoding or decoding failed."""
 
     def __init__(self, what, name, note):
         """Construct an instance of FileEncoding."""
-        FileFailure.__init__(self, what, name, note, 0)
+        FileIOFailure.__init__(self, what, name, note, None)
 
 #
 #
 class File(object):
     """Store and recover application values using files.
 
     :param name: name of the file
@@ -161,15 +209,15 @@
         :param kwargs: remaining named parameters
         :type kwargs: dict
         :return: 2-tuple of an application value and a version.
         :rtype: value matching the saved ``expression`` and a ``str``
         """
         try:
             r, v = read_from_file(self.fixed, self.name, encoding=self.encoding, decorate_names=self.decorate_names)
-        except FileNotFoundError:
+        except FileNotFound:
             if self.create_default:
                 c = self.fixed
                 a = make(c)
                 return a, None
             raise
         if v is not None and upgrade:
             a = upgrade(r, v, *args, **kwargs)
@@ -188,16 +236,33 @@
     # Cannot read from /home/root (access or permissions)
     what = what or 'read from'
 
     # Add the encoding suffix according
     # to automation settings.
     name = encoding.full_name(name)
 
-    with open(name, 'r') as f:
+    try:
+        f = open(name, 'r')
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            raise FileNotFound(what, name, 'name does not exist')
+        elif e.errno in (errno.EACCES, errno.EPERM):
+            raise FileNoAccess(what, name, 'access or permissions')
+        elif e.errno == errno.ENOTDIR:
+            raise FileNotAFile(what, name, 'name in path is not a folder')
+        elif e.errno == errno.EISDIR:
+            raise FileNotAFile(what, name, 'name refers to a folder')
+        raise
+
+    try:
         s = f.read()
+    except OSError as e:
+        raise FileIOFailure(what, name, 'device I/O failed', e.errno)
+    finally:
+        f.close()
 
     try:
         d, v = encoding.decode(s, expression)
     except CodecFailed as e:
         s = str(e)
         raise FileEncoding(what, name, s)
     return d, v
@@ -213,18 +278,42 @@
 
     # Add the encoding suffix according
     # to automation settings.
     name = encoding.full_name(name)
 
     if expression is None:
         if not is_message(a):
-            raise FileFailure(what, name, 'type expression required for non-message', code=0)
+            raise FileFailure(what, name, 'type expression required for non-message', None)
         expression = UserDefined(a.__class__)
 
     try:
         s = encoding.encode(a, expression, version)
     except CodecFailed as e:
         s = str(e)
         raise FileEncoding(what, name, s)
 
-    with open(name, 'w') as f:
+    try:
+        # json.dumps produces a str that the file
+        # module will not write to a binary handle.
+        # Fair enough.
+        f = open(name, 'w')
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            # Not sure this happens, but cover the
+            # case anyway.
+            raise FileNotFound(what, name, 'name does not exist')
+        elif e.errno == errno.EEXIST:
+            raise FileAlreadyExists(what, name, 'name already exists')
+        elif e.errno in (errno.EACCES, errno.EPERM):
+            raise FileNoAccess(what, name, 'access or permissions')
+        elif e.errno == errno.ENOTDIR:
+            raise FileNotAFile(what, name, 'name in path is not a folder')
+        elif e.errno == errno.EISDIR:
+            raise FileNotAFile(what, name, 'name refers to a folder')
+        raise
+
+    try:
         f.write(s)
+    except OSError as e:
+        raise FileIOFailure(what, name, 'device I/O failed', e.errno)
+    finally:
+        f.close()
```

### Comparing `ansar-encode-0.1.76/src/ansar/encode/folder.py` & `ansar-encode-0.1.77/src/ansar/encode/folder.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,51 +59,81 @@
 CREATE_FOLDER = 'create folder'
 REMOVE_FOLDER = 'remove folder'
 REMOVE_FILE = 'remove file'
 #
 #
 def remove_contents(path):
     """Delete everything under the given folder, down."""
+
+    what = 'remove contents from'
     try:
         for f in os.listdir(path):
             p = os.path.join(path, f)
             if os.path.isdir(p):
                 remove_folder(p)
             elif os.path.isfile(p):
                 os.remove(p)
-    except FileNotFoundError:
-        pass
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            return
+        elif e.errno in (errno.EACCES, errno.EPERM):
+            raise FileNoAccess(what, path, 'access or permissions')
+        elif e.errno == errno.ENOTDIR:
+            raise FileNotAFile(what, path, 'name in path is not a folder')
+        elif e.errno == errno.EISDIR:
+            raise FileNotAFile(what, path, 'name refers to a folder')
+        raise FileFailure(what, path, e.strerror, e.errno)
+
 #
 #
 def remove_folder(path):
     """Delete everything under the given folder, and then the folder."""
+
+    remove_contents(path)
+
+    what = 'remove folder'
+
     try:
-        remove_contents(path)
         os.rmdir(path)
-    except FileNotFoundError:
-        pass
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            return
+        elif e.errno in (errno.EACCES, errno.EPERM):
+            raise FileNoAccess(what, path, 'access or permissions')
+        elif e.errno == errno.ENOTDIR:
+            raise FileNotAFile(what, path, 'name in path is not a folder')
+        raise FileFailure(what, path, e.strerror, e.errno)
+
 #
 #
 def shape_of_folder(path):
     """Walk the given folder, acumulating folders, files and bytes (3-tuple)."""
     folders, files, bytes = 0, 0, 0
-
-    for f in os.listdir(path):
-        p = os.path.join(path, f)
-        if os.path.isdir(p):
-            folders += 1
-            fo, fi, by = shape_of_folder(p)
-            folders += fo
-            files += fi
-            bytes += by
-        elif os.path.isfile(p):
-            s = os.stat(p)
-            files += 1
-            bytes += s.st_size
-
+    try:
+        p = path
+        for f in os.listdir(path):
+            p = os.path.join(path, f)
+            if os.path.isdir(p):
+                folders += 1
+                fo, fi, by = shape_of_folder(p)
+                folders += fo
+                files += fi
+                bytes += by
+            elif os.path.isfile(p):
+                s = os.stat(p)
+                files += 1
+                bytes += s.st_size
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist')
+        elif e.errno in (errno.EACCES, errno.EPERM):
+            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions')
+        elif e.errno == errno.ENOTDIR:
+            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder')
+        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', e.errno)
     return folders, files, bytes
 
 #
 #
 class Folder(object):
     """Create and manage a collection of application values, using a folder.
 
@@ -149,19 +179,24 @@
         self.decorate_names = decorate_names
         self.create_default = create_default
         self.keys_names = keys_names
         self.auto_create = auto_create
 
         if not auto_create:
             return
-
         try:
             os.makedirs(self.path)
-        except FileExistsError:
-            pass
+        except OSError as e:
+            if e.errno == errno.EEXIST:
+                return
+            elif e.errno in (errno.EACCES, errno.EPERM):
+                raise FileNoAccess(CREATE_FOLDER, self.path, 'access or permissions')
+            elif e.errno == errno.ENOTDIR:
+                raise FileNotAFile(CREATE_FOLDER, self.path, 'name in path is not a folder')
+            raise FileFailure(CREATE_FOLDER, self.path, 'unexpected platform code', e.errno)
 
     def folder(self, name, te=None, re=None, encoding=None,
             pretty_format=None, decorate_names=None, create_default=None,
             auto_create=None, keys_names=None):
         """Create a new :py:class:`~ansar.folder.Folder` object representing a sub-folder at the current location.
 
         :param path: the name to be added to the saved ``path``
@@ -341,58 +376,58 @@
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be added
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('add to', self.path, 'key/name functions not set', code=0)
+            raise FileFailure('add to', self.path, 'key/name functions not set', None)
 
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         io = self.file(name, self.te)
         if key in values:
-            raise FileFailure('add', io.name, 'entry already present', code=0)
+            raise FileFailure('add', io.name, 'entry already present', None)
         io.store(item)
         values[key] = item
 
     def update(self, values, item):
         """Update a value, both in a ``dict`` of values and as a file in the folder.
 
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be updated
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('update', self.path, 'key/name functions not set', code=0)
+            raise FileFailure('update', self.path, 'key/name functions not set', None)
 
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         io = self.file(name, self.te)
         if key not in values:
-            raise FileFailure('update', io.name, 'not an existing entry', code=0)
+            raise FileFailure('update', io.name, 'not an existing entry', None)
 
         io.store(item)
         values[key] = item
 
     def remove(self, values, item):
         """Remove a value, both from a ``dict`` of values and as a file in the folder.
 
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be removed
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('remove from', self.path, 'key/name functions not set', code=0)
+            raise FileFailure('remove from', self.path, 'key/name functions not set', None)
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         self.erase(name)
         del values[key]
 
     def clear(self, values):
@@ -415,15 +450,24 @@
         :type name: str
         """
         path = os.path.join(self.path, name)
         name = path
         if self.decorate_names:
             name = '%s.%s' % (path, self.encoding.EXTENSION)
         if os.path.isfile(name):
-            os.remove(name)
+            try:
+                os.remove(name)
+            except OSError as e:
+                if e.errno == errno.ENOENT:
+                    raise FileNotFound(REMOVE_FILE, name, 'name does not exist')
+                elif e.errno in (errno.EACCES, errno.EPERM):
+                    raise FileNoAccess(REMOVE_FILE, name, 'access or permissions')
+                elif e.errno == errno.ENOTDIR:
+                    raise FileNotAFile(REMOVE_FILE, name, 'name in path is not a folder')
+                raise FileFailure(REMOVE_FILE, name, 'unexpected platform code', e.errno)
             return True
         elif os.path.isdir(path):
             remove_folder(path)
             return True
         return False
 
     def exists(self, name=None):
@@ -453,22 +497,22 @@
         :param item: an application value
         :type name: see ``Folder.te``
         :return: the key
         :rtype: folder dependent
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('compose key', self.path, 'key/name functions not set', code=0)
+            raise FileFailure('compose key', self.path, 'key/name functions not set', None)
         return keys_names[0](item)
 
     def name(self, item):
         """Generate the stable filename for a given application value.
 
         :param item: an application value
         :type name: see ``Folder.te``
         :return: the filename
         :rtype: str
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('compose name', self.path, 'key/name functions not set', code=0)
+            raise FileFailure('compose name', self.path, 'key/name functions not set', None)
         return keys_names[1](item)
```

### Comparing `ansar-encode-0.1.76/src/ansar/encode/json.py` & `ansar-encode-0.1.77/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/message.py` & `ansar-encode-0.1.77/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/portable.py` & `ansar-encode-0.1.77/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/release.py` & `ansar-encode-0.1.77/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/runtime.py` & `ansar-encode-0.1.77/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/version.py` & `ansar-encode-0.1.77/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar/encode/xml.py` & `ansar-encode-0.1.77/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.76/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.77/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.76
+Version: 0.1.77
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.76/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.77/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

