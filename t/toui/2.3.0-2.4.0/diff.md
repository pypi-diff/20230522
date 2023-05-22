# Comparing `tmp/toui-2.3.0.tar.gz` & `tmp/toui-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.3.0.tar", last modified: Sun May 21 08:43:28 2023, max compression
+gzip compressed data, was "toui-2.4.0.tar", last modified: Mon May 22 17:36:06 2023, max compression
```

## Comparing `toui-2.3.0.tar` & `toui-2.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.377112 toui-2.3.0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.3.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-21 08:43:28.377112 toui-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 08:43:27.926295 toui-2.3.0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.3.0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.3.0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:43:27.942813 toui-2.3.0/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.3.0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-21 08:43:28.377112 toui-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1635 2023-05-21 08:35:49.000000 toui-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.345535 toui-2.3.0/toui/
--rw-rw-rw-   0        0        0      266 2023-05-21 08:35:19.000000 toui-2.3.0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.3.0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.3.0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10987 2023-05-21 08:30:10.000000 toui-2.3.0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.3.0/toui/_signals.py
--rw-rw-rw-   0        0        0    27737 2023-05-21 08:22:11.000000 toui-2.3.0/toui/apps.py
--rw-rw-rw-   0        0        0    21814 2023-05-21 08:07:45.000000 toui-2.3.0/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.3.0/toui/exceptions.py
--rw-rw-rw-   0        0        0    18018 2023-05-21 08:27:48.000000 toui-2.3.0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.3.0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.369948 toui-2.3.0/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.858692 toui-2.4.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2994 2023-05-22 17:36:06.857692 toui-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.709721 toui-2.4.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.713919 toui-2.4.0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:36:06.859692 toui-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-05-21 08:35:49.000000 toui-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.846500 toui-2.4.0/toui/
+-rw-rw-rw-   0        0        0      266 2023-05-22 16:15:34.000000 toui-2.4.0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.4.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.4.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10611 2023-05-22 17:16:43.000000 toui-2.4.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.4.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    29077 2023-05-22 16:49:37.000000 toui-2.4.0/toui/apps.py
+-rw-rw-rw-   0        0        0    23003 2023-05-22 17:25:05.000000 toui-2.4.0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    18042 2023-05-22 17:32:38.000000 toui-2.4.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.856697 toui-2.4.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     2994 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.3.0/LICENSE` & `toui-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/PKG-INFO` & `toui-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.3.0
+Version: 2.4.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.3.0/README.md` & `toui-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/advanced_example_1_toui_blueprint.py` & `toui-2.4.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/example_1_simple_website.py` & `toui-2.4.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/example_2_simple_desktop_app.py` & `toui-2.4.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/example_3_updating_page.py` & `toui-2.4.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/example_4_function_with_arg.py` & `toui-2.4.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/examples/example_5_user_variables.py` & `toui-2.4.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/images/logo.png` & `toui-2.4.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/setup.py` & `toui-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/toui/_helpers.py` & `toui-2.4.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/toui/_javascript_templates.py` & `toui-2.4.0/toui/_javascript_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,28 +188,17 @@
                                               end: true})
             var dataSent = _send(jsonString)
         }
         reader.readAsText(file)
     }
 }
     
-function _getElement(kwargs) {
-    var number = 0
-    if ('number' in kwargs) {
-        var number = parseInt(kwargs['number'])
-    }
-    if ('parent' in kwargs) {
-        const parent = _getElement(kwargs['parent'])
-        const element = parent.querySelectorAll(kwargs['selector'])[number]
-        return element
-    } else {
-        const elements = document.querySelectorAll(kwargs['selector'])
-        const element = elements[number]
-        return element
-    }
+function _getElement(selector) {
+    const element = document.querySelector(selector)
+    return element
 }
 
 var _getElementSelector = function(el) {
   if (!(el instanceof Element))
             return;
         var path = [];
         while (el.nodeType === Node.ELEMENT_NODE) {
```

### Comparing `toui-2.3.0/toui/_signals.py` & `toui-2.4.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/toui/apps.py` & `toui-2.4.0/toui/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         name: str (optional)
             The name of the app.
 
         assets_folder: str (optional)
             The path to the folder that contains the HTML files and other assets.
 
         secret_key: str (optional)
-            Sets the `secret_key` attribute for `flask.Flask`
+            Sets the `secret_key` attribute for `flask.Flask`. You can also set the environment variable SECRET_KEY from
+            the command line and ToUI will get it using `os.environ`.
 
             
         Attributes
         ----------
         flask_app: Flask
             ToUI creates applications using `Flask`. You can access the `Flask` object using the attribute `flask_app`.
 
@@ -110,18 +111,21 @@
             if hasattr(__main__, "__file__"):
                 name = os.path.basename(__main__.__file__).split(".")[0]
             else:
                 name = "app"
         if not assets_folder:
             assets_folder = "/"
         self.flask_app = Flask(name, static_folder=assets_folder, static_url_path="/")
-        if secret_key is None:
+        if secret_key is not None:
+            self.flask_app.secret_key = secret_key
+        elif os.environ.get('SECRET_KEY') is not None:
+            self.flask_app.secret_key = os.environ.get('SECRET_KEY')
+        else:
             warn("No secret key was set. Generating a random secret key for Flask.")
-            secret_key = os.urandom(50)
-        self.flask_app.secret_key = secret_key
+            self.flask_app.secret_key = os.urandom(50)
         self.pages = []
         self._add_communication_method()
         self._add_user_vars()
         self.flask_app.route("/toui-download-<path_id>", methods=['POST', 'GET'])(self._download)
         self.forbidden_urls = ['/toui-communicate', "/toui-download-<path_id>"]
         self._validate_ws = validate_ws
         self._validate_data = validate_data
@@ -392,25 +396,53 @@
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
         user = self._user_cls.query.filter_by(username=username, password=password, **other_info).first()
         if user:
             login_user(user)
+            self._cache.set("user-id", user.id)
+            return True
+        else:
+            return False
+        
+    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
+    def signin_user_from_id(self, user_id, **other_info):
+        """
+        Loads the data of a user from database using the user's ID.
+
+        Parameters
+        ----------
+        id: int
+
+        other_info
+            Other information required for signing in.
+
+        Returns
+        -------
+        bool
+            ``True`` if the user is signed in, and ``False`` if it is not signed in.
+
+        """
+        self._confirm_user_database_created()
+        user = self._user_cls.query.filter_by(id=user_id, **other_info).first()
+        if user:
+            login_user(user)
+            self._cache.set("user-id", user_id)
             return True
         else:
             return False
 
-    @staticmethod
     @_ReqsChecker(['flask-login'])
-    def signout_user():
+    def signout_user(self):
         """
-        A static method that signs out the current user.
+        A method that signs out the current user.
         """
         logout_user()
+        self._cache.set('user-id', None)
 
     @_ReqsChecker(['flask-sqlalchemy'])
     def username_exists(self, username):
         """
         Checks if the username is exists in the database.
         
         Parameters
@@ -555,14 +587,18 @@
         """This is a private function."""
         try:
             session.keys()
         except RuntimeError as e:
             return False
         if not "user page" in session.keys():
             session['user page'] = None
+        if not "_user_id" in session.keys():
+            user_id = self._cache.get('user-id')
+            if user_id:
+                session['_user_id'] = user_id
         return True
     
     def _download(self, path_id):
         debug(f"PATH: {path_id}")
         file_to_download = self._cache.get(f'toui-download-{path_id}')
         debug(f"File to download: {file_to_download}")
         if file_to_download:
@@ -614,15 +650,15 @@
             debug(f"TIME: {e - s}s")
 
     def _confirm_user_database_created(self):
         if self._user_cls is None:
             raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database`.")
 
     def _load_user(self, user_id):
-        return self._user_cls.get(int(user_id))
+        return self._user_cls.query.filter_by(id=int(user_id)).first()
 
 
 class _FuncWithPage:
     """Currently this class is unused, but it might be used later."""
     def __init__(self, func, page):
         self.func = func
         self.page = page
```

### Comparing `toui-2.3.0/toui/elements.py` & `toui-2.4.0/toui/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     These signals are related the methods of the `Element` object.
     """
 
     @staticmethod
     def _default_kwargs(kwargs):
         original_copy = kwargs['original_copy']
-        return {"selector": original_copy._selector}
+        return {"selector": original_copy.get_unique_selector()}
 
     @staticmethod
     def from_str(**kwargs):
         js_func = "_replaceElement"
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['element'] = kwargs['element_as_str']
@@ -105,16 +105,14 @@
     <button name="button-name">Click me</button>
 
     """
 
     def __init__(self, tag_name="div"):
         self._element = Tag(name=tag_name)
         self._parent_page = None
-        self._parent_element =None
-        self._selector = {}
         self._signal_mode = False
         self._functions = {}
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
@@ -208,17 +206,14 @@
         element = Element()
         if do_copy:
             element.from_bs4_tag(bs4_tag)
         else:
             element._from_bs4_tag_no_copy(bs4_tag)
         element._signal_mode = self._signal_mode
         element._parent_page = self._parent_page
-        element._parent_element = self
-        element._selector = {"selector": f"[id={element_id}]",
-                             "parent": self._selector}
         return element
 
     def get_elements(self, tag_name=None, class_name=None, name=None, do_copy=False, attrs=None):
         """
         Get children elements by their tag name and attributes.
 
         Parameters
@@ -256,36 +251,92 @@
             element = Element()
             if do_copy:
                 element.from_bs4_tag(bs4_tag)
             else:
                 element._from_bs4_tag_no_copy(bs4_tag)
             element._signal_mode = self._signal_mode
             element._parent_page = self._parent_page
-            element._parent_element = self
-            element._selector = {"selector": selector_to_str(tag_name=tag_name, class_name=class_name,
-                                                             name=name, attrs=attrs),
-                                 "number": tag_num,
-                                 "parent": self._selector}
             elements_list.append(element)
         return elements_list
     
+    def get_parent(self, do_copy=False) -> 'Element':
+        """
+        Gets the parent element.
+
+        Parameters
+        ----------
+        do_copy: bool, default = False
+            If ``True``, the element will be copied.
+
+        Returns
+        -------
+        element: Element
+            If a parent was found, an `Element` object will be returned.
+
+        None
+            If a parent was not found.
+
+        """
+        bs4_tag = self._element.parent
+        if not isinstance(bs4_tag, Tag):
+            return None
+        element = Element()
+        if do_copy:
+            element.from_bs4_tag(bs4_tag)
+        else:
+            element._from_bs4_tag_no_copy(bs4_tag)
+        element._signal_mode = self._signal_mode
+        element._parent_page = self._parent_page
+        return element
+    
     def get_selector(self) -> str:
         """
         Gets the CSS selector of an element.
 
         Returns
         -------
         str
 
         None:
             If the element is not part of a page.
 
         """
         selector = self._element.name + ''.join([f'[{attr}="{value}"]' for attr, value in self._element.attrs.items()])
         return selector
+    
+    def get_unique_selector(self):
+        """
+        Gets the unique CSS selector of an element.
+
+        Returns
+        -------
+        str
+
+        None:
+            If the element is not part of a page.
+
+        """
+        element = self._element
+        path = []
+        while element is not None and element.name != "[document]":
+            selector = element.name.lower()
+
+            if element.get('id'):
+                selector += '#' + element['id']
+                path.insert(0, selector)
+                break
+            else:
+                index = [child for child in element.parent.children if child.name == element.name].index(element) + 1
+                if index != 1:
+                    selector += ":nth-of-type(" + str(index) + ")"
+
+            path.insert(0, selector)
+            element = element.parent
+
+        return ' > '.join(path)
 
     def get_attr(self, name):
         """
         Gets the value of an HTML element attribute.
 
         Parameters
         ----------
```

### Comparing `toui-2.3.0/toui/pages.py` & `toui-2.4.0/toui/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,15 +283,14 @@
         element = Element()
         if do_copy:
             element.from_bs4_tag(bs4_tag)
         else:
             element._from_bs4_tag_no_copy(bs4_tag)
         element._parent_page = self
         element._signal_mode = self._signal_mode
-        element._selector = {"selector": f"[id={element_id}]"}
         return element
 
     def get_elements(self, tag_name=None, class_name=None, name=None, do_copy=False, attrs=None):
         """
         Get elements from the `Page` by their tag name and attributes.
 
         Parameters
@@ -329,17 +328,14 @@
             element = Element()
             if do_copy:
                 element.from_bs4_tag(bs4_tag)
             else:
                 element._from_bs4_tag_no_copy(bs4_tag)
             element._parent_page = self
             element._signal_mode = self._signal_mode
-            element._selector = {"selector": selector_to_str(tag_name=tag_name, class_name=class_name,
-                                                             name=name, attrs=attrs),
-                                 "number": tag_num}
             elements_list.append(element)
         return elements_list
     
     def get_element_from_selector(self, selector, do_copy=False):
         """
         Gets an element from its CSS selector.
 
@@ -363,15 +359,14 @@
         element = Element()
         if do_copy:
             element.from_bs4_tag(bs4_tag)
         else:
             element._from_bs4_tag_no_copy(bs4_tag)
         element._parent_page = self
         element._signal_mode = self._signal_mode
-        element._selector = {"selector": selector}
         return element
 
     def get_html_element(self) -> Element:
         """
         Gets the first ``<html>`` element.
 
         Returns
@@ -472,21 +467,31 @@
             If ``True``, the browser will display the return value of the function when the URL is loaded. If ``False``,
             the return value will be ignored.
 
         """
         def new_func():
             original_return = self._basic_view_func()
             session['user page'] = copy(self)
-            new_return = func()
-            if display_return_value:
-                return new_return
-            else:
-                pg = session['user page']
-                del session['user page']
-                return pg.to_str()
+            try:
+                user_id = self._app._cache.get("user-id")
+                if user_id:
+                    session['_user_id'] = user_id
+                new_return = func()
+                if display_return_value:
+                    del session['user page']
+                    return new_return
+                else:
+                    pg = session['user page']
+                    del session['user page']
+                    return pg.to_str()
+            except Exception as e:
+                if 'user page' in session:
+                    del session['user page']
+                raise e
+
         self._view_func = new_func
 
     def get_window(self):
         for window in webview.windows:
             if window.uid == self._uid:
                 return window
```

### Comparing `toui-2.3.0/toui/structure.py` & `toui-2.4.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.3.0/toui.egg-info/PKG-INFO` & `toui-2.4.0/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.3.0
+Version: 2.4.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.3.0/toui.egg-info/SOURCES.txt` & `toui-2.4.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

