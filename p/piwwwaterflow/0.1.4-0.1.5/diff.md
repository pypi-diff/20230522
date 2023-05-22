# Comparing `tmp/piwwwaterflow-0.1.4.tar.gz` & `tmp/piwwwaterflow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.4.tar", last modified: Mon May  8 07:10:28 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.5.tar", last modified: Mon May 22 06:30:33 2023, max compression
```

## Comparing `piwwwaterflow-0.1.4.tar` & `piwwwaterflow-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.452219 piwwwaterflow-0.1.5/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:30:33.000000 piwwwaterflow-0.1.5/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:33.456219 piwwwaterflow-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:30:24.000000 piwwwaterflow-0.1.5/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.4/PKG-INFO` & `piwwwaterflow-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.4
+Version: 0.1.5
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.1.5/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.1.5/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.1.5/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.1.5/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.1.5/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.1.5/piwwwaterflow/static/js/code.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -77,14 +77,20 @@
         }
     }
 }
 
 socket.on('connect', function() {
     update(true);
 });
+
+socket.on('disconnect', function() {
+    document.cookie = "token=; expires=Thu, 01 Jan 1970 00:00:00 UTC; ";
+    location.reload();
+});
+
 setInterval("update(false);", 30000);
 
 function update(first_time) {
     socket.emit('service_request', function service(response) {
         // Version label update
         var versionlabel = document.getElementById('version');
         frontend = '1.4.0'
@@ -225,15 +231,15 @@
         _setEnableForceTriggers(false)
     } else {
         control.checked = false
     }
 }
 
 function stopWaterflow(button) {
-    socket.emit('stop', {});
+    socket.emit('stop');
     button.disabled = true;
 }
 
 function save(button) {
     socket.emit('save', {
         'prog1': {
             'time': document.getElementById("time1").value,
```

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.1.5/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.5/piwwwaterflow/webservice.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 """ Webservice to control and manage the piwaterflow loop """
 from datetime import datetime
 
-from flask import Flask, render_template
+from flask import Flask, render_template, request
 from flask_compress import Compress
 from flask_socketio import SocketIO
 from importlib_metadata import version, PackageNotFoundError
 
 from piwaterflow import Waterflow
+from revproxy_auth import RevProxyAuth
 
 
 class PiWWWaterflowService:
     """Class for the web service... its an interface to the real functionality in piwaterflow package.
     """
     def __init__(self,  template_folder, static_folder):
         self.waterflow = Waterflow()
 
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
-        self.app.add_url_rule('/', 'index', self.waterflow_endpoint, methods=['GET'])
+        self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
+
+        self.app.add_url_rule('/', 'index', self.waterflow_endpoint, methods=['GET', 'POST'])
         Compress(self.app)
         self.socketio = SocketIO(self.app)
         self.socketio.on_event('service_request', self.on_service_request)
         self.socketio.on_event('force', self.on_force)
         self.socketio.on_event('stop', self.on_stop)
         self.socketio.on_event('save', self.on_save)
 
     def get_app(self):
+        """ Returns WSGI app
+        Returns:
+            WSGI app:
+        """
         return self.app
 
-    def get_socket_app(self):
-        return self.socketio
-
     def run(self):
         # self.app.run()
         self.socketio.run(self.app)
 
     def waterflow_endpoint(self):
         """ Main endpoint that returns the main page for piwaterflow
         Returns:
             response: The main html content
         """
-        return render_template('form.html')
-
-
-    def _get_public_config(self):
-        config = self.waterflow.config.get_dict_copy()
-        del config['influxdbconn']
-        return config
+        return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
 
     def on_service_request(self) -> dict:
         """ Gets all the information from the waterflow service
         Args:
             data (dict):'first_time': This value is only bypassed to the caller
         Returns:
             dict:Dictionary with all the information about the status of the waterflow system
@@ -79,33 +77,39 @@
                          'value': Must be the index of the program or value to be forced
         """
         print(f'Force requested... {data}')
         type_force = data['type']
         value_force = data['value']
         self.waterflow.force(type_force, int(value_force))
 
-    def on_stop(self, data):
+    def on_stop(self):
+        """ Event to stop current operation """
         print('Stop requested...')
         self.waterflow.stop()
 
-    def _changeProgram(self, program, new_program):
-        inputbox_text = new_program['time']
-        time1 = datetime.strptime(inputbox_text, '%H:%M')
-        new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
-        program['start_time'] = new_datetime
-        program['valves_times']['valve1'] = new_program['valve1']
-        program['valves_times']['valve2'] = new_program['valve2']
-        program['enabled'] = new_program['enabled'] is not None
-
     def on_save(self, data):
         """ Event to save the changes in the watering system schedulling
         Args:
             data (dict): Information about the required schedulling
         Returns:
-            _type_: _description_
+            bool: If everything went ok
         """
         parsed_config = self.waterflow.config.get_dict_copy()
-        self._changeProgram(parsed_config['programs']['first'], data['prog1'])
-        self._changeProgram(parsed_config['programs']['second'], data['prog2'])
+        self._change_program(parsed_config['programs']['first'], data['prog1'])
+        self._change_program(parsed_config['programs']['second'], data['prog2'])
 
         self.waterflow.update_config(programs=parsed_config['programs'])
         return True
+
+    def _get_public_config(self):
+        config = self.waterflow.config.get_dict_copy()
+        del config['influxdbconn']
+        return config
+
+    def _change_program(self, program, new_program):
+        inputbox_text = new_program['time']
+        time1 = datetime.strptime(inputbox_text, '%H:%M')
+        new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
+        program['start_time'] = new_datetime
+        program['valves_times']['valve1'] = new_program['valve1']
+        program['valves_times']['valve2'] = new_program['valve2']
+        program['enabled'] = new_program['enabled'] is not None
```

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.5/piwwwaterflow/wsgi.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,18 @@
        Webservice class instantiated
     """
     templates_path = os.path.join(Path(__file__).parent.resolve(), 'templates')
     static_path = os.path.join(Path(__file__).parent.resolve(), 'static')
     return PiWWWaterflowService(template_folder=templates_path, static_folder=static_path)
 
 def create_app():
-    """ WSGI standard
-    Args:
-        environ (_type_): _description_
-        start_response (_type_): _description_
+    """ Creates a WSGI standard callable function
     Returns:
-        WSGI app
+        WSGI app provided by the PiWWWaterflowService/Flask
     """
     wtf_service = create_service()
-    return wtf_service.get_socket_app()
+    return wtf_service.get_app()
 
 # __main__ used for standalone execution (debugging). For WSGI call, the "wsgi:create_app()" function should be called
 if __name__ == '__main__':
     service = create_service()
     service.get_socket_app().run(service.app, host='0.0.0.0', port=5000, debug=True, use_reloader=False)
```

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.5/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.4
+Version: 0.1.5
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.4/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.1.5/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.4/setup.py` & `piwwwaterflow-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.4",
+    version="0.1.5",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -24,11 +24,12 @@
     install_requires=[
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'python-socketio>=5.8.0',
         'flask-socketio>=5.3.3',
         'eventlet>=0.33.3',
-        'piwaterflow>=0.5.2'
+        'piwaterflow>=0.5.4',
+        'revproxy_auth>=0.1.1'
     ],
     python_requires='>=3.6',
 )
```

