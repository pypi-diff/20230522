# Comparing `tmp/exodia-1.0.0.tar.gz` & `tmp/exodia-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exodia-1.0.0.tar", last modified: Sun May 21 22:45:11 2023, max compression
+gzip compressed data, was "exodia-1.0.1.tar", last modified: Mon May 22 12:51:27 2023, max compression
```

## Comparing `exodia-1.0.0.tar` & `exodia-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-21 22:45:11.235750 exodia-1.0.0/
--rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.0/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-21 22:45:11.235638 exodia-1.0.0/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     1514 2023-05-21 21:47:28.000000 exodia-1.0.0/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-21 22:45:11.234367 exodia-1.0.0/exodia/
--rw-r--r--   0 leondaz    (501) staff       (20)      147 2023-05-21 21:31:27.000000 exodia-1.0.0/exodia/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)      596 2023-05-21 21:56:16.000000 exodia-1.0.0/exodia/bases.py
--rw-r--r--   0 leondaz    (501) staff       (20)      106 2023-05-21 17:39:57.000000 exodia-1.0.0/exodia/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     3306 2023-05-21 20:34:55.000000 exodia-1.0.0/exodia/fields.py
--rw-r--r--   0 leondaz    (501) staff       (20)      234 2023-05-21 21:33:26.000000 exodia-1.0.0/exodia/utils.py
--rw-r--r--   0 leondaz    (501) staff       (20)     5585 2023-05-21 20:56:16.000000 exodia-1.0.0/exodia/validators.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-21 22:45:11.234974 exodia-1.0.0/exodia.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-21 22:45:11.000000 exodia-1.0.0/exodia.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-21 22:45:11.000000 exodia-1.0.0/exodia.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-21 22:45:11.000000 exodia-1.0.0/exodia.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-21 22:45:11.000000 exodia-1.0.0/exodia.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-21 22:45:11.235785 exodia-1.0.0/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-21 21:10:41.000000 exodia-1.0.0/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-21 22:45:11.235367 exodia-1.0.0/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      920 2023-05-21 21:43:59.000000 exodia-1.0.0/tests/test_instance_creation.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1089 2023-05-21 20:57:45.000000 exodia-1.0.0/tests/test_validation.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 12:51:27.041479 exodia-1.0.1/
+-rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.1/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 12:51:27.041365 exodia-1.0.1/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     1577 2023-05-21 22:46:05.000000 exodia-1.0.1/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 12:51:27.040561 exodia-1.0.1/exodia/
+-rw-r--r--   0 leondaz    (501) staff       (20)      147 2023-05-21 21:31:27.000000 exodia-1.0.1/exodia/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1366 2023-05-22 12:30:29.000000 exodia-1.0.1/exodia/bases.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 12:28:08.000000 exodia-1.0.1/exodia/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     3503 2023-05-22 12:34:34.000000 exodia-1.0.1/exodia/fields.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      234 2023-05-21 21:33:26.000000 exodia-1.0.1/exodia/utils.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     6522 2023-05-22 12:49:23.000000 exodia-1.0.1/exodia/validators.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 12:51:27.040994 exodia-1.0.1/exodia.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 12:51:27.000000 exodia-1.0.1/exodia.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-22 12:51:27.000000 exodia-1.0.1/exodia.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-22 12:51:27.000000 exodia-1.0.1/exodia.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-22 12:51:27.000000 exodia-1.0.1/exodia.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-22 12:51:27.041513 exodia-1.0.1/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-22 12:51:04.000000 exodia-1.0.1/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 12:51:27.041224 exodia-1.0.1/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1230 2023-05-22 12:31:08.000000 exodia-1.0.1/tests/test_instance_creation.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1357 2023-05-22 12:50:34.000000 exodia-1.0.1/tests/test_validation.py
```

### Comparing `exodia-1.0.0/LICENSE` & `exodia-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exodia-1.0.0/README.md` & `exodia-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 
 ### EXODIA validation
 
 This library is heavily inspired by [Yup](https://github.com/jquense/yup) & [Joi](https://joi.dev/api/?v=17.9.1) in JavaScript.
 
+## Installation
+```shell
+pip install exodia
+```
+
+
+## Examples
+
 ```python
 import exodia as ex
 
 
 class Person:
     first_name = ex.String().required().max(250)
     last_name = ex.String().required().max(250)
```

### Comparing `exodia-1.0.0/exodia/fields.py` & `exodia-1.0.1/exodia/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,41 @@
 
     def __set_name__(self, owner, name):
         self._name = name
 
     def _add_validator(self, v: validators.Validator):
         for validator in self._validators:
             if validator == v:
-                raise ExodiaException("You can't have multiple validators of type {t}".format(
-                    t=v.__class__.__name__,
-                ))
+                raise ExodiaException(
+                    "You can't have multiple validators of type {t}".format(
+                        t=v.__class__.__name__,
+                    )
+                )
 
         self._validators.append(v)
 
     def _has_validator(self, v):
         return v in self._validators
 
-    def run_validators(self, field_name, value, instance):
+    def _run_validators(self, value, field_name=None, instance=None):
         for validator in self._validators:
-            validator(field_name, value, instance)
+            validator(value, field_name=field_name, instance=instance)
 
     def _no_validator_of_type(self, v):
         for validator in self._validators:
             if isinstance(validator, v):
-                raise ExodiaException("Can't have validators [{v1}, {v2}] at the same time".format(
-                    v1=validator.__class__.__name__,
-                    v2=v.__name__,
-                ))
+                raise ExodiaException(
+                    "Can't have validators [{v1}, {v2}] at the same time".format(
+                        v1=validator.__class__.__name__,
+                        v2=v.__name__,
+                    )
+                )
+
+    def validate(self, value):
+        self._run_validators(value)
 
     def optional(self):
         self._no_validator_of_type(validators.Required)
         self._add_validator(validators.Optional())
         return self
 
     def required(self):
@@ -55,15 +62,15 @@
         return self
 
     def enum(self, options):
         self._add_validator(validators.Enum(options))
         return self
 
     def __set__(self, instance, value):
-        self.run_validators(self._name, value, instance)
+        self._run_validators(value, self._name, instance)
         instance.__dict__[self._name] = value
 
     def __get__(self, instance, owner):
         return self.of_type(instance.__dict__[self._name])
 
 
 class String(Field):
@@ -79,14 +86,17 @@
         self._add_validator(validators.MinLength(value))
         return self
 
     def max(self, value: int):
         self._add_validator(validators.MaxLength(value))
         return self
 
+    def not_empty(self):
+        self._add_validator(validators.NotEmpty())
+
 
 class Integer(Field):
     of_type = int
 
     def min(self, value: int):
         self._add_validator(validators.MinValue(value))
         return self
@@ -100,20 +110,17 @@
         return self
 
     def multiple_of(self, n):
         self._add_validator(validators.MultipleOf(n))
         return self
 
 
-class List(Field):
+class List(String):
     of_type = list
 
-    def not_empty(self):
-        self._add_validator(validators.NotEmpty())
-
 
 class Func(Field):
     of_type = Callable
 
 
 class Exodia(Field):
     of_type = Mapping
```

### Comparing `exodia-1.0.0/tests/test_instance_creation.py` & `exodia-1.0.1/tests/test_instance_creation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import pytest
 import exodia as ex
 
 
 def test_same_validation_more_than_once():
     with pytest.raises(ex.ExodiaException):
         class TestClass:
-            my_number = ex.String().optional().optional()
+            _ = ex.String().optional().optional()
 
 
 def test_required_then_optional_should_fail():
     with pytest.raises(ex.ExodiaException):
         class TestClass:
-            my_x = ex.String().optional().required()
+            _ = ex.String().optional().required()
 
 
 def test_base_without_kwargs():
     class Klass(ex.Base):
         required_string = ex.String().required()
 
     with pytest.raises(ex.ExodiaException):
-        instance = Klass()
+        _ = Klass()
 
 
-def test_base_with_incorrect_kwargs():
+def test_base_with_missing_kwargs():
     class Klass(ex.Base):
         required_string = ex.String().required()
 
     with pytest.raises(ex.ExodiaException):
-        instance = Klass(name="LeOndaz")
+        _ = Klass(name="LeOndaz")
 
 
 def test_base_with_correct_kwargs():
     class Klass(ex.Base):
         required_string = ex.String().required()
 
-    instance = Klass(required_string="PASS")
+    _ = Klass(required_string="PASS")
+
+
+def test_instance_with_incorrect_kwargs():
+    class Klass(ex.Base):
+        required_string = ex.String().required()
+
+    with pytest.raises(ex.ExodiaException):
+        _ = Klass(required_string="LeOndaz", required_integer=1, required_func=2)
+
+
+def test_instantiate_base():
+    with pytest.raises(ex.ExodiaException):
+        _ = ex.Base()
```

### Comparing `exodia-1.0.0/tests/test_validation.py` & `exodia-1.0.1/tests/test_validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import pytest
 
-from exodia import ExodiaException
+import exodia as ex
+import exodia.validators as exv
 
 
 def test_put_invalid_choice(instance):
-    with pytest.raises(ExodiaException):
+    with pytest.raises(ex.ExodiaException):
         instance.size = 'MEDIUM'
 
 
 def test_put_valid_choice(instance):
     instance.choices = 'BIG'
     instance.choices = 'SMALL'
 
 
 def test_optional_field(instance):
     instance.last_name = None
 
 
 def test_required_field(instance):
-    with pytest.raises(ExodiaException):
+    with pytest.raises(ex.ExodiaException):
         instance.first_name = None
 
 
 def test_put_invalid_type(instance):
-    with pytest.raises(ExodiaException):
+    with pytest.raises(ex.ExodiaException):
         instance.first_name = 1
 
 
 def test_put_dict_with_all_keys(instance):
     instance.obj = {
         "name": "LeOndaz",
         "age": 23
     }
 
 
 def test_put_dict_with_missing_required_key(instance):
-    with pytest.raises(ExodiaException):
+    with pytest.raises(ex.ExodiaException):
         instance.obj = {
             "age": 23
         }
 
 
 def test_put_dict_with_missing_optional_key(instance):
     instance.obj = {
@@ -50,7 +51,15 @@
 def test_nested_object(instance):
     instance.nested_obj = {
         "nested": {
             "random": "yes",
             "age": 23
         }
     }
+
+
+def test_imperative_validation():
+    with pytest.raises(ex.ExodiaException):
+        ex.String().required().validate(None)
+
+    with pytest.raises(ex.ExodiaException):
+        ex.String().min(250).validate("STRING_LESS_THAN_250_CHARS")
```

