# Comparing `tmp/cognicept-shell-1.6.0.tar.gz` & `tmp/cognicept-shell-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognicept-shell-1.6.0.tar", last modified: Mon May 15 07:55:08 2023, max compression
+gzip compressed data, was "cognicept-shell-1.6.1.tar", last modified: Mon May 22 06:45:12 2023, max compression
```

## Comparing `cognicept-shell-1.6.0.tar` & `cognicept-shell-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/
--rw-r--r--   0     1000     1000    11357 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/LICENSE.txt
--rw-r--r--   0     1000     1000    16073 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/PKG-INFO
--rw-r--r--   0     1000     1000    15209 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/README.md
-drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/cognicept_shell.egg-info/
--rw-r--r--   0     1000     1000    16073 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/PKG-INFO
--rw-r--r--   0     1000     1000      628 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1000        1 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1000       61 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/entry_points.txt
--rw-r--r--   0     1000     1000      141 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/requires.txt
--rw-r--r--   0     1000     1000       21 2023-05-15 07:55:08.000000 cognicept-shell-1.6.0/cognicept_shell.egg-info/top_level.txt
-drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/cogniceptshell/
--rw-r--r--   0     1000     1000        0 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/__init__.py
--rw-r--r--   0     1000     1000    48094 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/agent_life_cycle.py
--rw-r--r--   0     1000     1000     2461 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/cogniceptshell/common.py
--rw-r--r--   0     1000     1000    23787 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/configuration.py
--rw-r--r--   0     1000     1000     8763 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/cogniceptshell/interface.py
--rw-r--r--   0     1000     1000    11482 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/pusher.py
--rw-r--r--   0     1000     1000    19344 2021-10-22 09:01:45.000000 cognicept-shell-1.6.0/cogniceptshell/rosbag_record.py
--rw-r--r--   0     1000     1000       38 2023-05-15 07:55:08.592476 cognicept-shell-1.6.0/setup.cfg
--rw-r--r--   0     1000     1000     1395 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/setup.py
-drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/tests/
--rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/__init__.py
-drwxr-sr-x   0     1000     1000        0 2023-05-15 07:55:08.588476 cognicept-shell-1.6.0/tests/unit/
--rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/unit/__init__.py
--rw-r--r--   0     1000     1000     2414 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/mock_docker_client.py
--rw-r--r--   0     1000     1000     9247 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/test_config.py
--rw-r--r--   0     1000     1000     3485 2021-06-29 07:13:53.000000 cognicept-shell-1.6.0/tests/unit/test_keyrotate.py
--rw-r--r--   0     1000     1000    30840 2023-05-15 07:54:54.000000 cognicept-shell-1.6.0/tests/unit/test_lifecycle.py
+drwxr-sr-x   0     1000     1000        0 2023-05-22 06:45:12.345332 cognicept-shell-1.6.1/
+-rw-r--r--   0     1000     1000    11357 2021-06-29 07:13:53.000000 cognicept-shell-1.6.1/LICENSE.txt
+-rw-r--r--   0     1000     1000    16073 2023-05-22 06:45:12.345332 cognicept-shell-1.6.1/PKG-INFO
+-rw-r--r--   0     1000     1000    15209 2023-05-15 07:54:54.000000 cognicept-shell-1.6.1/README.md
+drwxr-sr-x   0     1000     1000        0 2023-05-22 06:45:12.341332 cognicept-shell-1.6.1/cognicept_shell.egg-info/
+-rw-r--r--   0     1000     1000    16073 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      628 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       61 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/entry_points.txt
+-rw-r--r--   0     1000     1000      182 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/requires.txt
+-rw-r--r--   0     1000     1000       21 2023-05-22 06:45:12.000000 cognicept-shell-1.6.1/cognicept_shell.egg-info/top_level.txt
+drwxr-sr-x   0     1000     1000        0 2023-05-22 06:45:12.341332 cognicept-shell-1.6.1/cogniceptshell/
+-rw-r--r--   0     1000     1000        0 2021-10-22 09:01:45.000000 cognicept-shell-1.6.1/cogniceptshell/__init__.py
+-rw-r--r--   0     1000     1000    48825 2023-05-22 06:44:57.000000 cognicept-shell-1.6.1/cogniceptshell/agent_life_cycle.py
+-rw-r--r--   0     1000     1000     2461 2021-06-29 07:13:53.000000 cognicept-shell-1.6.1/cogniceptshell/common.py
+-rw-r--r--   0     1000     1000    24301 2023-05-22 06:44:57.000000 cognicept-shell-1.6.1/cogniceptshell/configuration.py
+-rw-r--r--   0     1000     1000     8890 2023-05-22 06:44:57.000000 cognicept-shell-1.6.1/cogniceptshell/interface.py
+-rw-r--r--   0     1000     1000    11482 2021-10-22 09:01:45.000000 cognicept-shell-1.6.1/cogniceptshell/pusher.py
+-rw-r--r--   0     1000     1000    19344 2021-10-22 09:01:45.000000 cognicept-shell-1.6.1/cogniceptshell/rosbag_record.py
+-rw-r--r--   0     1000     1000       38 2023-05-22 06:45:12.345332 cognicept-shell-1.6.1/setup.cfg
+-rw-r--r--   0     1000     1000     1443 2023-05-22 06:44:57.000000 cognicept-shell-1.6.1/setup.py
+drwxr-sr-x   0     1000     1000        0 2023-05-22 06:45:12.341332 cognicept-shell-1.6.1/tests/
+-rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.1/tests/__init__.py
+drwxr-sr-x   0     1000     1000        0 2023-05-22 06:45:12.345332 cognicept-shell-1.6.1/tests/unit/
+-rw-r--r--   0     1000     1000        0 2021-06-29 07:13:53.000000 cognicept-shell-1.6.1/tests/unit/__init__.py
+-rw-r--r--   0     1000     1000     2414 2023-05-15 07:54:54.000000 cognicept-shell-1.6.1/tests/unit/mock_docker_client.py
+-rw-r--r--   0     1000     1000     9247 2023-05-15 07:54:54.000000 cognicept-shell-1.6.1/tests/unit/test_config.py
+-rw-r--r--   0     1000     1000     3485 2021-06-29 07:13:53.000000 cognicept-shell-1.6.1/tests/unit/test_keyrotate.py
+-rw-r--r--   0     1000     1000    30840 2023-05-15 07:54:54.000000 cognicept-shell-1.6.1/tests/unit/test_lifecycle.py
```

### Comparing `cognicept-shell-1.6.0/LICENSE.txt` & `cognicept-shell-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/PKG-INFO` & `cognicept-shell-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognicept-shell
-Version: 1.6.0
+Version: 1.6.1
 Summary: Shell utility to configure Cognicept tools.
 Home-page: https://kabam.ai
 Author: Jakub Tomasek
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cognicept-shell-1.6.0/README.md` & `cognicept-shell-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/cognicept_shell.egg-info/PKG-INFO` & `cognicept-shell-1.6.1/cognicept_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognicept-shell
-Version: 1.6.0
+Version: 1.6.1
 Summary: Shell utility to configure Cognicept tools.
 Home-page: https://kabam.ai
 Author: Jakub Tomasek
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cognicept-shell-1.6.0/cognicept_shell.egg-info/SOURCES.txt` & `cognicept-shell-1.6.1/cognicept_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/cogniceptshell/agent_life_cycle.py` & `cognicept-shell-1.6.1/cogniceptshell/agent_life_cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from docker.errors import DockerException
 import glob
 from multiprocessing import Process, Queue
 import requests
 import botocore
 import shutil
 import pkg_resources
+import compose
 from tabulate import tabulate
 from cogniceptshell.common import bcolors
 from cogniceptshell.common import generate_progress_bar
 from cogniceptshell.common import permission_safe_docker_call
 from subprocess import DEVNULL
 from docker.types import LogConfig
 from compose.cli.main import TopLevelCommand, project_from_options
@@ -675,14 +676,18 @@
                 print(bcolors.WARNING + "IMAGE NOT FOUND" +
                       bcolors.ENDC + " (run `cognicept update`)")
                 success_flag = False
             except docker.errors.APIError as exp:
                 print(exp)
                 print(bcolors.FAIL + "DOCKER ERROR" + bcolors.ENDC)
                 success_flag = False
+            except compose.project.ProjectError as exp:
+                print(exp)
+                print(bcolors.FAIL+ "DOCKER-COMPOSE ERROR" + bcolors.ENDC)
+                success_flag = False
         return success_flag
 
     def status_datadog(object, args):
         """
         Prints datadog status.
 
                 Parameters:
@@ -741,23 +746,31 @@
         except docker.errors.ImageNotFound:
             print(bcolors.WARNING + "IMAGE NOT FOUND" +
                   bcolors.ENDC + " (run `cognicept update`)")
         except docker.errors.APIError:
             print(bcolors.FAIL + "DOCKER ERROR" + bcolors.ENDC)
         os.system("xhost -local:root")
 
-    def cognicept_version_update(object):
+    def cognicept_version_update(object,args):
         current_version = pkg_resources.require("cognicept-shell")[0].version
         package = 'cognicept-shell'
         response = requests.get(f'https://pypi.org/pypi/{package}/json')
         latest_version = response.json()['info']['version']
         if latest_version != current_version:
-            print(f"{package} current version {current_version} - Installing Version {latest_version}")
-            os.system(f'pip3 install -q {package}=={latest_version}')
-            print(f'Installation {package} to version {latest_version}:'+bcolors.OKBLUE + " DONE" + bcolors.ENDC)
+            if args.skip:
+                user_input = 'y'
+            else:
+                user_input = input(f"New Cognicept Shell version {latest_version} is available! Proceed with update? ")
+
+            if user_input == 'Y' or user_input == 'y':
+                print(f"{package} current version {current_version} - Installing Version {latest_version}")
+                os.system(f'pip3 install -q {package}=={latest_version}')
+                print(f'Installation {package} to version {latest_version}:'+bcolors.OKBLUE + " DONE" + bcolors.ENDC)
+            else:
+                print(f"{package} was not updated. Current version: {current_version}")
         else:
             print(f"{package} already in latest version={latest_version}")
 
     def pull_image(object,image_name,N,i):
         """
         Pulls a Docker image and displays a progress bar.
 
@@ -805,15 +818,15 @@
             # load extra images to update
             if("COG_EXTRA_IMAGES" in args.config.config):
                 image_names = args.config.config["COG_EXTRA_IMAGES"].split(";")
                 if(len(image_names) > 0):
                     images = images.union(set(image_names))
             
             N = len(images)
-            object.cognicept_version_update()
+            object.cognicept_version_update(args)
             print("Info: This may take a while depending on your connection.")
         # if list of agents is specified, update only that particular set of agents
         else: 
             images = set()
             if args.list:
                 for container_name in args.list:
                     if container_name in object._docker_container_names:
@@ -827,41 +840,41 @@
                     images.add(image_name)
 
             N = len(images)
             print("Info: Update " + str(N) + " agent_image(s).")
 
         i = 0 # For indexing
         success_flag = True
-
         for image_name in images:
             i = i + 1
+            image_name_short = image_name.replace("412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/", "cognicept/")
             try:
                 if('412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/' in image_name):
                     object.pull_image(image_name, N=N, i=i)
                 else:
                     object.pull_image('412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/' + image_name, N=N, i=i)
 
             except docker.errors.NotFound:
                 try:
                     object.pull_image(image_name,N=N, i=i)
                     
                 except docker.errors.NotFound:
-                    print(bcolors.FAIL + "Error: " + bcolors.ENDC + f"Image {image_name} can’t be accessed in ECR or Docker Hub.")
-                    print("[" + str(i) + "/" + str(N) + "] " + image_name +
+                    print(bcolors.FAIL + "Error: " + bcolors.ENDC + f"Image {image_name_short} can’t be accessed in ECR or Docker Hub.")
+                    print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
                         " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
                     success_flag = False
                     
                 except DockerException as ex:
-                    print("[" + str(i) + "/" + str(N) + "] " + image_name +
+                    print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
                         " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
                     print(f"Error: {ex}")
                     success_flag = False
                     continue  # skip the current image and continue with the next one
             except:
-                print("[" + str(i) + "/" + str(N) + "] " + image_name +
+                print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
                     " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
                 success_flag = False
 
         if not success_flag:
             print("There were errors while updating some images.")
         print("Info: Run `cognicept restart` to redeploy updated agents.")
```

### Comparing `cognicept-shell-1.6.0/cogniceptshell/common.py` & `cognicept-shell-1.6.1/cogniceptshell/common.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/cogniceptshell/configuration.py` & `cognicept-shell-1.6.1/cogniceptshell/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,30 +517,39 @@
                     if new_key == auth_key:    
                         print("Failed to initialized robot: Invalid OTP entered 3 times")
                         return False
                     else:
                         auth_key=new_key
 
                 r = requests.get(api_uri + 'spinup/config/' + args.org_id + '/' + args.robot_id, headers={'Authorization': 'Bearer {}'.format(auth_key)})
+                r.raise_for_status()
                 j = r.json()
-                if j is not None:
+                if j:
                     for key in j:
                         object.config[key] = j[key]
                     object.save_config()
                     print("Successfully initialized configuration for the robot `" + args.robot_id + "`. To start agents run `cognicept start`")
                     return True
                 else:
                     print("Failed to initialize the robot: ID `" + args.robot_id + "` in organization `" + args.org_id + "` not found")
                     return False
         except requests.exceptions.Timeout:
             print("Cognicept REST API error: time out.")
             return False
         except requests.exceptions.TooManyRedirects:
             print("Cognicept REST API error: Wrong endpoint.")
             return False
+        except requests.exceptions.HTTPError as err:
+            error_code = err.response.status_code
+            if error_code != 400:
+                print(f"Cognicept REST API error: {error_code} status code.\nPlease check configurations and report error if necessary.")
+                raise SystemExit()
+            else:
+                print("Failed to initialize the robot: ID `" + args.robot_id + "` in organization `" + args.org_id + "` not found")
+                return False
         except Exception as e:
             print("Cognicept REST API error" + str(e))
             raise SystemExit()
 
     def mfa_verfication(object,api_uri,auth_key):
         otp_trial = 3
         loop = True
```

### Comparing `cognicept-shell-1.6.0/cogniceptshell/interface.py` & `cognicept-shell-1.6.1/cogniceptshell/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 parser_update.add_argument("-d", "--detach", help="Runs update in detached mode", action="store_true")
 
 """Adding an add_argument to parser_update"""
 parser_update.add_argument(
     '--image', '-i', dest ='image',help='List of docker images to update', metavar='flag', type=str, nargs='*')  
 parser_update.add_argument(
     'list', help='List of agents to update, leave empty to start all agents', metavar='list', type=str, nargs='*',choices=container_names)
+parser_update.add_argument("-y","--skip", help="Skips user prompt when updating cognicept-shell version", action="store_true")
 
 
 parser_orbitty.add_argument(
     '--path', help='Cognicept configuration directory (default: `'
     + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 
 parser_record.add_argument(
```

### Comparing `cognicept-shell-1.6.0/cogniceptshell/pusher.py` & `cognicept-shell-1.6.1/cogniceptshell/pusher.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/cogniceptshell/rosbag_record.py` & `cognicept-shell-1.6.1/cogniceptshell/rosbag_record.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/setup.py` & `cognicept-shell-1.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 import re
 import ast
 
 from setuptools import setup, find_packages
 
 
-requires = ['python-dotenv>=0.13.0', 'boto3>=1.14.0', 'docker>=5.0.0',  'PyCryptodome >=3.9.8', 'argcomplete>=1.12.3', 'tabulate', 'ping3', 'docker-compose==1.29.2', 'PyJWT==1.7.1']
+requires = ['python-dotenv>=0.13.0', 'boto3>=1.14.0', 'docker>=5.0.0',  'PyCryptodome >=3.9.8', 'argcomplete>=1.12.3', 'tabulate', 'ping3', 'docker-compose==1.29.2', 'PyJWT==1.7.1', 'websocket-client==0.59.0', 'paramiko>=2.4.2']
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup(
     name='cognicept-shell',
-    version='1.6.0',
+    version='1.6.1',
     description='Shell utility to configure Cognicept tools.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Jakub Tomasek',
     url='https://kabam.ai',
     packages=find_packages(),
     install_requires=requires,
@@ -34,8 +34,8 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8'
     ),
-)
+)
```

### Comparing `cognicept-shell-1.6.0/tests/unit/mock_docker_client.py` & `cognicept-shell-1.6.1/tests/unit/mock_docker_client.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/tests/unit/test_config.py` & `cognicept-shell-1.6.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/tests/unit/test_keyrotate.py` & `cognicept-shell-1.6.1/tests/unit/test_keyrotate.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.6.0/tests/unit/test_lifecycle.py` & `cognicept-shell-1.6.1/tests/unit/test_lifecycle.py`

 * *Files identical despite different names*

