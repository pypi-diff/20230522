# Comparing `tmp/num_stack_arithmac-0.0.1.tar.gz` & `tmp/num_stack_arithmac-0.0.2.tar.gz`

## Comparing `num_stack_arithmac-0.0.1.tar` & `num_stack_arithmac-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/src/num_stack_arithmac/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/src/num_stack_arithmac/compile.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/LICENSE
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/README.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/src/num_stack_arithmac/__init__.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/src/num_stack_arithmac/compile.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/README.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 num_stack_arithmac-0.0.2/PKG-INFO
```

### Comparing `num_stack_arithmac-0.0.1/LICENSE` & `num_stack_arithmac-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `num_stack_arithmac-0.0.1/README.md` & `num_stack_arithmac-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Num Stack Arithmac
 Install via:<br>
-`pip install num_stack_arithmac`
+`pip install num-stack-arithmac`
 ## Pre-execution
 Input is given by specifying the start number.
 ## Instructions
 Here are the different instructions:<br>
 `+` increments the number.<br>
 `-` decrements the number.<br>
 `%` performs reduction modulo 2 on the number.<br>
 `^` squares the number.<br>
 `r` takes the square root of the number.<br>
 `p` prints the decimal representation of the number.<br>
 `q` prints the character with the codepoint of the number.<br>
 `b` prints the binary representation of the number.<br>
 `x` prints the hexadecimal representation of the number.<br>
 `o` prints the boolean representation of the number.<br>
+`<` starts a comment. Comments are ignored by the compiler.<br>
+`>` ends a comment. Comments are ignored by the compiler.<br>
 `s` halts the programme.<br><br>
-All other characters are no-ops. If you use `\\` or `.` in your programme, the compiler will incorrectly think you are specifying the file path if you are typing in raw code.
+All other characters are no-ops. If you use `\\` or `.` in your programme, the compiler will incorrectly think you are specifying the file path if you are typing in raw code. You can also access a graphical editor by typing in `g`.
 ## Example
 Here is an example programme that checks whether a number is even or odd (the number is given by the starting value):<br><br>
 `%+%o`
```

### Comparing `num_stack_arithmac-0.0.1/pyproject.toml` & `num_stack_arithmac-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "num_stack_arithmac"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="PlaceReporter99", email="sfurman35@outlook.com" },
 ]
 description = "The Num Stack Arithmac programming language."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `num_stack_arithmac-0.0.1/PKG-INFO` & `num_stack_arithmac-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: num_stack_arithmac
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Num Stack Arithmac programming language.
 Project-URL: Homepage, https://github.com/PlaceReporter99/Num-Stack-Arithmac/
 Project-URL: Bug Tracker, https://github.com/PlaceReporter99/Num-Stack-Arithmac/issues
 Author-email: PlaceReporter99 <sfurman35@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Num Stack Arithmac
 Install via:<br>
-`pip install num_stack_arithmac`
+`pip install num-stack-arithmac`
 ## Pre-execution
 Input is given by specifying the start number.
 ## Instructions
 Here are the different instructions:<br>
 `+` increments the number.<br>
 `-` decrements the number.<br>
 `%` performs reduction modulo 2 on the number.<br>
 `^` squares the number.<br>
 `r` takes the square root of the number.<br>
 `p` prints the decimal representation of the number.<br>
 `q` prints the character with the codepoint of the number.<br>
 `b` prints the binary representation of the number.<br>
 `x` prints the hexadecimal representation of the number.<br>
 `o` prints the boolean representation of the number.<br>
+`<` starts a comment. Comments are ignored by the compiler.<br>
+`>` ends a comment. Comments are ignored by the compiler.<br>
 `s` halts the programme.<br><br>
-All other characters are no-ops. If you use `\\` or `.` in your programme, the compiler will incorrectly think you are specifying the file path if you are typing in raw code.
+All other characters are no-ops. If you use `\\` or `.` in your programme, the compiler will incorrectly think you are specifying the file path if you are typing in raw code. You can also access a graphical editor by typing in `g`.
 ## Example
 Here is an example programme that checks whether a number is even or odd (the number is given by the starting value):<br><br>
 `%+%o`
```

