# Comparing `tmp/nsdotpy-1.3.2.tar.gz` & `tmp/nsdotpy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.3.2.tar", max compression
+gzip compressed data, was "nsdotpy-1.3.3.tar", max compression
```

## Comparing `nsdotpy-1.3.2.tar` & `nsdotpy-1.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-20 08:21:06.868322 nsdotpy-1.3.2/LICENSE.md
--rw-r--r--   0        0        0     2440 2023-05-20 08:21:06.868322 nsdotpy-1.3.2/README.md
--rw-r--r--   0        0        0      790 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/__init__.py
--rw-r--r--   0        0        0    44907 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/valid.py
--rw-r--r--   0        0        0      719 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-22 07:36:09.269865 nsdotpy-1.3.3/LICENSE.md
+-rw-r--r--   0        0        0     2440 2023-05-22 07:36:09.269865 nsdotpy-1.3.3/README.md
+-rw-r--r--   0        0        0      790 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    46894 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/valid.py
+-rw-r--r--   0        0        0      719 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.3/PKG-INFO
```

### Comparing `nsdotpy-1.3.2/LICENSE.md` & `nsdotpy-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.2/README.md` & `nsdotpy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.2/nsdotpy/__init__.py` & `nsdotpy-1.3.3/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.2/nsdotpy/session.py` & `nsdotpy-1.3.3/nsdotpy/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.3.2"
+        self.VERSION = "1.3.3"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -93,14 +93,15 @@
         # Initialize nationstates specific stuff
         self._auth_region = "rwby"
         self.chk: str = ""
         self.localid: str = ""
         self.pin: str = ""
         self.nation: str = ""
         self.region: str = ""
+        self.api_pin: str = ""
         self.current_page: tuple[str, str] = ("", "")
         self.keybind = keybind
         self.logger.info(f"Initialized. Keybind to continue is {self.keybind}.")
 
     def _set_user_agent(
         self,
         script_name: str,
@@ -336,35 +337,43 @@
             response = self._session.post(
                 url, data=data, follow_redirects=follow_redirects
             )
         self.current_page = (url, response.text)
         self._lock = False
         return response
 
-    def api_request(self, data: dict, _auth=()) -> httpx.Response:
+    def api_request(self, data: dict, password: str = "", _auth=()) -> httpx.Response:
         """Sends a request to the nationstates api with the given data.
 
         Args:
             data (dict): Payload to send with the request, e.g. {"nation": "testlandia", "q": "region"}
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "".
+            _auth (tuple, optional): The username and password to use for authentication to an alternative nationstates server. Defaults to ().
 
         Returns:
             httpx.Response: The response from the server
         """
         # TODO: probably move this responsibility to a third party api library to avoid reinventing the wheel
         # if one exists of sufficient quality thats AGPLv3 compatible
         data |= {"v": "12"}
         url = (
             f"https://www.nationstates{self._ns_server}.net/cgi-bin/api.cgi"
             if _auth
             else "https://www.nationstates.net/cgi-bin/api.cgi"
         )
+        if password:
+            self._session.headers["X-Password"] = password
+        if self.api_pin:
+            self._session.headers["X-Pin"] = self.api_pin
         # rate limiting section
         response = self._session.post(url, data=data, auth=_auth)
         # if the server tells us to wait, wait
         head = response.headers
+        if "X-Pin" in head:
+            self.api_pin = head["X-Pin"]
         if waiting_time := head.get("Retry-After"):
             self.logger.warning(f"Rate limited. Waiting {waiting_time} seconds.")
             time.sleep(int(waiting_time))
         # slow down requests so we dont hit the rate limit in the first place
         requests_left = int(head["RateLimit-Remaining"])
         seconds_until_reset = int(head["RateLimit-Reset"])
         # only slow down if we're close to the limit to avoid slowing down one off or infrequent requests
@@ -729,14 +738,52 @@
         if "?founded=new" not in response.headers["location"]:
             return False
         self._refresh_auth_values()
         return True
 
     # methods for region control
 
+    def create_region(
+        self,
+        region_name: str,
+        wfe: str,
+        *,
+        password: str = "",
+        frontier: bool = False,
+        executive_delegacy: bool = False,
+    ) -> bool:
+        """Creates a new region.
+
+        Args:
+            region_name (str): Name of the region
+            wfe (str): WFE of the region
+            password (str, optional): Password to the region. Defaults to "".
+            frontier (bool, optional): Whether or not the region is a frontier. Defaults to False.
+            executive_delegacy (bool, optional): Whether or not the region has an executive WA delegacy. Defaults to False. Ignored if frontier is True.
+
+        Returns:
+            bool: Whether the region was successfully created or not
+        """
+        self.logger.info(f"Creating new region {region_name}")
+        url = "https://www.nationstates.net/template-overall=none/page=create_region"
+        data = {
+            "page": "create_region",
+            "region_name": region_name,
+            "desc": wfe,
+            "create_region": "1",
+        }
+        if password:
+            data |= {"pw": "1", "rpassword": password}
+        if frontier:
+            data |= {"is_frontier": "1"}
+        elif executive_delegacy:
+            data |= {"delegate_control": "1"}
+        response = self.request(url, data)
+        return "Success! You have founded " in response.text
+
     def upload_to_region(self, type: str, filename: str) -> str:
         """Uploads a file to the current region.
 
         Args:
             type (str): Type of file to upload. Must be "flag" or "banner".
             filename (str): Name of the file to upload. e.g. "myflag.png"
 
@@ -809,15 +856,17 @@
             bool: True if successful, False otherwise
         """
         self.logger.info(f"Changing WFE for {self.region}")
         if not wfe:
             wfe = self._get_detag_wfe()  # haku im sorry for hitting your site so much
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
-            "message": wfe.encode("iso-8859-1", "xmlcharrefreplace").decode(),  # lol.
+            "message": wfe.encode("iso-8859-1", "xmlcharrefreplace")
+            .decode()
+            .strip(),  # lol.
             "setwfebutton": "1",
         }
         response = self.request(url, data)
         return "World Factbook Entry updated!" in response.text
 
     # methods for embassies
```

### Comparing `nsdotpy-1.3.2/nsdotpy/valid.py` & `nsdotpy-1.3.3/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.2/pyproject.toml` & `nsdotpy-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.3.2"
+version = "1.3.3"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.3.2/PKG-INFO` & `nsdotpy-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

