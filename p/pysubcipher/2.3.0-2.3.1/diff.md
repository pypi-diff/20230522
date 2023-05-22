# Comparing `tmp/pysubcipher-2.3.0.tar.gz` & `tmp/pysubcipher-2.3.1.tar.gz`

## Comparing `pysubcipher-2.3.0.tar` & `pysubcipher-2.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/LICENSE
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/README.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 pysubcipher-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/LICENSE
+-rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/PKG-INFO
```

### Comparing `pysubcipher-2.3.0/src/pysubcipher/__init__.py` & `pysubcipher-2.3.1/src/pysubcipher/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.0/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.3.1/src/pysubcipher/pysubcipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             max_key_length (int): The maximum length of a cipher key.
             seed (int | float | str | bytes | bytearray | None, optional): The seed that cipher keys will be generated with. Defaults to os.urandom(1024).
             charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
         """
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
         self.__charset: str = charset
-        self._current_seed: int | float | str | bytes | bytearray | None = seed
+        self.__current_seed: int | float | str | bytes | bytearray | None = seed
         if not isinstance(charset, str):
             raise TypeError(f"Parameter charset cannot be of type {type(charset)}")
         super().__init__(min_key_length, max_key_length, seed = seed, charset = self.__charset)
     def encrypt(self, s: str, /) -> bytes:
         """Encrypts a string of text using pre-defined cipher keys.
 
         Args:
@@ -140,15 +140,15 @@
         return __decrypted_string.getvalue().encode()
     def set_seed(self, seed: int | float | str | bytes | bytearray | None, /) -> None:
         """Sets the random seed for cipher keys to be generated with.
 
         Args:
             seed (int | float | str | bytes | bytearray | None): The seed to override.
         """
-        self._current_seed = seed
+        self.__current_seed = seed
         super().__init__(self.__min_key_length, self.__max_key_length, seed = seed, charset = self.__charset)
     def regenerate_keys(self, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), /) -> None:
         """Regenerates encryption and decryption keys.
 
         Args:
             seed (int | float | str | bytes | bytearray | None, optional): The seed to generate cipher keys with. Defaults to os.urandom(1024).
         """
@@ -175,29 +175,29 @@
     def save_keys(self, file: str, /, *, truncate: bool = False) -> None:
         """Saves the current cipher keys to a file.
 
         Args:
             file (str): The filepath.
             truncate (bool, optional): If True, file will be truncated prematurely before storing the keys. Defaults to False.
         """
-        self._current_seed = None
+        self.__current_seed = None
         with open(file, "wb") as f:
             if truncate:
                 f.truncate(0)
             f.write(pickle.dumps([self._encryption_keys, self._decryption_keys]))
     def load_keys(self, file: str, /) -> None:
         """Loads cipher keys into the current instance.
 
         Args:
             file (str): The path to the file where the keys are stored.
 
         Raises:
             InvalidKeysError: Raised if the cipher keys are not valid.
         """
-        self._current_seed = None
+        self.__current_seed = None
         with open(file, "rb") as f:
             contents = f.read()
             try:
                 keys = pickle.loads(contents)
             except pickle.UnpicklingError:
                 raise InvalidKeysError()
             encryption_keys = keys[0]
@@ -217,15 +217,15 @@
             raise exit_type(exit_value)
 
     def __str__(self) -> str:
         return f"SubstitutionCipher(minimum_key_length={self.__min_key_length}, maximum_key_length={self.__max_key_length})"
 
     def __repr__(self) -> str:
         __quote: str = "'"
-        return f"SubstitutionCipher(minimum_key_length={self.__min_key_length}, maximum_key_length={self.__max_key_length}, seed={__quote if isinstance(self._current_seed, str) else ''}{self._current_seed}{__quote if isinstance(self._current_seed, str) else ''}, charset='{self.__charset.strip()}')"
+        return f"SubstitutionCipher(minimum_key_length={self.__min_key_length}, maximum_key_length={self.__max_key_length}, seed={__quote if isinstance(self.__current_seed, str) else ''}{self.__current_seed}{__quote if isinstance(self.__current_seed, str) else ''}, charset='{self.__charset.strip()}')"
 
 class FileSubstitutionCipher(SubstitutionCipher):
     def __init__(self, min_key_length: int = 10, max_key_length: int = 20, *, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), charset: str = HEXDIGITS) -> None:
         """A simple substitution cipher encryption tool to encrypt file's and their contents.
 
         Args:
             min_key_length (int): The minimum length of a cipher key.
```

### Comparing `pysubcipher-2.3.0/LICENSE` & `pysubcipher-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.0/README.md` & `pysubcipher-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.0/pyproject.toml` & `pysubcipher-2.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysubcipher"
-version = "2.3.0"
+version = "2.3.1"
 authors = [
   {name = "mxngo", email = ""}
 ]
 description = "pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pysubcipher-2.3.0/PKG-INFO` & `pysubcipher-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubcipher
-Version: 2.3.0
+Version: 2.3.1
 Summary: pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm.
 Author: mxngo
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

