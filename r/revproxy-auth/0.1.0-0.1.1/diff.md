# Comparing `tmp/revproxy_auth-0.1.0.tar.gz` & `tmp/revproxy_auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.0.tar", last modified: Thu May 18 12:11:04 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.1.tar", last modified: Mon May 22 06:15:09 2023, max compression
```

## Comparing `revproxy_auth-0.1.0.tar` & `revproxy_auth-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:11:04.300763 revproxy_auth-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/data/test_result
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.395557 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.0/PKG-INFO` & `revproxy_auth-0.1.1/revproxy_auth.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 Metadata-Version: 2.1
-Name: revproxy_auth
-Version: 0.1.0
+Name: revproxy-auth
+Version: 0.1.1
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
-Description: # Authproxy
+Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
         Have you setup the reverse proxy in your synology NAS, but don´t want that everyone who knows your services´ URL can have access to your services?
         This repo will allow you to restrict the access from internet to your internal Api REST webservices, using the credentials and users that you have created in your Synology NAS.
         It will also request the OTP code if you have that configured in your NAS.
         
-        The steps are simple:
+        Configuration yml file will be place in the /home/var/{yourservicename}
         
-        1. You need to make available a new service inside your LAN with the authproxy.
-        2. You may want to include synology-revproxy-auth as part of you already existing services... no need to create an specific flask or any newwsgi just for this. Just make the API REST call available.
-        3. Configure the service so that it can redirect all the requests to the proper internal host & port.
-        4. Create all your entry points in the synology reverse procy menu, and make all of them point to the authproxy endpoint
+        Revproxy_auth can work in two mode:
+        
+        1. Embeded. You can embed the authentication by modifying your Flask based service:
+            self.app = Flask(__name__, template_folder=template_folder, static_folder=static_folder)
+            self.revproxy_auth = RevProxyAuth(self.app, root_class='yourservicename')
+            self.app.add_url_rule('/', 'index', self.main_endpoint, methods=['GET', 'POST'])
+            ...
+            def main_endpoint(self):
+                """ Main endpoint that returns the main page for your service
+                Returns:
+                    response: The main html content
+                """
+                return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
+        
+        2. Proxy
+            You need to make available a new service inside your LAN with the authproxy.
+            You may want to include revproxy-auth as part of you already existing services... no need to create an specific flask or any newwsgi just for this. Just make the API REST call available.
+            Configure the service in the config.yml so that it can redirect all the requests to the proper internal host & port.
+            Create all your entry points in the synology reverse proxy menu, and make all of them point to the authproxy endpoint
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.6
```

### Comparing `revproxy_auth-0.1.0/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.1/revproxy_auth/revproxy_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from urllib import parse
 import json
 from pathlib import Path
 import secrets
 import jinja2
 import requests
-from flask import Flask, request, Response, send_from_directory, redirect
+from flask import Flask, request, Response, send_from_directory, redirect, Request
 
 from config_yml import Config
 
 COOKIE_LIFE_MINUTES = 15
 
 HTTP_200_OK = 200
 HTTP_501_NOT_IMPLEMENTED = 501
@@ -65,95 +65,84 @@
         """ If valid auth token comes fromt he client, return none
             Otherwise, it will return a response so that the client opens again the Auth Popup
         Returns:
             Response: Http response with the auth popup, or 
                       None if auth request is not needed because already are authenticated
         """
         response = None
-        # Try to get authentication from the cookie
-        cookie_name = req.cookies.get('token', None)
-        print(f'Incomming Session token Cookie name: {cookie_name}')
 
-        if cookie_name and not req.form.get('auth', None):
-            # We get a session token... lets verify if its legitimate, and still alive
-            cookie = self._get_local_session_cookie(cookie_name)
-            if cookie: # Already authenticated --> Lets tunnel info back to client
-                print(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
-                response = callback()
-            else: # We got a session, but its no longer valid --> ask again for credentials
-                print(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
-                response = self._reask_credentials(self._get_request_dict(req.path), old_cookie_name=cookie_name)
-        else:  # Not authenticated yet... Two options:
-               # 1) We have to pop the authentication popup to the user
-               # 2) We already did, and we need to look for the auth info in the form to verify it
-            print('Not authenticated yet')
-            request_dict = self._get_request_dict(req.path)
-            session_cookie, session_cookie_name = self._auth_from_popup_data(request_dict)
+        if req.form.get('revproxy_auth', None):
+            print('Credentials validated by synology NAS')
+            session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
             if session_cookie_name:
                 # To get rid of the POST form data, and reenter with the valid session token
-                response = redirect(session_cookie['endpoint'])
+                response = redirect(parse.urljoin(session_cookie['host'], session_cookie['endpoint']))
                 response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else:
-                response = self._reask_credentials(request_dict)
+                response = self._reask_credentials(req)
+        else:
+            # Try to get authentication from the cookie
+            cookie_name = req.cookies.get('token', None)
+            print(f'Incomming Session token Cookie name: {cookie_name}')
+            if cookie_name:
+                # We get a session token... lets verify if its legitimate, and still alive
+                cookie = self._get_local_session_cookie(cookie_name)
+                if cookie: # Already authenticated --> Lets tunnel info back to client
+                    print(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
+                    response = callback()
+                else: # We got a session, but its no longer valid --> ask again for credentials
+                    print(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
+                    response = self._reask_credentials(req, old_cookie_name=cookie_name)
+            else:  # No session cookie... and no form data with credendials
+                response = self._reask_credentials(req)
 
         return response
 
     def path_redirect(self, path) -> Response:
         """Main entry point
         Returns:
             http_response: response string
         """
         print(f'---------------------- Path requested: {path} --------------------')
-        resp = self._path_redirect(self._get_request_dict(path))
+        resp = self._path_redirect(request)
         return resp
 
-    def _build_auth_cookie(self, req_dict: dict) -> tuple:
-        mapping_info = self._config['mapping'].get(req_dict['host'])
+    def _build_auth_cookie(self, req: Request) -> tuple:
+        mapping_info = self._config['mapping'].get(req.host)
         if not mapping_info:
             return None, None
 
         host = mapping_info.get('host')
         endpoint = mapping_info.get('endpoint')
         method = mapping_info.get('method')
-        params = req_dict['params']
 
         ser_head = {}
-        for head in req_dict['headers']:
+        for head in req.headers:
             ser_head[head[0]] = head[1]
         headers = json.dumps(ser_head)
 
         # Stores the internal URL into a cookie file to be read later
         cookie_name = secrets.token_urlsafe(16)
-        content = str(req_dict['data'])
+        content = str(req.data)
         cookie = {'host': host,
                   'endpoint': endpoint, 
                   'method': method,
-                  'params': params, 
+                  'params': req.query_string.decode("utf-8"), 
                   'headers': headers,
                   'content': content}
 
         return cookie, cookie_name
 
     def _build_session_cookie(self, auth_cookie: dict) -> tuple:
-        cookie = {'session': True,
-                  'endpoint': parse.urljoin(auth_cookie['host'], auth_cookie['endpoint'])
-                 }
+        # cookie = {'session': True,
+        #           'endpoint': parse.urljoin(auth_cookie['host'], auth_cookie['endpoint'])
+        #          }
+        cookie = auth_cookie
         return cookie, secrets.token_urlsafe(16)
 
-    def _get_request_dict(self, endpoint):
-        return {'host': request.host,
-                'endpoint': endpoint,
-                'method': request.method,
-                'params': request.query_string.decode("utf-8"),
-                'data': request.get_data(),
-                'headers': request.headers,
-                'cookies': request.cookies,
-                'form': request.form
-               }
-
     def _get_static_content(self, path: str):
         """Get revproxy_auth custom static content
         Args:
             path (str): Resource to be retrieved from revproxy_aut_static folder
 
         Returns:
             _type_: Resouce
@@ -194,15 +183,15 @@
         # Get the auth html form template and send back to the user, so he can authenticate
         form_path = os.path.join(Path(__file__).parent.resolve(), 'templates', 'form.html')
         with open(form_path, 'r', encoding="utf8") as form:
             buff = form.read()
             # replace the cookie name
             env = jinja2.Environment()
             template = env.from_string(buff)
-            content = template.render(auth=cookie_name)
+            content = template.render(revproxy_auth=cookie_name)
             return Response(content, status=HTTP_200_OK,  content_type='text/html')
 
     def _get_local_auth_cookie(self, cookie_name:str = None):
         cookie = None
         if cookie_name:
             cookie_path = os.path.join(self.auth_cookie_folder, cookie_name)
             if os.path.exists(cookie_path):
@@ -218,15 +207,15 @@
             cookie_path = os.path.join(self.session_cookie_folder, cookie_name)
             if os.path.exists(cookie_path):
                 with open(cookie_path, 'r', encoding="utf-8") as cookie_file:
                     cookie = json.load(cookie_file)
         return cookie
 
     def _credentials_valid(self, form):
-        token = form.get('auth', None)
+        token = form.get('revproxy_auth', None)
         if token:
             user = form.get('user', '').strip(' \t\n\r')
             password = form.get('password', '').strip(' \t\n\r')
             otp = form.get('OTP', '').strip(' \t\n\r')
             testing_credentials = self._config['testing_credentials']
             if not testing_credentials:
                 url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
@@ -252,113 +241,135 @@
         fullpath = parse.urljoin(host, endpoint)
         resp = requests.post(fullpath,
                              data = data,
                              headers = headers,
                              timeout=10)
         return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
-    def _reask_credentials(self, request_dict: dict, old_cookie_name: str = None) -> Response:
-        new_cookie, new_cookie_name = self._build_auth_cookie(request_dict)
+    def _reask_credentials(self, req: Request, old_cookie_name: str = None) -> Response:
+        new_cookie, new_cookie_name = self._build_auth_cookie(req)
         if not new_cookie: # Unable to build cookie for requested path: host unknown
-            return Response(request_dict['host'], status=HTTP_501_NOT_IMPLEMENTED, content_type='text/plain')
+            return Response(req.host, status=HTTP_501_NOT_IMPLEMENTED, content_type='text/plain')
             # return ApiRestResponse(request_dict['host'], status=501)
         print(f'Creating new auth cookie {new_cookie_name} and reasking to user...')
         self._write_cookie(new_cookie, self.auth_cookie_folder, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
-        # response.set_cookie('auth', new_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
         if old_cookie_name:
             print(f'Deleting cookie in response: {old_cookie_name}')
-            response.delete_cookie('auth',  request_dict['host'])
             self._clear_local_cookie(self.auth_cookie_folder, old_cookie_name)
         return response
 
-    def _auth_from_popup_data(self, request_dict) -> str:
+    def _creates_session_token_from_popup_data(self, req: Request) -> str:
+        """ Creates valid session token if valid credentials sent from the auth popup
+        Args:
+            req (Request): Request fro client... hopefully with valod auth credentials
+
+        Returns:
+            Tuple(dict, str): Dict with the new session cookie created (None if credentials invalid or not found)
+                              str with the name of the session cookie created
+        """
         session_cookie_name = None
         session_cookie = None
-        # cookie_name = request_dict['form'].get('token', None) if request_dict['form'].get('from_auth') else None
-        cookie_name = request_dict['form'].get('auth', None)
+        cookie_name = req.form.get('revproxy_auth', None)
         auth_cookie = self._get_local_auth_cookie(cookie_name)
         if auth_cookie:
-            if self._credentials_valid(request_dict['form']):
+            if self._credentials_valid(req.form):
                 print(f'Auth Local cookie {cookie_name} still alive and valid.')
                 session_cookie, session_cookie_name = self._build_session_cookie(auth_cookie)
                 print(f'Creating new session cookie {session_cookie_name} and reasking to user...')
                 self._write_cookie(session_cookie, self.session_cookie_folder, session_cookie_name)
             else:
                 print(f'Auth Local cookie {cookie_name} still alive but credentials are invalid.')
         else:
             print(f'Auth Local cookie {cookie_name} doesnt exist.')
         return session_cookie, session_cookie_name
 
-    def _first_auth_and_redirect(self, request_dict) -> Response:
-        cookie_name = request_dict['form'].get('auth', None)
+    def _first_auth_and_redirect(self, req: Request) -> Response:
+        cookie_name = req.form.get('revproxy_auth', None)
         cookie = self._get_local_auth_cookie(cookie_name)
         if cookie:
             print(f'Local cookie {cookie_name} still alive')
-            if self._credentials_valid(request_dict['form']):
+            if self._credentials_valid(req.form):
                 print('Credentials validated by synology NAS')
                 # Search for the cookie and redirect to related URL if present
                 if cookie['method'] == 'GET':
-                    response = self._call_inner_get(cookie['host'], cookie['endpoint'], cookie['params'], {})
+                    response = self._call_inner_get(cookie['host'], cookie['endpoint'], cookie['params'], cookie['headers'])
                 else:
-                    response = self._call_inner_post(cookie['host'], cookie['endpoint'], cookie['content'], {})
+                    response = self._call_inner_post(cookie['host'], cookie['endpoint'], cookie['content'], cookie['headers'])
                 response.set_cookie('token', cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else: # We come from the auth popup, but credentials are invalid --> ask again for credentials
                 print('Credentials rejected by synology NAS. Reopening auth popup')
                 response = self._build_auth_popup(cookie_name)
         else: # We got a token, but its no longer valid --> ask again for credentials
             print('Local cookie expired. Reopening auth popup')
-            response = self._reask_credentials(request_dict, cookie_name)
+            response = self._reask_credentials(req, cookie_name)
         return response
 
-    def _path_redirect(self, request_dict) -> Response:
+    def _path_redirect(self, req: Request) -> Response:
         """ Flask independent internal function
         Returns:
             http_response: response string
         """
-        if request_dict['endpoint'] == 'favicon.ico':
-            cookie, cookie_name = self._build_auth_cookie(request_dict)
+        if req.path == '/favicon.ico':
+            cookie, cookie_name = self._build_auth_cookie(req)
             if not cookie: # Unable to build cookie for requested path: host unknown
-                return Response(request_dict['host'], status=501, content_type='text/plain')
+                return Response(req.path, status=501, content_type='text/plain')
             print(f"favicon.ico requested: Directly returning from inner endpoint {cookie['host']}")
+            if req.url == parse.urljoin(cookie['host'], req.path):
+                return Response(req.path, status=400, content_type='text/plain')
             return self._call_inner_get(host=cookie['host'],
-                                        endpoint=request_dict['endpoint'],
-                                        params=request_dict['params'],
-                                        headers=request_dict['headers'])
-
-        if request_dict['endpoint'].startswith('revproxy_auth_static'):
-            return self._get_static_content(request_dict['endpoint'])
-
-        # Try to get authentication from the cookie
-        cookie_name = request_dict['cookies'].get('token', None)
-        print(f'Incomming Cookie name: {cookie_name}')
-        if cookie_name:  # We get a token... lets verify if its legitimate, and still alive
-            cookie = self._get_local_session_cookie(cookie_name)
-            if cookie: # Already authenticated --> Lets tunnel info back to client
-                print(f'AUTHENTICATED: Cookie {cookie_name} exists in local')
-                if request_dict['endpoint'] == '/': # If path is the root, lets go to the configured initial entrypoint.
-                    method = cookie['method']
-                    path = cookie['endpoint']
-                    headers = {}
+                                        endpoint=req.path,
+                                        params=req.query_string.decode("utf-8"),
+                                        headers=req.headers)
+
+        if req.path.startswith('revproxy_auth_static'):
+            return self._get_static_content(req.path)
+
+        if req.form.get('revproxy_auth', None):
+            session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
+            if session_cookie_name:
+                print('Credentials validated by synology NAS')
+                if session_cookie['method'] == 'GET':
+                    response = self._call_inner_get(session_cookie['host'], session_cookie['endpoint'], session_cookie['params'], {})
+                else:
+                    response = self._call_inner_post(session_cookie['host'], session_cookie['endpoint'], session_cookie['content'], {})
+                # # To get rid of the POST form data, and reenter with the valid session token
+                # response = redirect(session_cookie['endpoint'])
+                response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
+            else:
+                response = self._reask_credentials(req)
+        else:
+            # Try to get authentication from the cookie
+            cookie_name = req.cookies.get('token', None)
+            print(f'Incomming Session token Cookie name: {cookie_name}')
+            if cookie_name:
+                # We get a session token... lets verify if its legitimate, and still alive
+                cookie = self._get_local_session_cookie(cookie_name)
+                if cookie: # Already authenticated --> Lets tunnel info back to client
+                    print(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
+                    # response = callback()
+                    if req.path == '/': # If path is the root, lets go to the configured initial entrypoint.
+                        method = cookie['method']
+                        path = cookie['endpoint']
+                        headers = {}
+                        if method == 'GET':
+                            params = cookie['params']
+                        else:
+                            data = cookie['content']
+                    else:
+                        method = req.method
+                        path = req.path
+                        headers = req.headers
+                        params = req.query_string.decode("utf-8")
+                        data = req.data
+                    # Lets get the response from the internal host, and tunnel it back to client
                     if method == 'GET':
-                        params = cookie['params']
+                        response = self._call_inner_get(cookie['host'], path, params, headers)
                     else:
-                        data = cookie['content']
-                else:
-                    method = request_dict['method']
-                    path = request_dict['endpoint']
-                    headers = request_dict['headers']
-                    params = request_dict['params']
-                    data = request_dict['data']
-                # Lets get the response from the internal host, and tunnel it back to client
-                if method == 'GET':
-                    response = self._call_inner_get(cookie['host'], path, params, headers)
-                else:
-                    response = self._call_inner_post(cookie['host'], path, data, headers)
-            else: # We got a token, but its no longer valid --> ask again for credentials
-                print(f'NOT AUTHENTICATED: Cookie {cookie_name} DOESNT exist in local')
-                response = self._reask_credentials(request_dict, cookie_name)
-        else:  # Not authenticated yet... lets pop the authentication popup to the user
-            print('Not authenticated yet')
-            response = self._first_auth_and_redirect(request_dict)
-
+                        response = self._call_inner_post(cookie['host'], path, data, headers)
+                else: # We got a session, but its no longer valid --> ask again for credentials
+                    print(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
+                    response = self._reask_credentials(req, old_cookie_name=cookie_name)
+            else:  # No session cookie... and no form data with credendials
+                response = self._reask_credentials(req)
+      
         return response
```

### Comparing `revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.0/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.1/revproxy_auth/templates/form.html`

 * *Files 16% similar despite different names*

```diff
@@ -18,12 +18,12 @@
             </div>
             <div style="margin: 1px">
                 <input name = "OTP" type="text" placeholder="OTP Code" class="edit_text">
             </div>
             <div style="margin: 1px">
                 <input type="submit" value="Sign in" class="button_text">
             </div>
-            <input name = "auth" type="hidden" value="{{auth}}" id="auth">
+            <input name = "revproxy_auth" type="hidden" value="{{revproxy_auth}}" id="revproxy_auth">
         </form>  
   </div>
   </body>
 </html>
```

### Comparing `revproxy_auth-0.1.0/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1
-Name: revproxy-auth
-Version: 0.1.0
-Summary: Reverse proxy with synology authentication
-Home-page: https://github.com/Phornee/revproxy_auth
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # Authproxy
-        This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
-        Have you setup the reverse proxy in your synology NAS, but don´t want that everyone who knows your services´ URL can have access to your services?
-        This repo will allow you to restrict the access from internet to your internal Api REST webservices, using the credentials and users that you have created in your Synology NAS.
-        It will also request the OTP code if you have that configured in your NAS.
-        
-        The steps are simple:
-        
-        1. You need to make available a new service inside your LAN with the authproxy.
-        2. You may want to include synology-revproxy-auth as part of you already existing services... no need to create an specific flask or any newwsgi just for this. Just make the API REST call available.
-        3. Configure the service so that it can redirect all the requests to the proper internal host & port.
-        4. Create all your entry points in the synology reverse procy menu, and make all of them point to the authproxy endpoint
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# revproxy_auth
+This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
+Have you setup the reverse proxy in your synology NAS, but don´t want that everyone who knows your services´ URL can have access to your services?
+This repo will allow you to restrict the access from internet to your internal Api REST webservices, using the credentials and users that you have created in your Synology NAS.
+It will also request the OTP code if you have that configured in your NAS.
+
+Configuration yml file will be place in the /home/var/{yourservicename}
+
+Revproxy_auth can work in two mode:
+
+1. Embeded. You can embed the authentication by modifying your Flask based service:
+    self.app = Flask(__name__, template_folder=template_folder, static_folder=static_folder)
+    self.revproxy_auth = RevProxyAuth(self.app, root_class='yourservicename')
+    self.app.add_url_rule('/', 'index', self.main_endpoint, methods=['GET', 'POST'])
+    ...
+    def main_endpoint(self):
+        """ Main endpoint that returns the main page for your service
+        Returns:
+            response: The main html content
+        """
+        return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
+
+2. Proxy
+    You need to make available a new service inside your LAN with the authproxy.
+    You may want to include revproxy-auth as part of you already existing services... no need to create an specific flask or any newwsgi just for this. Just make the API REST call available.
+    Configure the service in the config.yml so that it can redirect all the requests to the proper internal host & port.
+    Create all your entry points in the synology reverse proxy menu, and make all of them point to the authproxy endpoint
```

### Comparing `revproxy_auth-0.1.0/setup.py` & `revproxy_auth-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.1.0",
+    version="0.1.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
     package_data={
         '': ['*.yml']
     },
     data_files=[
-        ('tests/data', ['tests/data/config.yml', 'tests/data/test_result']),
+        ('tests/data', ['tests/data/config.yml']),
         ('revproxy_auth/revproxy_auth_static/css/', ['revproxy_auth/revproxy_auth_static/css/view.css']),
         ('revproxy_auth/templates', ['revproxy_auth/templates/form.html'])
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `revproxy_auth-0.1.0/tests/test_000.py` & `revproxy_auth-0.1.1/tests/test_000.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ unittesting """
 import unittest
+from unittest.mock import Mock
 from pathlib import Path
 
 from flask import Flask, Response
 from bs4 import BeautifulSoup
 from revproxy_auth import RevProxyAuth
 
 
@@ -26,53 +27,46 @@
     def _test_endpoint(self) -> Response:
         return 'test response OK'
 
     def test_0000_w3_noauth(self):
         """ Test redirection to external site, without previously being authorized
             Response should be the content of the sign in popup itself
         """
-        mock_request = {'host': 'w3test.fakedomain.com',
-                        'method': 'GET',
-                        'endpoint': 'MarkUp/Test/HTML401/current/tests/sec5_3_1-BF-01.html',
-                        'headers': {},
-                        'params': '',
-                        'data': {},
-                        'cookies': {},
-                        'form': {}}
+        mock_request = Mock()
+        mock_request.host = 'w3test.fakedomain.com'
+        mock_request.method = 'GET'
+        mock_request.path ='MarkUp/Test/HTML401/current/tests/sec5_3_1-BF-01.html'
+        mock_request.headers = {}
+        mock_request.query_string = b''
+        mock_request.data = {}
+        mock_request.cookies = {}
+        mock_request.form = {}
 
         # Get response: as we are not authorized we should get the html of the sign in popup
         response = self.revproxy_auth._path_redirect(mock_request) # pylint: disable=protected-access
 
         self.__class__.auth_cookie_name = self._get_auth_cookie_name(response)
 
         self.assertEqual(response.status_code, 200)
         # Chech that it is indeed the popup
         self.assertTrue(response.data.decode('utf-8').startswith('<!--authproxy-->'))
 
     def test_0001_w3_auth(self):
         """ Test redirection to external site, being previously authorized
             We simulate the authorization by using the freshly created cookie from the previous test
         """
-        # mock_request = {'host': 'w3test.fakedomain.com',
-        #                 'method': 'GET',
-        #                 'endpoint': 'MarkUp/Test/HTML401/current/tests/5_3_1-BF-01.html',
-        #                 'headers': {},
-        #                 'params': '',
-        #                 'data': {},
-        #                 'cookies': {'token':self.__class__.auth_cookie_name},
-        #                 'form': {}}
-
-        mock_request = {'host': 'localhost',
-                        'method': 'GET',
-                        'endpoint': 'test/',
-                        'headers': {},
-                        'params': '',
-                        'data': {},
-                        'cookies': {'token':self.__class__.auth_cookie_name},
-                        'form': {}}
+        mock_request = Mock()
+        mock_request.host = 'localhost'
+        mock_request.method = 'GET'
+        mock_request.path ='test/'
+        mock_request.headers = {}
+        mock_request.query_string = b''
+        mock_request.data = {}
+        mock_request.cookies = {'token':self.__class__.auth_cookie_name}
+        mock_request.form = {}
 
         # Get response: as we are not authorized we should get the html of the sign in popup
         response = self.revproxy_auth._path_redirect(mock_request) # pylint: disable=protected-access
         self.assertEqual(response.status_code, 200)
 
         auth_cookie_name = self._get_auth_cookie_name(response)
         # We simulate the client action by sending back the right testing credentials.
@@ -84,15 +78,15 @@
         # Checks that it is indeed the result
         self.assertTrue(response.data.decode('utf-8') == 'test response OK')
 
 
     def _get_auth_cookie_name(self, resp: Response) -> str:
         html = resp.get_data().decode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
-        return soup.find(id='auth')['value']
+        return soup.find(id='revproxy_auth')['value']
 
     def _get_client_cookie(self, cookie_name: str) -> str:
         """ Get a incomming cookie from a http response
         Args:
             resp (Response): 
             cookie_name (str):
         Returns:
```

### Comparing `revproxy_auth-0.1.0/tests/test_001.py` & `revproxy_auth-0.1.1/tests/test_001.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,38 +28,33 @@
 
     def test_0000_integrated_noauth(self):
         """ Test integrated call with noauth
         """
         # Get response: as we are not authorized we should get the html of the sign in popup
         response = self.client.get('/')
 
-        # Gets the 'token' cookie if set by previous request
-        # for cookie in self.client.cookie_jar:
-        #     if cookie.name == 'auth':
-        #         self.__class__.auth_cookie_name = cookie.value
-
         self.assertEqual(response.status_code, 200)
 
         # Chech that it is indeed the popup
         self.assertTrue(response.data.decode('utf-8').startswith('<!--authproxy-->'))
 
         self.__class__.auth_cookie_name = self._get_auth_cookie_name(response)
         self.assertIsNotNone(self.__class__.auth_cookie_name, 'Cookie name was not send by server.')
 
         # We simulate the client action by sending back the right testing credentials.
         response = self.client.post('/', data={'user': ' pepe', # Note the leading space before pepe... should work
                                                'password': '123456',
                                                'OTP': '1234',
-                                               'auth': self.__class__.auth_cookie_name})
+                                               'revproxy_auth': self.__class__.auth_cookie_name})
 
         # We should get a redirect to the original endpoint after the authentication
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.location, 'http://localhost/')
 
-        # Follow redirection
+        # Simulate redirection
         response = self.client.get(response.location)
 
         self.assertTrue(response.data.decode('utf-8').startswith('test result OK'))
 
     def test_0001_integrated_auth(self):
         """ Test integrated, being previously authorized
             We simulate the authorization by using the freshly created cookie from the previous test
@@ -72,11 +67,11 @@
         self.assertEqual(response.status_code, 200)
         # We tried to fake session cookie, so we should get authproxy popup instead
         self.assertTrue(response.data.decode('utf-8').startswith('<!--authproxy-->'))
 
     def _get_auth_cookie_name(self, resp: Response) -> str:
         html = resp.get_data().decode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
-        return soup.find(id='auth')['value']
+        return soup.find(id='revproxy_auth')['value']
 
 if __name__ == '__main__':
     unittest.main()
```

