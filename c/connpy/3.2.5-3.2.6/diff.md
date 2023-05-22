# Comparing `tmp/connpy-3.2.5.tar.gz` & `tmp/connpy-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.5.tar", last modified: Thu May 18 21:28:32 2023, max compression
+gzip compressed data, was "connpy-3.2.6.tar", last modified: Mon May 22 21:33:59 2023, max compression
```

## Comparing `connpy-3.2.5.tar` & `connpy-3.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:28:32.090690 connpy-3.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 21:28:19.000000 connpy-3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-18 21:28:32.090690 connpy-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-18 21:28:19.000000 connpy-3.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:28:32.090690 connpy-3.2.5/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21014 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-18 21:28:19.000000 connpy-3.2.5/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:28:32.090690 connpy-3.2.5/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 21:28:32.000000 connpy-3.2.5/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-18 21:28:32.090690 connpy-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 21:28:19.000000 connpy-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.711212 connpy-3.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 21:33:47.000000 connpy-3.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 21:33:59.711212 connpy-3.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-22 21:33:47.000000 connpy-3.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.707212 connpy-3.2.6/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21366 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.707212 connpy-3.2.6/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-22 21:33:59.711212 connpy-3.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 21:33:47.000000 connpy-3.2.6/setup.py
```

### Comparing `connpy-3.2.5/LICENSE` & `connpy-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/PKG-INFO` & `connpy-3.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.5
+Version: 3.2.6
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.5/README.md` & `connpy-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/__init__.py` & `connpy-3.2.6/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/ai.py` & `connpy-3.2.6/connpy/ai.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,57 +58,64 @@
         else:
             try: 
                 openai.api_key = self.config.config["openai"]["api_key"]
             except:
                 raise ValueError("Missing openai api_key")
         self.__prompt = {}
         self.__prompt["original_system"] = """
-            When provided with user input for an SSH connection management application, analyze the input and extract the following information:
+            You are the AI assistant of a network connection manager and automation app called connpy. When provided with user input analyze the input and extract the following information:
 
-            - app_related: True if the input is related to the application's purpose and the request is understood; False if the input is not related, not understood, or if mandatory information like filter is missing.
+            - app_related: True if the input is related to the application's purpose and the request is understood; False if the input is not related, not understood, or if mandatory information like filter is missing. If user ask information about the app it should be false 
             - type: Given a user input, identify the type of request they want to make. The input will represent one of two options: 
-            1. "command" - The user wants to get information from devices by running commands.
-            2. "list_nodes" - The user wants to get a list of nodes, devices, servers, or routers.
-            Response wich command or list_nodes type depending on the request.
+
+                1. "command" - The user wants to get information from devices by running commands.
+                2. "list_nodes" - The user wants to get a list of nodes, devices, servers, or routers.
+                The 'type' field should reflect whether the user input is a command or a request for a list of nodes.
+
             - filter: One or more regex patterns indicating the device or group of devices the command should be run on, returned as a Python list (e.g., ['hostname', 'hostname@folder', '@subfolder@folder']). The filter can have different formats, such as:
                 - hostname
                 - hostname@folder
                 - hostname@subfolder@folder
                 - partofhostname
                 - @folder
                 - @subfolder@folder
                 - regex_pattern
+
                 The filter should be extracted from the user input exactly as it was provided.
                 Always preserve the exact filter pattern provided by the user, with no modifications. Do not process any regex, the application can do that.
                 If no filter is specified, set it to None.
-            - Expected: A value representing an expected output to search for when running the command. For the user this is a optional value. Set it to 'None' if no value was captured.
-              expected value should ALWAYS come from the user input explicitly.
+
+            - Expected: This field represents an expected output to search for when running the command. It's an optional value for the user.
+Set it to 'None' if no value was captured.
+The expected value should ALWAYS come from the user input explicitly.
+Users will typically use words like verify, check, make sure, or similar to refer to the expected value.
+
             - response: An optional field to be filled when app_related is False or when providing an explanation related to the app. This is where you can engage in small talk, answer questions not related to the app, or provide explanations about the extracted information.
-                
+            
             Always respond in the following format:
                 
                 app_related: {{app_related}}
                 Type: {{command}}
                 Filter: {{filter}}
                 Expected: {{expected}}
                 Response: {{response}}
     """ 
         self.__prompt["original_user"] = "Get the IP addresses of loopback0 for all routers from w2az1 and e1.*(prod|dev) and check if they have the ip 192.168.1.1"
         self.__prompt["original_assistant"] = "app_related: True\nType: Command\nFilter: ['w2az1', 'e1.*(prod|dev)']\nExpected: 192.168.1.1"
         self.__prompt["command_system"] = """
         For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server). Always format your response as a Python list (e.g., ['command1', 'command2']). 
 
-        It's very important to note: If a user has provided a specific command to be run, you should include that command exactly as provided, even if it's not recognized or understood. No alterations should be made to the user-provided commands under any circumstances. 
-
         The application knows how to connect to devices via SSH, so you only need to provide the command(s) to run after connecting. 
 
         If the commands needed are not for the specific OS type, just send an empty list (e.g., []). 
 
         It is crucial to always include the device name provided in your response, even when there is only one device.
 
+        Note: Preserving the integrity of user-provided commands is of utmost importance. If a user has provided a specific command to run, include that command exactly as it was given, even if it's not recognized or understood. Under no circumstances should you modify or alter user-provided commands.
+
         Your response has to be always like this:
             node1: ["command1", "command2"]
             node2: ["command1", "command2", "command3"]
             node1@folder: ["command1"]
             Node4@subfolder@folder: []
     """
         self.__prompt["command_user"]= """
@@ -225,17 +232,17 @@
                 os_value = tags.get('os', '')
             except:
                 os_value = ""
             output_list.append(f"{key}: {os_value}")
         output_str = "\n".join(output_list)
         command_input = f"input: {user_input}\n\nDevices:\n{output_str}"
         message = []
-        message.append({"role": "system", "content": dedent(self.__prompt["command_system"])})
-        message.append({"role": "user", "content": dedent(self.__prompt["command_user"])})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["command_assistant"])})
+        message.append({"role": "system", "content": dedent(self.__prompt["command_system"]).strip()})
+        message.append({"role": "user", "content": dedent(self.__prompt["command_user"]).strip()})
+        message.append({"role": "assistant", "content": dedent(self.__prompt["command_assistant"]).strip()})
         message.append({"role": "user", "content": command_input})
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
             temperature=self.temp
             )
         output = {}
@@ -243,17 +250,17 @@
         output["raw_response"] = response["choices"][0]["message"]["content"] 
         output["response"] = self._clean_command_response(output["raw_response"])
         return output
 
     def _get_filter(self, user_input, chat_history = None):
         #Send the request to identify the filter and other attributes from the user input to GPT.
         message = []
-        message.append({"role": "system", "content": dedent(self.__prompt["original_system"])})
-        message.append({"role": "user", "content": dedent(self.__prompt["original_user"])})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["original_assistant"])})
+        message.append({"role": "system", "content": dedent(self.__prompt["original_system"]).strip()})
+        message.append({"role": "user", "content": dedent(self.__prompt["original_user"]).strip()})
+        message.append({"role": "assistant", "content": dedent(self.__prompt["original_assistant"]).strip()})
         if not chat_history:
             chat_history = []
         chat_history.append({"role": "user", "content": user_input})
         message.extend(chat_history)
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
@@ -269,17 +276,17 @@
         clear_response = self._clean_original_response(output["raw_response"])
         output["response"] = self._clean_original_response(output["raw_response"])
         return output
         
     def _get_confirmation(self, user_input):
         #Send the request to identify if user is confirming or denying the task
         message = []
-        message.append({"role": "system", "content": dedent(self.__prompt["confirmation_system"])})
-        message.append({"role": "user", "content": dedent(self.__prompt["confirmation_user"])})
-        message.append({"role": "assistant", "content": dedent(self.__prompt["confirmation_assistant"])})
+        message.append({"role": "system", "content": dedent(self.__prompt["confirmation_system"]).strip()})
+        message.append({"role": "user", "content": dedent(self.__prompt["confirmation_user"]).strip()})
+        message.append({"role": "assistant", "content": dedent(self.__prompt["confirmation_assistant"]).strip()})
         message.append({"role": "user", "content": user_input})
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
             temperature=self.temp,
             top_p=1
             )
@@ -400,15 +407,15 @@
                 if not commands:
                     output["app_related"] = False
                     output["response"] = f"{self.model} api is not responding right now, please try again later."
                     return output
                 output["args"] = {}
                 output["args"]["commands"] = commands["response"]["commands"]
                 output["args"]["vars"] = commands["response"]["variables"]
-                if original["response"]["expected"]:
+                if original["response"].get("expected"):
                     output["args"]["expected"] = original["response"]["expected"]
                     output["action"] = "test"
                 else:
                     output["action"] = "run"
                 if dryrun:
                     output["task"] = []
                     if output["action"] == "test":
```

### Comparing `connpy-3.2.5/connpy/api.py` & `connpy-3.2.6/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/completion.py` & `connpy-3.2.6/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/configfile.py` & `connpy-3.2.6/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/connapp.py` & `connpy-3.2.6/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy/core.py` & `connpy-3.2.6/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.5/connpy.egg-info/PKG-INFO` & `connpy-3.2.6/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.5
+Version: 3.2.6
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.5/setup.cfg` & `connpy-3.2.6/setup.cfg`

 * *Files identical despite different names*

