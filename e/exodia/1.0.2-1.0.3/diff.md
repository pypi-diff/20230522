# Comparing `tmp/exodia-1.0.2.tar.gz` & `tmp/exodia-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exodia-1.0.2.tar", last modified: Mon May 22 16:11:06 2023, max compression
+gzip compressed data, was "exodia-1.0.3.tar", last modified: Mon May 22 16:36:33 2023, max compression
```

## Comparing `exodia-1.0.2.tar` & `exodia-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:11:06.100032 exodia-1.0.2/
--rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.2/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:11:06.099918 exodia-1.0.2/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     3962 2023-05-22 15:01:07.000000 exodia-1.0.2/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:11:06.098921 exodia-1.0.2/exodia/
--rw-r--r--   0 leondaz    (501) staff       (20)      185 2023-05-22 13:06:40.000000 exodia-1.0.2/exodia/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1396 2023-05-22 13:06:40.000000 exodia-1.0.2/exodia/bases.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.2/exodia/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     4321 2023-05-22 16:06:17.000000 exodia-1.0.2/exodia/fields.py
--rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.2/exodia/utils.py
--rw-r--r--   0 leondaz    (501) staff       (20)     8210 2023-05-22 16:10:06.000000 exodia-1.0.2/exodia/validators.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:11:06.099357 exodia-1.0.2/exodia.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:11:06.000000 exodia-1.0.2/exodia.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-22 16:11:06.000000 exodia-1.0.2/exodia.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-22 16:11:06.000000 exodia-1.0.2/exodia.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-22 16:11:06.000000 exodia-1.0.2/exodia.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-22 16:11:06.100072 exodia-1.0.2/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-22 16:10:35.000000 exodia-1.0.2/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:11:06.099735 exodia-1.0.2/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.2/tests/test_instance_creation.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1339 2023-05-22 15:35:15.000000 exodia-1.0.2/tests/test_validation.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455678 exodia-1.0.3/
+-rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.3/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:36:33.455571 exodia-1.0.3/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     3962 2023-05-22 15:01:07.000000 exodia-1.0.3/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.454757 exodia-1.0.3/exodia/
+-rw-r--r--   0 leondaz    (501) staff       (20)      185 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1396 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/bases.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     4294 2023-05-22 16:30:32.000000 exodia-1.0.3/exodia/fields.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.3/exodia/utils.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     8516 2023-05-22 16:30:32.000000 exodia-1.0.3/exodia/validators.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455180 exodia-1.0.3/exodia.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-22 16:36:33.455711 exodia-1.0.3/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-22 16:36:17.000000 exodia-1.0.3/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455416 exodia-1.0.3/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.3/tests/test_instance_creation.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1629 2023-05-22 16:35:33.000000 exodia-1.0.3/tests/test_validation.py
```

### Comparing `exodia-1.0.2/LICENSE` & `exodia-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exodia-1.0.2/README.md` & `exodia-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `exodia-1.0.2/exodia/bases.py` & `exodia-1.0.3/exodia/bases.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.2/exodia/exceptions.py` & `exodia-1.0.3/exodia/exceptions.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.2/exodia/fields.py` & `exodia-1.0.3/exodia/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,16 @@
         return self
 
     def required(self):
         self._no_validator_of_type(validators.Optional)
         self._add_validator(validators.Required())
         return self
 
-    def custom(self, v):
-        self._no_validator_of_type(v)
-        # check validity of v
-        self._add_validator(v)
+    def function(self, f, message):
+        self._add_validator(validators.Function(f, message))
         return self
 
     def enum(self, options):
         self._add_validator(validators.Enum(options))
         return self
 
     def __set__(self, instance, value):
```

### Comparing `exodia-1.0.2/exodia/validators.py` & `exodia-1.0.3/exodia/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,19 @@
             values.append(getattr(self, parameter))
 
         format_params = dict(zip(parameter_names, values))
         format_params.update({"class_name": self.__class__.__name__})
 
         return format_params
 
+    def get_message(self, field_name):
+        return self.field_message if field_name else self.generic_message
+
     def fail(self, field_name=None, value=None, **kw):
-        message = self.field_message if field_name else self.generic_message
+        message = self.get_message(field_name)
 
         raise ExodiaException(
             message.format(
                 field_name=field_name,
                 value=value,
                 **kw,
             )
@@ -129,17 +132,14 @@
         self.ts = ts
         super().__init__()
 
     def merge(self, v):
         return self.__class__(ts=self.ts + v.ts)
 
     def validate(self, value, field_name=None, instance=None):
-        print("33333333333")
-        print(self.ts)
-        print("33333333333")
         return isinstance(value, tuple(self.ts))
 
     def get_format_params(self, value):
         return dict(
             **super().get_format_params(value),
             actual_type=type(value).__name__,
             expected_types=", ".join(item.__class__.__name__ for item in self.ts),
@@ -255,7 +255,20 @@
             if isinstance(v, self.__class__):  # is another Exodia
                 self(key, item, instance)
             else:  # is a Field object
                 v._run_validators(item, "{}.".format(field_name) + key, instance)
 
     def __call__(self, value, field_name=None, instance=None):
         self._recursive_validate_schema(value, field_name, instance)
+
+
+class Function(Validator):
+    def __init__(self, f, message):
+        self.f = f
+        self.message = message
+        super().__init__()
+
+    def get_message(self, field_name):
+        return self.message
+
+    def validate(self, value, field_name=None, instance=None):
+        return self.f(value)
```

### Comparing `exodia-1.0.2/tests/test_instance_creation.py` & `exodia-1.0.3/tests/test_instance_creation.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.2/tests/test_validation.py` & `exodia-1.0.3/tests/test_validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,7 +51,17 @@
 
 def test_imperative_validation():
     with pytest.raises(ex.ExodiaException):
         ex.String().required().validate(None)
 
     with pytest.raises(ex.ExodiaException):
         ex.String().min(250).validate("STRING_LESS_THAN_250_CHARS")
+
+
+def test_custom_validation():
+    with pytest.raises(ex.ExodiaException):
+        ex.String().function(lambda v: len(v) >= 2, "value has len smaller than 2").validate("A")
+
+    # which is equivalent to
+
+    with pytest.raises(ex.ExodiaException):
+        ex.String().min(2).validate('A')
```

