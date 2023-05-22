# Comparing `tmp/ansar-encode-0.1.75.tar.gz` & `tmp/ansar-encode-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.75.tar", last modified: Mon May 15 02:16:43 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.76.tar", last modified: Mon May 22 05:15:35 2023, max compression
```

## Comparing `ansar-encode-0.1.75.tar` & `ansar-encode-0.1.76.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-05-15 02:16:40.000000 ansar-encode-0.1.75/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    18929 2023-05-15 02:16:28.000000 ansar-encode-0.1.75/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.75/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.75/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-15 02:16:43.951713 ansar-encode-0.1.75/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-15 02:16:43.000000 ansar-encode-0.1.75/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4857 2023-05-22 05:15:32.000000 ansar-encode-0.1.76/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8167 2023-05-22 05:12:17.000000 ansar-encode-0.1.76/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    17364 2023-05-22 01:27:37.000000 ansar-encode-0.1.76/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.76/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.76/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 05:15:35.897525 ansar-encode-0.1.76/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-22 05:15:35.000000 ansar-encode-0.1.76/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.75/LICENSE` & `ansar-encode-0.1.76/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/PKG-INFO` & `ansar-encode-0.1.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.75
+Version: 0.1.76
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.75/README.md` & `ansar-encode-0.1.76/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/setup.py` & `ansar-encode-0.1.76/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/command/show_release.py` & `ansar-encode-0.1.76/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/__init__.py` & `ansar-encode-0.1.76/src/ansar/encode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: 07d41b16fec830c88b0ff5f8fee6a80e17bde747
-Version: 0.1.74 (2023-05-15@14:16:40+NZST)
+Commit: e5cbed66e67b6cf75319557b0f9decb59fc222a5
+Version: 0.1.75 (2023-05-22@17:15:32+NZST)
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
 
-from .file import FileFailure, FileNotFound, FileNoAccess, FileNotAFile, FileIoFailed, FileEncoding
+from .file import FileFailure, FileEncoding
 from .file import File
 from .file import read_from_file, write_to_file
 
 from .folder import Folder, remove_contents, remove_folder, shape_of_folder
 
 from .version import migrate, cannot_upgrade
```

### Comparing `ansar-encode-0.1.75/src/ansar/encode/codec.py` & `ansar-encode-0.1.76/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/convert.py` & `ansar-encode-0.1.76/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/file.py` & `ansar-encode-0.1.76/src/ansar/encode/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,33 +34,28 @@
    :member-order: bysource
 """
 
 __docformat__ = 'restructuredtext'
 
 __all__ = [
     'FileFailure',
-    'FileNotFound',
-    'FileNoAccess',
-    'FileNotAFile',
-    'FileIoFailed',
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
 
-
 # Exceptions.
 class FileFailure(Exception):
     """Base exception for all file exceptions.
 
     :param what: the failed operation
     :type what: str
     :param name: the name of the file
@@ -82,49 +77,14 @@
         """Auto-convert to string representation."""
         if self.code == 0:
             s = 'cannot %s "%s", %s' % (self.what, self.name, self.note)
         else:
             s = 'cannot %s "%s", %s (%s)' % (self.what, self.name, self.note, self.code)
         return s
 
-class FileNotFound(FileFailure):
-    """The named file did not exist."""
-
-    def __init__(self, what, name, note, code=0):
-        """Construct an instance of FileNotFound."""
-        FileFailure.__init__(self, what, name, note, code)
-
-class FileNoAccess(FileFailure):
-    """No access or a permissions problem."""
-
-    def __init__(self, what, name, note, code=0):
-        """Construct an instance of FileNoAccess."""
-        FileFailure.__init__(self, what, name, note, code)
-
-class FileNotAFile(FileFailure):
-    """Refers to a folder or the path includes a non-folder."""
-
-    def __init__(self, what, name, note, code=0):
-        """Construct an instance of FileNotAFile."""
-        FileFailure.__init__(self, what, name, note, code)
-
-class FileAlreadyExists(FileFailure):
-    """The named file already exists."""
-
-    def __init__(self, what, name, note, code=0):
-        """Construct an instance of FileAlreadyExists."""
-        FileFailure.__init__(self, what, name, note, code)
-
-class FileIoFailed(FileFailure):
-    """A device I/O operation failed."""
-
-    def __init__(self, what, name, note, code=0):
-        """Construct an instance of FileIoFailed."""
-        FileFailure.__init__(self, what, name, note, code)
-
 class FileEncoding(FileFailure):
     """File or object content problem, encoding or decoding failed."""
 
     def __init__(self, what, name, note):
         """Construct an instance of FileEncoding."""
         FileFailure.__init__(self, what, name, note, 0)
 
@@ -201,15 +161,15 @@
         :param kwargs: remaining named parameters
         :type kwargs: dict
         :return: 2-tuple of an application value and a version.
         :rtype: value matching the saved ``expression`` and a ``str``
         """
         try:
             r, v = read_from_file(self.fixed, self.name, encoding=self.encoding, decorate_names=self.decorate_names)
-        except FileNotFound:
+        except FileNotFoundError:
             if self.create_default:
                 c = self.fixed
                 a = make(c)
                 return a, None
             raise
         if v is not None and upgrade:
             a = upgrade(r, v, *args, **kwargs)
@@ -228,35 +188,16 @@
     # Cannot read from /home/root (access or permissions)
     what = what or 'read from'
 
     # Add the encoding suffix according
     # to automation settings.
     name = encoding.full_name(name)
 
-    try:
-        f = open(name, 'r')
-    except IOError as e:
-        if e.errno == errno.ENOENT:
-            raise FileNotFound(what, name, 'name does not exist', e.errno)
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(what, name, 'access or permissions', e.errno)
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(what, name, 'name in path is not a folder', e.errno)
-        elif e.errno == errno.EISDIR:
-            raise FileNotAFile(what, name, 'name refers to a folder', e.errno)
-        raise
-
-    try:
+    with open(name, 'r') as f:
         s = f.read()
-    except IOError as e:
-        if e.errno == errno.EIO:
-            raise FileIoFailed(what, name, 'device I/O failed', e.errno)
-        raise
-    finally:
-        f.close()
 
     try:
         d, v = encoding.decode(s, expression)
     except CodecFailed as e:
         s = str(e)
         raise FileEncoding(what, name, s)
     return d, v
@@ -281,35 +222,9 @@
 
     try:
         s = encoding.encode(a, expression, version)
     except CodecFailed as e:
         s = str(e)
         raise FileEncoding(what, name, s)
 
-    try:
-        # json.dumps produces a str that the file
-        # module will not write to a binary handle.
-        # Fair enough.
-        f = open(name, 'w')
-    except IOError as e:
-        if e.errno == errno.ENOENT:
-            # Not sure this happens, but cover the
-            # case anyway.
-            raise FileNotFound(what, name, 'name does not exist', e.errno)
-        elif e.errno == errno.EEXIST:
-            raise FileAlreadyExists(what, name, 'name already exists', e.errno)
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(what, name, 'access or permissions', e.errno)
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(what, name, 'name in path is not a folder', e.errno)
-        elif e.errno == errno.EISDIR:
-            raise FileNotAFile(what, name, 'name refers to a folder', e.errno)
-        raise
-
-    try:
+    with open(name, 'w') as f:
         f.write(s)
-    except IOError as e:
-        if e.errno == errno.EIO:
-            raise FileIoFailed(what, name, 'device I/O failed', e.errno)
-        raise
-    finally:
-        f.close()
```

### Comparing `ansar-encode-0.1.75/src/ansar/encode/folder.py` & `ansar-encode-0.1.76/src/ansar/encode/folder.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,35 +82,28 @@
     except FileNotFoundError:
         pass
 #
 #
 def shape_of_folder(path):
     """Walk the given folder, acumulating folders, files and bytes (3-tuple)."""
     folders, files, bytes = 0, 0, 0
-    try:
-        for f in os.listdir(path):
-            p = os.path.join(path, f)
-            if os.path.isdir(p):
-                folders += 1
-                fo, fi, by = shape_of_folder(p)
-                folders += fo
-                files += fi
-                bytes += by
-            elif os.path.isfile(p):
-                s = os.stat(p)
-                files += 1
-                bytes += s.st_size
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist', e.errno)
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions', e.errno)
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder', e.errno)
-        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', code=0)
+
+    for f in os.listdir(path):
+        p = os.path.join(path, f)
+        if os.path.isdir(p):
+            folders += 1
+            fo, fi, by = shape_of_folder(p)
+            folders += fo
+            files += fi
+            bytes += by
+        elif os.path.isfile(p):
+            s = os.stat(p)
+            files += 1
+            bytes += s.st_size
+
     return folders, files, bytes
 
 #
 #
 class Folder(object):
     """Create and manage a collection of application values, using a folder.
 
@@ -156,24 +149,19 @@
         self.decorate_names = decorate_names
         self.create_default = create_default
         self.keys_names = keys_names
         self.auto_create = auto_create
 
         if not auto_create:
             return
+
         try:
             os.makedirs(self.path)
-        except OSError as e:
-            if e.errno == errno.EEXIST:
-                return
-            elif e.errno in (errno.EACCES, errno.EPERM):
-                raise FileNoAccess(CREATE_FOLDER, self.path, 'access or permissions', code=e.errno)
-            elif e.errno == errno.ENOTDIR:
-                raise FileNotAFile(CREATE_FOLDER, self.path, 'name in path is not a folder', code=e.errno)
-            raise FileFailure(CREATE_FOLDER, self.path, 'unexpected platform code', code=e.errno)
+        except FileExistsError:
+            pass
 
     def folder(self, name, te=None, re=None, encoding=None,
             pretty_format=None, decorate_names=None, create_default=None,
             auto_create=None, keys_names=None):
         """Create a new :py:class:`~ansar.folder.Folder` object representing a sub-folder at the current location.
 
         :param path: the name to be added to the saved ``path``
@@ -427,24 +415,15 @@
         :type name: str
         """
         path = os.path.join(self.path, name)
         name = path
         if self.decorate_names:
             name = '%s.%s' % (path, self.encoding.EXTENSION)
         if os.path.isfile(name):
-            try:
-                os.remove(name)
-            except IOError as e:
-                if e.errno == errno.ENOENT:
-                    raise FileNotFound(REMOVE_FILE, name, 'name does not exist', e.errno)
-                elif e.errno in (errno.EACCES, errno.EPERM):
-                    raise FileNoAccess(REMOVE_FILE, name, 'access or permissions', e.errno)
-                elif e.errno == errno.ENOTDIR:
-                    raise FileNotAFile(REMOVE_FILE, name, 'name in path is not a folder', e.errno)
-                raise FileFailure(REMOVE_FILE, name, 'unexpected platform code', code=0)
+            os.remove(name)
             return True
         elif os.path.isdir(path):
             remove_folder(path)
             return True
         return False
 
     def exists(self, name=None):
```

### Comparing `ansar-encode-0.1.75/src/ansar/encode/json.py` & `ansar-encode-0.1.76/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/message.py` & `ansar-encode-0.1.76/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/portable.py` & `ansar-encode-0.1.76/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/release.py` & `ansar-encode-0.1.76/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/runtime.py` & `ansar-encode-0.1.76/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/version.py` & `ansar-encode-0.1.76/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar/encode/xml.py` & `ansar-encode-0.1.76/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.75/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.76/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.75
+Version: 0.1.76
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.75/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.76/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

