# Comparing `tmp/pyxecm-0.0.16.tar.gz` & `tmp/pyxecm-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.16.tar", last modified: Wed May  3 09:45:46 2023, max compression
+gzip compressed data, was "pyxecm-0.0.17.tar", last modified: Mon May 22 10:44:53 2023, max compression
```

## Comparing `pyxecm-0.0.16.tar` & `pyxecm-0.0.17.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.248448 pyxecm-0.0.16/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-03 09:45:22.000000 pyxecm-0.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-03 09:45:46.248448 pyxecm-0.0.16/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-05-03 09:45:22.000000 pyxecm-0.0.16/README.md
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-03 09:45:33.000000 pyxecm-0.0.16/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.246448 pyxecm-0.0.16/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30481 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    49947 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   216194 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   113213 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   226245 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.248448 pyxecm-0.0.16/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 09:45:46.248448 pyxecm-0.0.16/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-03 09:45:22.000000 pyxecm-0.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.725262 pyxecm-0.0.17/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-22 10:44:36.000000 pyxecm-0.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 10:44:53.725262 pyxecm-0.0.17/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-22 10:44:36.000000 pyxecm-0.0.17/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-22 10:44:43.000000 pyxecm-0.0.17/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.723262 pyxecm-0.0.17/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33694 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    15046 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/llm.py
+-rw-rw-rw-   0 root         (0) root         (0)    77524 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    50994 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9554 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256092 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   117829 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10240 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   250685 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5986 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.725262 pyxecm-0.0.17/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 10:44:53.725262 pyxecm-0.0.17/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-22 10:44:36.000000 pyxecm-0.0.17/setup.py
```

### Comparing `pyxecm-0.0.16/LICENSE` & `pyxecm-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.16/PKG-INFO` & `pyxecm-0.0.17/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.16
-Summary: A library to connect to Opentext Extended ECM
+Version: 0.0.17
+Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYXECM
 
-A python library to connect to Opentext Extended ECM
+A python library to interact with Opentext Extended ECM REST API.
+API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `pyxecm-0.0.16/README.md` & `pyxecm-0.0.17/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # PYXECM
 
-A python library to connect to Opentext Extended ECM
+A python library to interact with Opentext Extended ECM REST API.
+API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `pyxecm-0.0.16/pyproject.toml` & `pyxecm-0.0.17/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 [build-system]
   build-backend = "setuptools.build_meta"
   requires = ["setuptools >= 61.0"]
 
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
-  description = "A library to connect to Opentext Extended ECM"
+  description = "A Python library to interact with Opentext Extended ECM REST API"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.16"
+  version = "0.0.17"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.16/pyxecm/k8s.py` & `pyxecm-0.0.17/pyxecm/k8s.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,58 +6,57 @@
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
 https://github.com/kubernetes-client/python/tree/master/examples
 
 Class: K8s
 Methods:
 
 __init__ : class initializer
-getCoreV1Api : get Kubernetes API object for Core APIs
-getAppsV1Api : get Kubernetes API object for Applications (e.g. Stateful Sets)
-getNetworkingV1Api : get Kubernetes API object for Networking (e.g. Ingress)
-
-getNamespace : get the Kubernetes Namespace the K8s object is configured for
-
-getPod : get a Kubernetes Pod based on its name
-listPods : get a list of Kubernetes Pods based on field and label selectors
-execPodCommand : execute a list of commands in a Kubernetes Pod
-execPodCommendInteractive: write commands to stdin and wait for response
-deletePod: delete a running pod (e.g. to make Kubernetes restart it)
-
-getConfigMap : get a Kubernetes Config Map based on its name
-listConfigMaps : get a list of Kubernetes Config Maps based on field and label selectors
-findConfigMap : find a Kubernetes Config Map based on its name
-replaceConfigMap : replace the data body of a Kubernetes Config Map
-
-getStatefulSet : get a Kubernetes Stateful Set based on its name
-getStatefulSetScale : get the number of replicas for a Kubernetes Stateful Set
-patchStatefulSet : update the specification of a Kubernetes Stateful Set
-scaleStatefulSet : change number of replicas for a Kubernetes Stateful Set
-
-getService : get a Kubernetes Service based on its name
-listServices : get a list of Kubernetes Services based on field and label selectors
-patchService : update the specification of a Kubernetes Service
-
-getIngress : get a Kubernetes Ingress based on its name
-patchIngress : update the specification of a Kubernetes Ingress
-updateIngressBackendServices: replace the backend service and port for an ingress host
+getCoreV1Api: Get Kubernetes API object for Core APIs
+getAppsV1Api: Get Kubernetes API object for Applications (e.g. Stateful Sets)
+getNetworkingV1Api: Get Kubernetes API object for Networking (e.g. Ingress)
+getNamespace: Get the Kubernetes namespace the K8s object is configured for
+
+getPod: Get a Kubernetes Pod based on its name
+listPods: Get a list of Kubernetes pods based on field and label selectors
+execPodCommand: Execute a list of commands in a Kubernetes Pod
+execPodCommendInteractive: Write commands to stdin and wait for response
+deletePod: Delete a running pod (e.g. to make Kubernetes restart it)
+
+getConfigMap: Get a Kubernetes Config Map based on its name
+listConfigMaps: Get a list of Kubernetes Config Maps based on field and label selectors
+findConfigMap: Find a Kubernetes Config Map based on its name
+replaceConfigMap: Replace the data body of a Kubernetes Config Map
+
+getStatefulSet: Gets a Kubernetes Stateful Set based on its name
+getStatefulSetScale: Gets the number of replicas for a Kubernetes Stateful Set
+patchStatefulSet: Updates the specification of a Kubernetes Stateful Set
+scaleStatefulSet: Changes number of replicas for a Kubernetes Stateful Set
+
+getService: Get a Kubernetes Service based on its name
+listServices: Get a list of Kubernetes Services based on field and label selectors
+patchService: Update the specification of a Kubernetes Service
+
+getIngress: Get a Kubernetes Ingress based on its name
+patchIngress: Update the specification of a Kubernetes Ingress
+updateIngressBackendServices: Replace the backend service and port for an ingress host
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
 import time
 from kubernetes import client, config
 from kubernetes.stream import stream
-from kubernetes.client.exceptions import ApiException, ApiValueError
+from kubernetes.client.exceptions import ApiException
 
 # Configure Kubernetes API authentication to use pod serviceAccount
 # config.load_incluster_config()
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 
@@ -99,50 +98,57 @@
     def getNetworkingV1Api(self):
         return self._networking_v1_api
 
     def getNamespace(self):
         return self._namespace
 
     def getPod(self, pod_name: str):
-        """getPod: get a pod in the configured namespace (the namespace is defined in the class constructor).
+        """Get a pod in the configured namespace (the namespace is defined in the class constructor).
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#read_namespaced_pod
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
-        Return: V1Pod (object):
-                api_version='v1',
-                kind='Pod',
-                metadata=V1ObjectMeta(...),
-                spec=V1PodSpec(...),
-                status=V1PodStatus(...)
+        Returns:
+            V1Pod (object) or None if the call fails.
+            - api_version='v1',
+            - kind='Pod',
+            - metadata=V1ObjectMeta(...),
+            - spec=V1PodSpec(...),
+            - status=V1PodStatus(...)
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_pod(
                 name=pod_name, namespace=self.getNamespace()
             )
         except ApiException as e:
-            logger.error("Failed to get Pod -> {}; error -> {}".format(pod_name, str(e)))
+            logger.error(
+                "Failed to get Pod -> {}; error -> {}".format(pod_name, str(e))
+            )
             return None
 
         return response
 
     # end method definition
 
     def listPods(self, field_selector: str = "", label_selector: str = ""):
-        """listPods: list all Kubernetes pods in a given namespace. The list can be further restricted
-                     by specifying a field or label selector.
+        """List all Kubernetes pods in a given namespace. The list can be further restricted
+            by specifying a field or label selector.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_pod
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
-        Return: V1PodList (object) or None if the call fails
-                Properties can be accessed with the "." notation (this is an object not a dict!):
-                - api_version: The Kubernetes API version.
-                - items: A list of V1Pod objects, each representing a pod. You can access the fields of a
-                        V1Pod object using dot notation, for example, pod.metadata.name to access the name of the pod
-                - kind: The Kubernetes object kind, which is always "PodList".
-                - metadata: Additional metadata about the pod list, such as the resource version.
+        Returns:
+            V1PodList (object) or None if the call fails
+            Properties can be accessed with the "." notation (this is an object not a dict!):
+            - api_version: The Kubernetes API version.
+            - items: A list of V1Pod objects, each representing a pod. You can access the fields of a
+                    V1Pod object using dot notation, for example, pod.metadata.name to access the name of the pod
+            - kind: The Kubernetes object kind, which is always "PodList".
+            - metadata: Additional metadata about the pod list, such as the resource version.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1PodList.md
         """
 
         try:
             response = self.getCoreV1Api().list_namespaced_pod(
                 field_selector=field_selector,
                 label_selector=label_selector,
                 namespace=self.getNamespace(),
@@ -156,19 +162,20 @@
             return None
 
         return response
 
     # end method definition
 
     def waitPodCondition(self, pod_name: str, condition_name: str):
-        """waitPodCondition: wait for the pod to reach a defined condition (e.g. "Ready").
+        """Wait for the pod to reach a defined condition (e.g. "Ready").
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             condition_name (string): name of the condition, e.g. "Ready"
-        Return: True once the pod reaches the condition - otherwise wait forever
+        Returns:
+            True once the pod reaches the condition - otherwise wait forever
         """
 
         ready = False
         while not ready:
             try:
                 pod_status = self.getCoreV1Api().read_namespaced_pod_status(
                     pod_name, self.getNamespace()
@@ -197,28 +204,29 @@
                 logger.error(
                     "Failed to wait for pod -> {}; error -> {}".format(pod_name, str(e))
                 )
 
     # end method definition
 
     def execPodCommand(self, pod_name: str, command: list):
-        """execPodCommand: execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
+        """Execute a command inside a Kubernetes Pod (similar to kubectl exec on command line).
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#connect_get_namespaced_pod_exec
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             command (list): list of command and its parameters, e.g. ["/bin/bash", "-c", "pwd"]
                             The "-c" is required to make the shell executing the command.
-        Return: response of the command or None if the call fails
+        Returns:
+            Response of the command or None if the call fails
         """
 
         pod = self.getPod(pod_name)
         if not pod:
             logger.error("Pod -> {} does not exist".format(pod_name))
 
-        logger.info(
-            "Execute command -> {} in pod -> {}".format(command, pod_name))
+        logger.info("Execute command -> {} in pod -> {}".format(command, pod_name))
 
         try:
             response = stream(
                 self.getCoreV1Api().connect_get_namespaced_pod_exec,
                 pod_name,
                 self.getNamespace(),
                 command=command,
@@ -236,30 +244,37 @@
             return None
 
         return response
 
     # end method definition
 
     # Some commands like the OTAC spawner need to run interactive - otherwise the command "hangs"
-    def execPodCommandInteractive(self, pod_name: str, commands: list, timeout: int = 30, write_stderr_to_error_log: bool = True):
-        """execPodCommandInteractive: execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
-                                      Other than execPodCommand() method above this is an interactive execution using
-                                      stdin and reading the output from stdout and stderr. This is required for longer
-                                      running commands. It is currently used for restarting the spawner of Archive Center.
-                                      The output of the command is pushed into the logging.
+    def execPodCommandInteractive(
+        self,
+        pod_name: str,
+        commands: list,
+        timeout: int = 30,
+        write_stderr_to_error_log: bool = True,
+    ):
+        """Execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
+            Other than execPodCommand() method above this is an interactive execution using
+            stdin and reading the output from stdout and stderr. This is required for longer
+            running commands. It is currently used for restarting the spawner of Archive Center.
+            The output of the command is pushed into the logging.
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
             commands (list): list of command and its parameters, e.g. ["/bin/bash", "/etc/init.d/spawner restart"]
                              Here we should NOT have a "-c" parameter!
-            timeout (integer): timeout duration that is waited for any response. 
+            timeout (integer): timeout duration that is waited for any response.
                                Each time a resonse is found in stdout or stderr we wait another timeout duration
                                to make sure we get the full output of the command.
             write_stderr_to_error_log (boolean): flag to control if output in stderr should be written to info or error log stream.
                                                  Default is write to error log (True)
-        Return: response of the connect_get_namespaced_pod_exec() or None if the call fails
+        Returns:
+            Response of the command (string) or None if the call fails
         """
 
         pod = self.getPod(pod_name)
         if not pod:
             logger.error("Pod -> {} does not exist".format(pod_name))
 
         if not commands:
@@ -274,15 +289,15 @@
                 pod_name,
                 self.getNamespace(),
                 command=command,
                 stderr=True,
                 stdin=True,  # This is important!
                 stdout=True,
                 tty=False,
-                _preload_content=False  # This is important!
+                _preload_content=False,  # This is important!
             )
         except ApiException as e:
             logger.error(
                 "Failed to execute command -> {} in pod -> {}; error -> {}".format(
                     command, pod_name, str(e)
                 )
             )
@@ -299,39 +314,43 @@
                     logger.error(response.read_stderr().replace("\n", " "))
                 else:
                     logger.info(response.read_stderr().replace("\n", " "))
                 got_response = True
             if commands:
                 command = commands.pop(0)
                 logger.info(
-                    "Execute command -> {} in pod -> {}".format(command, pod_name))
+                    "Execute command -> {} in pod -> {}".format(command, pod_name)
+                )
                 response.write_stdin(command + "\n")
             else:
                 # We continue as long as we get some response during timeout period
                 if not got_response:
                     break
 
         response.close()
 
         return response
 
     # end method definition
 
     def deletePod(self, pod_name: str):
-        """deletePod: delete a pod in the configured namespace (the namespace is defined in the class constructor).
+        """Delete a pod in the configured namespace (the namespace is defined in the class constructor).
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#delete_namespaced_pod
         Args:
             pod_name (string): name of the Kubernetes pod in the current namespace
-        Return: V1Status (object):
-                api_version: The Kubernetes API version.
-                kind: The Kubernetes object kind, which is always "Status".
-                metadata: Additional metadata about the status object, such as the resource version.
-                status: The status of the operation, which is either "Success" or an error status.
-                message: A human-readable message explaining the status.
-                reason: A short string that describes the reason for the status.
-                code: An HTTP status code that corresponds to the status.
+        Return:
+            V1Status (object) or None if the call fails.
+            - api_version: The Kubernetes API version.
+            - kind: The Kubernetes object kind, which is always "Status".
+            - metadata: Additional metadata about the status object, such as the resource version.
+            - status: The status of the operation, which is either "Success" or an error status.
+            - message: A human-readable message explaining the status.
+            - reason: A short string that describes the reason for the status.
+            - code: An HTTP status code that corresponds to the status.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Status.md
         """
 
         pod = self.getPod(pod_name)
         if not pod:
             logger.error("Pod -> {} does not exist".format(pod_name))
 
         try:
@@ -345,28 +364,30 @@
             return None
 
         return response
 
     # end method definition
 
     def getConfigMap(self, config_map_name: str):
-        """getConfigMap: get a config map in the configured namespace (the namespace is defined in the class constructor).
+        """Get a config map in the configured namespace (the namespace is defined in the class constructor).
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#read_namespaced_config_map
         Args:
             config_map_name (string): name of the Kubernetes config map in the current namespace
-        Return: V1ConfigMap (object) that includes these fields:
-                api_version: The Kubernetes API version.
-                metadata: A V1ObjectMeta object representing metadata about the V1ConfigMap object,
-                          such as its name, labels, and annotations.
-                data: A dictionary containing the non-binary data stored in the ConfigMap,
-                      where the keys represent the keys of the data items and the values represent
-                      the values of the data items.
-                binary_data: A dictionary containing the binary data stored in the ConfigMap,
-                             where the keys represent the keys of the binary data items and the values
-                             represent the values of the binary data items. Binary data is encoded as base64
-                             strings in the dictionary values.
+        Returns:
+            V1ConfigMap (object) that includes these fields:
+            - api_version: The Kubernetes API version.
+            - metadata: A V1ObjectMeta object representing metadata about the V1ConfigMap object,
+                        such as its name, labels, and annotations.
+            - data: A dictionary containing the non-binary data stored in the ConfigMap,
+                    where the keys represent the keys of the data items and the values represent
+                    the values of the data items.
+            - binary_data: A dictionary containing the binary data stored in the ConfigMap,
+                           where the keys represent the keys of the binary data items and the values
+                           represent the values of the binary data items. Binary data is encoded as base64
+                           strings in the dictionary values.
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_config_map(
                 name=config_map_name, namespace=self.getNamespace()
             )
         except ApiException as e:
@@ -374,27 +395,29 @@
             return None
 
         return response
 
     # end method definition
 
     def listConfigMaps(self, field_selector: str = "", label_selector: str = ""):
-        """listConfigMaps: lists all Kubernetes Config Maps in the current namespace.
-                           The list can be filtered by providing field selectors and
-                           label selectors.
+        """List all Kubernetes Config Maps in the current namespace.
+            The list can be filtered by providing field selectors and label selectors.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_config_map
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
-        Return: V1ConfigMapList (object) or None if the call fails
-                Properties can be accessed with the "." notation (this is an object not a dict!):
-                - api_version: The Kubernetes API version.
-                - items: A list of V1ConfigMap objects, each representing a config map. You can access the fields of a
-                        V1Pod object using dot notation, for example, cm.metadata.name to access the name of the config map
-                - kind: The Kubernetes object kind, which is always "ConfigMapList".
-                - metadata: Additional metadata about the config map list, such as the resource version.
+        Returns:
+            V1ConfigMapList (object) or None if the call fails
+            Properties can be accessed with the "." notation (this is an object not a dict!):
+            - api_version: The Kubernetes API version.
+            - items: A list of V1ConfigMap objects, each representing a config map. You can access the fields of a
+                     V1Pod object using dot notation, for example, cm.metadata.name to access the name of the config map
+            - kind: The Kubernetes object kind, which is always "ConfigMapList".
+            - metadata: Additional metadata about the config map list, such as the resource version.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ConfigMapList.md
         """
 
         try:
             response = self.getCoreV1Api().list_namespaced_config_map(
                 field_selector=field_selector,
                 label_selector=label_selector,
                 namespace=self.getNamespace(),
@@ -408,14 +431,24 @@
             return None
 
         return response
 
     # end method definition
 
     def findConfigMap(self, config_map_name: str):
+        """Find a Kubernetes Config Map based on its name.
+           This is just a wrapper method for listConfigMaps()
+           that uses the name as a field selector.
+
+        Args:
+            config_map_name (string): name of the Config Map
+        Returns:
+            object: V1ConfigMapList (object) or None if the call fails
+        """
+
         try:
             response = self.listConfigMaps(
                 field_selector="metadata.name={}".format(config_map_name)
             )
         except ApiException as e:
             logger.error(
                 "Failed to find Config Map -> {}; error -> {}".format(
@@ -425,14 +458,25 @@
             return None
 
         return response
 
     # end method definition
 
     def replaceConfigMap(self, config_map_name: str, config_map_data: dict):
+        """Replace a Config Map with a new specification.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#replace_namespaced_config_map
+
+        Args:
+            config_map_name (string): name of the Kubernetes Config Map
+            config_map_data (dictionary): new specification of the Config Map
+        Returns:
+            V1ConfigMap (object) or None if the call fails.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ConfigMap.md
+        """
+
         try:
             response = self.getCoreV1Api().replace_namespaced_config_map(
                 name=config_map_name,
                 namespace=self.getNamespace(),
                 body=client.V1ConfigMap(
                     metadata=client.V1ObjectMeta(
                         name=config_map_name,
@@ -449,21 +493,22 @@
             return None
 
         return response
 
     # end method definition
 
     def getStatefulSet(self, sts_name: str):
-        """Get a Kubernetes Stateful Set based on its name
+        """Get a Kubernetes Stateful Set based on its name.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#read_namespaced_stateful_set
 
         Args:
             sts_name (string): name of the Kubernetes stateful set
-
         Returns:
-            K8s response
+            V1StatefulSet (object) or None if the call fails.
+            See : https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
             response = self.getAppsV1Api().read_namespaced_stateful_set(
                 name=sts_name, namespace=self.getNamespace()
             )
         except ApiException as e:
@@ -473,21 +518,22 @@
             return None
 
         return response
 
     # end method definition
 
     def getStatefulSetScale(self, sts_name: str):
-        """Get the number of replicas for a Kubernetes Stateful Set
+        """Get the number of replicas for a Kubernetes Stateful Set.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#read_namespaced_stateful_set_scale
 
         Args:
-            sts_name (string): name of the Kubernetes stateful set
-
+            sts_name (string): name of the Kubernetes Stateful Set
         Returns:
-            K8S response: response of the Kubernetes API
+            V1Scale (object) or None if the call fails.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Scale.md
         """
 
         try:
             response = self.getAppsV1Api().read_namespaced_stateful_set_scale(
                 name=sts_name, namespace=self.getNamespace()
             )
         except ApiException as e:
@@ -499,19 +545,23 @@
             return None
 
         return response
 
     # end method definition
 
     def patchStatefulSet(self, sts_name: str, sts_body: dict):
-        """patchStatefulSet: patch a Stateful set with new values
+        """Patch a Stateful set with new values.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/AppsV1Api.md#patch_namespaced_stateful_set
+
         Args:
             sts_name (string): name of the Kubernetes stateful set in the current namespace
             sts_body (string): patch string
-        Return: response of the Kubernetes patch command or None if the call fails
+        Returns:
+            V1StatefulSet (object) or None if the call fails.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
             response = self.getAppsV1Api().patch_namespaced_stateful_set(
                 name=sts_name, namespace=self.getNamespace(), body=sts_body
             )
         except ApiException as e:
@@ -523,18 +573,21 @@
             return None
 
         return response
 
     # end method definition
 
     def scaleStatefulSet(self, sts_name: str, scale: int):
-        """scaleStatefulSet: scale a stateful set to a specific number of replicas. It uses the class method patchStatefulSet() above.
+        """Scale a stateful set to a specific number of replicas. It uses the class method patchStatefulSet() above.
+
         Args:
             sts_name (string): name of the Kubernetes stateful set in the current namespace
-        Return: response of the Kubernetes patch command or None if the call fails
+        Returns:
+            V1StatefulSet (object) or None if the call fails.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1StatefulSet.md
         """
 
         try:
             response = self.patchStatefulSet(
                 sts_name, sts_body={"spec": {"replicas": scale}}
             )
         except ApiException as e:
@@ -546,48 +599,55 @@
             return None
 
         return response
 
     # end method definition
 
     def getService(self, service_name: str):
-        """getService: gets a Kubernetes service with a defined name in the
-        current namespace
+        """Get a Kubernetes Service with a defined name in the current namespace
+
         Args:
-            service_name (string): name of the Kubernetes service in the current namespace
-        Return: <class 'kubernetes.client.models.v1_service.V1Service'> or None if the call fails
-                This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements
+            service_name (string): name of the Kubernetes Service in the current namespace
+        Returns:
+            V1Service (object) or None if the call fails
+            This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Service.md
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_service(
                 name=service_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
                 "Failed to get Service -> {}; error -> {}".format(service_name, str(e))
             )
             return None
 
         return response
 
+    # end method definition
+
     def listServices(self, field_selector: str = "", label_selector: str = ""):
-        """listServices: lists all Kubernetes Service in the current namespace.
-                         The list can be filtered by providing field selectors and
-                        label selectors.
+        """List all Kubernetes Service in the current namespace.
+            The list can be filtered by providing field selectors and label selectors.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/CoreV1Api.md#list_namespaced_service
+
         Args:
             field_selector (string): filter result based on fields
             label_selector (string): filter result based on labels
-        Return: V1ServiceList (object) or None if the call fails
-                Properties can be accessed with the "." notation (this is an object not a dict!):
-                - api_version: The Kubernetes API version.
-                - items: A list of V1Service objects, each representing a service. You can access the fields of a
-                        V1Service object using dot notation, for example, service.metadata.name to access the name of the service
-                - kind: The Kubernetes object kind, which is always "ServiceList".
-                - metadata: Additional metadata about the pod list, such as the resource version.
+        Returns:
+            V1ServiceList (object) or None if the call fails
+            Properties can be accessed with the "." notation (this is an object not a dict!):
+            - api_version: The Kubernetes API version.
+            - items: A list of V1Service objects, each representing a service. You can access the fields of a
+                     V1Service object using dot notation, for example, service.metadata.name to access the name of the service
+            - kind: The Kubernetes object kind, which is always "ServiceList".
+            - metadata: Additional metadata about the pod list, such as the resource version.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1ServiceList.md
         """
 
         try:
             response = self.getCoreV1Api().list_namespaced_service(
                 field_selector=field_selector,
                 label_selector=label_selector,
                 namespace=self.getNamespace(),
@@ -601,20 +661,23 @@
             return None
 
         return response
 
     # end method definition
 
     def patchService(self, service_name: str, service_body: dict):
-        """patchService: patches a Kubernetes Service with an updated spec
+        """Patches a Kubernetes Service with an updated spec
+
         Args:
             service_name (string): name of the Kubernetes Ingress in the current namespace
             service_body (dict): new / updated Service body spec (will be merged with existing values)
-        Return: Object of <class 'kubernetes.client.models.v1_service.V1Service'> or None if the call fails
-                This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+        Returns:
+            V1Service object or None if the call fails
+            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Service.md
         """
 
         try:
             response = self.getCoreV1Api().patch_namespaced_service(
                 name=service_name, namespace=self.getNamespace(), body=service_body
             )
         except ApiException as e:
@@ -626,20 +689,22 @@
             return None
 
         return response
 
     # end method definition
 
     def getIngress(self, ingress_name: str):
-        """getIngress: gets a Kubernetes Ingress with a defined name in the
-        current namespace
+        """Get a Kubernetes Ingress with a defined name in the current namespace
+
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
-        Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
-                This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements
+        Returns:
+            V1Ingress object or None if the call fails
+            This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
         try:
             response = self.getNetworkingV1Api().read_namespaced_ingress(
                 name=ingress_name, namespace=self.getNamespace()
             )
         except ApiException as e:
@@ -649,20 +714,24 @@
             return None
 
         return response
 
     # end method definition
 
     def patchIngress(self, ingress_name: str, ingress_body: dict):
-        """patchIngress: patches a Kubernetes Ingress with a updated spec
+        """Patch a Kubernetes Ingress with a updated spec.
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/NetworkingV1Api.md#patch_namespaced_ingress
+
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
             ingress_body (dict): new / updated ingress body spec (will be merged with existing values)
-        Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
-                This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+        Returns:
+            V1Ingress object or None if the call fails
+            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
         try:
             response = self.getNetworkingV1Api().patch_namespaced_ingress(
                 name=ingress_name,
                 namespace=self.getNamespace(),
                 body=ingress_body,
@@ -678,15 +747,15 @@
         return response
 
     # end method definition
 
     def updateIngressBackendServices(
         self, ingress_name: str, hostname: str, service_name: str, service_port: int
     ):
-        """updateIngressBackendService: updates a backend service and port of an Kubernetes Ingress
+        """Updates a backend service and port of an Kubernetes Ingress
 
         "spec": {
             "rules": [
                 {
                     "host": host,
                     "http": {
                         "paths": [
@@ -710,16 +779,18 @@
         }
 
         Args:
             ingress_name (string): name of the Kubernetes Ingress in the current namespace
             hostname (string): hostname that should get an updated backend service / port
             service_name (string): new backend service name
             service_port (integer): new backend service port
-        Return: V1Ingress Object or None if the call fails
-                This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+        Returns:
+            V1Ingress Object or None if the call fails
+            This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            See: https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Ingress.md
         """
 
         ingress = self.getIngress(ingress_name)
         if not ingress:
             return None
 
         host = ""
```

### Comparing `pyxecm-0.0.16/pyxecm/m365.py` & `pyxecm-0.0.17/pyxecm/m365.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,63 +20,77 @@
 
 getUsers: Get list all all users in M365 tenant 
 getUser: Get a M365 User based on its email
 getGroups: Get list all all groups in M365 tenant
 getGroup: Get a M365 Group based on its name
 addGroup: Add a M365 Group
 addUser: Add a M365 User
-hasTeam: checks if a M365 Group has a M365 Team connected or not
+hasTeam: Check if a M365 Group has a M365 Team connected or not
 addTeam: Add a M365 Team (based on an existing group)
-getUserLicenses: get the assigned license SKUs of a user
+deleteTeams: Delete MS teams with a given name
+getUserLicenses: Get the assigned license SKUs of a user
 assignLicenseToUser: Add an M365 license to a user (e.g. to use Office 365)
-getUserPhoto: retrieves the photo of a M365 user
+getUserPhoto: Retriev the photo of a M365 user
 updateUserPhoto: Update a user with a profile photo (which must be in local file system)
 getGroupMembers: Get members (users and groups) of the specified group
 getGroupOwners: Get owners (users) of the specified group
 addGroupMember: Add a user or group to a target group
-isMember: Checks whether a M365 user is already in a M365 group
+isMember: Check whether a M365 user is already in a M365 group
 addGroupOwner: Add a user as owner to a group
 purgeDeletedItems: Purge all deleted users and groups in the organization
 purgeDeletedItem: Help function that purges a single user or group
 getTeamsApps: Get a list of MS Teams apps in catalog that match a given filter criterium
 uploadTeamsApp: Upload a new app package to the catalog of MS Teams apps
-deleteTeamsApp: delete an existing MS teams app (currently not used)
-addSensitivityLabel: Assigns a existing sensitivity label to a user.
+removeTeamsApp: Remove MS Teams App for the app catalog
+assignTeamsAppToUser: Assign (add) a MS teams app to a M365 user.
+upgradeTeamsAppOfUser: Upgrade a MS teams app for a user.
+addSensitivityLabel: Assign a existing sensitivity label to a user.
                      THIS IS CURRENTLY NOT WORKING!
 assignSensitivityLabelToUser: Create a new sensitivity label in M365
                               THIS IS CURRENTLY NOT WORKING!
-
-
 """
 
+__author__ = "Dr. Marc Diefenbruch"
+__copyright__ = "Copyright 2023, OpenText"
+__credits__ = ["Kai-Philip Gatzweiler"]
+__maintainer__ = "Dr. Marc Diefenbruch"
+__email__ = "mdiefenb@opentext.com"
+
 import os
 import logging
 import requests
 import json
 import urllib.parse
-import base64
 import zipfile
+from urllib.parse import quote
+import re
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestLoginHeaders = {
     "Content-Type": "application/x-www-form-urlencoded",
-    "Accept": "application/json"
+    "Accept": "application/json",
 }
 
 
 class M365(object):
     """Used to automate stettings in Microsoft 365 via the Graph API."""
 
     _config = None
     _access_token = None
     _user_access_token = None
 
     def __init__(
-        self, tenant_id: str, client_id: str, client_secret: str, domain: str, sku_id: str, teams_app_name: str
+        self,
+        tenant_id: str,
+        client_id: str,
+        client_secret: str,
+        domain: str,
+        sku_id: str,
+        teams_app_name: str,
     ):
         """Initialize the M365 object
 
         Args:
             tenant_id (string): M365 Tenant ID
             client_id (string): M365 Client ID
             client_secret (string): M365 Client Secret
@@ -90,100 +104,110 @@
         # Set the authentication endpoints and credentials
         m365Config["tenantId"] = tenant_id
         m365Config["clientId"] = client_id
         m365Config["clientSecret"] = client_secret
         m365Config["domain"] = domain
         m365Config["skuId"] = sku_id
         m365Config["teamsAppName"] = teams_app_name
-        m365Config["authenticationUrl"] = "https://login.microsoftonline.com/{}/oauth2/v2.0/token".format(
-            tenant_id)
+        m365Config[
+            "authenticationUrl"
+        ] = "https://login.microsoftonline.com/{}/oauth2/v2.0/token".format(tenant_id)
         m365Config["graphUrl"] = "https://graph.microsoft.com/v1.0/"
         m365Config["betaUrl"] = "https://graph.microsoft.com/beta/"
-        m365Config["directoryObjects"] = m365Config["graphUrl"] + \
-            "directoryObjects"
+        m365Config["directoryObjects"] = m365Config["graphUrl"] + "directoryObjects"
 
         # Set the data for the token request
         m365Config["tokenData"] = {
             "client_id": client_id,
             "scope": "https://graph.microsoft.com/.default",
             "client_secret": client_secret,
-            "grant_type": "client_credentials"
+            "grant_type": "client_credentials",
         }
 
         m365Config["groupsUrl"] = m365Config["graphUrl"] + "groups"
         m365Config["usersUrl"] = m365Config["graphUrl"] + "users"
         m365Config["teamsUrl"] = m365Config["graphUrl"] + "teams"
-        m365Config["teamsTemplatesUrl"] = m365Config["graphUrl"] + \
-            "teamsTemplates"
+        m365Config["teamsTemplatesUrl"] = m365Config["graphUrl"] + "teamsTemplates"
         m365Config["teamsAppsUrl"] = m365Config["graphUrl"] + "appCatalogs/teamsApps"
         m365Config["directoryUrl"] = m365Config["graphUrl"] + "directory"
         m365Config["securityUrl"] = m365Config["betaUrl"] + "security"
 
         self._config = m365Config
 
     def config(self):
         return self._config
 
     def credentials(self):
         return self.config()["tokenData"]
 
-    def credentialsUser(self, username: str, password: str):
-        """ In some cases MS Graph APIs cannot be called via
+    def credentialsUser(self, username: str, password: str) -> dict:
+        """In some cases MS Graph APIs cannot be called via
             application permissions (client_id, client_secret)
-            but required a token of a user authenticated
+            but requires a token of a user authenticated
             with username + password. This is e.g. the case
             to upload a MS teams app to the catalog.
             See https://learn.microsoft.com/en-us/graph/api/teamsapp-publish
 
         Args:
             username (string): username
             password (string): password
-
         Returns:
-            Dict with the credentials for M365
+            dictionary: user credentials for M365
         """
+
         credentials = {
             "client_id": self.config()["clientId"],
             "scope": "https://graph.microsoft.com/.default",
             "client_secret": self.config()["clientSecret"],
             "grant_type": "password",
             "username": username,
             "password": password,
         }
         return credentials
 
-    def requestHeader(self, content_type: str = "application/json"):
+    # end method definition
+
+    def requestHeader(self, content_type: str = "application/json") -> dict:
         request_header = {
             "Authorization": "Bearer {}".format(self._access_token),
-            "Content-Type": content_type
+            "Content-Type": content_type,
         }
         return request_header
 
-    def requestHeaderUser(self, content_type: str = "application/json"):
+    # end method definition
+
+    def requestHeaderUser(self, content_type: str = "application/json") -> dict:
         request_header = {
             "Authorization": "Bearer {}".format(self._user_access_token),
-            "Content-Type": content_type
+            "Content-Type": content_type,
         }
         return request_header
 
+    # end method definition
+
     def parseRequestResponse(
         self,
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
     ) -> dict:
-        """Converts the request response to a Python dict in a safe way
-           that also handles exceptions. It first tries toload the response.text
+        """Converts the request response (JSon) to a Python dict in a safe way
+           that also handles exceptions. It first tries to load the response.text
            via json.loads() that produces a dict output. Only if response.text is
            not set or is empty it just converts the response_object to a dict using
            the vars() built-in method.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
-        Return: a python dict object or null in case of an error
+            additional_error_message (string, optional): use a more specific error message
+                                                         in case of an error
+            show_error (boolean): True: write an error to the log file 
+                                  False: write a warning to the log file
+        Returns:
+            dictionary: response information or None in case of an error
         """
 
         if not response_object:
             return None
 
         try:
             if response_object.text:
@@ -192,36 +216,38 @@
                 dict_object = vars(response_object)
         except json.JSONDecodeError as e:
             if additional_error_message:
                 message = "Cannot decode response as JSon. {}; error -> {}".format(
                     additional_error_message, e
                 )
             else:
-                message = "Cannot decode response as JSon; error -> {}".format(
-                    e)
+                message = "Cannot decode response as JSon; error -> {}".format(e)
             if show_error:
                 logger.error(message)
             else:
                 logger.warning(message)
             return None
         else:
             return dict_object
 
-    def existResultItem(self, response: dict, key: str, value: str, sub_dict_name: str = "") -> bool:
+    # end method definition
+
+    def existResultItem(
+        self, response: dict, key: str, value: str, sub_dict_name: str = ""
+    ) -> bool:
         """Check existence of key / value pair in the response properties of an MS Graph API call.
 
         Args:
             response (dictionary): REST response from an MS Graph REST Call
             key (string): property name (key)
             value (string): value to find in the item with the matching key
             sub_dict_name (string): some MS Graph API calls include nested
                                     dict structures that can be requested
                                     with an "expand" query parameter. In such
-                                    a case we use the sub_dict_name to access it. 
-
+                                    a case we use the sub_dict_name to access it.
         Returns:
             boolean: True if the value was found, False otherwise
         """
 
         if not response:
             return False
         if not "value" in response:
@@ -239,57 +265,59 @@
             for item in values:
                 if not sub_dict_name in item:
                     return False
                 if value == item[sub_dict_name][key]:
                     return True
         return False
 
+    # end method definition
+
     def getResultValue(self, response: dict, key: str, index: int = 0) -> str:
         """Get value of a result property with a given key of an MS Graph API call.
 
         Args:
             response (dictionary): REST response from an MS Graph REST Call
             key (string): property name (key)
             index (integer, optional): Index to use (1st element has index  0).
                                        Defaults to 0.
-
         Returns:
             string: value for the key, None otherwise
         """
 
         if not response:
             return None
         if not "value" in response:
             return None
 
         values = response["value"]
-        if not values or not isinstance(values, list) or len(values)-1 < index:
+        if not values or not isinstance(values, list) or len(values) - 1 < index:
             return None
 
         return values[index][key]
 
+    # end method definition
+
     def authenticate(self, revalidate: bool = False):
         """Authenticate at M365 Graph API with client ID and client secret.
 
         Args:
-            revalidate (boolean): determinse if a re-athentication is enforced
-                                  (e.g. if session has timed out with 401 error)
-        Return: Access token. Also stores access token in self._access_token
+            revalidate (boolean, optional): determinse if a re-athentication is enforced
+                                            (e.g. if session has timed out with 401 error)
+        Returns:
+            Access token. Also stores access token in self._access_token
         """
 
         # Already authenticated and session still valid?
         if self._access_token and not revalidate:
             return self._access_token
 
         request_url = self.config()["authenticationUrl"]
         request_header = requestLoginHeaders
 
-        logger.info(
-            "Requesting M365 Access Token from -> {}".format(request_url)
-        )
+        logger.info("Requesting M365 Access Token from -> {}".format(request_url))
 
         authenticate_post_body = self.credentials()
         authenticate_response = None
 
         try:
             authenticate_response = requests.post(
                 request_url,
@@ -301,17 +329,15 @@
                 "Unable to connect to -> {} : {}".format(
                     self.config()["authenticationUrl"], e
                 )
             )
             return None
 
         if authenticate_response.ok:
-            authenticate_dict = self.parseRequestResponse(
-                authenticate_response
-            )
+            authenticate_dict = self.parseRequestResponse(authenticate_response)
             if not authenticate_dict:
                 return None
             else:
                 access_token = authenticate_dict["access_token"]
                 logger.debug("Access Token -> {}".format(access_token))
         else:
             logger.error(
@@ -329,22 +355,25 @@
 
     def authenticateUser(self, username: str, password: str):
         """Authenticate at M365 Graph API with username and password.
 
         Args:
             username (string): name (emails) of the M365 user
             password (string): password of the M365 user
-        Return: Access token. Also stores access token in self._access_token
+        Returns:
+            Access token. Also stores access token in self._access_token
         """
 
         request_url = self.config()["authenticationUrl"]
         request_header = requestLoginHeaders
 
         logger.info(
-            "Requesting M365 Access Token for user -> {} from -> {}".format(username, request_url)
+            "Requesting M365 Access Token for user -> {} from -> {}".format(
+                username, request_url
+            )
         )
 
         authenticate_post_body = self.credentialsUser(username, password)
         authenticate_response = None
 
         try:
             authenticate_response = requests.post(
@@ -357,17 +386,15 @@
                 "Unable to connect to -> {} with username -> {}: {}".format(
                     self.config()["authenticationUrl"], username, e
                 )
             )
             return None
 
         if authenticate_response.ok:
-            authenticate_dict = self.parseRequestResponse(
-                authenticate_response
-            )
+            authenticate_dict = self.parseRequestResponse(authenticate_response)
             if not authenticate_dict:
                 return None
             else:
                 access_token = authenticate_dict["access_token"]
                 logger.debug("User Access Token -> {}".format(access_token))
         else:
             logger.error(
@@ -383,32 +410,30 @@
 
     # end method definition
 
     def getUsers(self):
         """Get list all all users in M365 tenant
 
         Returns:
-            List of all users. Example Values:
+            List of all users.
         """
 
         request_url = self.config()["usersUrl"]
         request_header = self.requestHeader()
 
-        logger.info(
-            "Get list of all users; calling -> {}".format(request_url))
+        logger.info("Get list of all users; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of users; status -> {}; error -> {}".format(
                         response.status_code, response.text
@@ -419,15 +444,14 @@
     # end method definition
 
     def getUser(self, user_email: str, show_error: bool = False):
         """Get a M365 User based on its email
 
         Args:
             user_email (string): M365 user email
-
         Returns:
             User information (json) or None if the user couldn't be retrieved (e.g. because it doesn't exist).
             Example Output:
             {
                 '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#users/$entity',
                 'businessPhones': [],
                 'displayName': 'Bob Davis',
@@ -442,26 +466,24 @@
                 'userPrincipalName': 'bdavis@M365x61936377.onmicrosoft.com'
             }
         """
 
         request_url = self.config()["usersUrl"] + "/" + user_email
         request_header = self.requestHeader()
 
-        logger.info(
-            "Get user -> {}; calling -> {}".format(user_email, request_url))
+        logger.info("Get user -> {}; calling -> {}".format(user_email, request_url))
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get user -> {}; status -> {}; error -> {}".format(
@@ -473,54 +495,54 @@
                 return None
 
     # end method definition
 
     def getGroups(self):
         """Get list all all groups in M365 tenant
 
+        Args:
+            None
         Returns:
-            List of all groups. Example Values:
+            List of all groups.
         """
 
         request_url = self.config()["groupsUrl"]
         request_header = self.requestHeader()
 
-        logger.info(
-            "Get list of all groups; calling -> {}".format(request_url))
+        logger.info("Get list of all groups; calling -> {}".format(request_url))
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of groups; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroup(self, group_name: str, show_error: bool = False):
+    def getGroup(self, group_name: str, show_error: bool = False) -> dict:
         """Get a M365 Group based on its name
 
         Args:
             group_name (string): M365 Group name
-
+            show_error (boolean): should an error be logged if group is not found.
         Returns:
-            Group information (json) or None if the group couldn't be created (e.g. because it exisits already).
+            dictionary: Group information or None if the group couldn't be created (e.g. because it exisits already).
             Example Output:
             {
                 '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#groups',
                 'value': [
                     {
                         'id': 'b65f7dba-3ed1-49df-91bf-2bf99affcc8d',
                         'deletedDateTime': None,
@@ -565,26 +587,24 @@
 
         query = {"$filter": "displayName eq '" + group_name + "'"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = self.config()["groupsUrl"] + "?" + encoded_query
         request_header = self.requestHeader()
 
-        logger.info(
-            "Get group -> {}; calling -> {}".format(group_name, request_url))
+        logger.info("Get group -> {}; calling -> {}".format(group_name, request_url))
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get group -> {}; status -> {}; error -> {}".format(
@@ -593,30 +613,34 @@
                     )
                 else:
                     logger.info("Group -> {} not found.".format(group_name))
                 return None
 
     # end method definition
 
-    def addGroup(self, name: str, security_enabled: bool = False, mail_enabled: bool = True):
+    def addGroup(
+        self, name: str, security_enabled: bool = False, mail_enabled: bool = True
+    ):
         """Add a M365 Group.
 
         Args:
             name (string): name of the group
+            security_enabled (boolean, optional): whether or not this group is used for permission management
+            mail_enabled (boolean, optional): whether or not this group is email enabled
         Returns:
-            Group information (json) or None if the group couldn't be created (e.g. because it exisits already).
+            dictionary: Group information or None if the group couldn't be created (e.g. because it exisits already).
             Example Output:
             {
                 '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#groups/$entity',
                 'id': '28906460-a69c-439e-84ca-c70becf37655',
                 'deletedDateTime': None,
                 'classification': None,
                 'createdDateTime': '2023-04-01T11:40:13Z',
                 'creationOptions': [],
-                'description': None, 
+                'description': None,
                 'displayName': 'Test',
                 'expirationDateTime': None,
                 'groupTypes': ['Unified'],
                 'isAssignableToRole': None,
                 'mail': 'Diefenbruch@M365x61936377.onmicrosoft.com',
                 'mailEnabled': True,
                 'mailNickname': 'Test',
@@ -643,37 +667,35 @@
         """
 
         group_post_body = {
             "displayName": name,
             "mailEnabled": mail_enabled,
             "mailNickname": name.replace(" ", ""),
             "securityEnabled": security_enabled,
-            "groupTypes": ["Unified"]
+            "groupTypes": ["Unified"],
         }
 
         request_url = self.config()["groupsUrl"]
         request_header = self.requestHeader()
 
-        logger.info(
-            "Adding M365 group -> {}; calling -> {}".format(name, request_url))
+        logger.info("Adding M365 group -> {}; calling -> {}".format(name, request_url))
         logger.debug("M365 group attributes -> {}".format(group_post_body))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(group_post_body),
                 headers=request_header,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add M365 group -> {}; status -> {}; error -> {}".format(
                         name, response.status_code, response.text
@@ -687,120 +709,117 @@
         self,
         email: str,
         password: str,
         first_name: str,
         last_name: str,
         location: str = "US",
         department: str = "",
-    ):
-        """Add M365 user.
+    ) -> dict:
+        """Add a M365 user.
 
         Args:
             email (string): email address of the user. This is also the unique identifier
             password (string): password of the user
             first_name (string): first name of the user
             last_name (string): last name of the user
             location (string, optional): country ISO 3166-1 alpha-2 format (e.g. US, CA, FR, DE, CN, ...)
             department (string, optional): department of the user
-
-        Return:
-            User information (json) or None if the user couldn't be created (e.g. because it exisits already).
+        Returns:
+            dictionary: User information or None if the user couldn't be created (e.g. because it exisits already).
         """
 
         user_post_body = {
             "accountEnabled": True,
             "displayName": first_name + " " + last_name,
             "givenName": first_name,
             "surname": last_name,
             "mailNickname": email.split("@")[0],
             "userPrincipalName": email,
             "passwordProfile": {
                 "forceChangePasswordNextSignIn": False,
-                "password": password
+                "password": password,
             },
-            "usageLocation": location
+            "usageLocation": location,
         }
         if department:
             user_post_body["department"] = department
 
         request_url = self.config()["usersUrl"]
         request_header = self.requestHeader()
 
-        logger.info(
-            "Adding M365 user -> {}; calling -> {}".format(email, request_url))
+        logger.info("Adding M365 user -> {}; calling -> {}".format(email, request_url))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(user_post_body),
                 headers=request_header,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add M365 user -> {}; status -> {}; error -> {}".format(
                         email, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def hasTeam(self, group_name: str) -> bool:
-        """ Checks if a M365 Group has a M365 Team connected or not
+        """Check if a M365 Group has a M365 Team connected or not
 
         Args:
             group_name (str): name of the M365 group
-
         Returns:
-            bool: Returns True if a Team is assigned and False otherwise
+            boolean: Returns True if a Team is assigned and False otherwise
         """
 
         response = self.getGroup(group_name)
         if response is None or not "value" in response or not response["value"]:
-            logger.error(
-                "M365 group -> {} not found.".format(
-                    group_name)
-            )
+            logger.error("M365 group -> {} not found.".format(group_name))
             return False
         group_id = response["value"][0]["id"]
 
-        request_url = self.config()["groupsUrl"] + "/" + group_id + '/team'
+        request_url = self.config()["groupsUrl"] + "/" + group_id + "/team"
         request_header = self.requestHeader()
 
         logger.info(
-            "Check if group -> {} has a M365 Team connected; calling -> {}".format(group_name, request_url))
+            "Check if group -> {} has a M365 Team connected; calling -> {}".format(
+                group_name, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
                 headers=request_header,
             )
 
             if response.status_code == 200:  # Group has a Team assigned!
                 logger.info(
-                    "Group -> {} has has a M365 team connected.".format(group_name))
+                    "Group -> {} has has a M365 team connected.".format(group_name)
+                )
                 return True
             elif response.status_code == 404:  # Group does not have a Team assigned!
                 logger.info(
-                    "Group -> {} has has no M365 team connected.".format(group_name))
+                    "Group -> {} has has no M365 team connected.".format(group_name)
+                )
                 return False
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to check if group -> {} has a Team connected; status -> {}; error -> {}".format(
                         group_name, response.status_code, response.text
@@ -811,234 +830,368 @@
     # end method definition
 
     def addTeam(self, name: str, template_name: str = "standard"):
         """Add M365 Team based on an existing M365 Group.
 
         Args:
             name (string): name of the team. It is assumed that a group with the same name does already exist!
-            template_name (string): name of the team template. "standard" is the default value.
+            template_name (string, optional): name of the team template. "standard" is the default value.
         Returns:
             Team information (json - empty text!) or None if the team couldn't be created (e.g. because it exisits already).
         """
 
         response = self.getGroup(name)
         if response is None or not "value" in response or not response["value"]:
             logger.error(
                 "M365 group -> {} not found. It is required for creating a corresponding M365 Team.".format(
-                    name)
+                    name
+                )
             )
             return None
         group_id = response["value"][0]["id"]
 
         response = self.getGroupOwners(name)
         if response is None or not "value" in response or not response["value"]:
             logger.warning(
                 "M365 group -> {} has no owners. This is required for creating a corresponding M365 Team.".format(
-                    name)
+                    name
+                )
             )
             return None
 
         team_post_body = {
-            "template@odata.bind": "{}('{}')".format(self.config()["teamsTemplatesUrl"], template_name),
+            "template@odata.bind": "{}('{}')".format(
+                self.config()["teamsTemplatesUrl"], template_name
+            ),
             "group@odata.bind": "{}('{}')".format(self.config()["groupsUrl"], group_id),
         }
 
         request_url = self.config()["teamsUrl"]
         request_header = self.requestHeader()
 
-        logger.info(
-            "Adding team -> {}; calling -> {}".format(name, request_url))
+        logger.info("Adding team -> {}; calling -> {}".format(name, request_url))
         logger.debug("Team Attributes -> {}".format(team_post_body))
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 data=json.dumps(team_post_body),
                 headers=request_header,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add team -> {}; status -> {}; error -> {}".format(
                         name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getUserLicenses(self, user_id: str) -> list:
-        """ Get the assigned license SKUs of a user
+    def deleteTeams(self, name: str) -> bool:
+        """Delete Microsoft 365 Teams with a specific name. Microsoft 365 allows
+            to have multiple teams with the same name. So this method may delete
+            multiple teams if the have the same name. The Graph API we use here
+            is the M365 Group API as deleting the group also deletes the associated team.
+
+        Args:
+            name (string): name of the Microsoft 365 Team
+        Returns:
+            boolean: True if teams have been deleted, False otherwise.
+        """
+
+        # We need a special handling of team names with single quotes:
+        escaped_group_name = name.replace("'", "''")
+        encoded_group_name = quote(escaped_group_name, safe="")
+        request_url = self.config()[
+            "groupsUrl"
+        ] + "?$filter=displayName eq '{}'".format(encoded_group_name)
+
+        request_header = self.requestHeader()
+
+        logger.info(
+            "Delete all Microsoft 365 Teams with name -> {}; calling -> {}".format(
+                name, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(request_url, headers=request_header)
+            if response.ok:
+                existing_teams = self.parseRequestResponse(response)
+                break
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                request_header = self.requestHeader()
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to get list of groups; status -> {}; error -> {}".format(
+                        response.status_code, response.text
+                    )
+                )
+                existing_teams = None
+                break
+
+        if existing_teams:
+            data = existing_teams.get("value")
+            if data:
+                counter = 0
+                for team in data:
+                    team_id = team.get("id")
+                    request_url = self.config()["groupsUrl"] + "/" + team_id
+                    response = requests.delete(request_url, headers=request_header)
+
+                    if not response.ok:
+                        logger.error(
+                            "Failed to delete team -> {} with ID -> {}".format(
+                                name, team_id
+                            )
+                        )
+                        continue
+                    counter += 1
+
+                logger.info(
+                    "{} teams with name -> {} have been deleted.".format(counter, name)
+                )
+                return True
+            else:
+                logger.info("No teams with name -> {} found.".format(name))
+                return False
+        else:
+            logger.error("Failed to retrieve teams with name -> {}".format(name))
+            return False
+
+    # end method definition
+
+    def deleteAllTeams(self, exception_list: list, pattern_list: list) -> bool:
+        """Delete all teams (groups) that are NOT on the exception list AND
+           that are matching at least one of the patterns in the provided pattern list.
+           This method is used for general cleanup of teams. Be aware that deleted teams
+           are still listed under https://admin.microsoft.com/#/deletedgroups
+
+        Args:
+            exception_list (list): list of group names that should not be deleted
+            pattern_list (list): list of patterns for group names to be deleted
+                                 (regular expression)
+        Returns:
+            boolean: True if teams have been deleted, False otherwise.
+        """
+
+        # Get list of all existing M365 groups/teams:
+        response = self.getGroups()
+        if not "value" in response or not response["value"]:
+            return False
+        groups = response["value"]
+
+        # Process all groups and check if the< should be
+        # deleted:
+        for group in groups:
+            group_name = group["displayName"]
+            # Check if group is in exception list:
+            if group_name in exception_list:
+                logger.info(
+                    "Group name -> {} is on the exception list. Skipping.".format(
+                        group_name
+                    )
+                )
+                continue
+            # Check that at least one pattern is found that matches the group:
+            for pattern in pattern_list:
+                result = re.search(pattern, group_name)
+                if result:
+                    logger.info(
+                        "Group name -> {} is matching pattern -> {}. Delete it now...".format(
+                            group_name, pattern
+                        )
+                    )
+                    self.deleteTeams(group_name)
+                    break
+            else:
+                logger.info(
+                    "Group name -> {} is not matching any delete pattern. Skipping.".format(
+                        group_name, pattern
+                    )
+                )
+        return True
+
+    # end method definition
+
+    def getUserLicenses(self, user_id: str) -> dict:
+        """Get the assigned license SKUs of a user
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
         Returns:
-            Response (dict) or None if request fails.
+            dictionary: List of user licenses or None if request fails.
             Example Output:
             {
                 '@odata.context': "https://graph.microsoft.com/v1.0/$metadata#users('a5875311-f0a5-486d-a746-bd7372b91115')/licenseDetails",
                 'value': [
                     {
                         'id': '8DRPYHK6IUOra-Nq6L0A7GAn38eBLPdOtXhbU5K1cd8',
                         'skuId': 'c7df2760-2c81-4ef7-b578-5b5392b571df',
                         'skuPartNumber': 'ENTERPRISEPREMIUM',
                         'servicePlans': [{...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, ...]
                     }
                 ]
-            }                                    
-        """ 
+            }
+        """
 
-        request_url = self.config()["usersUrl"] + \
-            "/" + user_id + "/licenseDetails"
+        request_url = self.config()["usersUrl"] + "/" + user_id + "/licenseDetails"
         request_header = self.requestHeader()
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
                 headers=request_header,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get licenses of user -> {}; status -> {}; error -> {}".format(
                         user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def assignLicenseToUser(self, user_id: str, sku_id: str):
+    def assignLicenseToUser(self, user_id: str, sku_id: str) -> dict:
         """Add an M365 license to a user (e.g. to use Office 365)
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             sku_id (string): M365 GUID of the SKU
                             (e.g. c7df2760-2c81-4ef7-b578-5b5392b571df for E5 and
                                   6fd2c87f-b296-42f0-b197-1e91e994b900 for E3)
 
         Returns:
-            Response (dict) or None if request fails
+            dictionary: response or None if request fails
         """
 
-        request_url = self.config()["usersUrl"] + \
-            "/" + user_id + "/assignLicense"
+        request_url = self.config()["usersUrl"] + "/" + user_id + "/assignLicense"
         request_header = self.requestHeader()
 
         # Construct the request body for assigning the E5 license
         license_post_body = {
             "addLicenses": [
                 {
                     "disabledPlans": [],
-                    "skuId": sku_id  # "c42b9cae-ea4f-4a69-9ca5-c53bd8779c42"
+                    "skuId": sku_id,  # "c42b9cae-ea4f-4a69-9ca5-c53bd8779c42"
                 }
             ],
-            "removeLicenses": []
+            "removeLicenses": [],
         }
 
         logger.info(
-            "Assign license -> {} to user -> {}; calling -> {}".format(sku_id, user_id, request_url))
+            "Assign license -> {} to user -> {}; calling -> {}".format(
+                sku_id, user_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 json=license_post_body,
                 headers=request_header,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add license -> {} to user -> {}; status -> {}; error -> {}".format(
                         sku_id, user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getUserPhoto(self, user_id: str):
+    def getUserPhoto(self, user_id: str, show_error: bool = True):
         """Get the photo of a M365 user
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
+            show_error (boolean): whether or not an error should be logged if the user
+                                  does not have a photo in M365
         Returns:
-            Response of Graph REST API (json) or None if the user photo couldn't be updated.
+            string: Image of the user photo or None if the user photo couldn't be retrieved.
         """
 
-        request_url = self.config()["usersUrl"] + \
-            "/" + user_id + "/photo/$value"
+        request_url = self.config()["usersUrl"] + "/" + user_id + "/photo/$value"
         # Set image as content type:
         request_header = self.requestHeader("image/*")
 
         logger.info(
-            "Get photo of user -> {}; calling -> {}".format(user_id, request_url))
+            "Get photo of user -> {}; calling -> {}".format(user_id, request_url)
+        )
 
         retries = 0
         while True:
-            response = requests.get(
-                request_url, headers=request_header)
+            response = requests.get(request_url, headers=request_header)
             if response.ok:
-                return response.content # this is the actual image - not json!
+                return response.content  # this is the actual image - not json!
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
-                logger.error(
-                    "Failed to get photo of user -> {}; status -> {}; error -> {}".format(
-                        user_id, response.status_code, response.text
+                if show_error:
+                    logger.error(
+                        "Failed to get photo of user -> {}; status -> {}; error -> {}".format(
+                            user_id, response.status_code, response.text
+                        )
                     )
-                )
+                else:
+                    logger.info("User -> {} does not yet have a photo.".format(user_id))
                 return None
 
     # end method definition
 
-    def updateUserPhoto(self, user_id: str, photo_path: str):
+    def updateUserPhoto(self, user_id: str, photo_path: str) -> dict:
         """Update the M365 user photo
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             photo_path (string): file system path with the location of the photo
-
         Returns:
-            Response of Graph REST API (json) or None if the user photo couldn't be updated.
+            dictionary: Response of Graph REST API or None if the user photo couldn't be updated.
         """
 
-        request_url = self.config()["usersUrl"] + \
-            "/" + user_id + "/photo/$value"
+        request_url = self.config()["usersUrl"] + "/" + user_id + "/photo/$value"
         # Set image as content type:
         request_header = self.requestHeader("image/*")
 
         # Check if the photo file exists
         if not os.path.isfile(photo_path):
             logger.error("Photo file -> {} not found!".format(photo_path))
             return None
@@ -1046,156 +1199,166 @@
         try:
             # Read the photo file as binary data
             with open(photo_path, "rb") as image_file:
                 photo_data = image_file.read()
         except OSError as e:
             # Handle any errors that occurred while reading the photo file
             logger.error(
-                "Error reading photo file -> {}; error -> {}".format(photo_path, e))
+                "Error reading photo file -> {}; error -> {}".format(photo_path, e)
+            )
             return None
 
         data = photo_data
 
         logger.info(
-            "Update user -> {} with photo -> {}; calling -> {}".format(user_id, photo_path, request_url))
+            "Update user -> {} with photo -> {}; calling -> {}".format(
+                user_id, photo_path, request_url
+            )
+        )
 
         retries = 0
         while True:
-            response = requests.put(
-                request_url, headers=request_header, data=data)
+            response = requests.put(request_url, headers=request_header, data=data)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user -> {} with photo -> {}; status -> {}; error -> {}".format(
                         user_id, photo_path, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroupMembers(self, group_name: str):
+    def getGroupMembers(self, group_name: str) -> dict:
         """Get members (users and groups) of the specified group.
 
         Args:
             group_name (string): name of the group
-
         Returns:
-            Response of Graph REST API (json) or None if the REST call fails.
+            dictionary: Response of Graph REST API or None if the REST call fails.
         """
 
         response = self.getGroup(group_name)
         if not response or not "value" in response or not response["value"]:
             logger.error(
-                "Group -> {} does not exist! Cannot retrieve group members.".format(group_name))
+                "Group -> {} does not exist! Cannot retrieve group members.".format(
+                    group_name
+                )
+            )
             return None
         group_id = response["value"][0]["id"]
 
         query = {"$select": "id,displayName,mail,userPrincipalName"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
-        request_url = self.config()["groupsUrl"] + "/" + \
-            group_id + "/members?" + encoded_query
+        request_url = (
+            self.config()["groupsUrl"] + "/" + group_id + "/members?" + encoded_query
+        )
         request_header = self.requestHeader()
 
         logger.info(
-            "Get members of group -> {} ({}); calling -> {}".format(group_name, group_id, request_url))
+            "Get members of group -> {} ({}); calling -> {}".format(
+                group_name, group_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get members of group -> {} ({}); status -> {}; error -> {}".format(
                         group_name, group_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroupOwners(self, group_name: str):
+    def getGroupOwners(self, group_name: str) -> dict:
         """Get owners (users) of the specified group.
 
         Args:
             group_name (string): name of the group
-
         Returns:
-            Response of Graph REST API (json) or None if the REST call fails.
+            dictionary: Response of Graph REST API or None if the REST call fails.
         """
 
         response = self.getGroup(group_name)
         if not response or not "value" in response or not response["value"]:
             logger.error(
-                "Group -> {} does not exist! Cannot retrieve group owners.".format(group_name))
+                "Group -> {} does not exist! Cannot retrieve group owners.".format(
+                    group_name
+                )
+            )
             return None
         group_id = response["value"][0]["id"]
 
         query = {"$select": "id,displayName,mail,userPrincipalName"}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
-        request_url = self.config()["groupsUrl"] + "/" + \
-            group_id + "/owners?" + encoded_query
+        request_url = (
+            self.config()["groupsUrl"] + "/" + group_id + "/owners?" + encoded_query
+        )
         request_header = self.requestHeader()
 
         logger.info(
-            "Get owners of group -> {} ({}); calling -> {}".format(group_name, group_id, request_url))
+            "Get owners of group -> {} ({}); calling -> {}".format(
+                group_name, group_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get owners of group -> {} ({}); status -> {}; error -> {}".format(
                         group_name, group_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addGroupMember(self, group_id: str, member_id: str):
-        """Add a member (user or group) to a (parent) group 
+    def addGroupMember(self, group_id: str, member_id: str) -> dict:
+        """Add a member (user or group) to a (parent) group
 
         Args:
             group_id (string): M365 GUID of the group
             member_id (string): M365 GUID of the new member
-
         Returns:
-            Result JSon
+            dictionary: response of the MS Graph API call or None if the call fails.
         """
 
-        request_url = self.config()["groupsUrl"] + \
-            "/" + group_id + "/members/$ref"
+        request_url = self.config()["groupsUrl"] + "/" + group_id + "/members/$ref"
         request_header = self.requestHeader()
 
         group_member_post_body = {
             "@odata.id": self.config()["directoryObjects"] + "/" + member_id
         }
 
         logger.info(
@@ -1203,49 +1366,52 @@
                 member_id, group_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
-                request_url, headers=request_header, data=json.dumps(group_member_post_body))
+                request_url,
+                headers=request_header,
+                data=json.dumps(group_member_post_body),
+            )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add member -> {} to group -> {}; status -> {}; error -> {}".format(
                         member_id, group_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def isMember(self, group_id: str, member_id: str, show_error: bool = True) -> bool:
-        """ Checks whether a M365 user is already in a M365 group
+        """Checks whether a M365 user is already in a M365 group
 
         Args:
             group_id (string): M365 GUID of the group
             member_id (string): M365 GUID of the user (member)
             show_error (boolean): whether or not an error should be logged if the user
                                   is not a member of the group
         Returns:
-            bool: True if the user is in the group. False otherwise.
+            boolean: True if the user is in the group. False otherwise.
         """
 
         # don't encode this URL - this has not been working!!
-        request_url = self.config(
-        )["groupsUrl"] + "/{}/members?$filter=id eq '{}'".format(group_id, member_id)
+        request_url = self.config()[
+            "groupsUrl"
+        ] + "/{}/members?$filter=id eq '{}'".format(group_id, member_id)
         request_header = self.requestHeader()
 
         logger.info(
             "Check if user -> {} is in group -> {}; calling -> {}".format(
                 member_id, group_id, request_url
             )
         )
@@ -1256,16 +1422,15 @@
             if response.ok:
                 response = self.parseRequestResponse(response)
                 if not "value" in response or len(response["value"]) == 0:
                     return False
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 # MS Graph API returns an error if the member is not in the
                 # group. This is typically not what we want. We just return False.
                 if show_error:
@@ -1274,27 +1439,25 @@
                             member_id, group_id, response.status_code, response.text
                         )
                     )
                 return False
 
     # end method definition
 
-    def addGroupOwner(self, group_id: str, owner_id: str):
-        """Add an owner (user) to a group 
+    def addGroupOwner(self, group_id: str, owner_id: str) -> dict:
+        """Add an owner (user) to a group
 
         Args:
-            group_id (string): M365 GUID of the groups
+            group_id (string): M365 GUID of the group
             owner_id (string): M365 GUID of the new member
-
         Returns:
-            Result JSon
+            dictionary: response of the MS Graph API call or None if the call fails.
         """
 
-        request_url = self.config()["groupsUrl"] + \
-            "/" + group_id + "/owners/$ref"
+        request_url = self.config()["groupsUrl"] + "/" + group_id + "/owners/$ref"
         request_header = self.requestHeader()
 
         group_member_post_body = {
             "@odata.id": self.config()["directoryObjects"] + "/" + owner_id
         }
 
         logger.info(
@@ -1302,56 +1465,60 @@
                 owner_id, group_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
-                request_url, headers=request_header, data=json.dumps(group_member_post_body))
+                request_url,
+                headers=request_header,
+                data=json.dumps(group_member_post_body),
+            )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to add owner -> {} to group -> {}; status -> {}; error -> {}".format(
                         owner_id, group_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def purgeDeletedItems(self):
-        """This purges all deleted users and groups.
-           Purging users and groups requires administrative rights that typically
-           are not provided in Contoso example org.
+        """Purge all deleted users and groups.
+        Purging users and groups requires administrative rights that typically
+        are not provided in Contoso example org.
         """
 
         request_header = self.requestHeader()
 
-        request_url = self.config()["directoryUrl"] + \
-            "/deletedItems/microsoft.graph.group"
+        request_url = (
+            self.config()["directoryUrl"] + "/deletedItems/microsoft.graph.group"
+        )
         response = requests.get(
             request_url,
             headers=request_header,
         )
         deleted_groups = self.parseRequestResponse(response)
 
         for group in deleted_groups["value"]:
             group_id = group["id"]
             response = self.purgeDeletedItem(group_id)
 
-        request_url = self.config()["directoryUrl"] + \
-            "/deletedItems/microsoft.graph.user"
+        request_url = (
+            self.config()["directoryUrl"] + "/deletedItems/microsoft.graph.user"
+        )
         response = requests.get(
             request_url,
             headers=request_header,
         )
         deleted_users = self.parseRequestResponse(response)
 
         for user in deleted_users["value"]:
@@ -1363,163 +1530,164 @@
     def purgeDeletedItem(self, item_id: str):
         """Helper method to purge a single deleted user or group.
            This requires elevated permissions that are typically
            not available via Graph API.
 
         Args:
             item_id (string): M365 GUID of the user or group to purge
-
         Returns:
-            Reponse of the REST API or None if the call fails.
+            dictionary: response of the MS Graph API call or None if the call fails.
         """
 
-        request_url = self.config()["directoryUrl"] + \
-            "/deletedItems/" + item_id
+        request_url = self.config()["directoryUrl"] + "/deletedItems/" + item_id
         request_header = self.requestHeader()
 
         logger.info(
-            "Purging deleted item -> {}; calling -> {}".format(item_id, request_url))
+            "Purging deleted item -> {}; calling -> {}".format(item_id, request_url)
+        )
 
         retries = 0
         while True:
-            response = requests.delete(
-                request_url,
-                headers=request_header
-            )
+            response = requests.delete(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to purge deleted item -> {}; status -> {}; error -> {}".format(
                         item_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getTeamsApps(self, filter_expression: str = ""):
-        """ Get a list of MS Teams apps in catalog that match a given filter criterium
+    def getTeamsApps(self, filter_expression: str = "") -> dict:
+        """Get a list of MS Teams apps in catalog that match a given filter criterium
 
         Args:
             filter_expression (string, optional): filter string see https://learn.microsoft.com/en-us/graph/filter-query-parameter
-
         Returns:
-            Request response (dict) or None if request fails
+            dictionary: response of the MS Graph API call or None if the call fails.
         """
 
         if filter_expression:
             query = {"$filter": filter_expression}
             encoded_query = urllib.parse.urlencode(query, doseq=True)
             request_url = self.config()["teamsAppsUrl"] + "?" + encoded_query
             logger.info(
-                "Get list of MS Teams Apps using filter -> {}; calling -> {}".format(filter_expression, request_url))
+                "Get list of MS Teams Apps using filter -> {}; calling -> {}".format(
+                    filter_expression, request_url
+                )
+            )
         else:
             request_url = self.config()["teamsAppsUrl"]
             logger.info(
-                "Get list of all MS Teams Apps; calling -> {}".format(request_url))
+                "Get list of all MS Teams Apps; calling -> {}".format(request_url)
+            )
 
         request_header = self.requestHeader()
 
         retries = 0
         while True:
-            response = requests.get(
-                request_url,
-                headers=request_header
-            )
+            response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of MS Teams apps; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getTeamsAppsOfUser(self, user_id: str, filter_expression: str = ""):
-        """ Get a list of MS Teams apps of a user that match a given filter criterium
+    def getTeamsAppsOfUser(self, user_id: str, filter_expression: str = "") -> dict:
+        """Get a list of MS Teams apps of a user that match a given filter criterium
 
         Args:
             user_id (string): M365 GUID of the user (can also be the M365 email of the user)
             filter_expression (string, optional): filter string see https://learn.microsoft.com/en-us/graph/filter-query-parameter
-
         Returns:
-            Request response (dict) or None if request fails
+            dictionary: response of the MS Graph API call or None if the call fails.
         """
 
         query = {"$expand": "teamsAppDefinition"}
         if filter_expression:
             query["$filter"] = filter_expression
 
         encoded_query = urllib.parse.urlencode(query, doseq=True)
-        request_url = self.config()["usersUrl"] + "/" + user_id + f"/teamwork/installedApps?" + encoded_query
+        request_url = (
+            self.config()["usersUrl"]
+            + "/"
+            + user_id
+            + "/teamwork/installedApps?"
+            + encoded_query
+        )
         logger.info(
-            "Get list of MS Teams Apps for user -> {} using query -> {}; calling -> {}".format(user_id, query, request_url))
+            "Get list of MS Teams Apps for user -> {} using query -> {}; calling -> {}".format(
+                user_id, query, request_url
+            )
+        )
 
         request_header = self.requestHeader()
 
         retries = 0
         while True:
-            response = requests.get(
-                request_url,
-                headers=request_header
-            )
+            response = requests.get(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of MS Teams for user -> {}; status -> {}; error -> {}".format(
                         user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def uploadTeamsApp(self, app_path: str, update_existing_app: bool = False, app_id: str = ""):
-        """ Upload a new app package to the catalog of MS Teams apps.
+    def uploadTeamsApp(
+        self, app_path: str, update_existing_app: bool = False, app_id: str = ""
+    ) -> dict:
+        """Upload a new app package to the catalog of MS Teams apps.
             This is not possible with client secret credentials
             but requires a token of a user authenticated
             with username + password.
             See https://learn.microsoft.com/en-us/graph/api/teamsapp-publish
             (permissions table on that page)
 
         Args:
             app_path (string): file path (with directory) to the app package to upload
-
         Returns:
-            Response of the REST call or None if the reuqest fails
+            dictionary: Response of the MS GRAPH API REST call or None if the request fails
         """
 
         if update_existing_app and not app_id:
-            logger.error("To update an existing app you need to provide the existing App ID!")
+            logger.error(
+                "To update an existing app you need to provide the existing App ID!"
+            )
             return None
 
         if not os.path.exists(app_path):
             logger.error("Teams App file -> {} does not exist!")
             return None
 
         # Ensure that the app file is a zip file
@@ -1538,33 +1706,37 @@
 
         with open(app_path, "rb") as f:
             app_data = f.read()
 
         with zipfile.ZipFile(app_path) as z:
             # Ensure that the app file contains a manifest.json file
             if "manifest.json" not in z.namelist():
-                logger.error("Teams App file -> {} does not contain a manifest.json file!")
+                logger.error(
+                    "Teams App file -> {} does not contain a manifest.json file!"
+                )
                 return None
 
         logger.info(
-            "Upload Teams App -> {} to the MS Teams catalog; calling -> {}".format(app_path, request_url))
+            "Upload Teams App -> {} to the MS Teams catalog; calling -> {}".format(
+                app_path, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
-                # headers=request_header, files=upload_files
-                headers=request_header, data=app_data
+                headers=request_header,
+                data=app_data,
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 if update_existing_app:
                     logger.warning(
                         "Failed to update existing MS teams app -> {} (may be because it is not a new version); status -> {}; error -> {}".format(
@@ -1578,115 +1750,168 @@
                         )
                     )
                 return None
 
     # end method definition
 
     def removeTeamsApp(self, app_id: str):
+        """Remove MS Teams App for the app catalog
+
+        Args:
+            app_id (string): Microsoft 365 GUID of the MS Teams app
+        """
+
         request_url = self.config()["teamsAppsUrl"] + "/" + app_id
         # Here we need the credentials of an authenticated user!
         # (not the application credentials (client_id, client_secret))
         request_header = self.requestHeaderUser()
 
         # Make the DELETE request to remove the app from the app catalog
         response = requests.delete(request_url, headers=request_header)
 
         # Check the status code of the response
         if response.status_code == 204:
-            logger.info("The app with ID -> {} has been successfully removed from the app catalog.".format(app_id))
+            logger.info(
+                "The app with ID -> {} has been successfully removed from the app catalog.".format(
+                    app_id
+                )
+            )
         else:
-            logger.error("An error occurred while removing the app from the app catalog. Status code -> {}. Error message -> {}".format(response.status_code, response.text))
+            logger.error(
+                "An error occurred while removing the app from the app catalog. Status code -> {}. Error message -> {}".format(
+                    response.status_code, response.text
+                )
+            )
 
     # end method definition
 
-    def assignTeamsAppToUser(self, user_id: str, app_name: str):
+    def assignTeamsAppToUser(self, user_id: str, app_name: str) -> dict:
+        """Assigns (adds) a MS teams app to a M365 user.
+
+        Args:
+            user_id (string): M365 GUID of the user (can also be the M365 email of the user)
+            app_name (string): exact name of the app
+        Returns:
+            dictionary: response of the MS Graph API call or None if the call fails.
+        """
 
         app = self.getTeamsApps("contains(displayName, '{}')".format(app_name))
         if not app or not app["value"]:
             logger.error("App -> {} not found!".format(app_name))
             return None
         app_id = self.getResultValue(app, "id", 0)
 
-        request_url = self.config()["usersUrl"] + "/" + user_id + "/teamwork/installedApps"
+        request_url = (
+            self.config()["usersUrl"] + "/" + user_id + "/teamwork/installedApps"
+        )
         request_header = self.requestHeader()
 
         post_body = {
             "teamsApp@odata.bind": self.config()["teamsAppsUrl"] + "/" + app_id
         }
 
         logger.info(
-            "Assign teams app -> {} ({}) to user -> {}; calling -> {}".format(app_name, app_id, user_id, request_url))
+            "Assign teams app -> {} ({}) to user -> {}; calling -> {}".format(
+                app_name, app_id, user_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.post(
-                request_url,
-                json=post_body,
-                headers=request_header
+                request_url, json=post_body, headers=request_header
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign teams app -> {} ({}) to user -> {}; status -> {}; error -> {}".format(
                         app_name, app_id, user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def upgradeTeamsAppOfUser(self, user_id: str, app_name: str):
+    def upgradeTeamsAppOfUser(self, user_id: str, app_name: str) -> dict:
+        """Upgrade a MS teams app for a user. The call will fail if the user does not
+            already have the app assigned. So this needs to be checked before
+            calling this method.
 
-        app = self.getTeamsAppsOfUser(user_id, "contains(teamsAppDefinition/displayName, '{}')".format(app_name))
+        Args:
+            user_id (string): M365 GUID of the user (can also be the M365 email of the user)
+            app_name (string): exact name of the app
+        Returns:
+            dictionary: response of the MS Graph API call or None if the call fails.
+        """
+
+        app = self.getTeamsAppsOfUser(
+            user_id, "contains(teamsAppDefinition/displayName, '{}')".format(app_name)
+        )
         if not app or not app["value"]:
             logger.error("App -> {} not found!".format(app_name))
             return None
         app_id = self.getResultValue(app, "id", 0)
 
-        request_url = self.config()["usersUrl"] + "/" + user_id + "/teamwork/installedApps/" + app_id + "/upgrade"
+        request_url = (
+            self.config()["usersUrl"]
+            + "/"
+            + user_id
+            + "/teamwork/installedApps/"
+            + app_id
+            + "/upgrade"
+        )
         request_header = self.requestHeader()
 
         logger.info(
-            "Upgrade teams app -> {} ({}) of user -> {}; calling -> {}".format(app_name, app_id, user_id, request_url))
+            "Upgrade teams app -> {} ({}) of user -> {}; calling -> {}".format(
+                app_name, app_id, user_id, request_url
+            )
+        )
 
         retries = 0
         while True:
-            response = requests.post(
-                request_url,
-                headers=request_header
-            )
+            response = requests.post(request_url, headers=request_header)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to upgrade teams app -> {} ({}) of user -> {}; status -> {}; error -> {}".format(
                         app_name, app_id, user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addSensitivityLabel(self, name: str, display_name: str, description: str = "", color: str = "red", enabled: bool = True, admin_description: str = "", user_description: str = "", enable_encryption: bool = False, enable_marking: bool = False):
-        """ Create a new sensitivity label in M365
+    def addSensitivityLabel(
+        self,
+        name: str,
+        display_name: str,
+        description: str = "",
+        color: str = "red",
+        enabled: bool = True,
+        admin_description: str = "",
+        user_description: str = "",
+        enable_encryption: bool = False,
+        enable_marking: bool = False,
+    ):
+        """Create a new sensitivity label in M365
             THIS IS CURRENTLY NOT WORKING!
 
         Args:
             name (string): _description_
             display_name (string): _description_
             description (string, optional): _description_. Defaults to "".
             color (string, optional): _description_. Defaults to "red".
@@ -1705,81 +1930,82 @@
             "displayName": display_name,
             "description": description,
             "isEnabled": enabled,
             "labelColor": color,
             "adminDescription": admin_description,
             "userDescription": user_description,
             "encryptContent": enable_encryption,
-            "contentMarking": enable_marking
+            "contentMarking": enable_marking,
         }
 
         request_url = self.config()["securityUrl"] + "/sensitivityLabels"
         request_header = self.requestHeader()
 
         logger.info(
-            "Create sensitivity label -> {}; calling -> {}".format(name, request_url))
+            "Create sensitivity label -> {}; calling -> {}".format(name, request_url)
+        )
 
         # Send the POST request to create the label
-        response = requests.post(request_url, headers=request_header,
-                                 data=json.dumps(payload))
+        response = requests.post(
+            request_url, headers=request_header, data=json.dumps(payload)
+        )
 
         # Check the response status code
         if response.status_code == 201:
-            logger.info(
-                "Label -> {} has been created successfully!".format(name))
+            logger.info("Label -> {} has been created successfully!".format(name))
             return response
         else:
-            logger.error("Failed to create the label -> {}! Response status code: {}".format(
-                name, response.status_code))
+            logger.error(
+                "Failed to create the label -> {}! Response status code: {}".format(
+                    name, response.status_code
+                )
+            )
             return None
 
     # end method definition
 
     def assignSensitivityLabelToUser(self, user_email: str, label_name: str):
-        """ Assigns a existing sensitivity label to a user.
+        """Assigns a existing sensitivity label to a user.
             THIS IS CURRENTLY NOT WORKING!
 
         Args:
             user_email (string): email address of the user (as unique identifier)
             label_name (string): name of the label (need to exist)
 
         Returns:
             Return the request response or None if the request fails.
         """
 
         # Set up the request body with the label name
-        body = {
-            "labelName": label_name
-        }
+        body = {"labelName": label_name}
 
-        request_url = self.config()["usersUrl"] + \
-            "/" + user_email + "/assignSensitivityLabels"
+        request_url = (
+            self.config()["usersUrl"] + "/" + user_email + "/assignSensitivityLabels"
+        )
         request_header = self.requestHeader()
 
         logger.info(
-            "Assign label -> {} to user -> {}; calling -> {}".format(label_name, user_email, request_url))
+            "Assign label -> {} to user -> {}; calling -> {}".format(
+                label_name, user_email, request_url
+            )
+        )
 
         retries = 0
         while True:
-            response = requests.post(
-                request_url,
-                headers=request_header, json=body
-            )
+            response = requests.post(request_url, headers=request_header, json=body)
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign label -> {} to user -> {}; status -> {}; error -> {}".format(
                         label_name, user_email, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
-
```

### Comparing `pyxecm-0.0.16/pyxecm/main.py` & `pyxecm-0.0.17/pyxecm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 O365_CLIENT_ID = os.environ.get("O365_CLIENT_ID")
 O365_CLIENT_SECRET = os.environ.get("O365_CLIENT_SECRET")
 O365_USER = os.environ.get("O365_USER", "")
 O365_PASSWORD = os.environ.get("O365_PASSWORD", "")
 O365_DOMAIN = os.environ.get("O365_DOMAIN")
 O365_SKU_ID = os.environ.get(
     "O365_SKU_ID", "c7df2760-2c81-4ef7-b578-5b5392b571df"
-)  # Office 365 E5
+)  # Office 365 E5, used as default SKU for users
 O365_TEAMS_APP_NAME = "OpenText Extended ECM"
 
 # Configure logging output
 logging.basicConfig(
     format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=logging.INFO if LOGLEVEL == "INFO" else logging.DEBUG,
@@ -182,43 +182,54 @@
 )
 logger = logging.getLogger(os.path.basename(__file__))
 
 
 def initM365() -> object:
     """Initialize the M365 object we use to talk to the Microsoft Graph API.
 
-    Args: None
-    Return:
-        M365 object
+    Args:
+        None
+    Returns:
+        object: M365 object or None if the object couldn't be created or
+                the authentication fails.
     """
 
-    logger.info("Microsoft 365 Tenant ID     = " + O365_TENANT_ID)
-    logger.info("Microsoft 365 Client ID     = " + O365_CLIENT_ID)
-    logger.debug("Microsoft 365 Client Secret = " + O365_CLIENT_SECRET)
-    logger.info("Microsoft 365 User          = "
+    logger.info("Microsoft 365 Tenant ID             = " + O365_TENANT_ID)
+    logger.info("Microsoft 365 Client ID             = " + O365_CLIENT_ID)
+    logger.debug("Microsoft 365 Client Secret         = " + O365_CLIENT_SECRET)
+    logger.info(
+        "Microsoft 365 User                  = "
         + (O365_USER if O365_USER != "" else "<not configured>")
     )
-    logger.debug("Microsoft 365 Password      = "
+    logger.debug(
+        "Microsoft 365 Password              = "
         + (O365_PASSWORD if O365_PASSWORD != "" else "<not configured>")
     )
-    logger.info("Microsoft 365 Domain        = " + O365_DOMAIN)
-    logger.info("Microsoft 365 License SKU   = " + O365_SKU_ID)
-    logger.info("Microsoft 365 Teams App     = " + O365_TEAMS_APP_NAME)
+    logger.info("Microsoft 365 Domain                = " + O365_DOMAIN)
+    logger.info("Microsoft 365 Default License SKU   = " + O365_SKU_ID)
+    logger.info("Microsoft 365 Teams App             = " + O365_TEAMS_APP_NAME)
 
     m365_object = m365.M365(
-        O365_TENANT_ID, O365_CLIENT_ID, O365_CLIENT_SECRET, O365_DOMAIN, O365_SKU_ID, O365_TEAMS_APP_NAME
+        O365_TENANT_ID,
+        O365_CLIENT_ID,
+        O365_CLIENT_SECRET,
+        O365_DOMAIN,
+        O365_SKU_ID,
+        O365_TEAMS_APP_NAME,
     )
 
     if m365_object and m365_object.authenticate():
         logger.info("Connected to Microsoft Graph API.")
         return m365_object
     else:
-        logger.error("Failed toconnect to Microsoft Graph API.")
+        logger.error("Failed to connect to Microsoft Graph API.")
         return None
 
+    # end function definition
+
 
 def initK8s(inCluster: bool = True) -> object:
     """Initialize the Kubernetes object we use to talk to the Kubernetes API.
 
     Args:
         inCluster (boolean): controls wether the code runs inside a pod (inCluster = True)
                              or locally (access via .kube / kubectl, inCluster = False)
@@ -268,21 +279,24 @@
         "Stateful Set -> {} has -> {} replicas".format(
             OTCS_K8S_STATEFUL_SET_BACKEND, otcs_replicas_backend
         )
     )
 
     return k8s_object
 
+    # end function definition
+
 
 def initOTDS():
     """Initialize the OTDS object and parameters and authenticate at OTDS once it is ready.
 
-    Args: None
-    Return:
-        OTDS object
+    Args:
+        None
+    Returns:
+        object: OTDS object
     """
 
     logger.info("Connection parameters OTDS:")
     logger.info("OTDS Protocol          = " + OTDS_PROTOCOL)
     logger.info("OTDS Public Protocol   = " + OTDS_PUBLIC_PROTOCOL)
     logger.info("OTDS Hostname          = " + OTDS_HOSTNAME)
     logger.info("OTDS Public URL        = " + OTDS_PUBLIC_URL)
@@ -303,14 +317,15 @@
         otds_cookie = otds_object.authenticate()
     logger.info("OTDS is ready now.")
 
     logger.info("Enable OTDS audit...")
     otds_object.enableAudit()
 
     return otds_object
+
     # end function definition
 
 
 def initOTAC(k8s_object: object) -> object:
     """Initialize the OTAC object and parameters.
        Configure the Archive Server as a known server
        if environment variable OTAC_KNOWN_SERVER is set.
@@ -329,15 +344,21 @@
     logger.debug("OTAC Admin Password   = " + OTAC_PASSWORD)
     logger.info(
         "OTAC Known Server      = "
         + (OTAC_KNOWN_SERVER if OTAC_KNOWN_SERVER != "" else "<not configured>")
     )
 
     otac_object = otac.OTAC(
-        OTAC_PROTOCOL, OTAC_HOSTNAME, OTAC_PORT, OTAC_ADMIN, OTAC_PASSWORD, OTDS_ADMIN, OTDS_PASSWORD
+        OTAC_PROTOCOL,
+        OTAC_HOSTNAME,
+        OTAC_PORT,
+        OTAC_ADMIN,
+        OTAC_PASSWORD,
+        OTDS_ADMIN,
+        OTDS_PASSWORD,
     )
 
     # is there a known server configured for Archive Center (to sync content with)
     if otac_object and OTAC_KNOWN_SERVER != "":
         # wait until the OTAC pod is in ready state
         logger.info("Waiting for Archive Center to become ready...")
         k8s_object.waitPodCondition(OTAC_K8S_POD_NAME, "Ready")
@@ -372,26 +393,26 @@
 
 
 def initOTCS(
     otds_object: object,
     hostname: str = OTCS_HOSTNAME,
     port: int = OTCS_HOSTNAME,
     partition_name: str = OTCS_PARTITION,
-    resource_name: str = OTCS_RESOURCE_NAME
+    resource_name: str = OTCS_RESOURCE_NAME,
 ) -> object:
     """Initialize the OTCS class and parameters and authenticate at OTCS once it is ready.
 
     Args:
         otds_object (object): OTDS object that has been created before
         hostname (string): OTCS hostname
         port (integer): port number of OTCS
         partition_name: name of OTDS Partition for Extended ECM users
         resource_name: name of OTDS resource for Extended ECM
-    Return:
-        OTCS object
+    Returns:
+        object: OTCS object
     """
 
     global placeholder_values
 
     logger.info("Connection parameters OTCS (Extended ECM):")
     logger.info("OTCS Protocol              = " + OTCS_PROTOCOL)
     logger.info("OTCS Public Protocol       = " + OTCS_PUBLIC_PROTOCOL)
@@ -403,15 +424,21 @@
     logger.info("OTCS User Partition        = " + partition_name)
     logger.info("OTCS Resource Name         = " + resource_name)
     logger.info("OTCS User Default License  = " + OTCS_LICENSE_FEATURE)
     logger.info("OTCS K8s Frontend Pods     = " + OTCS_K8S_STATEFUL_SET_FRONTEND)
     logger.info("OTCS K8s Backend Pods      = " + OTCS_K8S_STATEFUL_SET_BACKEND)
 
     otcs_object = otcs.OTCS(
-        OTCS_PROTOCOL, hostname, port, OTCS_ADMIN, OTCS_PASSWORD, partition_name, resource_name
+        OTCS_PROTOCOL,
+        hostname,
+        port,
+        OTCS_ADMIN,
+        OTCS_PASSWORD,
+        partition_name,
+        resource_name,
     )
 
     # It is important to wait for OTCS to be configured - otherwise we
     # may interfere with the OTCS container automation and run into errors
     logger.info("Wait for OTCS to be configured...")
     otcs_configured = otcs_object.isConfigured()
     while not otcs_configured:
@@ -446,62 +473,73 @@
             "logoutURL"
         ] = f"{OTAWP_PUBLIC_PROTOCOL}://{OTAWP_PUBLIC_URL}/home/system/wcp/sso/sso_logout.htm"
         otcs_resource["logoutMethod"] = "GET"
 
         otds_object.updateResource(name="cs", resource=otcs_resource)
 
     return otcs_object
+
     # end function definition
 
+
 def initOTIV(otds_object: object) -> object:
     """Initialize the OTIV (Intelligent Viewing) object and its OTDS settings.
 
     Args:
         otds_object (object): OTDS object
-    Return:
-        otiv_object (object): OTIV object
+    Returns:
+        objects: OTIV object
     """
 
     logger.info("Parameters for OTIV (Intelligent Viewing):")
     logger.info("OTDS Resource Name       = " + OTIV_RESOURCE_NAME)
     logger.info("OTIV License File        = " + OTIV_LICENSE_FILE)
     logger.info("OTIV Product Name        = " + OTIV_PRODUCT_NAME)
     logger.info("OTIV Product Description = " + OTIV_PRODUCT_DESCRIPTION)
     logger.info("OTIV License Feature     = " + OTIV_LICENSE_FEATURE)
 
-    otiv_object = otiv.OTIV(OTIV_RESOURCE_NAME, OTIV_PRODUCT_NAME,
-                            OTIV_PRODUCT_DESCRIPTION, OTIV_LICENSE_FILE, OTIV_LICENSE_FEATURE)
+    otiv_object = otiv.OTIV(
+        OTIV_RESOURCE_NAME,
+        OTIV_PRODUCT_NAME,
+        OTIV_PRODUCT_DESCRIPTION,
+        OTIV_LICENSE_FILE,
+        OTIV_LICENSE_FEATURE,
+    )
 
     otds_resource = otds_object.getResource(OTIV_RESOURCE_NAME)
     if not otds_resource:
         logger.error("OTDS Resource -> {} for Intelligent Viewing not found.")
         return
 
     otiv_license = otds_object.addLicenseToResource(
         OTIV_LICENSE_FILE,
         OTIV_PRODUCT_NAME,
         OTIV_PRODUCT_DESCRIPTION,
         otds_resource["resourceID"],
     )
     if not otiv_license:
         logger.info(
-            "Couldn't apply license -> {} for product -> {}. Intelligent Viewing may not be deployed!".format(OTIV_LICENSE_FILE, OTIV_PRODUCT_NAME))
+            "Couldn't apply license -> {} for product -> {}. Intelligent Viewing may not be deployed!".format(
+                OTIV_LICENSE_FILE, OTIV_PRODUCT_NAME
+            )
+        )
         return None
-    
+
     return otiv_object
 
     # end function definition
 
 
 def initOTPD(k8s_object: object) -> object:
     """Initialize the OTPD (PowerDocs) object and parameters.
 
-    Args: None
-    Return:
-        OTPD (PowerDocs) object
+    Args:
+        None
+    Returns:
+        object: OTPD (PowerDocs) object
     """
 
     logger.info("Connection parameters OTPD (PowerDocs):")
     logger.info("OTPD Protocol             = " + OTPD_PROTOCOL)
     logger.info("OTPD Hostname             = " + OTPD_HOSTNAME)
     logger.info("OTPD Port                 = " + str(OTPD_PORT))
     logger.info("OTPD API User             = " + OTPD_USER)
@@ -880,18 +918,20 @@
     otds_object.impersonateResource(OTAWP_RESOURCE_NAME)
 
     # end function definition
 
 
 def restartOTCSPods(otcs_object: object, k8s_object: object):
     """Restart the Content Server service in all OTCS pods
+
     Args:
         otcs_object: OTCS class instance (object)
         k8s_object: Kubernetes object
-    Return: None
+    Returns:
+        None
     """
 
     global otcs_replicas_frontend
     global otcs_replicas_backend
 
     # Restart all frontends:
     for x in range(0, otcs_replicas_frontend):
@@ -938,51 +978,56 @@
 
     for x in range(0, otcs_replicas_backend):
         pod_name = OTCS_K8S_STATEFUL_SET_BACKEND + "-" + str(x)
 
         logger.info("Reactivate Liveness probe for pod -> {}".format(pod_name))
         k8s_object.execPodCommand(pod_name, ["/bin/sh", "-c", "rm /tmp/keepalive"])
 
-    return True
-
     # end function definition
 
 
-def restartOTACPod(k8s_object: object):
+def restartOTACPod(k8s_object: object) -> bool:
     """Restart the Archive Center spawner service in OTAC pod
+
     Args:
-        k8s_object: Kubernetes object
-    Return: None
+        k8s_object (object): Kubernetes object
+    Returns:
+        boolean: True if restart was done, False if error occured 
     """
 
     if not OTAC_ENABLED:
         return False
 
     logger.info(
         "Restarting spawner service in Archive Center pod -> {}".format(
             OTAC_K8S_POD_NAME
         )
     )
     # The Archive Center Spawner needs to be run in "interactive" mode - otherwise the command will "hang":
     # The "-c" parameter is not required in this case
     # False is given as parameter as OTAC writes non-errors to stderr
-    k8s_object.execPodCommandInteractive(
+    response = k8s_object.execPodCommandInteractive(
         OTAC_K8S_POD_NAME, ["/bin/sh", "/etc/init.d/spawner restart"], 60, False
     )
 
-    return True
+    if response:
+        return True
+    else:
+        return False
 
     # end function definition
 
 
 def restartOTAWPPod(k8s_object: object):
-    """Delete the AppWorks Platform Pod to make Kubernetes restart it
+    """Delete the AppWorks Platform Pod to make Kubernetes restart it.
+
     Args:
         k8s_object: Kubernetes object
-    Return: None
+    Returns:
+        None
     """
 
     k8s_object.deletePod(OTAWP_K8S_STATEFUL_SET + "-0")
 
     # end function definition
 
 
@@ -1042,14 +1087,15 @@
             )
         )
         response = otpd_object.importDatabase(filename=filename)
         logger.info("Response -> {}".format(response))
 
     # end function definition
 
+
 def customization_run():
     # Initialize the OTDS, OTCS and OTPD objects and wait for the
     # pods to be ready. If any of this fails we bail out:
 
     logger.info("========== Initialize OTDS ==============")
 
     otds_object = initOTDS()
@@ -1062,15 +1108,15 @@
     if K8S_ENABLED:
         k8s_object = initK8s(inCluster=True)
 
         if not k8s_object:
             logger.error("Failed to initialize Kubernetes - exiting...")
             sys.exit()
     else:
-        k8s_object = ""
+        k8s_object = None
 
     # Put Frontend in Maintenance mode to make sure nobody interferes
     # during customization:
     if OTCS_MAINTENANCE_MODE:
         logger.info("========== Enable Maintenance Mode ==========")
         logger.info(
             "Put OTCS frontends in Maitenance Mode by changing the Kubernetes Ingress backend service..."
@@ -1118,47 +1164,71 @@
     if OTAC_ENABLED == "true":  # is Archive Center deployed?
         logger.info("========== Initialize OTAC ==============")
 
         otac_object = initOTAC(k8s_object)
         if not otac_object:
             logger.error("Failed to initialize OTAC - exiting...")
             sys.exit()
+    else:
+        otac_object = None
 
     if OTIV_ENABLED == "true":  # is PowerDocs deployed?
         logger.info("========== Initialize OTIV ==============")
 
         otiv_object = initOTIV(otds_object)
+    else:
+        otiv_object = None
 
     if OTPD_ENABLED == "true":  # is PowerDocs deployed?
         logger.info("========== Initialize OTPD ==============")
 
         otpd_object = initOTPD(k8s_object)
         if not otpd_object:
             logger.error("Failed to initialize OTPD - exiting...")
             sys.exit()
+    else:
+        otpd_object = None
 
-    if O365_ENABLED == "true" and O365_USER and O365_PASSWORD:  # is M365 enabled and do we have the required credentials?
+    if (
+        O365_ENABLED == "true" and O365_USER and O365_PASSWORD
+    ):  # is M365 enabled and do we have the required credentials?
         logger.info("======== Upload MS Teams App ============")
 
         # Download MS Teams App from OTCS (this has with 23.2 a nasty side-effect
         # of unsetting 2 checkboxes on that config page - we reset these checkboxes
         # with the settings file "O365Settings.xml"):
-        response = otcs_frontend_object.downloadConfigFile("/cs/cs?func=officegroups.DownloadTeamsPackage", "/tmp/ot.xecm.teams.zip")
+        response = otcs_frontend_object.downloadConfigFile(
+            "/cs/cs?func=officegroups.DownloadTeamsPackage", "/tmp/ot.xecm.teams.zip"
+        )
         user_access_token = m365_object.authenticateUser(O365_USER, O365_PASSWORD)
 
         # Check if the app is already installed:
-        response = m365_object.getTeamsApps("contains(displayName, '{}')".format(O365_TEAMS_APP_NAME))
+        response = m365_object.getTeamsApps(
+            "contains(displayName, '{}')".format(O365_TEAMS_APP_NAME)
+        )
         if m365_object.existResultItem(response, "displayName", O365_TEAMS_APP_NAME):
-            logger.info("Extended ECM Teams App is already in app catalog. Trying to install an update (may give a warning if it is not a new version)...")
-            app_id = m365_object.getResultValue(response, "id", 0) # 0 = Index = first item
-            logger.info("Extended ECM Teams App is already in app catalog (app ID -> {}). Updating existing app...".format(app_id))
-            response = m365_object.uploadTeamsApp("/tmp/ot.xecm.teams.zip", update_existing_app=True, app_id=app_id)
+            logger.info(
+                "Extended ECM Teams App is already in app catalog. Trying to install an update (may give a warning if it is not a new version)..."
+            )
+            app_id = m365_object.getResultValue(
+                response, "id", 0
+            )  # 0 = Index = first item
+            logger.info(
+                "Extended ECM Teams App is already in app catalog (app ID -> {}). Updating existing app...".format(
+                    app_id
+                )
+            )
+            response = m365_object.uploadTeamsApp(
+                "/tmp/ot.xecm.teams.zip", update_existing_app=True, app_id=app_id
+            )
         else:
             # this upload will be done with the user credentials - this is required:
-            logger.info("Extended Teams ECM App is not yet in app catalog. Installing as new app...")
+            logger.info(
+                "Extended Teams ECM App is not yet in app catalog. Installing as new app..."
+            )
             response = m365_object.uploadTeamsApp("/tmp/ot.xecm.teams.zip")
 
     # Set totalStartTime for duration calculation
     totalStartTime = datetime.now()
 
     logger.info("========== Processing Payload ===========")
 
@@ -1181,14 +1251,15 @@
         totalStartTime = datetime.now()
 
         payload_object = payload.Payload(
             cust_payload,
             CUST_SETTINGS_DIR,
             k8s_object,
             otds_object,
+            otac_object,
             otcs_backend_object,
             otcs_frontend_object,
             otiv_object,
             m365_object,
             placeholder_values,
             True if LOGLEVEL == "DEBUG" else False,
         )
@@ -1303,8 +1374,8 @@
             )
 
     totalDuration = datetime.now() - totalStartTime
     logger.info("======= Script execution completed in {} ===".format(totalDuration))
 
 
 if __name__ == "__main__":
-  customization_run()
+    customization_run()
```

### Comparing `pyxecm-0.0.16/pyxecm/otac.py` & `pyxecm-0.0.17/pyxecm/otac.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import requests
 import os
 import logging
+import base64
 
 from suds.client import Client
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestHeaders = {"Content-Type": "application/x-www-form-urlencoded"}
 
@@ -45,16 +46,16 @@
     ):
         """Initialize the OTAC object
 
         Args:
             protocol (string): Either http or https.
             hostname (string): The hostname of the Archive Center  to communicate with.
             port (integer): The port number used to talk to the Archive Center .
-            username (string): The admin user name of Archive Center (dsadmin).
-            password (string): The admin password of Archive Center (dsadmin).
+            ds_username (string): The admin user name of Archive Center (dsadmin).
+            ds_password (string): The admin password of Archive Center (dsadmin).
             admin_username (string): The admin user name of Archive Center (otadmin@otds.admin).
             admin_password (string): The admin password of Archive Center (otadmin@otds.admin).
         """
 
         otacConfig = {}
 
         if hostname:
@@ -139,96 +140,147 @@
 
     def baseUrl(self):
         return self.config()["baseUrl"]
 
     def execUrl(self):
         return self.config()["execUrl"]
 
+    def _soapLogin(self):
+        """Authenticate via SOAP with admin User
+
+        Args:
+            None
+        Returns:
+            string: soap_token
+        """
+
+        url = self.baseUrl() + "/archive/services/Authentication?wsdl"
+        client = Client(url)
+        self._soap_token = client.service.Authenticate(
+            username=self.config()["admin_username"],
+            password=self.config()["admin_password"],
+        )
+
+        return self._soap_token
+
+    # end method definition
+
     def execCommand(self, command: str):
+        """Execute a command on Archive Center
+
+        Args:
+            command (string): command to execute
+        Returns:
+            _type_: _description_
+        """
+
         payload = {
             "command": command,
             "user": self.config()["ds_username"],
             "passwd": self.config()["ds_password"],
         }
 
-        requestUrl = self.execUrl()
+        request_url = self.execUrl()
         logger.info(
             "Execute command -> {} on Archive Center (user -> {}); calling -> {}".format(
-                command, payload["user"], requestUrl
+                command, payload["user"], request_url
             )
         )
-        execResponse = requests.post(requestUrl, data=payload, headers=requestHeaders)
-        if not execResponse.ok:
+        response = requests.post(request_url, data=payload, headers=requestHeaders)
+        if not response.ok:
             logger.error(
-                "Failed to execute command -> {}; error -> {}".format(
-                    command, execResponse.text.replace("\n", " ")
+                "Failed to execute command -> {} on Archive Center; error -> {}".format(
+                    command, response.text.replace("\n", " ")
                 )
             )
 
-        return execResponse
+        return response
+
+    # end method definition
 
     def putCert(
         self,
-        authId: str,
-        contRep: str,
-        certPath: str,
+        auth_id: str,
+        logical_archive: str,
+        cert_path: str,
         permissions: str = "rcud",
     ):
-        """put Certificate to Archive Center
+        """Put Certificate on Archive Center
 
         Args:
-            authId (str): ID of Certification
-            contRep (str): ArchiveID
-            certPath (str): local path to certificate (base64)
-            permissions (str, optional): _description_. Defaults to "rcud".
-
+            auth_id (string): ID of Certification
+            logical_archive (string): Archive ID
+            certPath (string): local path to certificate (base64)
+            permissions (string, optional): Permissions. Defaults to "rcud" (read-create-update-delete).
         Returns:
-            _type_: _description_
+            response or None if the request fails
         """
 
-        with open(certPath, "r") as file:
-            data = file.read()
+        # Check if the photo file exists
+        if not os.path.isfile(cert_path):
+            logger.error("Certificate file -> {} not found!".format(cert_path))
+            return None
+
+        with open(cert_path, "r") as file:
+            cert_content = file.read().strip()
+
+        # Check that we have the pem certificate file - this is what OTAC expects. If the file content is
+        # base64 encoded we will decode it
+        if "BEGIN CERTIFICATE" in cert_content:
+            logger.info("Certificate file -> {} is not base64 encoded".format(cert_path))
+        elif "BEGIN CERTIFICATE" in base64.b64decode(
+            cert_content, validate=True
+        ).decode("utf-8"):
+            logger.info("Certificate file -> {} is base64 encoded".format(cert_path))
+            cert_content = base64.b64decode(cert_content, validate=True).decode("utf-8")
+        else:
+            logger.error(
+                "Cerfificate file -> {} is not in the right format".format(cert_path)
+            )
+            return None
 
-        requestUrl = (
+        request_url = (
             self.baseUrl()
-            + f"/archive?putCert&pVersion=0046&authId={authId}&contRep={contRep}&permissions={permissions}"
+            + "/archive?putCert&pVersion=0046&authId="
+            + auth_id
+            + "&contRep="
+            + logical_archive
+            + "&permissions="
+            + permissions
         )
-        logger.info(f"Execute putCert -> {certPath} on Archive ; calling -> {contRep}")
-        execResponse = requests.put(requestUrl, data=data, headers=requestHeaders)
+        logger.info(
+            "Putting certificate -> {} on Archive -> {}; calling -> {}".format(
+                cert_path, logical_archive, request_url
+            )
+        )
+        response = requests.put(request_url, data=cert_content, headers=requestHeaders)
 
-        if not execResponse.ok:
+        if not response.ok:
+            message = response.text.split(
+                '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN'
+            )[0]
             logger.error(
-                "Failed to execute putCert -> {}; error -> {}".format(
-                    authId, execResponse.text.replace("\n", " ")
+                "Failed to put certificate -> {} on Archive -> {}; error -> {}".format(
+                    cert_path, logical_archive, message
                 )
             )
 
-        return execResponse
+        return response
 
-    def _soapLogin(self):
-        """Authenticate via SOAP with admin User
+    # end method definition
 
-        Returns:
-            string: soap_token
-        """
-        url = self.baseUrl() + "/archive/services/Authentication?wsdl"
-        client = Client(url)
-        self._soap_token = client.service.Authenticate(
-            username=self.config()["admin_username"],
-            password=self.config()["admin_password"],
-        )
-        return self._soap_token
-
-    def enableCert(self, authId: str, contRep: str, enable: bool = True):
-        """enable Certitifacate
+    def enableCert(self, auth_id: str, logical_archive: str, enable: bool = True):
+        """Enable Certitificate
 
         Args:
-            authId (str): ClientID
-            contRep (str): ArchiveID
-            enable (bool, optional): Enable or Disable certificate. Defaults to True.
+            auth_id (string): Client ID
+            logical_archive (string): Archive ID
+            enable (boolean, optional): Enable or Disable certificate. Defaults to True.
+        Returns:
+            response or None if request fails.
         """
 
         if self._soap_token == "":
             self._soapLogin()
 
         if enable == True:
             enabled: int = 1
@@ -238,20 +290,28 @@
         url = self.baseUrl() + "/ot-admin/services/ArchiveAdministration?wsdl"
         client = Client(url)
 
         token_header = client.factory.create("ns0:OTAuthentication")
         token_header.AuthenticationToken = self._soap_token
         client.set_options(soapheaders=token_header)
 
-        response = client.service.invokeCommand(
-            command="SetCertificateFlags",
-            parameters=[
-                {"key": "CERT_TYPE", "data": f"@{contRep}"},
-                {"key": "CERT_NAME", "data": authId},
-                {"key": "CERT_FLAGS", "data": enabled},
-            ],
-        )
+        try:
+            response = client.service.invokeCommand(
+                command="SetCertificateFlags",
+                parameters=[
+                    {"key": "CERT_TYPE", "data": "@{}".format(logical_archive)},
+                    {"key": "CERT_NAME", "data": auth_id},
+                    {"key": "CERT_FLAGS", "data": enabled},
+                ],
+            )
+            return response
 
-        return response
+        except Exception as e:
+            logger.error(
+                "Failed to execute SetCertificateFlags for Client -> {} on Archive -> {}; error -> {}".format(
+                    auth_id, logical_archive, e
+                )
+            )
+            return None
 
 
 # end method definition
```

### Comparing `pyxecm-0.0.16/pyxecm/otcs.py` & `pyxecm-0.0.17/pyxecm/otcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,120 +4,144 @@
 
 Class: OTCS
 Methods:
 
 __init__ : class initializer
 config : returns config data set
 cookie : returns cookie information
-credentials: returns set of username and password
-setCredentials: set new credentials
-isConfigured: returns true if the OTCS pod is ready to serve requests
-baseUrl : returns OTCS base URL
-csUrl: return the Extended ECM (OTCS) URL
-restUrl : returns OTCS REST base URL
-
-parseRequestResponse: process result into Json
-lookupResultValue: lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call
-existResultItem: returns True if an item with a key/value pair is in a REST response. False otherwise.
-getResultValue: read a value from the REST response. This handles many specifics of OTCS REST APIs
+credentials: Get credentials (username and password)
+setCredentials: Set new credentials
+hostname: Get the configured OTCS hostname
+setHostname: Set the hostname of OTCS
+baseUrl : Get OTCS base URL
+csUrl: Get the Extended ECM (OTCS) URL
+restUrl : Get OTCS REST base URL
+
+requestFormHeader: Deliver the request header used for the CRUD REST API calls.
+requestJsonHeader: Deliver the request header for REST calls that require content type application/json.
+requestDownloadHeader: Deliver the request header used for download REST API calls. These calls accept application/octet-stream.
+
+parseRequestResponse: Converts the text property of a request response object to a Python dict in a safe way
+lookupResultValue: Lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call
+existResultItem: Check existence of key / value pair in the response properties of an Extended ECM REST API call.
+getResultValue: Read an item value from the REST API response. This is considering the most typical structures delivered by V2 REST API of Extended ECM
 
-authenticate : authenticates at OTCS server
+isConfigured: returns true if the OTCS pod is ready to serve requests
+authenticate : Authenticates at Content Server and retrieve OTCS Ticket.
 
 applyConfig: Apply Content Server administration settings from XML file
 
-getGroup: Lookup Content Server group
 getUser: Lookup Content Server user
-addGroup: Add Content Server group
 addUser: Add Content Server user
 searchUser: Find a user based on search criteria
 updateUser: Update a defined field for a user
 updateUserProfile: Update a defined field for a user profile
 updateUserPhoto: Update a user with a profile photo (which must be an existing node)
-isProxy: check if a user (login name) is a proxy of the current user
-getUserProxies: get the list of proxy users for the current user
-updateUserProxy: add a proxy to the current (authenticated) user
+isProxy: Check if a user (login name) is a proxy of the current user
+getUserProxies: Get the list of proxy users for the current user
+updateUserProxy: Add a proxy to the current (authenticated) user
 addFavorite: Add a favorite for the current (authenticated) user
+
+getGroup: Lookup Content Server group
+addGroup: Add Content Server group
 getGroupMembers: Get Content Server group members
 addGroupMember: Add a user or group to a target group
 
 getNode: Get a node based on the node ID
 getNodeByParentAndName: Get a node based on the parent ID and name
+getNodeByWorkspaceAndPath: Get a node based on the workspace ID and path (list of folder names)
 getNodeByVolumeAndPath: Get a node based on the volume ID and path
 getNodeFromNickname: Get a node based on the nickname
 getSubnodes: get children nodes of a parent node
 renameNode: Change the name and description of a node
 getVolumes: Get all Volumes
 getVolume: Get Volume information based on the volume type ID
+checkNodeName: Check if a a node name in a parent location has a name collision
 uploadFileToVolume: Fetch a file from a URL or local filesystem and upload
                     it to a Extended ECM volume
-uploadFileToParent: upload a document to a parent folder
-addDocumentVersion: add a version to an Extended ECM document
-downloadDocument: download a document
+uploadFileToParent: Upload a document to a parent folder
+addDocumentVersion: Add a version to an Extended ECM document
+getLatestDocumentVersion: Get latest version of a document node based on the node ID.
+downloadDocument: Download a document
+downloadConfigFile: Download a config file from a given OTCS URL. This is NOT for downloading documents from within the OTCS repository
 
 search: search for a search term using Extended ECM search engine
 
 getExternalSystemConnection: Get Extended ECM external system connection
 addExternalSystemConnection: Add Extended ECM external system connection
 
 createTransportWorkbench: Create a Workbench in the Transport Volume
 unpackTransportPackage: Unpack an existing Transport Package into an existing Workbench
 deployWorkbench: Deploy an existing Workbench
 deployTransport: Main method to deploy a transport. This uses subfunctions to upload,
                  unpackage and deploy the transport, and creates the required workbench
-replaceInXmlFiles: Replaces all occurrences of the search pattern with the replace string in all
+replaceInXmlFiles: Replace all occurrences of the search pattern with the replace string in all
                    XML files in the directory and its subdirectories.
 replaceTransportPlaceholders: Search and replace strings in the XML files of the transport packlage
 
 getWorkspaceTypes: Get all workspace types configured in Extended ECM
 getBusinessObjectType: Get information for a specific business object type
 getWorkspaceCreateForm: Get the Workspace create form
-getWorkspace: get a workspace node
-getWorkspaceByNameAndType: Lookup workspace based on workspace name and workspace type name
+getWorkspace: Get a workspace node
+getWorkspaceInstances: Get all instances of a given workspace type 
+getWorkspaceByTypeAndName: Lookup workspace based on workspace type name and workspace name 
 createWorkspace: Create a new business workspace
 createWorkspaceRelationship: Create a relationship between two workspaces
 getWorkspaceRelationships: get a list of related workspaces
 getWorkspaceRoles: Get the Workspace roles
 addMemberToWorkspace: Add member to workspace role. Check that the user is not yet a member
 removeMemberFromWorkspace: Remove member from workspace role
-assignWorkspacePermissions: update workspace permissions for a given role
+assignWorkspacePermissions: Update workspace permissions for a given role
+updateWorkspaceIcon: Update a workspace with a with a new icon (which is uploaded)
 
-createItem: create an item in Extended ECM (e.g. folder or URL item)
-updateItem: update an item in Extended ECM (e.g. folder or URL item)
+createItem: Create an item in Extended ECM (e.g. folder or URL item)
+updateItem: Update an item in Extended ECM (e.g. folder or URL item)
+getDocumentTemplates: Get all document templates for a given target location
+createDocumentFromTemplate: Create a document based on a document template
 
 getWebReportParameters: Get parameters of a Web Report
 runWebReport: Run a Web Report that is identified by its nick name
+
 installCSApplication: Install a CS Application (based on WebReports)
 
-assignItemToUserGroup: assign an item (e.g. Workspace or document) to a list of users or groups
+assignItemToUserGroup: Assign an item (e.g. Workspace or document) to a list of users or groups
 
-assignPermission: assign permissions to an item for a defined user or group
-convertPermissionStringToPermissionValue: convert a list of permission names to a permission value
-convertPermissionValueToPermissionString: convert a permission value to a list of permission strings
-
-assignClassification: assign a classification to an item
-assignRMClassification: assign a Records management classification to an item
-
-registerWorkspaceTemplate: register a workspace template for Extended ECM for Engineering
-
-getRecordsManagementRSIs: get the ist of RSIs together with their RSI schedules
-getRecordsManagementCodes: get Records Management Codes
-updateRecordsManagementCodes: update the Records Management Codes
-createRecordsManagementRSI: create a new Records Management RSI item
-createRecordsManagementRSISchedule: create a schedule for an existing RSI item
-createRecordsManagementHold: create a Records Management Hold
-importRecordsManagementCodes: import RM codes from a config file
-importRecordsManagementRSIs: import RM RSIs from a config file
-importRecordsManagementSettings: import Records Management settings from a config file
-importPhysicalObjectsCodes: import Physical Objects codes from a config file
-importPhysicalObjectsSettings: import Physical Objects settings from a config file
-importPhysicalObjectsLocators: import Physical Objects locators from a config file
-importSecurityClearanceCodes: import Securioty Clearance codes from a config file
+convertPermissionStringToPermissionValue: Convert a list of permission names to a permission value
+convertPermissionValueToPermissionString: Convert a permission value to a list of permission strings
+assignPermission: Assign permissions to an item for a defined user or group
+
+getNodeCategories: Get categories assigned to a node
+getNodeCategory: Get a specific category assigned to a node
+getNodeCategoryIds: Get list of all category definition IDs that are assign to the node.
+getNodeCategoryDefinition: Get category definition (category id and attribute IDs and types)
+assignCategory: Assign a category to a node
+setCategoryValue: Set a value for a specific category attribute to a node
+
+assignClassification: Assign a classification to an item
+assignRMClassification: Assign a Records management classification to an item
+
+registerWorkspaceTemplate: Register a workspace template for Extended ECM for Engineering
+
+getRecordsManagementRSIs: Get the ist of RSIs together with their RSI schedules
+getRecordsManagementCodes: Get Records Management Codes
+updateRecordsManagementCodes: Update the Records Management Codes
+createRecordsManagementRSI: Create a new Records Management RSI item
+createRecordsManagementRSISchedule: Create a schedule for an existing RSI item
+createRecordsManagementHold: Create a Records Management Hold
+getRecordsManagementHolds: Get a list of all Records Management Holds in the system.
+importRecordsManagementCodes: Import RM codes from a config file
+importRecordsManagementRSIs: Import RM RSIs from a config file
+importRecordsManagementSettings: Import Records Management settings from a config file
+importPhysicalObjectsCodes: Import Physical Objects codes from a config file
+importPhysicalObjectsSettings: Import Physical Objects settings from a config file
+importPhysicalObjectsLocators: Import Physical Objects locators from a config file
+importSecurityClearanceCodes: Import Securioty Clearance codes from a config file
 
-assignUserSecurityClearance: assign a Security Clearance level to a user
-assignUserSupplementalMarkings: assign a list of Supplemental Markings to a user
+assignUserSecurityClearance: Assign a Security Clearance level to a user
+assignUserSupplementalMarkings: Assign a list of Supplemental Markings to a user
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
@@ -153,25 +177,35 @@
 class OTCS(object):
     """Used to automate stettings in OpenText Extended ECM."""
 
     _config = None
     _cookie = None
 
     def __init__(
-        self, protocol: str, hostname: str, port: int, username: str, password: str, user_partition: str = "Content Server Members", resource_name: str = "cs", default_license: str = "X3"
+        self,
+        protocol: str,
+        hostname: str,
+        port: int,
+        username: str,
+        password: str,
+        user_partition: str = "Content Server Members",
+        resource_name: str = "cs",
+        default_license: str = "X3",
     ):
         """Initialize the OTCS object
 
         Args:
             protocol (string): Either http or https.
             hostname (string): The hostname of Extended ECM server to communicate with.
             port (integer): The port number used to talk to the Extended ECM server.
             username (string): The admin user name of Extended ECM.
             password (string): The admin password of Extended ECM.
-            user_partition (string): Name of the OTDS partition for OTCS users.
+            user_partition (string): Name of the OTDS partition for OTCS users. Default is "Content Server Members".
+            resource_name (string, optional): Name of the OTDS resource for OTCS. Dault is "cs".
+            default_license (string, optional): name of the default user license. Default is "X3".
         """
 
         # Initialize otcsConfig as an empty dictionary
         otcsConfig = {}
 
         if hostname:
             otcsConfig["hostname"] = hostname
@@ -228,47 +262,43 @@
 
         otcsConfig["authenticationUrl"] = otcsRestUrl + "/v1/auth"
         otcsConfig["usersUrl"] = otcsRestUrl + "/v1/members"
         otcsConfig["groupsUrl"] = otcsRestUrl + "/v1/members"
         otcsConfig["membersUrl"] = otcsRestUrl + "/v2/members"
         otcsConfig["nodesUrl"] = otcsRestUrl + "/v1/nodes"
         otcsConfig["nodesUrlv2"] = otcsRestUrl + "/v2/nodes"
+        otcsConfig["doctemplatesUrl"] = otcsRestUrl + "/v2/doctemplates"
         otcsConfig["nicknameUrl"] = otcsRestUrl + "/v2/nicknames"
-        otcsConfig["importSettingsUrl"] = otcsRestUrl + \
-            "/v2/import/settings/admin"
+        otcsConfig["importSettingsUrl"] = otcsRestUrl + "/v2/import/settings/admin"
         otcsConfig["searchUrl"] = otcsRestUrl + "/v2/search"
         otcsConfig["volumeUrl"] = otcsRestUrl + "/v2/volumes"
         otcsConfig["externalSystem"] = otcsRestUrl + "/v2/externalsystems"
         otcsConfig["businessworkspacetypes"] = (
             otcsRestUrl + "/v2/businessworkspacetypes"
         )
         otcsConfig["businessworkspacecreateform"] = (
             otcsRestUrl + "/v2/forms/businessworkspaces/create"
         )
-        otcsConfig["businessworkspaces"] = otcsRestUrl + \
-            "/v2/businessworkspaces"
+        otcsConfig["businessworkspaces"] = otcsRestUrl + "/v2/businessworkspaces"
         otcsConfig["favoritesUrl"] = otcsRestUrl + "/v2/members/favorites"
         otcsConfig["webReportsUrl"] = otcsRestUrl + "/v1/webreports"
         otcsConfig["csApplicationsUrl"] = otcsRestUrl + "/v2/csapplications"
         otcsConfig["xEngProjectTemplateUrl"] = (
             otcsRestUrl + "/v2/xengcrt/projecttemplate"
         )
         otcsConfig["rsisUrl"] = otcsRestUrl + "/v2/rsis"
         otcsConfig["rsiSchedulesUrl"] = otcsRestUrl + "/v2/rsischedules"
-        otcsConfig["recordsManagementUrl"] = otcsRestUrl + \
-            "/v1/recordsmanagement"
-        otcsConfig["recordsManagementUrlv2"] = otcsRestUrl + \
-            "/v2/recordsmanagement"
-        otcsConfig["userSecurityUrl"] = otcsRestUrl + \
-            "/v2/members/usersecurity"
+        otcsConfig["recordsManagementUrl"] = otcsRestUrl + "/v1/recordsmanagement"
+        otcsConfig["recordsManagementUrlv2"] = otcsRestUrl + "/v2/recordsmanagement"
+        otcsConfig["userSecurityUrl"] = otcsRestUrl + "/v2/members/usersecurity"
         otcsConfig["physicalObjectsUrl"] = otcsRestUrl + "/v1/physicalobjects"
-        otcsConfig["securityClearancesUrl"] = otcsRestUrl + \
-            "/v1/securityclearances"
+        otcsConfig["securityClearancesUrl"] = otcsRestUrl + "/v1/securityclearances"
         otcsConfig["holdsUrl"] = otcsRestUrl + "/v1/holds"
         otcsConfig["holdsUrlv2"] = otcsRestUrl + "/v2/holds"
+        otcsConfig["validationUrl"] = otcsRestUrl + "/v1/validation/nodes/names"
 
         self._config = otcsConfig
 
     def config(self):
         return self._config
 
     def cookie(self):
@@ -276,88 +306,88 @@
 
     def credentials(self):
         return {
             "username": self.config()["username"],
             "password": self.config()["password"],
         }
 
-    def hostname(self):
-        return self.config()["hostname"]
-
-    def setHostname(self, hostname: str):
-        self.config()["hostname"] = hostname
-
     def setCredentials(self, username: str = "", password: str = ""):
         if username:
             self.config()["username"] = username
         else:
             self.config()["username"] = "admin"
 
         if password:
             self.config()["password"] = password
         else:
             self.config()["password"] = ""
 
+    def hostname(self):
+        return self.config()["hostname"]
+
+    def setHostname(self, hostname: str):
+        self.config()["hostname"] = hostname
+
     def baseUrl(self):
         return self.config()["baseUrl"]
 
     def csUrl(self):
         return self.config()["csUrl"]
 
     def restUrl(self):
         return self.config()["restUrl"]
 
-    def requestFormHeader(self):
+    def requestFormHeader(self) -> dict:
         """Deliver the request header used for the CRUD REST API calls.
-           Consists of Cookie + Form Headers (see global vasriable)
+           Consists of Cookie + Form Headers (see global variable)
 
         Args:
             None.
         Return:
-            Dict of request header values.
+            dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
         request_header.update(requestFormHeaders)
 
         return request_header
 
     # end method definition
 
-    def requestJsonHeader(self):
-        """Deliver the request header used for the CRUD REST API calls.
-           Consists of Cookie + Json Headers (see global vasriable)
+    def requestJsonHeader(self) -> dict:
+        """Deliver the request header for REST calls that require content type application/json.
+           Consists of Cookie + Json Headers (see global variable)
 
         Args:
             None.
         Return:
-            Dict of request header values.
+            dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
         request_header.update(requestJsonHeaders)
 
         return request_header
 
     # end method definition
 
-    def requestDownloadHeader(self):
+    def requestDownloadHeader(self) -> dict:
         """Deliver the request header used for the CRUD REST API calls.
            Consists of Cookie + Form Headers (see global vasriable)
 
         Args:
             None.
         Return:
-            Dict of request header values.
+            dictionary: request header values
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
         request_header = {}
         request_header.update(self.cookie())
         request_header.update(requestDownloadHeaders)
@@ -368,61 +398,64 @@
 
     def parseRequestResponse(
         self,
         response_object: object,
         additional_error_message: str = "",
         show_error: bool = True,
     ) -> dict:
-        """Converts the request response to a Python dict in a safe way
-           that also handles exceptions.
+        """Converts the text property of a request response object to a Python dict in a safe way
+            that also handles exceptions.
 
             Content Server may produce corrupt response when it gets restarted
             or hitting resource limits. So we try to avoid a fatal error and bail
             out more gracefully.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
             additional_error_message (string): print a custom error message
             show_error (boolean): if True log an error, if False log a warning
 
-        Return: a python dict object or null in case of an error
+        Returns:
+            dictionary: response or None in case of an error
         """
 
         if not response_object:
             return None
 
         try:
             dict_object = json.loads(response_object.text)
         except json.JSONDecodeError as e:
             if additional_error_message:
                 message = "Cannot decode response as JSon. {}; error -> {}".format(
                     additional_error_message, e
                 )
             else:
-                message = "Cannot decode response as JSon; error -> {}".format(
-                    e)
+                message = "Cannot decode response as JSon; error -> {}".format(e)
             if show_error:
                 logger.error(message)
             else:
                 logger.warning(message)
             return None
         else:
             return dict_object
 
-    def lookupResultValue(self, response: dict, key: str, value: str, return_key: str) -> str:
+    # end method definition
+
+    def lookupResultValue(
+        self, response: dict, key: str, value: str, return_key: str
+    ) -> str:
         """Lookup a property value based on a provided key / value pair in the response properties of an Extended ECM REST API call.
 
         Args:
             response (dictionary): REST response from an OTCS REST Call
             key (string): property name (key)
             value (string): value to find in the item with the matching key
             return_key (string): determines which value to return based on the name of the dict key
-
         Returns:
-            str: value of the property with the key defined in "return_key"
+            string: value of the property with the key defined in "return_key"
         """
 
         if not response:
             return None
         if not "results" in response:
             return None
 
@@ -430,55 +463,82 @@
         # check if results is a list or a dict (both is possible - dependent on the actual REST API):
         if isinstance(results, dict):
             # result is a dict - we don't need index value:
             data = results["data"]
             if isinstance(data, dict):
                 # data is a dict - we don't need index value:
                 properties = data["properties"]
-                if key in properties and properties[key] == value and return_key in properties:
+                if (
+                    key in properties
+                    and properties[key] == value
+                    and return_key in properties
+                ):
                     return properties[return_key]
                 else:
                     return None
             elif isinstance(data, list):
                 # data is a list - this has typically just one item, so we use 0 as index
                 for item in data:
                     properties = item["properties"]
-                    if key in properties and properties[key] == value and return_key in properties:
+                    if (
+                        key in properties
+                        and properties[key] == value
+                        and return_key in properties
+                    ):
                         return properties[return_key]
                 return None
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                )
                 return None
         elif isinstance(results, list):
             # result is a list - we need index value
             for result in results:
                 data = result["data"]
                 if isinstance(data, dict):
                     # data is a dict - we don't need index value:
                     properties = data["properties"]
-                    if key in properties and properties[key] == value and return_key in properties:
+                    if (
+                        key in properties
+                        and properties[key] == value
+                        and return_key in properties
+                    ):
                         return properties[return_key]
                 elif isinstance(data, list):
                     # data is a list we iterate through the list and try to find the key:
                     for item in data:
                         properties = item["properties"]
-                        if key in properties and properties[key] == value and return_key in properties:
+                        if (
+                            key in properties
+                            and properties[key] == value
+                            and return_key in properties
+                        ):
                             return properties[return_key]
                 else:
                     logger.error(
-                        "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                        "Data needs to be a list or dict but it is -> {}".format(
+                            type(data)
+                        )
+                    )
                     return None
             return None
         else:
             logger.error(
-                "Result needs to be a list or dict but it is -> {}".format(type(results)))
+                "Result needs to be a list or dict but it is -> {}".format(
+                    type(results)
+                )
+            )
             return None
 
-    def existResultItem(self, response: dict, key: str, value: str, property_name: str = "properties") -> bool:
+    # end method definition
+
+    def existResultItem(
+        self, response: dict, key: str, value: str, property_name: str = "properties"
+    ) -> bool:
         """Check existence of key / value pair in the response properties of an Extended ECM REST API call.
 
         Args:
             response (dictionary): REST response from an OTCS REST Call
             key (string): property name (key)
             value (string): value to find in the item with the matching key
 
@@ -509,26 +569,30 @@
                 elif isinstance(properties, list):
                     # properties is a list we iterate through the list and try to find the key:
                     for item in properties:
                         if key in item and item[key] == value:
                             return True
                 else:
                     logger.error(
-                        "Properties needs to be a list or dict but it is -> {}".format(type(properties)))
+                        "Properties needs to be a list or dict but it is -> {}".format(
+                            type(properties)
+                        )
+                    )
                     return False
             elif isinstance(data, list):
                 # data is a list - this has typically just one item, so we use 0 as index
                 for item in data:
                     properties = item[property_name]
                     if key in properties and properties[key] == value:
                         return True
                 return False
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                )
                 return False
         elif isinstance(results, list):
             # result is a list - we need index value
             for result in results:
                 if not "data" in result:
                     continue
                 data = result["data"]
@@ -541,33 +605,48 @@
                     # data is a list we iterate through the list and try to find the key:
                     for item in data:
                         properties = item[property_name]
                         if key in properties and properties[key] == value:
                             return True
                 else:
                     logger.error(
-                        "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                        "Data needs to be a list or dict but it is -> {}".format(
+                            type(data)
+                        )
+                    )
                     return False
             return False
         else:
             logger.error(
-                "Result needs to be a list or dict but it is -> {}".format(type(results)))
+                "Result needs to be a list or dict but it is -> {}".format(
+                    type(results)
+                )
+            )
             return False
 
-    def getResultValue(self, response: dict, key: str, index: int = 0, property_name: str = "properties") -> str:
+    # end method definition
+
+    def getResultValue(
+        self,
+        response: dict,
+        key: str,
+        index: int = 0,
+        property_name: str = "properties",
+    ) -> str:
         """Read an item value from the REST API response. This is considering
            the most typical structures delivered by V2 REST API of Extended ECM.
            See developer.opentext.com for more details.
 
         Args:
             response (dictionary): REST API response object
             key (string): key to find (e.g. "id", "name", ...)
             index (integer, optional): In case a list of results is delivered the index
                                        to use (1st element has index  0). Defaults to 0.
-
+            property_name (string, optional): name of the sub dictionary holding the actual values.
+                                              Default is "properties".
         Returns:
             string: value of the item with the given key
         """
 
         # First do some sanity checks:
         if not response:
             logger.info("Empty REST response - returning None")
@@ -594,104 +673,120 @@
                 # data is a dict - we don't need index value:
                 properties = data[property_name]
             elif isinstance(data, list):
                 # data is a list - this has typically just one item, so we use 0 as index
                 properties = data[0][property_name]
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                )
                 return None
-            logger.debug(
-                "Properties of results (dict) -> {}".format(properties))
+            logger.debug("Properties of results (dict) -> {}".format(properties))
             # For nearly all OTCS REST Calls perperties is a dict:
             if isinstance(properties, dict):
                 if not key in properties:
-                    logger.error(
-                        "Key -> {} is not in result properties!".format(key))
+                    logger.error("Key -> {} is not in result properties!".format(key))
                     return None
                 return properties[key]
             # but there are some strange ones that have other names for
             # properties and may use a list - see e.g. /v2/holds
             elif isinstance(properties, list):
                 if index > len(properties) - 1:
                     logger.error(
-                        "Illegal Index -> {} given. List has only -> {} elements!".format(index, len(properties)))
+                        "Illegal Index -> {} given. List has only -> {} elements!".format(
+                            index, len(properties)
+                        )
+                    )
                     return None
                 return properties[index][key]
             else:
                 logger.error(
-                    "Properties needs to be a list or dict but it is -> {}".format(type(properties)))
+                    "Properties needs to be a list or dict but it is -> {}".format(
+                        type(properties)
+                    )
+                )
                 return False
         elif isinstance(results, list):
             # result is a list - we need a valid index:
             if index > len(results) - 1:
                 logger.error(
-                    "Illegal Index -> {} given. List has only -> {} elements!".format(index, len(results)))
+                    "Illegal Index -> {} given. List has only -> {} elements!".format(
+                        index, len(results)
+                    )
+                )
                 return None
             data = results[index]["data"]
             if isinstance(data, dict):
                 # data is a dict - we don't need index value:
                 properties = data[property_name]
             elif isinstance(data, list):
                 # data is a list - this has typically just one item, so we use 0 as index
                 properties = data[0][property_name]
             else:
                 logger.error(
-                    "Data needs to be a list or dict but it is -> {}".format(type(data)))
+                    "Data needs to be a list or dict but it is -> {}".format(type(data))
+                )
                 return None
             logger.debug(
-                "Properties of results (list, index -> {}) -> {}".format(index, properties))
+                "Properties of results (list, index -> {}) -> {}".format(
+                    index, properties
+                )
+            )
             if not key in properties:
-                logger.error(
-                    "Key -> {} is not in result properties!".format(key))
+                logger.error("Key -> {} is not in result properties!".format(key))
                 return None
             return properties[key]
         else:
             logger.error(
-                "Result needs to be a list or dict but it is -> {}".format(type(results)))
+                "Result needs to be a list or dict but it is -> {}".format(
+                    type(results)
+                )
+            )
             return None
 
     # end method definition
 
     def isConfigured(self) -> bool:
         """Checks if the Content Server pod is ready to receive requests.
 
         Args:
             None.
-        Return: True if pod is ready. False if pod is not yet ready.
+        Returns:
+            boolean: True if pod is ready. False if pod is not yet ready.
         """
 
         request_url = self.config()["configuredUrl"]
 
         logger.info("Trying to retrieve OTCS url -> {}".format(request_url))
 
         try:
             checkcsConfiguredResponse = requests.get(
                 request_url, headers=requestJsonHeaders
             )
         except Exception as e:
-            logger.warning(
-                "Unable to connect to -> {} : {}".format(request_url, e))
+            logger.warning("Unable to connect to -> {} : {}".format(request_url, e))
             logger.warning("OTCS service may not be ready yet.")
             return False
 
         if checkcsConfiguredResponse.ok:
             return True
         else:
             return False
 
     # end method definition
 
-    def authenticate(self, revalidate: bool = False):
-        """Authenticate at Content Server and retrieve OTCS Ticket.
+    def authenticate(self, revalidate: bool = False) -> dict:
+        """Authenticates at Content Server and retrieve OTCS Ticket.
 
         Args:
             revalidate (boolean): determinse if a re-athentication is enforced
                                   (e.g. if session has timed out with 401 error)
-        Return: Cookie information. Also stores cookie information in self._cookie
+        Returns:
+            dictionary: Cookie information of None in case of an error.
+                        Also stores cookie information in self._cookie
         """
 
         # Already authenticated and session still valid?
         if self._cookie and not revalidate:
             return self._cookie
 
         otcs_ticket = "NotSet"
@@ -725,43 +820,37 @@
             if not authenticate_dict:
                 return None
             else:
                 otcs_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otcs_ticket))
         else:
             logger.error(
-                "Failed to request an OTCS ticket; error -> {}".format(
-                    response.text
-                )
+                "Failed to request an OTCS ticket; error -> {}".format(response.text)
             )
             return None
 
         # Store authentication ticket:
-        self._cookie = {
-          "otcsticket": otcs_ticket,
-          "LLCookie": otcs_ticket
-          }
+        self._cookie = {"otcsticket": otcs_ticket, "LLCookie": otcs_ticket}
         self.otcsticket = otcs_ticket
         return self._cookie
 
     # end method definition
 
-    def applyConfig(self, xmlfilepath: str):
+    def applyConfig(self, xmlfilepath: str) -> dict:
         """Apply Content Server administration settings from XML file
 
         Args:
             xmlfilepath (string): name + path of the XML settings file
-        Return:
-            Import response (json) or None if the import fails.
-            response["results"]["data"]["restart"] indicates if the settings
-            require a restart of the OTCS services.
+        Returns:
+            dictionary: Import response or None if the import fails.
+                        response["results"]["data"]["restart"] indicates if the settings
+                        require a restart of the OTCS services.
         """
 
-        logger.info(
-            "Applying admin settings from file -> {}".format(xmlfilepath))
+        logger.info("Applying admin settings from file -> {}".format(xmlfilepath))
         filename = os.path.basename(xmlfilepath)
 
         if not os.path.exists(xmlfilepath):
             logger.error(
                 "The file -> {} does not exist in path -> {}!".format(
                     filename, os.path.dirname(xmlfilepath)
                 )
@@ -779,94 +868,40 @@
                 request_url,
                 files=llconfig_file,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 logger.debug(
-                    "Admin settings in file -> {} have been applied".format(xmlfilepath))
+                    "Admin settings in file -> {} have been applied".format(xmlfilepath)
+                )
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import settings file -> {}; status -> {}; error -> {}".format(
                         xmlfilepath, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroup(self, name: str, show_error: bool = False):
-        """Lookup Content Server group.
-
-        Args:
-            name (string): name of the group
-            showError (boolean): if True, treat as error if group is not found
-        Return:
-            Group information (json) or None if the group is not found.
-            The returned information has a structure like this:
-            "data": [
-                {
-                    "id": 0,
-                    "name": "string",
-                    ...
-                }
-            ]
-            To access the id of the first group found use ["data"][0]["id"]
-        """
-
-        # Add query parameters (these are NOT passed via JSon body!)
-        # type = 1 ==> Group
-        request_url = self.config()["groupsUrl"] + \
-            "?where_type=1&query={}".format(name)
-        request_header = self.requestFormHeader()
-
-        logger.info(
-            "Get group with name -> {}; calling -> {}".format(name, request_url))
-
-        retries = 0
-        while True:
-            response = requests.get(
-                request_url, headers=request_header, cookies=self.cookie()
-            )
-            if response.ok:
-                return self.parseRequestResponse(response)
-            # Check if Session has expired - then re-authenticate and try once more
-            elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
-                self.authenticate(True)
-                retries += 1
-            else:
-                if show_error:
-                    logger.error(
-                        "Failed to get group -> {}; status -> {}; error -> {}".format(
-                            name, response.status_code, response.text
-                        )
-                    )
-                else:
-                    logger.info("Group -> {} not found.".format(name))
-                return None
-
-    # end method definition
-
-    def getUser(self, name: str, show_error: bool = False):
+    def getUser(self, name: str, show_error: bool = False) -> dict:
         """Lookup Content Server user based on the name.
 
         Args:
             name (string): name of the user
             show_error (boolean): treat as error if user is not found
-        Return:
-            User information (json) or None if the user is not found.
+        Returns:
+            dictionary: User information or None if the user is not found.
             The returned information has a structure like this:
             "data": [
                 {
                     "id": 0,
                     "name": "string",
                     "first_name": "string",
                     "last_name": "string",
@@ -876,32 +911,29 @@
                 }
             ]
             To access the (login) name of the first user found use ["data"][0]["name"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         # type = 0 ==> User
-        request_url = self.config()["usersUrl"] + \
-            "?where_type=0&query={}".format(name)
+        request_url = self.config()["usersUrl"] + "?where_type=0&query={}".format(name)
         request_header = self.requestFormHeader()
 
-        logger.info(
-            "Get user with name -> {}; calling -> {}".format(name, request_url))
+        logger.info("Get user with name -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get user -> {}; status -> {}; error -> {}".format(
                             name, response.status_code, response.text
@@ -909,81 +941,38 @@
                     )
                 else:
                     logger.info("User -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def addGroup(self, name: str):
-        """Add Content Server group.
-
-        Args:
-            name (string): name of the group
-        Return:
-            Group information (json) or None if the group couldn't be created (e.g. because it exisits already).
-        """
-
-        groupPostBody = {"type": 1, "name": name}
-
-        request_url = self.config()["groupsUrl"]
-        request_header = self.requestFormHeader()
-
-        logger.info(
-            "Adding group -> {}; calling -> {}".format(name, request_url))
-        logger.debug("Group Attributes -> {}".format(groupPostBody))
-
-        retries = 0
-        while True:
-            response = requests.post(
-                request_url,
-                data=groupPostBody,
-                headers=request_header,
-                cookies=self.cookie(),
-            )
-            if response.ok:
-                return self.parseRequestResponse(response)
-            # Check if Session has expired - then re-authenticate and try once more
-            elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
-                self.authenticate(True)
-                retries += 1
-            else:
-                logger.error(
-                    "Failed to add group -> {}; status -> {}; error -> {}".format(
-                        name, response.status_code, response.text
-                    )
-                )
-                return None
-
-    # end method definition
-
     def addUser(
         self,
         name: str,
         password: str,
         first_name: str,
         last_name: str,
         email: str,
         base_group: str,
         privileges: list = ["Login", "Public Access"],
-    ):
+    ) -> dict:
         """Add Content Server user.
 
         Args:
             name (string): login name of the user
             password (string): password of the user
             first_name (string): first name of the user
             last_name (string): last name of the user
             email (string): email address of the user
             base_group (string): base group of the user (e.g. department)
-            privileges (list): values are Login, Public Access, Content Manager, Modify Users, Modify Groups, User Admin Rights, Grant Discovery, System Admin Rights
-
-        Return:
-            User information (json) or None if the user couldn't be created (e.g. because it exisits already).
+            privileges (list, optional): values are Login, Public Access, Content Manager,
+                                         Modify Users, Modify Groups, User Admin Rights,
+                                         Grant Discovery, System Admin Rights
+        Returns:
+            dictionary: User information or None if the user couldn't be created (e.g. because it exisits already).
         """
 
         userPostBody = {
             "type": 0,
             "name": name,
             "password": password,
             "first_name": first_name,
@@ -993,15 +982,15 @@
             "privilege_login": ("Login" in privileges),
             "privilege_public_access": ("Public Access" in privileges),
             "privilege_content_manager": ("Content Manager" in privileges),
             "privilege_modify_users": ("Modify Users" in privileges),
             "privilege_modify_groups": ("Modify Groups" in privileges),
             "privilege_user_admin_rights": ("User Admin Rights" in privileges),
             "privilege_grant_discovery": ("Grant Discovery" in privileges),
-            "privilege_system_admin_rights": ("System Admin Rights" in privileges)
+            "privilege_system_admin_rights": ("System Admin Rights" in privileges),
         }
 
         request_url = self.config()["usersUrl"]
         request_header = self.requestFormHeader()
 
         logger.info("Adding user -> {}; calling -> {}".format(name, request_url))
 
@@ -1013,36 +1002,74 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user -> {}; status -> {}; error -> {}".format(
                         name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def searchUser(self, value: str, field: str = "where_name"):
+    def searchUser(self, value: str, field: str = "where_name") -> dict:
         """Find a user based on search criteria.
 
         Args:
             value (string): field value
             field (string): user field to search with (where_name, where_first_name, where_last_name)
-        Return:
-            User information (json) or None if the user couldn't be found (e.g. because it doesn't exist).
+        Returns:
+            dictionary: User information or None if the user couldn't be found (e.g. because it doesn't exist).
+            Example:
+            {
+                'collection': {
+                    'paging': {...},
+                    'sorting': {...}
+                },
+                'links': {
+                    'data': {...}
+                },
+                'results': [
+                    {
+                        'data': {
+                            'properties': {
+                                'birth_date': None,
+                                'business_email': 'dfoxhoven@M365x61936377.onmicrosoft.com',
+                                'business_fax': None,
+                                'business_phone': None,
+                                'cell_phone': None,
+                                'deleted': False,
+                                'display_language': None,
+                                'first_name': 'Deke',
+                                'gender': None,
+                                'group_id': 8005,
+                                'home_address_1': None,
+                                'home_address_2': None,
+                                'home_fax': None,
+                                'home_phone': None,
+                                'id': 8562,
+                                'initials': 'DF',
+                                'last_name': 'Foxhoven',
+                                'middle_name': None,
+                                'name': 'dfoxhoven',
+                                'name_formatted': 'Deke Foxhoven',
+                                ...
+                            }
+                        }
+                    }
+                ]
+            }
         """
 
         request_url = self.config()["membersUrl"] + "?" + field + "=" + value
         request_header = self.requestFormHeader()
 
         logger.info(
             "Searching user by field -> {}, value -> {}; calling -> {}".format(
@@ -1055,37 +1082,36 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Cannot find user with -> {} = {}; status -> {}; error -> {}".format(
                         field, value, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUser(self, user_id: int, field: str, value: str):
+    def updateUser(self, user_id: int, field: str, value: str) -> dict:
         """Update a defined field for a user.
 
         Args:
             user_id (integer): ID of the user
             value (string): field value
             field (string): user field
-        Return:
-            User information (json) or None if the user couldn't be updated (e.g. because it doesn't exist).
+        Returns:
+            dictionary: User information or None if the user couldn't be updated (e.g. because it doesn't exist).
         """
 
         userPutBody = {field: value}
 
         request_url = self.config()["membersUrl"] + "/" + str(user_id)
         request_header = self.requestFormHeader()
 
@@ -1104,37 +1130,37 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user -> {}; status -> {}; error -> {}".format(
                         user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def updateUserProfile(self, field: str, value):
+    def updateUserProfile(self, field: str, value) -> dict:
         """Update a defined field for a user profile.
            IMPORTANT: this method needs to be called by the authenticated user
 
         Args:
             value (string): field value
             field (string): user field
-        Return:
-            User information (json) or None if the user couldn't be updated (e.g. because it doesn't exist).
+        Returns:
+            dictionary: User information or None if the user couldn't be updated
+                        (e.g. because it doesn't exist).
         """
 
         userProfilePutBody = {"SmartUI": {field: value}}
 
         request_url = self.config()["membersUrl"] + "/preferences"
         request_header = self.requestFormHeader()
 
@@ -1154,16 +1180,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update profile of current user; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
@@ -1174,16 +1199,16 @@
 
     def updateUserPhoto(self, user_id: int, photo_id: int):
         """Update a user with a profile photo (which must be an existing node).
 
         Args:
             user_id (integer): ID of the user
             photo_id (integer): Node ID of the photo
-        Return:
-            Node information (json) or None if no node with this nickname is found.
+        Returns:
+            dictionary: Node information or None if photo node is not found.
         """
 
         updateUserPutBody = {"photo_id": photo_id}
 
         request_url = self.config()["usersUrl"] + "/" + str(user_id)
         request_header = self.requestFormHeader()
 
@@ -1201,16 +1226,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user with ID -> {}; status -> {}; error -> {}".format(
                         user_id, response.status_code, response.text
                     )
@@ -1220,93 +1244,90 @@
     # end method definition
 
     def isProxy(self, user_name: str) -> bool:
         """Check if a user is defined as proxy of the current user
 
         Args:
             user_name (string): user  to test (login name)
-
         Returns:
-            bool: True is user is proxy of current user. False if not.
+            boolean: True is user is proxy of current user. False if not.
         """
 
         response = self.getUserProxies()
         if not response or not "proxies" in response:
             return False
         proxies = response["proxies"]
 
         for proxy in proxies:
             if proxy["name"] == user_name:
                 return True
         return False
 
     # end method definition
 
-    def getUserProxies(self):
+    def getUserProxies(self) -> dict:
         """Get list of user proxies.
            This method needs to be called as the user the proxy is acting for.
-        Args: None
-        Return:
-            Node information (json) or None if REST call fails.
+        Args:
+            None
+        Returns:
+            dictionary: Node information or None if REST call fails.
         """
 
         request_url = self.config()["usersUrl"] + "/proxies"
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get proxy users for current user; calling -> {}".format(
-                request_url)
+            "Get proxy users for current user; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
-
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
             response = requests.get(
                 request_url,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get proxy users for current user; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUserProxy(
         self, proxy_user_id: int, from_date: str = None, to_date: str = None
-    ):
+    ) -> dict:
         """Update a user with a proxy user (which must be an existing user).
-           This method needs to be called as the user the proxy is acting for.
+           IMPORTANT: This method needs to be called as the user the proxy is acting for.
            Optional this method can be provided with a time span the proxy should be active.
 
            Example payload for proxy user 19340 without time span:
            add_proxy:  {"19340":{}}
 
            Example payload for proxy user 19340 with time span:
            add_proxy: {"19340":{"from_date": "2022-10-01", "to_date": "2022-10-31"}}
 
         Args:
             user_id (integer): ID of the user
-            from_date (string): Optional: start date for proxy (format YYYY-MM-DD)
-            to_date (string): Optional: end date for proxy (format YYYY-MM-DD)
-        Return:
-            Node information (json) or None if REST call fails.
+            from_date (string, optional): start date for proxy (format YYYY-MM-DD)
+            to_date (string, optional): end date for proxy (format YYYY-MM-DD)
+        Returns:
+            dictionary: Request response or None if call fails.
         """
 
         post_dict = {}
         if from_date and to_date:
             post_dict["from_date"] = from_date
             post_dict["to_date"] = to_date
 
@@ -1319,47 +1340,45 @@
             "Assign proxy user with ID -> {} to current user; calling -> {}".format(
                 proxy_user_id, request_url
             )
         )
 
         retries = 0
         while True:
-
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
             response = requests.post(
                 request_url,
                 data={"add_proxy": json.dumps(proxyPostBody)},
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign proxy user with ID -> {} to current user; status -> {}; error -> {}".format(
                         proxy_user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addFavorite(self, node_id: int):
+    def addFavorite(self, node_id: int) -> dict:
         """Add a favorite for the current (authenticated) user.
 
         Args:
             nodeid (integer): ID of the node.
-        Return:
-            Response (json) or None if the favorite creation has failed.
+        Returns:
+            dictionary: Request response or None if the favorite creation has failed.
         """
 
         request_url = self.config()["favoritesUrl"] + "/" + str(node_id)
         request_header = self.requestFormHeader()
 
         logger.info(
             "Adding favorite for node ID -> {}; calling -> {}".format(
@@ -1372,39 +1391,133 @@
             response = requests.post(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add favorite for node ID -> {}; status -> {}; error -> {}".format(
                         node_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getGroupMembers(self, group: int, member_type: int, limit: int = 100):
+    def getGroup(self, name: str, show_error: bool = False) -> dict:
+        """Lookup Content Server group.
+
+        Args:
+            name (string): name of the group
+            showError (boolean): if True, treat as error if group is not found
+        Returns:
+            dictionary: Group information or None if the group is not found.
+            The returned information has a structure like this:
+            "data": [
+                {
+                    "id": 0,
+                    "name": "string",
+                    ...
+                }
+            ]
+            To access the id of the first group found use ["data"][0]["id"]
+        """
+
+        # Add query parameters (these are NOT passed via JSon body!)
+        # type = 1 ==> Group
+        request_url = self.config()["groupsUrl"] + "?where_type=1&query={}".format(name)
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Get group with name -> {}; calling -> {}".format(name, request_url)
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                if show_error:
+                    logger.error(
+                        "Failed to get group -> {}; status -> {}; error -> {}".format(
+                            name, response.status_code, response.text
+                        )
+                    )
+                else:
+                    logger.info("Group -> {} not found.".format(name))
+                return None
+
+    # end method definition
+
+    def addGroup(self, name: str) -> dict:
+        """Add Content Server group.
+
+        Args:
+            name (string): name of the group
+        Returns:
+            dictionary: Group information or None if the group couldn't be created (e.g. because it exisits already).
+        """
+
+        groupPostBody = {"type": 1, "name": name}
+
+        request_url = self.config()["groupsUrl"]
+        request_header = self.requestFormHeader()
+
+        logger.info("Adding group -> {}; calling -> {}".format(name, request_url))
+        logger.debug("Group Attributes -> {}".format(groupPostBody))
+
+        retries = 0
+        while True:
+            response = requests.post(
+                request_url,
+                data=groupPostBody,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to add group -> {}; status -> {}; error -> {}".format(
+                        name, response.status_code, response.text
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def getGroupMembers(self, group: int, member_type: int, limit: int = 100) -> dict:
         """Get Content Server group members.
 
         Args:
             group (integer): ID of the group.
             member_type (integer): users = 0, groups = 1
-            limit (integer): max number of results (internal default is 25)
-        Return:
-            Group members (json) or None if the group members couldn't be found.
+            limit (integer, optional): max number of results (internal default is 25)
+        Returns:
+            dictionary: Group members or None if the group members couldn't be found.
         """
 
         # default limit is 25 which may not be enough for groups with many members
         # where_type = 1 makes sure we just get groups and not users
         request_url = (
             self.config()["membersUrl"]
             + "/"
@@ -1413,57 +1526,54 @@
             + str(member_type)
             + "&limit="
             + str(limit)
         )
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Getting members of group -> {}; calling -> {}".format(
-                group, request_url)
+            "Getting members of group -> {}; calling -> {}".format(group, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get members of group -> {}; status -> {}; error -> {}".format(
                         group,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def addGroupMember(self, member: int, group: int):
+    def addGroupMember(self, member: int, group: int) -> dict:
         """Add a user or group to a target group.
 
         Args:
             member (integer): ID of the user or group to add.
             group (integer): ID of the target group.
-        Return:
-            Response (json) or None if the adding fails.
+        Returns:
+            dictionary: Response or None if adding a the member fails.
         """
 
         groupMemberPostBody = {"member_id": member}
 
-        request_url = self.config()["membersUrl"] + \
-            "/" + str(group) + "/members"
+        request_url = self.config()["membersUrl"] + "/" + str(group) + "/members"
         request_header = self.requestFormHeader()
 
         logger.info(
             "Adding member -> {} to group -> {}; calling -> {}".format(
                 member, group, request_url
             )
         )
@@ -1476,16 +1586,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add member -> {} to group -> {}; status -> {}; error -> {}".format(
                         member,
                         group,
@@ -1493,21 +1602,21 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNode(self, node_id: int):
+    def getNode(self, node_id: int) -> dict:
         """Get a node based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the node
-        Return:
-            Node information (json) or None if no node with this ID is found.
+        Returns:
+            dictionary: Node information or None if no node with this ID is found.
             "results": [
                 {
                     "data": [
                         {
                             "columns": [
                                 {
                                 "data_type": 0,
@@ -1567,50 +1676,52 @@
             ]
         """
 
         request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get node with ID -> {}; calling -> {}".format(node_id, request_url))
+            "Get node with ID -> {}; calling -> {}".format(node_id, request_url)
+        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get node with ID -> {}; status -> {}; error -> {}".format(
                         node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getNodeByParentAndName(self, parent_id: int, name: str, show_error: bool = False):
+    def getNodeByParentAndName(
+        self, parent_id: int, name: str, show_error: bool = False
+    ) -> dict:
         """Get a node based on the parent ID and name. This method does basically
            a query with "where_name" and the "result" is a list.
 
         Args:
             parent_id (integer) is the node Id of the parent node
             name (string) is the name of the node to get
-            show_error (boolean): treat as error if node is not found
-        Return:
-            Node information (json) or None if no node with this name is found in parent.
-            Access to node ID with: response["results"][0]["data"]["properties"]["id"]
+            show_error (boolean, optional): treat as error if node is not found
+        Returns:
+            dictionary: Node information or None if no node with this name is found in parent.
+                        Access to node ID with: response["results"][0]["data"]["properties"]["id"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {"where_name": name}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = (
@@ -1632,16 +1743,15 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get node with name -> {} and parent ID -> {}; status -> {}; error -> {}".format(
                             name,
@@ -1656,15 +1766,54 @@
                             name, parent_id
                         )
                     )
                 return None
 
     # end method definition
 
-    def getNodeByVolumeAndPath(self, volume_type: int, path: list):
+    def getNodeByWorkspaceAndPath(
+        self, workspace_id: int, path: list, show_error: bool = False
+    ) -> dict:
+        """Get a node based on the workspace ID (= node ID) and path (list of folder names).
+
+        Args:
+            workspace_id (integer): node ID of the workspace
+            path (list): list of container items (top down), last item is name of to be retrieved item.
+                         If path is empty the node of the volume is returned.
+            show_error (boolean, optional): treat as error if node is not found
+        Returns:
+            dictionary: Node information or None if no node with this path is found.
+        """
+
+        current_item_id = workspace_id
+
+        # in case the path is an empty list
+        # we will have the node of the workspace:
+        node = self.getNode(current_item_id)
+
+        for path_element in path:
+            node = self.getNodeByParentAndName(current_item_id, path_element)
+            current_item_id = self.getResultValue(node, "id")
+            if not current_item_id:
+                if show_error:
+                    logger.error("Cannot find path element -> {}!".format(path_element))
+                else:
+                    logger.info("Cannot find path element -> {}.".format(path_element))
+                return None
+            logger.debug(
+                "Traversing path element -> {} ({})".format(
+                    path_element, current_item_id
+                )
+            )
+
+        return node
+
+    # end method definition
+
+    def getNodeByVolumeAndPath(self, volume_type: int, path: list) -> dict:
         """Get a node based on the volume and path (list of container items).
 
         Args:
             volume_type (integer): Volume type ID (default is 141 = Enterprise Workspace)
                 "Records Management"                = 550
                 "Content Server Document Templates" = 20541
                 "O365 Office Online Volume"         = 1296
@@ -1680,16 +1829,16 @@
                 "Support Asset Volume"              = 1309
                 "Physical Objects Workspace"        = 413
                 "Extended ECM"                      = 882
                 "Enterprise Workspace"              = 141
                 "Business Workspaces"               = 862
             path (list): list of container items (top down), last item is name of to be retrieved item.
                          If path is empty the node of the volume is returned.
-        Return:
-            Node information (json) or None if no node with this path is found.
+        Returns:
+            dictionary: Node information or None if no node with this path is found.
         """
 
         # Preparation: get volume IDs for Transport Warehouse (root volume and Transport Packages)
         response = self.getVolume(volume_type)
         if not response:
             logger.error("Volume Type -> {} not found!".format(volume_type))
             return None
@@ -1709,90 +1858,85 @@
             if not current_item_id:
                 logger.error(
                     "Cannot find path element -> {} in container with ID -> {}.".format(
                         path_element, current_item_id
                     )
                 )
                 return None
-            logger.debug(
-                "Traversing path element -> {}".format(current_item_id))
+            logger.debug("Traversing path element -> {}".format(current_item_id))
 
         return node
 
     # end method definition
 
-    def getNodeFromNickname(self, nickname: str, show_error: bool = False):
+    def getNodeFromNickname(self, nickname: str, show_error: bool = False) -> dict:
         """Get a node based on the nickname.
 
         Args:
             nickname (string): Nickname of the node.
             show_error (boolean): treat as error if node is not found
-        Return:
-            Node information (json) or None if no node with this nickname is found.
+        Returns:
+            dictionary: Node information or None if no node with this nickname is found.
         """
 
         request_url = self.config()["nicknameUrl"] + "/" + nickname + "/nodes"
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get node with nickname -> {}; calling -> {}".format(
-                nickname, request_url)
+            "Get node with nickname -> {}; calling -> {}".format(nickname, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get node with nickname -> {}; status -> {}; error -> {}".format(
                             nickname, response.status_code, response.text
                         )
                     )
                 else:
-                    logger.info(
-                        "Node with nickname -> {} not found.".format(
-                            nickname)
-                    )
+                    logger.info("Node with nickname -> {} not found.".format(nickname))
                 return None
 
     # end method definition
 
     def getSubnodes(
         self,
         parent_node_id: int,
         filter_node_types: int = -2,
         filter_name: str = "",
         show_hidden: bool = False,
         limit: int = 100,
         page: int = 1,
-    ):
+    ) -> dict:
         """Get a subnodes of a parent node ID.
 
         Args:
             parent_node_id (integer) is the node Id of the node
-            filter_node_types (integer): -1 get all containers
-                                         -2 get all searchable objects
-                                         -3 get all non-containers
-            filter_name (string): filter nodes for specific name
-            show_hidden (boolean): list also hidden items
-            limit (integer): maximum number of results
-            page (integer): number of result page
-        Return:
-            Subnodes information (json) or None if no node with this parent ID is found.
+            filter_node_types (integer, optional):
+                -1 get all containers
+                -2 get all searchable objects (default)
+                -3 get all non-containers
+            filter_name (string, optional): filter nodes for specific name (dfault = no filter)
+            show_hidden (boolean, optional): list also hidden items (default = False)
+            limit (integer, optional): maximum number of results (default = 100)
+            page (integer, optional): number of result page (default = 1 = 1st page)
+        Returns:
+            dictionary: Subnodes information or None if no node with this parent ID is found.
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {
             "where_type": filter_node_types,
             "limit": limit,
         }
@@ -1825,40 +1969,48 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get subnodes for parent node with ID -> {}; status -> {}; error -> {}".format(
                         parent_node_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def renameNode(self, node_id: int, name: str, description: str, name_multilingual: dict = {}, description_multilingual: dict = {}):
+    def renameNode(
+        self,
+        node_id: int,
+        name: str,
+        description: str,
+        name_multilingual: dict = {},
+        description_multilingual: dict = {},
+    ) -> dict:
         """Change the name and description of a node.
 
         Args:
             node_id (integer): ID of the node. You can use the getVolume() function below to
                                to the node id for a volume.
             name (string): New name of the node.
             description (string): New description of the node.
-        Return:
-            Rename response (json) or None if the renaming fails.
+            name_multilingual (dictionary, optional): multi-lingual node names
+            description_multilingual (dictionary, optional): multi-lingual description
+        Returns:
+            dictionary: Request response or None if the renaming fails.
         """
 
         renameNodePutBody = {"name": name, "description": description}
 
         if name_multilingual:
             renameNodePutBody["name_multilingual"] = name_multilingual
         if description_multilingual:
@@ -1881,16 +2033,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to rename node -> {} to -> {}; status -> {}; error -> {}".format(
                         node_id,
                         name,
@@ -1898,22 +2049,62 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getVolumes(self):
+    def getVolumes(self) -> dict:
         """Get all Volumes.
 
         Args:
             None
-        Return:
-            Volume Details (json) or None if an error occured.
-            ["results"]["data"]["properties"]["id"] is the node ID of the volume.
+        Returns:
+            dictionary: Volume Details or None if an error occured.
+            {
+                'links': {
+                    'data': {...}
+                },
+                'results': [
+                    {
+                        'data': {
+                            'properties': {
+                                'advanced_versioning': None,
+                                'container': True,
+                                'container_size': 16,
+                                'create_date': '2023-05-07T23:18:50Z',
+                                'create_user_id': 1000,
+                                'description': '',
+                                'description_multilingual': {'de': '', 'en': '', 'fr': '', 'it': '', 'ja': ''},
+                                'external_create_date': None,
+                                'external_identity': '',
+                                'external_identity_type': '',
+                                'external_modify_date': None,
+                                'external_source': '',
+                                'favorite': False,
+                                'hidden': False,
+                                ...
+                                'id': 2000,
+                                ...
+                                'name': 'Enterprise',
+                                'name_multilingual': {'de': '', 'en': 'Enterprise', 'fr': '', 'it': '', 'ja': ''},
+                                ...
+                                'parent_id': -1,
+                                'type': 141,
+                                'volume_id': -2000,
+                                ...
+                            }
+                            ...
+                        }
+                    },
+                    ...
+                ]
+            }
+            Example:
+            ["results"][0]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
         request_url = self.config()["volumeUrl"]
         request_header = self.requestFormHeader()
 
         logger.info("Get volumes; calling -> {}".format(request_url))
 
@@ -1922,359 +2113,134 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get volumes; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getVolume(self, volume_type: int):
+    def getVolume(self, volume_type: int) -> dict:
         """Get Volume information based on the volume type ID.
 
         Args:
             volume_type (integer): ID of the volume type
-        Return:
-            Volume Details (json) or None if volume is not found.
+        Returns:
+            dictionary: Volume Details or None if volume is not found.
             ["results"]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
         request_url = self.config()["volumeUrl"] + "/" + str(volume_type)
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get volume type -> {}; calling -> {}".format(
-                volume_type, request_url)
+            "Get volume type -> {}; calling -> {}".format(volume_type, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get volume type -> {}; status -> {}; error -> {}".format(
                         volume_type,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def search(
-        self,
-        search_term: str,
-        look_for: str = "complexQuery",
-        modifier: str = "",
-        slice_id: int = 0,
-        query_id: int = 0,
-        template_id: int = 0,
-        limit: int = 100,
-        page: int = 1,
-    ):
-        """Search for a search term.
+    def checkNodeName(self, parent_id: int, node_name: str) -> dict:
+        """Get Volume information based on the volume type ID.
 
         Args:
-            parent_node_id (integer) is the node Id of the node
-            search_term (string), e.g. "test or OTSubType: 189"
-            look_for (string): 'allwords', 'anywords', 'exactphrase', and 'complexquery'.
-                              If not specified, it defaults to 'complexQuery'.
-            modifier (string): 'synonymsof', 'relatedto', 'soundslike', 'wordbeginswith', and 'wordendswith'.
-                               If not specified or specify any value other than the available options,
-                               it will be ignored.
-            slide_id (integer): ID of an existing search slice
-            query_id (integer): ID of an saved search query
-            template_id (integer): ID of an saved search template
-            limit (integer): maximum number of results
-            page (integer): number of result page
-        Return:
-            Subnodes information (json) or None if no node with this parent ID is found.
+            parent_id (integer): ID of the parent location
+            node_name (string): name of the new node
+        Returns:
         """
 
-        searchPostBody = {
-            "where": search_term,
-            "lookfor": look_for,
-            "page": page,
-            "limit": limit,
-        }
-
-        if modifier:
-            searchPostBody["modifier"] = modifier
-        if slice_id > 0:
-            searchPostBody["slice_id"] = slice_id
-        if query_id > 0:
-            searchPostBody["query_id"] = query_id
-        if template_id > 0:
-            searchPostBody["template_id"] = template_id
-
-        request_url = self.config()["searchUrl"]
+        request_url = self.config()["validationUrl"]
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Serarch for term -> {}; calling -> {}".format(
-                search_term, request_url)
-        )
-
-        retries = 0
-        while True:
-            response = requests.post(
-                request_url,
-                data=searchPostBody,
-                headers=request_header,
-                cookies=self.cookie(),
-            )
-            if response.ok:
-                return self.parseRequestResponse(response)
-            # Check if Session has expired - then re-authenticate and try once more
-            elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
-                self.authenticate(True)
-                retries += 1
-            else:
-                logger.error(
-                    "Failed to search for term -> {}; status -> {}; error -> {}".format(
-                        search_term,
-                        response.status_code,
-                        response.text,
-                    )
-                )
-                return None
-
-    # end method definition
-
-    def getExternalSystemConnection(self, connection_name: str, show_error: bool = False):
-        """Get Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
-
-        Args:
-            connection_name (string): Name of the connection
-            show_error (boolean): treat as error if node is not found
-        Return:
-            External system Details (json) or None if the REST call fails.
-        """
-
-        request_url = self.config()["externalSystem"] + \
-            "/" + connection_name + "/config"
-        request_header = self.cookie()
-
-        logger.info(
-            "Get external system connection -> {}; calling -> {}".format(
-                connection_name, request_url
+            "Check if node with name -> {} can be created in parent with ID -> {}; calling -> {}".format(
+                node_name, parent_id, request_url
             )
         )
 
-        retries = 0
-        while True:
-            response = requests.get(
-                request_url, headers=request_header, cookies=self.cookie()
-            )
-            if response.ok:
-                return self.parseRequestResponse(response)
-            # Check if Session has expired - then re-authenticate and try once more
-            elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
-                self.authenticate(True)
-                retries += 1
-            else:
-                if show_error:
-                    logger.error(
-                        "Failed to get external system connection -> {}; status -> {}; error -> {}".format(
-                            connection_name,
-                            response.status_code,
-                            response.text,
-                        )
-                    )
-                else:
-                    logger.info(
-                        "External system -> {} not found.".format(
-                            connection_name)
-                    )
-                return None
-
-    # end method definition
-
-    def addExternalSystemConnection(
-        self,
-        connection_name: str,
-        connection_type: str,
-        as_url: str,
-        base_url: str,
-        username: str,
-        password: str,
-        authentication_method: str = "BASIC",  # either BASIC or OAUTH
-        client_id: str = None,
-        client_secret: str = None,
-    ):
-        """Add Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
-
-        Args:
-            connection_name (string): Name of the connection
-            connection_type (string): Type of the connection (HTTP, SF, SFInstance)
-            as_url (string)
-            base_url (string)
-            username (string)
-            password (string)
-            authentication_method: wither BASIC (using username and password) or OAUTH
-            client_id: OAUTH Client ID (only required if authenticationMethod = OAUTH)
-            client_secret: OAUTH Client Secret (only required if authenticationMethod = OAUTH)
-        Return:
-            External system Details (json) or None if the REST call fails.
-        """
-
-        externalSystemPostBody = {
-            "external_system_name": connection_name,
-            "conn_type": connection_type,
-            "asurl": as_url,
-            "baseurl": base_url,
-            "username": username,
-            "password": password,
-        }
-
-        if authentication_method == "OAUTH" and client_id and client_secret:
-            externalSystemPostBody["authentication_method"] = str(
-                authentication_method)
-            externalSystemPostBody["client_id"] = str(client_id)
-            externalSystemPostBody["client_secret"] = str(client_secret)
-
-        request_url = self.config()["externalSystem"]
-        request_header = self.cookie()
-
-        logger.info(
-            "Creating external system connection -> {} of type -> {} and URL -> {}; calling -> {}".format(
-                connection_name, connection_type, as_url, request_url
-            )
-        )
+        checkNodeNamePostData = {"parent_id": parent_id, "names": [node_name]}
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
-                data=externalSystemPostBody,
                 headers=request_header,
+                data={"body": json.dumps(checkNodeNamePostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to create external system connection -> {}; status -> {}; error -> {}".format(
-                        connection_name,
+                    "Failed to check if node name -> {} can be created in parent location -> {}; status -> {}; error -> {}".format(
+                        node_name,
+                        parent_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def downloadConfigFile(self, otcs_url_suffix: str, file_path: str) -> bool:
-        """ Download a config file from a given OTCS URL. This is NOT
-            for downloading documents from within the OTCS repository
-            but for configuration files such as app packages for MS Teams.
-
-        Args:
-            otcs_url_suffix (str): OTCS URL suffix starting typically starting 
-                                   with /cs/cs?func=,
-                                   e.g. /cs/cs?func=officegroups.DownloadTeamsPackage
-            file_path (str): local path to save the file (direcotry + filename)
-
-        Returns:
-            boolean: True if the download succeeds, False otherwise
-        """
-
-
-        request_url = self.config()["baseUrl"] + otcs_url_suffix
-        # request_header = self.cookie()
-        request_header = self.requestDownloadHeader()
-
-        logger.info(
-            "Download config file from URL -> {}".format(request_url))
-
-        try:
-            response = requests.get(request_url, headers=request_header, cookies=self.cookie())
-            response.raise_for_status()
-        except requests.exceptions.HTTPError as errh:
-            logger.error("Http Error -> {}".format(errh))
-            return False
-        except requests.exceptions.ConnectionError as errc:
-            logger.error("Error Connecting -> {}".format(errc))
-            return False
-        except requests.exceptions.Timeout as errt:
-            logger.error("Timeout Error -> {}".format(errt))
-            return False
-        except requests.exceptions.RequestException as err:
-            logger.error("Request error -> {}".format(err))
-            return False
-
-        content = response.content
-
-        # Open file in write binary mode
-        with open(file_path, 'wb') as file:
-            # Write the content to the file
-            file.write(content)
-
-        logger.info(
-            "Successfully downloaded config file -> {} to -> {}; status code -> {}".format(
-                request_url, file_path, response.status_code
-            )
-        )
-
-        return True
-
-    # end method definition
-
     def uploadFileToVolume(
         self, package_url: str, file_name: str, mime_type: str, volume_type: int
-    ):
+    ) -> dict:
         """Fetch a file from a URL or local filesystem and upload it to a Content Server volume.
 
         Args:
             package_url (string): URL to download file
             file_name (string): name of the file
             mime_type (string): mimeType of the file
             volume_type (integer): type (ID) of the volume
-        Return:
-            Upload response (json) or None if the upload fails.
+        Returns:
+            dictionary: Upload response or None if the upload fails.
         """
 
         if package_url.startswith("http"):
             # Download file from remote location specified by the packageUrl
             # this must be a public place without authentication:
-            logger.info(
-                "Download transport package from URL -> {}".format(package_url))
+            logger.info("Download transport package from URL -> {}".format(package_url))
 
             try:
                 package = requests.get(package_url)
                 package.raise_for_status()
             except requests.exceptions.HTTPError as errh:
                 logger.error("Http Error -> {}".format(errh))
                 return None
@@ -2326,16 +2292,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to upload file -> {} to volume -> {}; status -> {}; error -> {}".format(
                         package_url,
                         volume_type,
@@ -2345,24 +2310,24 @@
                 )
                 return None
 
     # end method definition
 
     def uploadFileToParent(
         self, file_url: str, file_name: str, mime_type: str, parent_id: int
-    ):
+    ) -> dict:
         """Fetch a file from a URL or local filesystem and upload it to a Content Server parent (folder).
 
         Args:
             file_url (string): URL to download file or local file
             file_name (string): name of the file
             mime_type (string): mimeType of the file
             parent_id (integer): parent (ID) of the file to upload
-        Return:
-            Upload response (json) or None if the upload fails.
+        Returns:
+            dictionary: Upload response or None if the upload fails.
         """
 
         if file_url.startswith("http"):
             # Download file from remote location specified by the fileUrl
             # this must be a public place without authentication:
             logger.info("Download file from URL -> {}".format(file_url))
 
@@ -2424,16 +2389,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to upload file -> {} to parent -> {}; status -> {}; error -> {}".format(
                         file_url,
                         parent_id,
@@ -2442,26 +2406,31 @@
                     )
                 )
                 return None
 
     # end method definition
 
     def addDocumentVersion(
-        self, node_id: int, file_url: str, file_name: str, mime_type: str = "text/plain", description: str = ""
-    ):
+        self,
+        node_id: int,
+        file_url: str,
+        file_name: str,
+        mime_type: str = "text/plain",
+        description: str = "",
+    ) -> dict:
         """Fetch a file from a URL or local filesystem and upload it as a new document version.
 
         Args:
             node_id (integer): ID of the document to add add version to
             file_url (string): URL to download file or local file
             file_name (string): name of the file
-            mime_type (string): mimeType of the file
-            description (string): description of the version
-        Return:
-            Add version response (json) or None if the upload fails.
+            mime_type (string, optional): mimeType of the file (default = text/plain)
+            description (string, optional): description of the version (default = no description)
+        Returns:
+            dictinary: Add version response or None if the upload fails.
         """
 
         if file_url.startswith("http"):
             # Download file from remote location specified by the fileUrl
             # this must be a public place without authentication:
             logger.info("Download file from URL -> {}".format(file_url))
 
@@ -2492,21 +2461,18 @@
             logger.info("Uploading local file -> {}".format(file_url))
             file_content = open(file_url, "rb")
 
         else:
             logger.warning("Cannot access -> {}".format(file_url))
             return None
 
-        uploadPostData = {
-            "description": description
-        }
+        uploadPostData = {"description": description}
         uploadPostFiles = [("file", (f"{file_name}", file_content, mime_type))]
 
-        request_url = self.config()["nodesUrlv2"] + \
-            "/" + str(node_id) + "/versions"
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id) + "/versions"
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 500 response
 
         logger.info(
             "Uploading document version -> {} with mime type -> {} to document node -> {}; calling -> {}".format(
                 file_name, mime_type, node_id, request_url
@@ -2522,16 +2488,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add version -> {} to document -> {}; status -> {}; error -> {}".format(
                         file_url,
                         node_id,
@@ -2539,127 +2504,404 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getLatestDocumentVersion(self, node_id: int):
-        """Get latest version of a node based on the node ID.
+    def getLatestDocumentVersion(self, node_id: int) -> dict:
+        """Get latest version of a document node based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the node
-        Return:
-            Node information (json) or None if no node with this ID is found.
+        Returns:
+            dictionary: Node information or None if no node with this ID is found.
         """
 
-        request_url = self.config()["nodesUrl"] + \
-            "/" + str(node_id) + "/versions/latest"
+        request_url = (
+            self.config()["nodesUrl"] + "/" + str(node_id) + "/versions/latest"
+        )
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get latest version of document with node ID -> {}; calling -> {}".format(node_id, request_url))
+            "Get latest version of document with node ID -> {}; calling -> {}".format(
+                node_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get latest version of document with node ID -> {}; status -> {}; error -> {}".format(
                         node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def downloadDocument(self, node_id: int, file_path: str, version_number: str = ""):
+    def downloadDocument(
+        self, node_id: int, file_path: str, version_number: str = ""
+    ) -> bool:
         """Download a document from Extended ECM to local file system.
 
         Args:
             node_id (integer): node ID of the document to download
-            version (string): version of the document to download.
-                              If version = "" then download the latest
-                              version.
             file_path (string): local file path (directory)
-            file_name (string): name of the file
-        Return:
-            True if the document has been download to the specified file.
-            False otherwise.
+            version_number (string): version of the document to download.
+                                     If version = "" then download the latest
+                                     version.
+        Returns:
+            boolean: True if the document has been download to the specified file.
+                     False otherwise.
         """
 
         directory = os.path.dirname(file_path)
         if not os.path.exists(directory):
             logger.error("Directory -> {} does not exist".format(directory))
             return False
 
         if not version_number:
             response = self.getLatestDocumentVersion(node_id)
+            if not response:
+                logger.error("Cannot get latest version of document with ID -> {}".format(node_id))
             version_number = response["data"]["version_number"]
 
-        request_url = self.config()["nodesUrlv2"] + \
-            "/" + str(node_id) + "/versions/" + \
-            str(version_number) + "/content/" + str(node_id)
+        request_url = (
+            self.config()["nodesUrlv2"]
+            + "/"
+            + str(node_id)
+            + "/versions/"
+            + str(version_number)
+            + "/content/"
+            + str(node_id)
+        )
         request_header = self.requestDownloadHeader()
 
         logger.info(
-            "Download document with node ID -> {}; calling -> {}".format(node_id, request_url))
+            "Download document with node ID -> {}; calling -> {}".format(
+                node_id, request_url
+            )
+        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
-                #                content = self.parseRequestResponse(getNodeResponse)["data"]
                 content = response.content
                 break
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to download document with node ID -> {}; status -> {}; error -> {}".format(
                         node_id, response.status_code, response.text
                     )
                 )
                 return False
 
-        logger.info(
-            "Writing document content to file -> {}".format(file_path))
+        logger.info("Writing document content to file -> {}".format(file_path))
 
         # Open file in write binary mode
-        with open(file_path, 'wb') as file:
+        with open(file_path, "wb") as file:
             # Write the content to the file
             file.write(content)
 
         return True
 
         # end method definition
 
-    def createTransportWorkbench(self, workbench_name: str):
+    def downloadConfigFile(self, otcs_url_suffix: str, file_path: str) -> bool:
+        """Download a config file from a given OTCS URL. This is NOT
+            for downloading documents from within the OTCS repository
+            but for configuration files such as app packages for MS Teams.
+
+        Args:
+            otcs_url_suffix (string): OTCS URL suffix starting typically starting
+                                      with /cs/cs?func=,
+                                      e.g. /cs/cs?func=officegroups.DownloadTeamsPackage
+            file_path (string): local path to save the file (direcotry + filename)
+        Returns:
+            boolean: True if the download succeeds, False otherwise
+        """
+
+        request_url = self.config()["baseUrl"] + otcs_url_suffix
+        # request_header = self.cookie()
+        request_header = self.requestDownloadHeader()
+
+        logger.info("Download config file from URL -> {}".format(request_url))
+
+        try:
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
+            )
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as errh:
+            logger.error("Http Error -> {}".format(errh))
+            return False
+        except requests.exceptions.ConnectionError as errc:
+            logger.error("Error Connecting -> {}".format(errc))
+            return False
+        except requests.exceptions.Timeout as errt:
+            logger.error("Timeout Error -> {}".format(errt))
+            return False
+        except requests.exceptions.RequestException as err:
+            logger.error("Request error -> {}".format(err))
+            return False
+
+        content = response.content
+
+        # Open file in write binary mode
+        with open(file_path, "wb") as file:
+            # Write the content to the file
+            file.write(content)
+
+        logger.info(
+            "Successfully downloaded config file -> {} to -> {}; status code -> {}".format(
+                request_url, file_path, response.status_code
+            )
+        )
+
+        return True
+
+    # end method definition
+
+    def search(
+        self,
+        search_term: str,
+        look_for: str = "complexQuery",
+        modifier: str = "",
+        slice_id: int = 0,
+        query_id: int = 0,
+        template_id: int = 0,
+        limit: int = 100,
+        page: int = 1,
+    ) -> dict:
+        """Search for a search term.
+
+        Args:
+            search_term (string), e.g. "test or OTSubType: 189"
+            look_for (string, optional): 'allwords', 'anywords', 'exactphrase', and 'complexquery'.
+                                         If not specified, it defaults to 'complexQuery'.
+            modifier (string, optional): 'synonymsof', 'relatedto', 'soundslike', 'wordbeginswith',
+                                         and 'wordendswith'.
+                                         If not specified or specify any value other than the available options,
+                                         it will be ignored.
+            slice_id (integer,optional): ID of an existing search slice
+            query_id (integer, optional): ID of an saved search query
+            template_id (integer, optional): ID of an saved search template
+            limit (integer, optional): maximum number of results (default = 100)
+            page (integer, optional): number of result page (default = 1 = 1st page)
+        Returns:
+            dictionary: search response or None if the search fails.
+        """
+
+        searchPostBody = {
+            "where": search_term,
+            "lookfor": look_for,
+            "page": page,
+            "limit": limit,
+        }
+
+        if modifier:
+            searchPostBody["modifier"] = modifier
+        if slice_id > 0:
+            searchPostBody["slice_id"] = slice_id
+        if query_id > 0:
+            searchPostBody["query_id"] = query_id
+        if template_id > 0:
+            searchPostBody["template_id"] = template_id
+
+        request_url = self.config()["searchUrl"]
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Serarch for term -> {}; calling -> {}".format(search_term, request_url)
+        )
+
+        retries = 0
+        while True:
+            response = requests.post(
+                request_url,
+                data=searchPostBody,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to search for term -> {}; status -> {}; error -> {}".format(
+                        search_term,
+                        response.status_code,
+                        response.text,
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def getExternalSystemConnection(
+        self, connection_name: str, show_error: bool = False
+    ) -> dict:
+        """Get Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
+
+        Args:
+            connection_name (string): Name of the connection
+            show_error (boolean): treat as error if node is not found
+        Returns:
+            dictionary: External system Details or None if the REST call fails.
+        """
+
+        request_url = (
+            self.config()["externalSystem"] + "/" + connection_name + "/config"
+        )
+        request_header = self.cookie()
+
+        logger.info(
+            "Get external system connection -> {}; calling -> {}".format(
+                connection_name, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                if show_error:
+                    logger.error(
+                        "Failed to get external system connection -> {}; status -> {}; error -> {}".format(
+                            connection_name,
+                            response.status_code,
+                            response.text,
+                        )
+                    )
+                else:
+                    logger.info(
+                        "External system -> {} not found.".format(connection_name)
+                    )
+                return None
+
+    # end method definition
+
+    def addExternalSystemConnection(
+        self,
+        connection_name: str,
+        connection_type: str,
+        as_url: str,
+        base_url: str,
+        username: str,
+        password: str,
+        authentication_method: str = "BASIC",  # either BASIC or OAUTH
+        client_id: str = None,
+        client_secret: str = None,
+    ) -> dict:
+        """Add Extended ECM external system connection (e.g. SAP, Salesforce, SuccessFactors).
+
+        Args:
+            connection_name (string): Name of the connection
+            connection_type (string): Type of the connection (HTTP, SF, SFInstance)
+            as_url (string)
+            base_url (string)
+            username (string)
+            password (string)
+            authentication_method: wither BASIC (using username and password) or OAUTH
+            client_id: OAUTH Client ID (only required if authenticationMethod = OAUTH)
+            client_secret: OAUTH Client Secret (only required if authenticationMethod = OAUTH)
+        Returns:
+            dictionary: External system Details or None if the REST call fails.
+        """
+
+        externalSystemPostBody = {
+            "external_system_name": connection_name,
+            "conn_type": connection_type,
+            "asurl": as_url,
+            "baseurl": base_url,
+            "username": username,
+            "password": password,
+        }
+
+        if authentication_method == "OAUTH" and client_id and client_secret:
+            externalSystemPostBody["authentication_method"] = str(authentication_method)
+            externalSystemPostBody["client_id"] = str(client_id)
+            externalSystemPostBody["client_secret"] = str(client_secret)
+
+        request_url = self.config()["externalSystem"]
+        request_header = self.cookie()
+
+        logger.info(
+            "Creating external system connection -> {} of type -> {} and URL -> {}; calling -> {}".format(
+                connection_name, connection_type, as_url, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.post(
+                request_url,
+                data=externalSystemPostBody,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to create external system connection -> {}; status -> {}; error -> {}".format(
+                        connection_name,
+                        response.status_code,
+                        response.text,
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def createTransportWorkbench(self, workbench_name: str) -> dict:
         """Create a Workbench in the Transport Volume.
 
         Args:
             workbench_name (string): name of the workbench to be created
-        Return:
-            Create response (json) or None if the creation fails.
+        Returns:
+            dictionary: Create response or None if the creation fails.
         """
 
         createWorbenchPostData = {"type": "528", "name": workbench_name}
 
         request_url = self.config()["nodesUrlv2"]
         request_header = self.requestFormHeader()
 
@@ -2676,42 +2918,40 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create transport workbench -> {}; status -> {}; error -> {}".format(
                         workbench_name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def unpackTransportPackage(self, package_id: int, workbench_id: int):
+    def unpackTransportPackage(self, package_id: int, workbench_id: int) -> dict:
         """Unpack an existing Transport Package into an existing Workbench.
 
         Args:
             package_iD (integer): ID of package to be unpacked
             workbench_iD (integer): ID of target workbench
-        Return:
-            Unpack response (json) or None if the unpacking fails.
+        Returns:
+            dictionary: Unpack response or None if the unpacking fails.
         """
 
         unpackPackagePostData = {"workbench_id": workbench_id}
 
-        request_url = self.config()["nodesUrlv2"] + \
-            "/" + str(package_id) + "/unpack"
+        request_url = self.config()["nodesUrlv2"] + "/" + str(package_id) + "/unpack"
         request_header = self.requestFormHeader()
 
         logger.info(
             "Unpack transport package with ID -> {} into workbench with ID -> {}; calling -> {}".format(
                 package_id, workbench_id, request_url
             )
         )
@@ -2724,16 +2964,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to unpack package -> {}; to workbench -> {}; status -> {}; error -> {}".format(
                         package_id,
                         workbench_id,
@@ -2741,25 +2980,24 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def deployWorkbench(self, workbench_id: int):
+    def deployWorkbench(self, workbench_id: int) -> dict:
         """Deploy an existing Workbench.
 
         Args:
             workbench_iD (integer): ID of the workbench to be deployed
-        Return:
-            Deploy response (json) or None if the deployment fails.
+        Returns:
+            dictionary: Deploy response or None if the deployment fails.
         """
 
-        request_url = self.config()["nodesUrlv2"] + \
-            "/" + str(workbench_id) + "/deploy"
+        request_url = self.config()["nodesUrlv2"] + "/" + str(workbench_id) + "/deploy"
         request_header = self.requestFormHeader()
 
         logger.info(
             "Deploy workbench with ID -> {}; calling -> {}".format(
                 workbench_id, request_url
             )
         )
@@ -2777,80 +3015,81 @@
                         workbench_id, e
                     )
                 )
                 return None
             if response.ok:
                 response_dict = self.parseRequestResponse(response)
                 if not response_dict:
-                    logger.error(
-                        "Error deploying workbench -> {}".format(workbench_id))
+                    logger.error("Error deploying workbench -> {}".format(workbench_id))
                     return None
                 return response_dict
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.warning(
                     "Failed to depoloy workbench -> {}; status -> {}; error -> {}".format(
                         workbench_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def deployTransport(
-        self, package_url: str, package_name: str, package_description: str = "", replacements: list = []
-    ):
+        self,
+        package_url: str,
+        package_name: str,
+        package_description: str = "",
+        replacements: list = [],
+    ) -> dict:
         """Main method to deploy a transport. This uses subfunctions to upload,
            unpackage and deploy the transport, and creates the required workbench.
 
         Args:
             package_url (string): URL to download the transport package.
             package_name (string): name of the transport package ZIP file
             package_description (string): description of the transport package
             replacements (list of dicts): list of replacement values to be applied
-                                          to all XML files in transport; dict needs to have two values:
-                                         * placeholder: text to replace
-                                         * value: text to replace with
-        Return:
-            Deploy response (json) or None if the deployment fails.
+                                          to all XML files in transport;
+                                          each dict needs to have two values:
+                                          - placeholder: text to replace
+                                          - value: text to replace with
+        Returns:
+            dictionary: Deploy response or None if the deployment fails.
         """
 
         # Preparation: get volume IDs for Transport Warehouse (root volume and Transport Packages)
         response = self.getVolume(525)
         transport_root_volume_id = self.getResultValue(response, "id")
         if not transport_root_volume_id:
             logger.error("Failed to retrieve transport root volume")
             return None
-        logger.info(
-            "Transport root volume ID -> {}".format(transport_root_volume_id))
+        logger.info("Transport root volume ID -> {}".format(transport_root_volume_id))
 
         response = self.getNodeByParentAndName(
             transport_root_volume_id, "Transport Packages"
         )
         transport_package_volume_id = self.getResultValue(response, "id")
         if not transport_package_volume_id:
             logger.error("Failed to retrieve transport package volume")
             return None
         logger.info(
-            "Transport package volume ID -> {}".format(
-                transport_package_volume_id)
+            "Transport package volume ID -> {}".format(transport_package_volume_id)
         )
 
         # Step 1: Upload Transport Package
         logger.info(
-            "Check if transport package -> {} already exists...".format(
-                package_name)
+            "Check if transport package -> {} already exists...".format(package_name)
         )
         response = self.getNodeByParentAndName(
-            transport_package_volume_id, package_name)
+            transport_package_volume_id, package_name
+        )
         package_id = self.getResultValue(response, "id")
         if package_id:
             logger.info(
                 "Transport package -> {} does already exist; existing package ID -> {}".format(
                     package_name, package_id
                 )
             )
@@ -2858,40 +3097,42 @@
             logger.info(
                 "Transport package -> {} does not yet exist, loading from -> {}".format(
                     package_name, package_url
                 )
             )
             # If we have string replacements configured execute them now:
             if replacements:
-                logger.info("Transport -> {} has replacements -> {}".format(package_name, replacements))
+                logger.info(
+                    "Transport -> {} has replacements -> {}".format(
+                        package_name, replacements
+                    )
+                )
                 self.replaceTransportPlaceholders(package_url, replacements)
             else:
                 logger.info("Transport -> {} has no replacements!".format(package_name))
             # Upload package to Extended ECM:
             response = self.uploadFileToVolume(
                 package_url, package_name, "application/zip", 531
             )
             package_id = self.getResultValue(response, "id")
             if not package_id:
                 logger.error(
-                    "Failed to upload transport package -> {}".format(
-                        package_url)
+                    "Failed to upload transport package -> {}".format(package_url)
                 )
                 return None
             logger.info(
                 "Successfully uploaded transport package -> {}; new package ID -> {}".format(
                     package_name, package_id
                 )
             )
 
         # Step 2: Create Transport Workbench (if not yet exist)
         workbench_name = package_name.split(".")[0]
         logger.info(
-            "Check if workbench -> {} is already deployed...".format(
-                workbench_name)
+            "Check if workbench -> {} is already deployed...".format(workbench_name)
         )
         # check if the package name has the suffix "(deployed)" - this indicates it is alreadey
         # successfully deployed (see renaming at the end of this method)
         response = self.getNodeByParentAndName(
             transport_root_volume_id, workbench_name + " (deployed)"
         )
         workbench_id = self.getResultValue(response, "id")
@@ -2901,16 +3142,15 @@
                     workbench_name, workbench_id
                 )
             )
             # we return and skip this transport...
             return response
         else:
             logger.info(
-                "Check if workbench -> {} already exists...".format(
-                    workbench_name)
+                "Check if workbench -> {} already exists...".format(workbench_name)
             )
             response = self.getNodeByParentAndName(
                 transport_root_volume_id, workbench_name
             )
             workbench_id = self.getResultValue(response, "id")
             if workbench_id:
                 logger.info(
@@ -2919,16 +3159,15 @@
                     )
                 )
             else:
                 response = self.createTransportWorkbench(workbench_name)
                 workbench_id = self.getResultValue(response, "id")
                 if not workbench_id:
                     logger.error(
-                        "Failed to create workbench -> {}".format(
-                            workbench_name)
+                        "Failed to create workbench -> {}".format(workbench_name)
                     )
                     return None
                 logger.info(
                     "Successfully created workbench -> {}; new workbench ID -> {}".format(
                         workbench_name, workbench_id
                     )
                 )
@@ -2938,31 +3177,28 @@
             "Unpack transport package -> {} ({}) to workbench -> {} ({})".format(
                 package_name, package_id, workbench_name, workbench_id
             )
         )
         response = self.unpackTransportPackage(package_id, workbench_id)
         if response == None:
             logger.error(
-                "Failed to unpack the transport package -> {}".format(
-                    package_name)
+                "Failed to unpack the transport package -> {}".format(package_name)
             )
             return None
         logger.info(
             "Successfully unpackaged to workbench -> {} ({})".format(
                 workbench_name, workbench_id
             )
         )
 
         # Step 4: Deploy Workbench
-        logger.info(
-            "Deploy workbench -> {} ({})".format(workbench_name, workbench_id))
+        logger.info("Deploy workbench -> {} ({})".format(workbench_name, workbench_id))
         response = self.deployWorkbench(workbench_id)
         if response == None:
-            logger.warning(
-                "Failed to to deploy workbench -> {}".format(workbench_name))
+            logger.warning("Failed to to deploy workbench -> {}".format(workbench_name))
             return None
 
         logger.info(
             "Successfully deployed workbench -> {} ({})".format(
                 workbench_name, workbench_id
             )
         )
@@ -2972,25 +3208,26 @@
             package_description,
         )
 
         return response
 
     # end method definition
 
-    def replaceInXmlFiles(self, directory: str, search_pattern: str, replace_string: str) -> bool:
-        """ Replaces all occurrences of the search pattern with the replace string in all XML files
+    def replaceInXmlFiles(
+        self, directory: str, search_pattern: str, replace_string: str
+    ) -> bool:
+        """Replaces all occurrences of the search pattern with the replace string in all XML files
             in the directory and its subdirectories.
 
         Args:
             directory (string): directory to traverse for XML files
             search_pattern (sting): string to search in the XML file
             replace_string (string): replacement string
-
         Returns:
-            bool: True if a replacement happened, False otherwise
+            boolean: True if a replacement happened, False otherwise
         """
         # Define the regular expression pattern to search for
         pattern = re.compile(search_pattern)
         found = False
 
         # Traverse the directory and its subdirectories
         for subdir, dirs, files in os.walk(directory):
@@ -3003,33 +3240,38 @@
                         contents = f.read()
 
                     # Replace all occurrences of the search pattern with the replace string
                     new_contents = pattern.sub(replace_string, contents)
 
                     # Write the updated contents to the file if there were replacements
                     if contents != new_contents:
-                        logger.info("Found search string -> {} in XML file -> {}. Updating content...".format(search_pattern, file_path))
+                        logger.info(
+                            "Found search string -> {} in XML file -> {}. Updating content...".format(
+                                search_pattern, file_path
+                            )
+                        )
                         # Write the updated contents to the file
                         with open(file_path, "w") as f:
                             f.write(new_contents)
                         found = True
 
         return found
-    
+
         # end method definition
 
-    def replaceTransportPlaceholders(self, zip_file_path: str, replacements: list) -> bool:
-        """ Search and replace strings in the XML files of the transport packlage
+    def replaceTransportPlaceholders(
+        self, zip_file_path: str, replacements: list
+    ) -> bool:
+        """Search and replace strings in the XML files of the transport packlage
 
         Args:
             zip_file_path (string): path to transport zip file
             replacements (list of dicts): list of replacement values; dict needs to have two values:
                                          * placeholder: text to replace
                                          * value: text to replace with
-
         Returns:
             Filename to the updated zip file
         """
 
         if not os.path.isfile(zip_file_path):
             logger.error("Zip file -> {} not found.".format(zip_file_path))
             return False
@@ -3039,56 +3281,97 @@
         with zipfile.ZipFile(zip_file_path, "r") as zfile:
             zfile.extractall(zip_file_folder)
 
         modified = False
 
         # Replace search pattern with replace string in all XML files in the directory and its subdirectories
         for replacement in replacements:
-            logger.info("Replace -> {} with -> {} in Transport package -> {}".format(replacement["placeholder"], replacement["value"], zip_file_folder))
-            found = self.replaceInXmlFiles(zip_file_folder, replacement["placeholder"], replacement["value"])
+            if replacement["placeholder"] == replacement["value"]:
+                logger.info(
+                    "Placeholder and replacement are identical -> {}. Skipping...".format(
+                        replacement["value"]
+                    )
+                )
+                continue
+            logger.info(
+                "Replace -> {} with -> {} in Transport package -> {}".format(
+                    replacement["placeholder"], replacement["value"], zip_file_folder
+                )
+            )
+            found = self.replaceInXmlFiles(
+                zip_file_folder, replacement["placeholder"], replacement["value"]
+            )
             if found:
-                logger.info("Found replacement string -> {} in Transport package -> {}".format(replacement["placeholder"], zip_file_folder))
+                logger.info(
+                    "Found replacement string -> {} in Transport package -> {}".format(
+                        replacement["placeholder"], zip_file_folder
+                    )
+                )
                 modified = True
             else:
-                logger.warning("Did not find replacement string -> {} in Transport package -> {}".format(replacement["placeholder"], zip_file_folder))
+                logger.warning(
+                    "Did not find replacement string -> {} in Transport package -> {}".format(
+                        replacement["placeholder"], zip_file_folder
+                    )
+                )
 
         if not modified:
-            logger.warning("None of the replacements have been found in transport -> {}".format(zip_file_folder))
+            logger.warning(
+                "None of the replacements have been found in transport -> {}".format(
+                    zip_file_folder
+                )
+            )
             return False
 
         # Create the new zip file and add all files from the directory to it
-        new_zip_file_path = os.path.dirname(zip_file_path) + "/new_" + os.path.basename(zip_file_path)
-        logger.info("Content of transport -> {} has been modified - repacking to new zip file -> {}".format(zip_file_folder, new_zip_file_path))
+        new_zip_file_path = (
+            os.path.dirname(zip_file_path) + "/new_" + os.path.basename(zip_file_path)
+        )
+        logger.info(
+            "Content of transport -> {} has been modified - repacking to new zip file -> {}".format(
+                zip_file_folder, new_zip_file_path
+            )
+        )
         with zipfile.ZipFile(new_zip_file_path, "w", zipfile.ZIP_DEFLATED) as zip_ref:
             for subdir, dirs, files in os.walk(zip_file_folder):
                 for file in files:
                     file_path = os.path.join(subdir, file)
                     rel_path = os.path.relpath(file_path, zip_file_folder)
                     zip_ref.write(file_path, arcname=rel_path)
 
         # Close the new zip file and delete the temporary directory
         zip_ref.close()
-        old_zip_file_path = os.path.dirname(zip_file_path) + "/old_" + os.path.basename(zip_file_path)
-        logger.info("Rename orginal transport zip file -> {} to -> {}".format(zip_file_path, old_zip_file_path))
+        old_zip_file_path = (
+            os.path.dirname(zip_file_path) + "/old_" + os.path.basename(zip_file_path)
+        )
+        logger.info(
+            "Rename orginal transport zip file -> {} to -> {}".format(
+                zip_file_path, old_zip_file_path
+            )
+        )
         os.rename(zip_file_path, old_zip_file_path)
-        logger.info("Rename new transport zip file -> {} to -> {}".format(new_zip_file_path, zip_file_path))
+        logger.info(
+            "Rename new transport zip file -> {} to -> {}".format(
+                new_zip_file_path, zip_file_path
+            )
+        )
         os.rename(new_zip_file_path, zip_file_path)
 
         # Return the path to the new zip file
         return True
 
         # end method definition
 
-    def getWorkspaceTypes(self):
+    def getWorkspaceTypes(self) -> dict:
         """Get all workspace types configured in Extended ECM.
 
         Args:
             None
-        Return:
-            Workspace Types (json) or None if the request fails.
+        Returns:
+            dictionary: Workspace Types or None if the request fails.
         """
 
         request_url = (
             self.config()["businessworkspacetypes"]
             + "?expand_templates=true&expand_wksp_info=true"
         )
         request_header = self.requestFormHeader()
@@ -3100,36 +3383,35 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace types; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getBusinessObjectType(self, external_system_id: str, type_name: str):
+    def getBusinessObjectType(self, external_system_id: str, type_name: str) -> dict:
         """Get business object type information.
 
         Args:
             external_system_id (string): external system Id (such as "TM6")
             type_name (string): type name (such as "SAP Customer")
-        Return:
-            Workspace Type information (json) or None if the request fails.
+        Returns:
+            dictionary: Workspace Type information or None if the request fails.
         """
 
         request_url = (
             self.config()["externalSystem"]
             + "/"
             + str(external_system_id)
             + "/botypes/"
@@ -3148,16 +3430,15 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get business object type -> {}; status -> {}; error -> {}".format(
                         type_name,
                         response.status_code,
@@ -3171,27 +3452,27 @@
     def getWorkspaceCreateForm(
         self,
         template_id: int,
         external_system_id: int = None,
         bo_type: int = None,
         bo_id: int = None,
         parent_id: int = None,
-    ):
+    ) -> dict:
         """Get the Workspace create form.
 
         Args:
             template_id (integer): ID of the workspace template
             external_system_id (string): identifier of the external system (None if no external system)
-            bo_type (string): business object type (None if no external system)
-            bo_id (string): business object identifier / key (None if no external system)
-            parent_id (string): parent ID of the workspaces. Needs only be specified in special
-                                cases where workspace location cannot be derived from workspace
-                                type definition, e.g. sub-workspace
-        Return:
-            Workspace Create Form data (json) or None if the request fails.
+            bo_type (string, optional): business object type (None if no external system)
+            bo_id (string, optional): business object identifier / key (None if no external system)
+            parent_id (string, optional): parent ID of the workspaces. Needs only be specified in special
+                                          cases where workspace location cannot be derived from workspace
+                                          type definition, e.g. sub-workspace
+        Returns:
+            dictionary: Workspace Create Form data or None if the request fails.
         """
 
         request_url = self.config()[
             "businessworkspacecreateform"
         ] + "?template_id={}".format(template_id)
         # Is a parent ID specifified? Then we need to add it to the request URL
         if parent_id is not None:
@@ -3219,128 +3500,163 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace create form for template -> {}; status -> {}; error -> {}".format(
                         template_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspace(self, node_id: int):
+    def getWorkspace(self, node_id: int) -> dict:
         """Get a workspace based on the node ID.
 
         Args:
             node_id (integer) is the node Id of the workspace
-        Return:
-            Node information (json) or None if no node with this ID is found.
+        Returns:
+            dictionary: Workspace node information or None if no node with this ID is found.
         """
 
         request_url = self.config()["businessworkspaces"] + "/" + str(node_id)
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get workspace with ID -> {}; calling -> {}".format(
-                node_id, request_url)
+            "Get workspace with ID -> {}; calling -> {}".format(node_id, request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace with ID -> {}; status -> {}; error -> {}".format(
                         node_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceByNameAndType(
-        self, name: str, type_name: str, expanded_view: bool = True
-    ):
-        """Lookup workspace based on workspace name and workspace type name.
+    def getWorkspaceInstances(self, type_name: str, expanded_view: bool = True):
+        """Get all workspace instances of a given type. This is a convenience
+           wrapper method for getWorkspaceByTypeAndName()
 
         Args:
-            name (string): name of the workspace
             type_name (string): name of the workspace type
-            expanded_view (boolean): if 'False' then just search in recently
-                                     accessed business workspace for this name and type
-                                     if 'True' (this is the default) then search in all
-                                     workspaces for this name and type
-        Return:
-            Workspace information (json) or None if the workspace is not found.
+            expanded_view (boolean, optional): if 'False' then just search in recently
+                                               accessed business workspace for this name and type
+                                               if 'True' (this is the default) then search in all
+                                               workspaces for this name and type
+        Returns:
+            dictionary: Workspace information or None if the workspace is not found.
+        """
+
+        return self.getWorkspaceByTypeAndName(
+            type_name, name="", expanded_view=expanded_view
+        )
+
+    # end method definition
+
+    def getWorkspaceByTypeAndName(
+        self, type_name: str, name: str = "", expanded_view: bool = True
+    ) -> dict:
+        """Lookup workspace based on workspace type and workspace name.
+
+        Args:
+            type_name (string): name of the workspace type
+            name (string, optional): name of the workspace, if "" then deliver all instances
+                                     of the given workspace type
+            expanded_view (boolean, optional): if 'False' then just search in recently
+                                               accessed business workspace for this name and type
+                                               if 'True' (this is the default) then search in all
+                                               workspaces for this name and type
+        Returns:
+            dictionary: Workspace information or None if the workspace is not found.
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {
-            "where_name": name,
+            #            "where_name": name,
             "where_workspace_type_name": type_name,
             "expanded_view": expanded_view,
         }
+        if name:
+            query["where_name"] = name
+
         encodedQuery = urllib.parse.urlencode(query, doseq=True)
 
-        request_url = self.config()["businessworkspaces"] + \
-            "?{}".format(encodedQuery)
+        request_url = self.config()["businessworkspaces"] + "?{}".format(encodedQuery)
         request_header = self.requestFormHeader()
 
-        logger.info(
-            "Get workspace with name -> {} and type -> {}; calling -> {}".format(
-                name, type_name, request_url
+        if name:
+            logger.info(
+                "Get workspace with name -> {} and type -> {}; calling -> {}".format(
+                    name, type_name, request_url
+                )
+            )
+        else:
+            logger.info(
+                "Get all workspace instances of type -> {}; calling -> {}".format(
+                    type_name, request_url
+                )
             )
-        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
-                logger.warning(
-                    "Failed to get workspace -> {} of type -> {}; status -> {}; error -> {}".format(
-                        name,
-                        type_name,
-                        response.status_code,
-                        response.text,
+                if name:
+                    logger.warning(
+                        "Failed to get workspace -> {} of type -> {}; status -> {}; error -> {}".format(
+                            name,
+                            type_name,
+                            response.status_code,
+                            response.text,
+                        )
+                    )
+                else:
+                    logger.warning(
+                        "Failed to get workspace instances of type -> {}; status -> {}; error -> {}".format(
+                            type_name,
+                            response.status_code,
+                            response.text,
+                        )
                     )
-                )
                 return None
 
     # end method definition
 
     def createWorkspace(
         self,
         workspace_template_id: int,
@@ -3348,31 +3664,31 @@
         workspace_description: str,
         workspace_type: int,
         category_data: dict = {},
         external_system_id: int = None,
         bo_type: int = None,
         bo_id: int = None,
         parent_id: int = None,
-    ):
+    ) -> dict:
         """Create a new business workspace.
 
         Args:
             workspace_template_id (integer): ID of the workspace template
             workspace_name (string): name of the workspace
             workspace_description (string): description of the workspace
             workspace_type (integer): type ID of the workspace
             category_data (dict): category and attributes
-            external_system_id (string): identifier of the external system (None if no external system)
-            bo_type (string): business object type (None if no external system)
-            bo_id (string): business object identifier / key (None if no external system)
-            parent_id (string): parent ID of the workspaces. Needs only be specified in special
-                                cases where workspace location cannot be derived from workspace
-                                type definition
-        Return:
-            Workspace Create Form data (json) or None if the request fails.
+            external_system_id (string, optional): identifier of the external system (None if no external system)
+            bo_type (string, optional): business object type (None if no external system)
+            bo_id (string, optional): business object identifier / key (None if no external system)
+            parent_id (string, optional): parent ID of the workspaces. Needs only be specified in special
+                                          cases where workspace location cannot be derived from workspace
+                                          type definition
+        Returns:
+            dictionary: Workspace Create Form data or None if the request fails.
         """
 
         createWorkspacePostData = {
             "template_id": str(workspace_template_id),
             "name": workspace_name,
             "description": workspace_description,
             "wksp_type_id": str(workspace_type),
@@ -3427,16 +3743,15 @@
                 data={"body": json.dumps(createWorkspacePostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create workspace -> {} from template -> {}; status -> {}; error -> {}".format(
                         workspace_name,
                         workspace_template_id,
@@ -3445,24 +3760,27 @@
                     )
                 )
                 return None
 
     # end method definition
 
     def createWorkspaceRelationship(
-        self, workspace_id: int, related_workspace_id: int, relationship_type: str = "child"
-    ):
+        self,
+        workspace_id: int,
+        related_workspace_id: int,
+        relationship_type: str = "child",
+    ) -> dict:
         """Create a relationship between two workspaces.
 
         Args:
-            workspace_id: ID of the workspace
-            related_workspace_id: ID of the related workspace
-            relationship_type: "parent" or "child" - "child is default if omitted
-        Return:
-            Workspace Relationship data (json) or None if the request fails.
+            workspace_id (integer): ID of the workspace
+            related_workspace_id (integer): ID of the related workspace
+            relationship_type (string, optional): "parent" or "child" - "child" is default if omitted
+        Returns:
+            dictionary: Workspace Relationship data (json) or None if the request fails.
         """
 
         createWorkspaceRelationshipPostData = {
             "rel_bw_id": str(related_workspace_id),
             "rel_type": relationship_type,
         }
 
@@ -3485,16 +3803,15 @@
                 data=createWorkspaceRelationshipPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create workspace relationship between -> {} and -> {}; status -> {}; error -> {}".format(
                         workspace_id,
                         related_workspace_id,
@@ -3502,26 +3819,28 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceRelationships(self, workspace_id: int):
+    def getWorkspaceRelationships(self, workspace_id: int) -> dict:
         """Get the Workspace relationships to other workspaces.
 
         Args:
-            workspace_id: ID of the workspace template
-        Return:
-            Workspace relationships (json) or None if the request fails.
+            workspace_id (integer): ID of the workspace template
+        Returns:
+            dictionary: Workspace relationships or None if the request fails.
         """
 
         request_url = (
-            self.config()["businessworkspaces"] + "/" +
-            str(workspace_id) + "/relateditems"
+            self.config()["businessworkspaces"]
+            + "/"
+            + str(workspace_id)
+            + "/relateditems"
         )
         request_header = self.requestFormHeader()
 
         logger.info(
             "Get related workspaces for workspace -> {}; calling -> {}".format(
                 workspace_id, request_url
             )
@@ -3532,42 +3851,40 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get related workspaces of workspace -> {}; status -> {}; error -> {}".format(
                         workspace_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getWorkspaceRoles(self, workspace_id: int):
+    def getWorkspaceRoles(self, workspace_id: int) -> dict:
         """Get the Workspace roles.
 
         Args:
-            workspace_id: ID of the workspace template
-        Return:
-            Workspace Roles data (json) or None if the request fails.
+            workspace_id (integer): ID of the workspace template
+        Returns:
+            dictionary: Workspace Roles data or None if the request fails.
         """
 
         request_url = (
-            self.config()["businessworkspaces"] + "/" +
-            str(workspace_id) + "/roles"
+            self.config()["businessworkspaces"] + "/" + str(workspace_id) + "/roles"
         )
         request_header = self.requestFormHeader()
 
         logger.info(
             "Get workspace roles of workspace -> {}; calling -> {}".format(
                 workspace_id, request_url
             )
@@ -3578,40 +3895,41 @@
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get roles of workspace -> {}; status -> {}; error -> {}".format(
                         workspace_id,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def addMemberToWorkspace(self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True):
+    def addMemberToWorkspace(
+        self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True
+    ) -> dict:
         """Add member to a workspace role. Check that the user is not yet a member.
 
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             member_id (integer): User or Group Id
-            show_warning: if True shows a warning if member is already in role
-        Return:
-            Workspace Role Membership (json) or None if the request fails.
+            show_warning (boolean, optional): if True shows a warning if member is already in role
+        Returns:
+            dictionary: Workspace Role Membership or None if the request fails.
         """
 
         addMemberToWorkspacePostData = {"id": str(member_id)}
 
         request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
@@ -3631,16 +3949,15 @@
                 "Failed to get workspace members; status -> {}; error -> {}".format(
                     response.status_code,
                     response.text,
                 )
             )
             return None
 
-        workspace_members = self.parseRequestResponse(
-            response)
+        workspace_members = self.parseRequestResponse(response)
 
         if self.existResultItem(workspace_members, "id", member_id):
             if show_warning:
                 logger.warning(
                     "User -> {} is already a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
@@ -3672,24 +3989,26 @@
                     response.text,
                 )
             )
             return None
 
     # end method definition
 
-    def removeMemberFromWorkspace(self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True):
+    def removeMemberFromWorkspace(
+        self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True
+    ) -> dict:
         """Remove a member from a workspace role. Check that the user is currently a member.
 
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             member_id (integer): User or Group Id
-            show_warning: if True shows a warning if member is not in role
-        Return:
-            Workspace Role Membership (json) or None if the request fails.
+            show_warning (boolean, optional): if True shows a warning if member is not in role
+        Returns:
+            dictionary: Workspace Role Membership or None if the request fails.
         """
 
         request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
         request_header = self.requestFormHeader()
 
@@ -3707,16 +4026,15 @@
                 "Failed to get workspace members; status -> {}; error -> {}".format(
                     workspaceMembershipResponse.status_code,
                     workspaceMembershipResponse.text,
                 )
             )
             return None
 
-        workspace_members = self.parseRequestResponse(
-            workspaceMembershipResponse)
+        workspace_members = self.parseRequestResponse(workspaceMembershipResponse)
 
         if not self.existResultItem(workspace_members, "id", member_id):
             if show_warning:
                 logger.warning(
                     "User -> {} is not a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
@@ -3753,15 +4071,15 @@
             )
             return None
 
     # end method definition
 
     def assignWorkspacePermissions(
         self, workspace_id: int, role_id: int, permissions: list, apply_to: int = 2
-    ):
+    ) -> dict:
         """Update permissions of a workspace role
         Args:
             workspace_id (integer): ID of the workspace
             role_id (integer): ID of the role
             permissions (list): list of permissions - potential elements:
                                 "see"
                                 "see_contents"
@@ -3771,18 +4089,18 @@
                                 "reserve"
                                 "add_major_version"
                                 "delete_versions"
                                 "delete"
                                 "edit_permissions"
             apply_to (integer):  0 = this item
                                  1 = sub-items
-                                 2 = This item and sub-items
+                                 2 = This item and sub-items (default)
                                  3 = This item and immediate sub-items
-        Return:
-            Workspace Role Membership (json) or None if the request fails.
+        Returns:
+            dictionary: Workspace Role Membership or None if the request fails.
         """
 
         request_url = self.config()["businessworkspaces"] + "/{}/roles/{}".format(
             workspace_id, role_id
         )
 
         request_header = self.requestFormHeader()
@@ -3806,16 +4124,15 @@
                 data={"body": json.dumps(permissionPostData)},
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update permissions for role -> {} of workspace -> {}; status -> {}; error -> {}".format(
                         role_id,
                         workspace_id,
@@ -3823,35 +4140,95 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
+    def updateWorkspaceIcon(
+        self, workspace_id: int, file_path: str, file_mimetype: str = "image/*"
+    ):
+        """Update a workspace with a with a new icon (which is uploaded).
+
+        Args:
+            workspace_id (integer): ID of the workspace
+            file_path (string): path + filename of icon file
+        Returns:
+            dictionary: Node information or None if REST call fails.
+        """
+
+        if not os.path.exists(file_path):
+            logger.error("Workdpace icon file does not exist -> {}".format(file_path))
+            return None
+        
+#        icon_file = open(file_path, "rb")
+
+        updateWorkspaceIconPutBody = {
+            "file_content_type": file_mimetype,
+            "file_filename": os.path.basename(file_path),
+            "file": file_path #icon_file
+        }
+
+        request_url = (
+            self.config()["businessworkspaces"] + "/" + str(workspace_id) + "/icons"
+        )
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Update icon for workspace ID -> {} with icon file -> {}; calling -> {}".format(
+                workspace_id, file_path, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.post(
+                request_url,
+                data=updateWorkspaceIconPutBody,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to update workspace ID -> {} with new icon -> {}; status -> {}; error -> {}".format(
+                        workspace_id, file_path, response.status_code, response.text
+                    )
+                )
+                return None
+
+    # end method definition
+
     def createItem(
         self,
         parent_id: int,
         item_type: str,
         item_name: str,
         item_description: str = "",
         url: str = "",
         original_id: int = 0,
-    ):
+    ) -> dict:
         """Create an Extended ECM item. This REST call is somewhat limited. It cannot set favortie (featured item) or hidden item.
            It does also not accept owner group information.
 
         Args:
             parent_id (integer): node ID of the parent
             item_type (string): type of the item (e.g. 0 = foler, 140 = URL)
             item_name (string): name of the item
-            item_description (string): description of the item
-            url (string): address of the URL item (if it is an URL item type)
-            original_id (integer)
-        Return:
-            Response (json) of the created item or None if the REST call has failed.
+            item_description (string, optional): description of the item
+            url (string, optional): address of the URL item (if it is an URL item type)
+            original_id (integer, optional): required if a shortcut item is created
+        Returns:
+            dictionary: Request response of the create item call or None if the REST call has failed.
         """
 
         createItemPostData = {
             "parent_id": parent_id,
             "type": item_type,
             "name": item_name,
             "description": item_description,
@@ -3880,16 +4257,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create item -> {}; status -> {}; error -> {}".format(
                         item_name,
                         response.status_code,
@@ -3902,25 +4278,25 @@
 
     def updateItem(
         self,
         node_id: int,
         parent_id: int = 0,
         item_name: str = "",
         item_description: str = "",
-    ):
+    ) -> dict:
         """Update an Extended ECM item (parent, name, description). Changing the parent ID is
            a move operation. If parent ID = 0 the item will not be moved.
 
         Args:
             node_id (integer): ID of the node
             parent_id (integer): node ID of the new parent (move operation)
             item_name (string): new name of the item
             item_description (string): new description of the item
-        Return:
-            Response (json) of the created item or None if the REST call has failed.
+        Returns:
+            dictionary: Response of the update item request or None if the REST call has failed.
         """
 
         updateItemPutData = {
             "name": item_name,
             "description": item_description,
         }
 
@@ -3946,37 +4322,196 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update item -> {}; status -> {}; error -> {}".format(
                         item_name,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
+    def getDocumentTemplates(self, parent_id: int):
+        """Get all document templates for a given target location.
+
+        Args:
+            parent_id (integer): node ID of target location (e.g. a folder)
+
+        Returns:
+            dictionary: response of the REST call (converted to a Python dictionary)
+                        Example output:
+                        'results': [
+                            {
+                                'container': False,
+                                'hasTemplates': False,
+                                'name': 'Document',
+                                'subtype': 144,
+                                'templates': [
+                                    {
+                                        'description_multilingual': {...},
+                                        'id': 16817,
+                                        'isDPWizardAvailable': False,
+                                        'mime_type': 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+                                        'name': 'Innovate Procurement Contract Template 2022.docx',
+                                        'name_multilingual': {...},
+                                        'size': 144365,
+                                        'sizeformatted': '141 KB',
+                                        'type': 144
+                                    },
+                                    {
+                                        ...
+                                    }
+                                ]
+                            }
+                        ]
+        """
+
+        request_url = (
+            self.config()["nodesUrlv2"]
+            + "/"
+            + str(parent_id)
+            + "/doctemplates?subtypes={144}&sidepanel_subtypes={144}"
+        )
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Get document templates for target location -> {} (parent); calling -> {}".format(
+                parent_id, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
+            response = requests.get(
+                request_url,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to get document templates for parent folder -> {}; status -> {}; error -> {}".format(
+                        parent_id,
+                        response.status_code,
+                        response.text,
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def createDocumentFromTemplate(
+        self,
+        template_id: int,
+        parent_id: int,
+        classification_id: int,
+        category_data: dict,
+        doc_name: str,
+        doc_desciption: str = "",
+    ):
+        """Create a document based on a document template
+
+        Args:
+            template_id (integer): node ID of the document template
+            parent_id (integer): node ID of the target location (parent)
+            classification_id (integer): node ID of the classification
+            category_data (dictionary): metadata / category data
+                                        Example: category ID = 12508
+                                        {
+                                            "12508": {
+                                                "12508_2": "Draft",         # Text drop-down
+                                                "12508_3": 8559,            # user ID
+                                                "12508_4": "2023-05-10",    # date
+                                                "12508_6": 7357,            # user ID
+                                                "12508_7": "2023-05-11",    # date
+                                                "12508_5": True,            # checkbox / bool
+                                                "12508_8": "EN",            # text drop-down
+                                                "12508_9": "MS Word",       # text drop-down
+                                            }
+                                        }
+            doc_name (string): name of the item
+            doc_description (string, optional): description of the item
+        """
+
+        createDocumentPostData = {
+            "template_id": template_id,
+            "parent_id": parent_id,
+            "name": doc_name,
+            "description": doc_desciption,
+            "type": 144,
+            "roles": {
+                "categories": category_data,
+                "classifications": {"create_id": [classification_id], "id": []},
+            },
+        }
+
+        request_url = self.config()["doctemplatesUrl"]
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Create document -> {} from template -> {} in target location -> {} (parent); calling -> {}".format(
+                doc_name, template_id, parent_id, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
+            response = requests.post(
+                request_url,
+                # this seems to only work with a "body" tag and is different form the documentation
+                # on developer.opentext.com
+                data={"body": json.dumps(createDocumentPostData)},
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to create document -> {}; status -> {}; error -> {}".format(
+                        doc_name,
+                        response.status_code,
+                        response.text,
+                    )
+                )
+                return None
+
+    # end method definition
+
     def getWebReportParameters(self, nickname: str):
         """Get parameters of a Web Report in Extended ECM. These are defined on the Web Report node
             (Properties --> Parameters)
 
         Args:
-            nickname (str): nickname of the Web Reports node.
-        Return:
+            nickname (string): nickname of the Web Reports node.
+        Returns:
             Response: list of Web Report parameters. Each list item is a dict describing the parameter.
             Structure of the list items:
             {
                 "type": "string",
                 "parm_name": "string",
                 "display_text": "string",
                 "prompt": true,
@@ -3984,16 +4519,15 @@
                 "default_value": null,
                 "description": "string",
                 "mandatory": true
             }
             None if the REST call has failed.
         """
 
-        request_url = self.config()["webReportsUrl"] + \
-            "/" + nickname + "/parameters"
+        request_url = self.config()["webReportsUrl"] + "/" + nickname + "/parameters"
         request_header = self.requestFormHeader()
 
         logger.info(
             "Retrieving parameters of Web Report with nickname -> {}; calling -> {}".format(
                 nickname, request_url
             )
         )
@@ -4001,45 +4535,43 @@
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 # Return the "data" element which is a list of dict items:
                 result_dict = self.parseRequestResponse(response)
-                logger.debug(
-                    "Web Report parameters result -> {}".format(result_dict))
+                logger.debug("Web Report parameters result -> {}".format(result_dict))
                 if not result_dict.get("data"):
                     return None
                 return result_dict["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve parameters of Web Report with nickname -> {}; status -> {}; error -> {}".format(
                         nickname,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def runWebReport(self, nickname: str, web_report_parameters: dict = {}):
+    def runWebReport(self, nickname: str, web_report_parameters: dict = {}) -> dict:
         """Run a Web Report that is identified by its nick name.
 
         Args:
-            nickname (str): nickname of the Web Reports node.
-            web_report_parameters (dict): Parameters of the Web Report (names + value pairs)
-        Return:
-            Response (json) or None if the Web Report execution has failed.
+            nickname (string): nickname of the Web Reports node.
+            web_report_parameters (dictionary): Parameters of the Web Report (names + value pairs)
+        Returns:
+            dictionary: Response of the run Web Report request or None if the Web Report execution has failed.
         """
 
         request_url = self.config()["webReportsUrl"] + "/" + nickname
         request_header = self.requestFormHeader()
 
         logger.info(
             "Running Web Report with nickname -> {}; calling -> {}".format(
@@ -4055,37 +4587,36 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to run web report with nickname -> {}; status -> {}; error -> {}".format(
                         nickname,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def installCSApplication(self, application_name: str):
+    def installCSApplication(self, application_name: str) -> dict:
         """Install a CS Application (based on WebReports)
 
         Args:
             application_name (string): name of the application (e.g. OTPOReports, OTRMReports, OTRMSecReports)
-        Return:
-            Response (json) or None if the installation of the CS Application has failed.
+        Returns:
+            dictionary: Response or None if the installation of the CS Application has failed.
         """
 
         installCSApplicationPostData = {"appName": application_name}
 
         request_url = self.config()["csApplicationsUrl"] + "/install"
         request_header = self.requestFormHeader()
 
@@ -4103,16 +4634,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to install CS Application -> {}; status -> {}; error -> {}".format(
                         application_name,
                         response.status_code,
@@ -4121,36 +4651,35 @@
                 )
                 return None
 
     # end method definition
 
     def assignItemToUserGroup(
         self, node_id: int, subject: str, instruction: str, assignees: list
-    ):
+    ) -> dict:
         """Assign an Extended ECM item to users and groups. This is a function used by
            Extended ECM for Government.
 
         Args:
             node_id (integer): node ID of the Extended ECM item (e.g. a workspace or a document)
             subject (string): title / subject of the assignment
             instructions (string): more detailed description or instructions for the assignment
             assignees (list): list of IDs of users or groups
-        Return:
-            Response (json) or None if the assignment has failed.
+        Returns:
+            dictionary: Response of the request or None if the assignment has failed.
         """
 
         assignmentPostData = {
             "subject": subject,
             "instruction": instruction,
             "assignees": assignees,
         }
 
         request_url = (
-            self.config()["nodesUrlv2"] + "/" +
-            str(node_id) + "/xgovassignments"
+            self.config()["nodesUrlv2"] + "/" + str(node_id) + "/xgovassignments"
         )
 
         request_header = self.requestFormHeader()
 
         logger.info(
             "Assign item with ID -> {} to assignees -> {} (subject -> {}); calling -> {}".format(
                 node_id, assignees, subject, request_url
@@ -4166,16 +4695,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign item with ID -> {} to assignees -> {} (subject -> {}); status -> {}; error -> {}".format(
                         node_id,
                         assignees,
@@ -4189,16 +4717,16 @@
     # end method definition
 
     def convertPermissionStringToPermissionValue(self, permissions: list) -> int:
         """Converts a list of permission names (strongs) to a bit-mask.
 
         Args:
             permissions (list): List of permission names - see conversion variable below.
-
-        Return: bit-encoded permission value (integer) 
+        Returns:
+            integer: bit-encoded permission value
         """
 
         conversion = {
             "see": 130,  # Bits 2 and 8
             "see_contents": 36865,  # Bit 17
             "modify": 65536,  # Bit 18
             "edit_attributes": 131072,  # Bit 19
@@ -4210,30 +4738,29 @@
             "edit_permissions": 16,  # Bit 5
         }
 
         permission_value = 0
 
         for permission in permissions:
             if not conversion.get(permission):
-                logger.error(
-                    "Illegal permission value -> {}".format(permission))
+                logger.error("Illegal permission value -> {}".format(permission))
                 return 0
             permission_value += conversion[permission]
 
         return permission_value
 
     # end method definition
 
     def convertPermissionValueToPermissionString(self, permission_value: int) -> list:
         """Converts a bit-encoded permission value to a list of permission names (strings).
 
         Args:
             permission_value (integer): bit-encoded permission value
-
-        Return: list of permission names
+        Returns:
+            list: list of permission names
         """
 
         conversion = {
             "see": 130,  # Bits 2 and 8
             "see_contents": 36865,  # Bit 17
             "modify": 65536,  # Bit 18
             "edit_attributes": 131072,  # Bit 19
@@ -4258,15 +4785,15 @@
     def assignPermission(
         self,
         node_id: int,
         assignee_type: str,
         assignee: int,
         permissions: list,
         apply_to: int = 0,
-    ):
+    ) -> dict:
         """Assign permissions for Extended ECM item to a user or group.
 
         Args:
             node_id (integer): node ID of the Extended ECM item
             assignee_type (string): this can be either "owner", "group" (for owner group),
                                     "public", or "custom" (assigned access)
             assignee (integer): ID of user or group ("right ID"). If 0 and assigneeType
@@ -4279,20 +4806,21 @@
                                 "edit_attributes"
                                 "add_items"
                                 "reserve"
                                 "add_major_version"
                                 "delete_versions"
                                 "delete"
                                 "edit_permissions"
-            apply_to (integer):  0 = this item
+            apply_to (integer, optional): elements to apply permissions to - potential values:
+                                 0 = this item (default)
                                  1 = sub-items
                                  2 = This item and sub-items
                                  3 = This item and immediate sub-items
-        Return:
-            Response (json) or None if the assignment of permissions has failed.
+        Returns:
+            dictionary: Response of the request or None if the assignment of permissions has failed.
         """
 
         if not assignee_type or not assignee_type in [
             "owner",
             "group",
             "public",
             "custom",
@@ -4351,16 +4879,15 @@
                     headers=request_header,
                     cookies=self.cookie(),
                 )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign permissions -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         permissions,
                         node_id,
@@ -4368,39 +4895,455 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
+    def getNodeCategories(self, node_id: int, metadata: bool = True):
+        """Get categories assigned to a node.
+
+        Args:
+            node_id (integer): ID of the node to get the categories for.
+            metadata (boolean, optional): expand the attribute definitions of the category. Default is True
+        Returns:
+            dictionary: category response or None if the call to the REST API fails.
+        """
+
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id) + "/categories"
+        if metadata:
+            request_url += "?metadata"
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Get categories of node with ID -> {}; calling -> {}".format(
+                node_id, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to get categories for node ID -> {}; status -> {}; error -> {}".format(
+                        node_id, response.status_code, response.text
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def getNodeCategory(self, node_id: int, category_id: int, metadata: bool = True):
+        """Get a specific category assigned to a node.
+
+        Args:
+            node_id (integer): ID of the node to get the categories for.
+            category_id (integer): ID of the category definition ID (in category volume)
+            metadata (boolean, optional): expand the attribute definitions of the category. Default is True
+        Returns:
+            dictionary: category response or None if the call to the REST API fails.
+        """
+
+        request_url = (
+            self.config()["nodesUrlv2"]
+            + "/"
+            + str(node_id)
+            + "/categories/"
+            + str(category_id)
+        )
+        if metadata:
+            request_url += "?metadata"
+        request_header = self.requestFormHeader()
+
+        logger.info(
+            "Get category with ID -> {} on node with ID -> {}; calling -> {}".format(
+                category_id, node_id, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to get category with ID -> {} for node ID -> {}; status -> {}; error -> {}".format(
+                        category_id, node_id, response.status_code, response.text
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def getNodeCategoryIds(self, node_id: int) -> list:
+        """Get list of all category definition IDs that are assign to the node.
+
+        Args:
+            node_id (integer): ID of the node to get the categories for.
+        Returns:
+            list: list of category IDs (all categories assigned to the node)
+        """
+
+        categories = self.getNodeCategories(node_id)
+        if not categories or not categories["results"]:
+            return None
+
+        category_id_list = []
+
+        for category in categories["results"]:
+            category_id_list += [
+                int(i) for i in category["metadata_order"]["categories"]
+            ]
+
+        return category_id_list
+
+    # end method definition
+
+    def getNodeCategoryDefinition(self, node_id: int, category_name: str):
+        """Get category definition (category id and attribute IDs and types)
+
+        Args:
+            node_id (integer): node to read the category definition from
+                               (e.g. a workspace template or a document template or a target folder)
+                               This should NOT be the category definition object!
+            category_name (string): name of the category
+        Returns:
+            integer: category ID
+            dictionary: keys are the attribute names. values are sub-dictionaries with the id and type of the attribute.
+                        Example:
+                        {
+                            'Status': {
+                                'id': '12532_2',
+                                'type': 'String'
+                            },
+                            'Legal Approval': {
+                                'id': '12532_3',
+                                'type': 'user'
+                            },
+                            ...
+                        }
+        """
+
+        response = self.getNodeCategories(node_id)
+        if response and response["results"]:
+            attribute_definitions = {}
+            for categories in response["results"]:
+                keys = categories["metadata"]["categories"].keys()
+                cat_id = next((key for key in keys if "_" not in key), -1)
+                cat_name = categories["metadata"]["categories"][cat_id]["name"]
+                if cat_name != category_name:
+                    cat_id = -1
+                    continue
+                for att_id in categories["metadata"]["categories"]:
+                    if not "_" in att_id:
+                        continue
+                    att_name = categories["metadata"]["categories"][att_id]["name"]
+                    if categories["metadata"]["categories"][att_id]["persona"]:
+                        att_type = categories["metadata"]["categories"][att_id][
+                            "persona"
+                        ]
+                    else:
+                        att_type = categories["metadata"]["categories"][att_id][
+                            "type_name"
+                        ]
+                    attribute_definitions[att_name] = {"id": att_id, "type": att_type}
+        return cat_id, attribute_definitions
+
+    def assignCategory(
+        self,
+        node_id: int,
+        category_id: list,
+        inheritance: bool = False,
+        apply_to_sub_items: bool = False,
+        apply_action: str = "add_upgrade",
+        add_version: bool = False,
+        clear_existing_categories: bool = False,
+    ):
+        """Assign a category to a node. Optionally turn on inheritance and apply
+           category to sub-items (if node_id is a container / folder / workspace).
+           If the category is already assigned to the node this method will
+           throw an error.
+
+        Args:
+            node_id (integer): node ID to apply the category to
+            category_id (list): ID of the category definition object
+            inheritance (boolean): turn on inheritance for the category
+                                   (this makes only sense if the node is a container like a folder or workspace)
+            apply_to_sub_items (boolean, optional): if True the category is applied to
+                                                    the item and all its sub-items
+                                                    if False the category is only applied
+                                                    to the item
+            apply_action (string, optional): supported values are "add", "add_upgrade", "upgrade", "replace", "delete", "none", None
+            add_version (boolean, optional): if a document version should be added for the category change (default = False)
+            clear_existing_categories (boolean, optional): whether or not existing (other) categories should be removed (default = False)
+        Returns:
+            boolean: True = success, False = error
+        """
+
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id) + "/categories"
+        request_header = self.requestFormHeader()
+
+        #
+        # 1. Assign Category to Node if not yet assigned:
+        #
+
+        existing_category_ids = self.getNodeCategoryIds(node_id)
+        if not category_id in existing_category_ids:
+            logger.info(
+                "Category with ID -> {} is not yet assigned to node ID -> {}. Assigning it now...".format(
+                    category_id, node_id
+                )
+            )
+            categoryPostData = {
+                "category_id": category_id,
+            }
+
+            logger.info(
+                "Assign category with ID -> {} to item with ID -> {}; calling -> {}".format(
+                    category_id, node_id, request_url
+                )
+            )
+
+            retries = 0
+            while True:
+                response = requests.post(
+                    request_url,
+                    data=categoryPostData,
+                    headers=request_header,
+                    cookies=self.cookie(),
+                )
+                if response.ok:
+                    break
+                # Check if Session has expired - then re-authenticate and try once more
+                elif response.status_code == 401 and retries == 0:
+                    logger.warning("Session has expired - try to re-authenticate...")
+                    self.authenticate(True)
+                    retries += 1
+                else:
+                    logger.error(
+                        "Failed to assign category with ID -> {} to node with ID -> {}; status -> {}; error -> {}".format(
+                            category_id, node_id, response.status_code, response.text
+                        )
+                    )
+                    return False
+
+        #
+        # 2. Set Inheritance
+        #
+
+        request_url_inheritance = request_url + "/" + str(category_id) + "/inheritance"
+
+        retries = 0
+        while True:
+            if inheritance:
+                # Enable inheritance
+                response = requests.post(
+                    request_url_inheritance,
+                    headers=request_header,
+                    cookies=self.cookie(),
+                )
+            else:
+                # Disable inheritance
+                response = requests.delete(
+                    request_url_inheritance,
+                    headers=request_header,
+                    cookies=self.cookie(),
+                )
+            if response.ok:
+                break
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to set inheritance for category with ID -> {} on node with ID -> {}; status -> {}; error -> {}".format(
+                        category_id, node_id, response.status_code, response.text
+                    )
+                )
+                return False
+
+        #
+        # 3. Apply to sub-items
+        #
+
+        if apply_to_sub_items:
+            request_url_apply_sub_items = request_url + "/apply"
+
+            categoryPostData = {
+                "categories": [{"id": category_id, "action": apply_action}],
+                "add_version": add_version,
+                "clear_existing_categories": clear_existing_categories,
+            }
+
+            retries = 0
+            while True:
+                # we need to wrap the body of this POST call into a "body"
+                # tag. This is documented worngly on developer.opentext.com
+                response = requests.post(
+                    request_url_apply_sub_items,
+                    data={"body": json.dumps(categoryPostData)},
+                    headers=request_header,
+                    cookies=self.cookie(),
+                )
+                if response.ok:
+                    break
+                # Check if Session has expired - then re-authenticate and try once more
+                elif response.status_code == 401 and retries == 0:
+                    logger.warning("Session has expired - try to re-authenticate...")
+                    self.authenticate(True)
+                    retries += 1
+                else:
+                    logger.error(
+                        "Failed to apply category with ID -> {} to sub-items of node with ID -> {}; status -> {}; error -> {}".format(
+                            category_id, node_id, response.status_code, response.text
+                        )
+                    )
+                    return False
+        return True
+
+    # end method definition
+
+    def setCategoryValue(
+        self,
+        node_id: int,
+        value,
+        category_id: int,
+        attribute_id: int,
+        set_id: int = 0,
+        set_row: int = 1,
+    ):
+        """Set a value to a specific attribute in a category. Categories and have sets (groupings), multi-line sets (matrix),
+           and multi-value attributes (list of values). This method supports all variants.
+
+        Args:
+            node_id (integer): ID of the node
+            value (multi-typed): value to be set - can be string or list of strings (for multi-value attributes)
+            category_id (integer):ID of the category object
+            attribute_id (integer): ID of the attribute
+            set_id (integer, optional): ID of the set. Defaults to 0.
+            set_row (integer, optional): Row of . Defaults to 1.
+
+        Returns:
+            dictionary: REST API response or None if the call fails
+        """
+
+        request_url = (
+            self.config()["nodesUrlv2"]
+            + "/"
+            + str(node_id)
+            + "/categories/"
+            + str(category_id)
+        )
+        request_header = self.requestFormHeader()
+
+        if set_id:
+            logger.info(
+                "Assign value -> {} to category -> {}, set -> {}, row -> {}, attribute -> {} on node -> {}; calling -> {}".format(
+                    value,
+                    category_id,
+                    set_id,
+                    set_row,
+                    attribute_id,
+                    node_id,
+                    request_url,
+                )
+            )
+            categoryPutData = {
+                "category_id": category_id,
+                "{}_{}_{}_{}".format(category_id, set_id, set_row, attribute_id): value,
+            }
+        else:
+            logger.info(
+                "Assign value -> {} to category -> {}, attribute -> {} on node -> {}; calling -> {}".format(
+                    value, category_id, attribute_id, node_id, request_url
+                )
+            )
+            categoryPutData = {
+                "category_id": category_id,
+                "{}_{}".format(category_id, attribute_id): value,
+            }
+
+        retries = 0
+        while True:
+            response = requests.put(
+                request_url,
+                data=categoryPutData,
+                headers=request_header,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to set value -> {} for category -> {}, attribute -> {} on node ID -> {}; status -> {}; error -> {}".format(
+                        value,
+                        category_id,
+                        attribute_id,
+                        node_id,
+                        response.status_code,
+                        response.text,
+                    )
+                )
+                return False
+
+    # end method definition
+
     def assignClassification(
         self, node_id: int, classifications: list, apply_to_sub_items: bool = False
-    ):
+    ) -> dict:
         """Assign one or multiple classifications to an Extended ECM item
         Args:
             node_id (integer): node ID of the Extended ECM item
             classifications (list): list of classification item IDs
-            apply_to_sub_items (boolean): if True the classification is applied to the item and all its sub-items
-                                          if False the classification is only applied to the item
-        Return:
-            Response (json) or None if the assignment of the classification has failed.
+            apply_to_sub_items (boolean, optional): if True the classification is applied to
+                                                    the item and all its sub-items
+                                                    if False the classification is only applied
+                                                    to the item
+        Returns:
+            dictionary: Response of the request or None if the assignment of the classification has failed.
         """
 
         # the REST API expects a list of dict elements with "id" and the actual IDs
         classification_list = []
         for classification in classifications:
             classification_list.append({"id": classification})
 
         classificationPostData = {
             "class_id": classification_list,
             "apply_to_sub_items": apply_to_sub_items,
         }
 
-        request_url = self.config()["nodesUrl"] + \
-            "/" + str(node_id) + "/classifications"
+        request_url = (
+            self.config()["nodesUrl"] + "/" + str(node_id) + "/classifications"
+        )
 
         request_header = self.requestFormHeader()
 
         logger.info(
             "Assign classifications with IDs -> {} to item with ID -> {}; calling -> {}".format(
                 classifications, node_id, request_url
             )
@@ -4414,16 +5357,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign classifications with IDs -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         classifications,
                         node_id,
@@ -4433,33 +5375,34 @@
                 )
                 return None
 
     # end method definition
 
     def assignRMClassification(
         self, node_id: int, rm_classification: int, apply_to_sub_items: bool = False
-    ):
+    ) -> dict:
         """Assign a RM classification to an Extended ECM item
         Args:
             node_id (integer): node ID of the Extended ECM item
             rm_classification (integer): Records Management classification ID
-            apply_to_sub_items (boolean): if True the RM classification is applied to the item and all its sub-items
-                                          if False the RM classification is only applied to the item
-        Return:
-            Response (json) or None if the assignment of the RM classification has failed.
+            apply_to_sub_items (boolean, optional): if True the RM classification is applied to
+                                                    the item and all its sub-items
+                                                    if False the RM classification is only applied
+                                                    to the item
+        Returns:
+            dictionary: Response of the request or None if the assignment of the RM classification has failed.
         """
 
         rmClassificationPostData = {
             "class_id": rm_classification,
             "apply_to_sub_items": apply_to_sub_items,
         }
 
         request_url = (
-            self.config()["nodesUrl"] + "/" +
-            str(node_id) + "/rmclassifications"
+            self.config()["nodesUrl"] + "/" + str(node_id) + "/rmclassifications"
         )
 
         request_header = self.requestFormHeader()
 
         logger.info(
             "Assign RM classifications with ID -> {} to item with ID -> {}; calling -> {}".format(
                 rm_classification, node_id, request_url
@@ -4474,16 +5417,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign RM classifications with ID -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         rm_classification,
                         node_id,
@@ -4491,20 +5433,20 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def registerWorkspaceTemplate(self, node_id: int):
+    def registerWorkspaceTemplate(self, node_id: int) -> dict:
         """Register a workspace template as project template for Extended ECM for Engineering
         Args:
             node_id (integer): node ID of the Extended ECM workspace template
-        Return:
-            Response (json) or None if the registration of the workspace template has failed.
+        Returns:
+            dictionary: Response of request or None if the registration of the workspace template has failed.
         """
 
         registrationPostData = {"ids": "{{ {} }}".format(node_id)}
 
         request_url = self.config()["xEngProjectTemplateUrl"]
 
         request_header = self.requestFormHeader()
@@ -4523,16 +5465,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to register Workspace Template with ID -> {}; status -> {}; error -> {}".format(
                         node_id,
                         response.status_code,
@@ -4543,17 +5484,17 @@
 
     # end method definition
 
     def getRecordsManagementRSIs(self, limit: int = 100):
         """Get all Records management RSIs togther with their RSI Schedules.
 
         Args:
-            limit (integer): max elements to return
-        Return:
-            List of Records Management RSIs or None if the request fails.
+            limit (integer, optional): max elements to return (default = 100)
+        Returns:
+            list: list of Records Management RSIs or None if the request fails.
             Each RSI list element is a dict with this structure:
             {
                 "RSIID": 0,
                 "RSI": "string",
                 "Title": "string",
                 "Subject": "string",
                 "Description": "string",
@@ -4591,30 +5532,28 @@
             }
         """
 
         request_url = self.config()["rsisUrl"] + "?limit=" + str(limit)
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get list of Records Management RSIs; calling -> {}".format(
-                request_url)
+            "Get list of Records Management RSIs; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 rsi_dict = self.parseRequestResponse(response)
                 return rsi_dict["results"]["data"]["rsis"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management RSIs; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
@@ -4624,39 +5563,38 @@
     # end method definition
 
     def getRecordsManagementCodes(self):
         """Get Records Management Codes. These are the most basic data types of
            the Records Management configuration and required to create RSIs and
            other higher-level Records Management configurations
 
-        Args: None
-        Return:
+        Args:
+            None
+        Returns:
             RSI data (json) or None if the request fails.
         """
 
         request_url = self.config()["recordsManagementUrlv2"] + "/rmcodes"
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get list of Records Management codes; calling -> {}".format(
-                request_url)
+            "Get list of Records Management codes; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=request_header, cookies=self.cookie()
             )
             if response.ok:
                 rm_codes_dict = self.parseRequestResponse(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management codes; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
@@ -4669,41 +5607,41 @@
     def updateRecordsManagementCodes(self, rm_codes: dict):
         """Update Records Management Codes. These are the most basic data types of
            the Records Management configuration and required to create RSIs and
            other higher-level Records Management configurations
 
         Args:
             rm_codes: dict with the updated codes
-        Return:
+        Returns:
             RSI data (json) or None if the request fails.
         """
 
         updateRMCodesPostData = {}
 
         request_url = self.config()["recordsManagementUrl"] + "/rmcodes"
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Update Records Management codes; calling -> {}".format(request_url))
+            "Update Records Management codes; calling -> {}".format(request_url)
+        )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
                 headers=request_header,
                 data=updateRMCodesPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 rm_codes_dict = self.parseRequestResponse(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update Records Management codes; status -> {}; error -> {}".format(
                         response.status_code, response.text
                     )
@@ -4717,27 +5655,27 @@
         name: str,
         status: str,
         status_date: str,
         description: str,
         subject: str,
         title: str,
         dispcontrol: bool,
-    ):
+    ) -> dict:
         """Create a new Records Management RSI.
 
         Args:
             name (string): name of the RSI
             status (string): status of the RSI
             status_date (string): statusDate of the RSI YYYY-MM-DDTHH:mm:ss
             description (string): description of the RSI
             subject (string): status of the RSI
             title (string): status of the RSI
             dispcontrol (boolean): status of the RSI
-        Return:
-            RSI data (json) or None if the request fails.
+        Returns:
+            dictionary: RSI data or None if the request fails.
         """
 
         if statusDate == "":
             now = datetime.now()
             statusDate = now.strftime("%Y-%m-%dT%H:%M:%S")
 
         createRSIPostData = {
@@ -4768,16 +5706,15 @@
                 data=createRSIPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management RSI -> {}; status -> {}; error -> {}".format(
                         name,
                         response.status_code,
@@ -4813,47 +5750,47 @@
         action_code: int = 0,
         description: str = "",
         new_status: str = "",
         min_num_versions_to_keep: int = 1,
         purge_superseded: bool = False,
         purge_majors: bool = False,
         mark_official_rendition: bool = False,
-    ):
+    ) -> dict:
         """Create a new Records Management RSI Schedule for an existing RSI.
 
         Args:
             rsi_id (integer): ID of an existing RSI the schedule should be created for
             object_type (string): either "LIV" - Classified Objects (default) or "LRM" - RM Classifications
-            stage: retention stage - this is the key parameter to define multiple stages (stages are basically schedules)
-            event_type: 1 Calculated Date, 2 Calendar Calculation, 3 Event Based, 4 Fixed Date, 5 Permanent
-            rule_code: rule code - this value must be defined upfront
-            rule_comment: comment for the rule
-            date_to_use: 91 Create Date, 92 Reserved Data, 93 Modification Date, 94 Status Date, 95 Records Date
-            retention_years: years to wait before disposition
-            retention_months: month to wait before disposition
-            retention_days: days to wait before disposition
+            stage (string): retention stage - this is the key parameter to define multiple stages (stages are basically schedules)
+            event_type (integer): 1 Calculated Date, 2 Calendar Calculation, 3 Event Based, 4 Fixed Date, 5 Permanent
+            rule_code (string): rule code - this value must be defined upfront
+            rule_comment (string): comment for the rule
+            date_to_use (integer): 91 Create Date, 92 Reserved Data, 93 Modification Date, 94 Status Date, 95 Records Date
+            retention_years (integer): years to wait before disposition
+            retention_months (integer): month to wait before disposition
+            retention_days (integer): days to wait before disposition
             category_id (integer): ID of the category
             attribute_id (integer): ID of the category attribute
             year_end_month (integer): month the year ends (normally 12)
             year_end_day (integer): day the year ends (normally 31)
             retention_intervals (integer): retention intervals
             fixed_retention (boolean): fixedRetention
-            maximum_retention: maximumRetention
+            maximum_retention (boolean): maximumRetention
             fixed_date(string): fixed date format : YYYY-MM-DDTHH:mm:ss
             event_condition (string): eventCondition
-            disposition: disposition
+            disposition (string): disposition
             action_code (integer): 0 None, 1 Change Status, 7 Close, 8 Finalize Record, 9 Mark Official, 10 Export, 11 Update Storage Provider, 12 Delete Electronic Format, 15 Purge Versions, 16 Make Rendition, 32 Destroy
             description (string): description
             new_status (string): new status
             min_num_versions_to_keep (integer): minimum document versions to keep
             purge_superseded (boolean): purge superseded
             purge_majors (boolean): purge majors
             mark_official_rendition (boolean): mark official rendition
-        Return:
-            RSI Schedule data (json) or None if the request fails.
+        Returns:
+            dictionary: RSI Schedule data or None if the request fails.
         """
 
         if fixedDate == "":
             now = datetime.now()
             fixedDate = now.strftime("%Y-%m-%dT%H:%M:%S")
 
         createRSISchedulePostData = {
@@ -4881,16 +5818,15 @@
             "newStatus": new_status,
             "minNumVersionsToKeep": min_num_versions_to_keep,
             "purgeSuperseded": purge_superseded,
             "purgeMajors": purge_majors,
             "markOfficialRendition": mark_official_rendition,
         }
 
-        request_url = self.config()["rsiSchedulesUrl"] + \
-            "/" + str(rsi_id) + "/stages"
+        request_url = self.config()["rsiSchedulesUrl"] + "/" + str(rsi_id) + "/stages"
 
         request_header = self.requestFormHeader()
 
         logger.info(
             "Create Records Management RSI Schedule -> {} for RSI -> {}; calling -> {}".format(
                 stage, rsi_id, request_url
             )
@@ -4904,16 +5840,15 @@
                 data=createRSISchedulePostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management RSI Schedule -> {}; status -> {}; error -> {}".format(
                         stage,
                         response.status_code,
@@ -4929,27 +5864,27 @@
         hold_type: str,
         name: str,
         comment: str,
         alternate_id: str = "",
         parent_id: int = 0,
         date_applied: str = "",
         date_to_remove: str = "",
-    ):
+    ) -> dict:
         """Create a new Records Management Hold.
 
         Args:
-            parent_id (integer): ID of the parent node. If no parent is 0 the item will be created right under "Hold Management" (top level item)
-            type (string): type of the Hold
+            hold_type (string): type of the Hold
             name (string): name of the RSI
             comment (string): comment
             alternate_id (string): alternate hold ID
-            date_applied (string): create date of the Hold in this format: YYYY-MM-DDTHH:mm:ss
-            date_to_remove (string): suspend date of the Hold in this format: YYYY-MM-DDTHH:mm:ss
-        Return:
-            Hold data (json) or None if the request fails. The JSon structure is this: {'holdID': <ID>}
+            parent_id (integer, optional): ID of the parent node. If parent_id is 0 the item will be created right under "Hold Management" (top level item)
+            date_applied (string, optional): create date of the Hold in this format: YYYY-MM-DDTHH:mm:ss
+            date_to_remove (string, optional): suspend date of the Hold in this format: YYYY-MM-DDTHH:mm:ss
+        Returns:
+            dictionary: Hold data or None if the request fails. The dict structure is this: {'holdID': <ID>}
         """
 
         if date_applied == "":
             now = datetime.now()
             date_applied = now.strftime("%Y-%m-%dT%H:%M:%S")
 
         createHoldPostData = {
@@ -4982,37 +5917,38 @@
                 data=createHoldPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management Hold -> {}; status -> {}; error -> {}".format(
                         name,
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def getRecordsManagementHolds(self):
+    def getRecordsManagementHolds(self) -> dict:
         """Get a list of all Records Management Holds in the system. Even though there are folders
-           in the holds management area in RM these are not real folders - they cannot be retrieved
-           with getNodeByParentAndName() thus we need this method to get them all.
+        in the holds management area in RM these are not real folders - they cannot be retrieved
+        with getNodeByParentAndName() thus we need this method to get them all.
 
-           Args: None
-           Return: response with list of holds:
+        Args:
+            None
+        Returns:
+            dictionary: Response with list of holds:
             "results": {
                 "data": {
                     "holds": [
                         {
                             "HoldID": 0,
                             "HoldName": "string",
                             "ActiveHold": 0,
@@ -5036,51 +5972,49 @@
         """
 
         request_url = self.config()["holdsUrlv2"]
 
         request_header = self.requestFormHeader()
 
         logger.info(
-            "Get list of Records Management Holds; calling -> {}".format(
-                request_url
-            )
+            "Get list of Records Management Holds; calling -> {}".format(request_url)
         )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url,
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management Holds; status -> {}; error -> {}".format(
                         response.status_code,
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def importRecordsManagementSettings(self, file_path: str):
+    def importRecordsManagementSettings(self, file_path: str) -> bool:
         """Import Records Management settings from a file that is uploaded from the python pod
+
         Args:
             file_path (string): path + filename of config file in Python container filesystem
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["recordsManagementUrl"] + "/importSettings"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5109,16 +6043,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management Settings from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
@@ -5127,22 +6060,22 @@
                 )
                 return False
 
     # end method definition
 
     def importRecordsManagementCodes(
         self, file_path: str, update_existing_codes: bool = True
-    ):
+    ) -> bool:
         """Import RM Codes from a file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of settings file in Python container filesystem
             update_existing_codes (boolean): Flag that controls whether existing table maintenance codes
                                              should be updated.
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["recordsManagementUrl"] + "/importCodes"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5174,16 +6107,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
@@ -5195,22 +6127,22 @@
     # end method definition
 
     def importRecordsManagementRSIs(
         self,
         file_path: str,
         update_existing_rsis: bool = True,
         delete_schedules: bool = False,
-    ):
+    ) -> bool:
         """Import RM RSIs from a config file that is uploaded from the Python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
-            update_existing_rsis (boolean): whether or not existing RSIs should be updated (or ignored)
-            delete_schedules (boolean): whether RSI Schedules should be deleted
-        Return:
-            True if if the REST call succeeds or False otherwise.
+            update_existing_rsis (boolean, optional): whether or not existing RSIs should be updated (or ignored)
+            delete_schedules (boolean, optional): whether RSI Schedules should be deleted
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["recordsManagementUrl"] + "/importRSIs"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5245,36 +6177,35 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management RSIs from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importPhysicalObjectsSettings(self, file_path: str):
+    def importPhysicalObjectsSettings(self, file_path: str) -> bool:
         """Import Physical Objects settings from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["physicalObjectsUrl"] + "/importSettings"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5303,16 +6234,15 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects settings from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
@@ -5321,21 +6251,21 @@
                 )
                 return False
 
     # end method definition
 
     def importPhysicalObjectsCodes(
         self, file_path: str, update_existing_codes: bool = True
-    ):
+    ) -> bool:
         """Import Physical Objects codes from a config file that is uploaded from the Python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             update_existing_codes (boolean): whether or not existing codes should be updated (default = True)
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["physicalObjectsUrl"] + "/importCodes"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5367,36 +6297,35 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importPhysicalObjectsLocators(self, file_path: str):
+    def importPhysicalObjectsLocators(self, file_path: str) -> bool:
         """Import Physical Objects locators from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["physicalObjectsUrl"] + "/importLocators"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5425,37 +6354,38 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects Locators from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def importSecurityClearanceCodes(self, file_path: str, include_users: bool = False):
+    def importSecurityClearanceCodes(
+        self, file_path: str, include_users: bool = False
+    ) -> bool:
         """Import Security Clearance codes from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             include_users (boolean): defines if users should be included or not
-        Return:
-            True if if the REST call succeeds or False otherwise.
+        Returns:
+            boolean: True if if the REST call succeeds or False otherwise.
         """
 
         request_url = self.config()["securityClearancesUrl"] + "/importCodes"
 
         request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
@@ -5487,38 +6417,39 @@
                 headers=request_header,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Security Clearance Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
                         response.status_code,
                         response.text,
                     )
                 )
                 return False
 
     # end method definition
 
-    def assignUserSecurityClearance(self, user_id: int, security_clearance: int):
+    def assignUserSecurityClearance(
+        self, user_id: int, security_clearance: int
+    ) -> dict:
         """Assign a Security Clearance level to an Extended ECM user
 
         Args:
-            user_id: ID of the user
-            security_clearance: security clearance level to be set
-        Return:
-            REST response or None if the REST call fails.
+            user_id (integer): ID of the user
+            security_clearance (integer): security clearance level to be set
+        Returns:
+            dictionary: REST response or None if the REST call fails.
         """
 
         assignUserSecurityClearancePostData = {
             "securityLevel": security_clearance,
         }
 
         request_url = self.config()[
@@ -5540,16 +6471,15 @@
                 data=assignUserSecurityClearancePostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign security clearance -> {} to user -> {}; status -> {}; error -> {}".format(
                         user_id,
                         security_clearance,
@@ -5557,23 +6487,24 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def assignUserSupplementalMarkings(self, user_id: int, supplemental_markings: list):
+    def assignUserSupplementalMarkings(
+        self, user_id: int, supplemental_markings: list
+    ) -> dict:
         """Assign a list of Supplemental Markings to a user
 
-
         Args:
             user_id (integer): ID of the user
             supplemental_markings (list of strings): list of Supplemental Markings to be set
-        Return:
-            REST response or None if the REST call fails.
+        Returns:
+            dictionary: REST response or None if the REST call fails.
         """
 
         assignUserSupplementalMarkingsPostData = {
             "suppMarks": supplemental_markings,
         }
 
         request_url = self.config()[
@@ -5595,16 +6526,15 @@
                 data=assignUserSupplementalMarkingsPostData,
                 cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
-                logger.warning(
-                    "Session has expired - try to re-authenticate...")
+                logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign supplemental markings -> {} to user -> {}; status -> {}; error -> {}".format(
                         user_id,
                         supplemental_markings,
@@ -5612,38 +6542,61 @@
                         response.text,
                     )
                 )
                 return None
 
     # end method definition
 
-    def volumeTranslator(self, current_node_id: int, translator: object, languages: list):
-
+    def volumeTranslator(
+        self, current_node_id: int, translator: object, languages: list
+    ):
         # Get current node based on the ID:
         current_node = self.getNode(current_node_id)
         current_node_id = self.getResultValue(current_node, "id")
 
         name = self.getResultValue(current_node, "name")
         description = self.getResultValue(current_node, "description")
         names_multilingual = self.getResultValue(current_node, "name_multilingual")
-        descriptions_multilingual = self.getResultValue(current_node, "description_multilingual")
+        descriptions_multilingual = self.getResultValue(
+            current_node, "description_multilingual"
+        )
 
         for language in languages:
             if language == "en":
                 continue
             # Does the language not exist as metadata language or is it already translated?
             # Then we skip this language:
-            if language in names_multilingual and names_multilingual["en"] and not names_multilingual[language]:
-                names_multilingual[language] = translator.translate("en", language, names_multilingual["en"])
-            if language in descriptions_multilingual and descriptions_multilingual["en"] and not descriptions_multilingual[language]:
-                descriptions_multilingual[language] = translator.translate("en", language, descriptions_multilingual["en"])
+            if (
+                language in names_multilingual
+                and names_multilingual["en"]
+                and not names_multilingual[language]
+            ):
+                names_multilingual[language] = translator.translate(
+                    "en", language, names_multilingual["en"]
+                )
+            if (
+                language in descriptions_multilingual
+                and descriptions_multilingual["en"]
+                and not descriptions_multilingual[language]
+            ):
+                descriptions_multilingual[language] = translator.translate(
+                    "en", language, descriptions_multilingual["en"]
+                )
 
         # Rename node multi-lingual:
-        response = self.renameNode(current_node_id, name, description, names_multilingual, descriptions_multilingual)
+        response = self.renameNode(
+            current_node_id,
+            name,
+            description,
+            names_multilingual,
+            descriptions_multilingual,
+        )
 
         # Get children nodes of the current node:
         results = self.getSubnodes(current_node_id, limit=200)["results"]
 
         for result in results:
-            self.volumeTranslator(result["data"]["properties"]["id"], translator, languages)
+            self.volumeTranslator(
+                result["data"]["properties"]["id"], translator, languages
+            )
 
     # end method definition
```

### Comparing `pyxecm-0.0.16/pyxecm/otds.py` & `pyxecm-0.0.17/pyxecm/otds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 OTDS Module to implement functions to read / write OTDS objects
-such as Ressources, Users, Groups, Licenses, Trusted Sites, ...
+such as Ressources, Users, Groups, Licenses, Trusted Sites, OAuth Clients, ...
 
 Important: userIDs consists of login name + "@" + partition name 
 
 Class: OTDS
 Methods:
 
 __init__ : class initializer
@@ -12,70 +12,71 @@
 cookie : returns cookie information
 credentials: returns set of username and password
 
 baseUrl : returns OTDS base URL
 restUrl : returns OTDS REST base URL
 credentialUrl : returns the OTDS Credentials REST URL
 authHandlerUrl : returns the OTDS Authentication Handler REST URL
-partitionUrl : returns OTDS Aartition REST URL
+partitionUrl : returns OTDS Partition REST URL
 accessRoleUrl : returns OTDS Access Role REST URL
 oauthClientUrl : returns OTDS OAuth Client REST URL
 resourceUrl : returns OTDS Resource REST URL
 licenseUrl : returns OTDS License REST URL
 tokenUrl : returns OTDS Token REST URL
 usersUrl : returns OTDS Users REST URL
 groupsUrl : returns OTDS Groups REST URL
 systemConfigUrl : returns OTDS System Config REST URL
 
 authenticate : authenticates at OTDS server
 
-addLicenseToResource : adds (or updates) a product license to OTDS
-getLicensesForResource : get list of licenses for a resource
-deleteLicenseFromResource : deletes a license from a resource
-assignUserToLicense : assign a user to a license for a resource
-
-addPartition : add an OTDS partition
-getPartition : get a partition with a specific name
-addUser : add a user to a partion
-getUser : get a user with a specific user ID (= login name @ partition)
-updateUser : update attributes of on OTDS user
-deleteUser : delete a user with a specific ID in a specific partition
-resetUserPassword : reset a password of a specific user ID
-addGroup: add an OTDS group
-getGroup: get a OTDS group by its name
-addUserToGroup : add an OTDS user to a OTDS group
-addGroupToParentGroup : add on OTDS group to a parent group
-
-addResource : add a new resource to OTDS
-getResource : get an OTDS resource with a specific name
-activateResource : activate an OTDS resource
-
-getAccessRoles : get all OTDS Access Roles
-getAccessRole: get an OTDS Access Role with a specific name
-addPartitionToAccessRole : add an OTDS Partition to to an OTDS Access Role
-addUserToAccessRole : add an OTDS user to to an OTDS Access Role
-addGroupToAccessRole : add an OTDS group to to an OTDS Access Role
-updateAccessRoleAttributes: update attributes of an existing access role
-
-addSystemAttribute : add an OTDS System Attribute
-
-getTrustedSites : get OTDS Trusted Sites
-addTrustedSite : add a new trusted site to OTDS
-
-addOauthClient : add a new OAuth client to OTDS
-getOauthClient : get an OAuth client with a specific client ID
-updateOauthClient : update an OAuth client
-addOauthClientsToAccessRole : add an OTDS OAuth Client to an OTDS Access Role
-getAccessToken : get an OTDS Access Token
-
-addAuthHandlerSAML: add an authentication handler for SAML (e.g. for SuccessFactors)
-addAuthHandlerSAP: add an authentication handler for SAP
-addAuthHandlerOAuth: add an authentication handler for OAuth (used for Salesforce)
+addLicenseToResource : Add (or update) a product license to OTDS
+getLicensesForResource : Get list of licenses for a resource
+deleteLicenseFromResource : Delete a license from a resource
+assignUserToLicense : Assign an OTDS user to a product license (feature) in OTDS.
+assignPartitionToLicense: Assign an OTDS user partition to a license (feature) in OTDS.
+
+addPartition : Add an OTDS partition
+getPartition : Get a partition with a specific name
+addUser : Add a user to a partion
+getUser : Get a user with a specific user ID (= login name @ partition)
+updateUser : Update attributes of on OTDS user
+deleteUser : Delete a user with a specific ID in a specific partition
+resetUserPassword : Reset a password of a specific user ID
+addGroup: Add an OTDS group
+getGroup: Get a OTDS group by its name
+addUserToGroup : Add an OTDS user to a OTDS group
+addGroupToParentGroup : Add on OTDS group to a parent group
+
+addResource : Add a new resource to OTDS
+getResource : Get an OTDS resource with a specific name
+activateResource : Activate an OTDS resource
+
+getAccessRoles : Get all OTDS Access Roles
+getAccessRole: Get an OTDS Access Role with a specific name
+addPartitionToAccessRole : Add an OTDS Partition to to an OTDS Access Role
+addUserToAccessRole : Add an OTDS user to to an OTDS Access Role
+addGroupToAccessRole : Add an OTDS group to to an OTDS Access Role
+updateAccessRoleAttributes: Update attributes of an existing access role
+
+addSystemAttribute : Add an OTDS System Attribute
+
+getTrustedSites : Get OTDS Trusted Sites
+addTrustedSite : Add a new trusted site to OTDS
+
+addOauthClient : Add a new OAuth client to OTDS
+getOauthClient : Get an OAuth client with a specific client ID
+updateOauthClient : Update an OAuth client
+addOauthClientsToAccessRole : Add an OTDS OAuth Client to an OTDS Access Role
+getAccessToken : Get an OTDS Access Token
+
+addAuthHandlerSAML: Add an authentication handler for SAML (e.g. for SuccessFactors)
+addAuthHandlerSAP: Add an authentication handler for SAP
+addAuthHandlerOAuth: Add an authentication handler for OAuth (used for Salesforce)
 
-consolidate: consolidate an OTDS resource
+consolidate: Consolidate an OTDS resource
 impersonateResource: Configure impersonation for an OTDS resource
 impersonateOauth: Configure impersonation for an OTDS OAuth Client
 
 """
 
 __author__ = "Dr. Marc Diefenbruch"
 __copyright__ = "Copyright 2023, OpenText"
@@ -236,16 +237,16 @@
         """Converts the request response to a Python dict in a safe way
            that also handles exceptions.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
             additional_error_message (string): print a custom error message
             show_error (boolean): if True log an error, if False log a warning
-
-        Return: a python dict object or null in case of an error
+        Returns:
+            dictionary: response dictionary or None in case of an error
         """
 
         if not response_object:
             return None
 
         try:
             dict_object = json.loads(response_object.text)
@@ -262,30 +263,31 @@
                 logger.warning(message)
             return None
         else:
             return dict_object
 
     # end method definition
 
-    def authenticate(self, revalidate: bool = False):
+    def authenticate(self, revalidate: bool = False) -> dict:
         """Authenticate at Directory Services and retrieve OTCS Ticket.
 
         Args:
-            revalidate (bool): determine if a re-athentication is enforced
-                               (e.g. if session has timed out with 401 error)
-        Return: Cookie information. Also stores cookie information in self._cookie
+            revalidate (boolean, optional): determine if a re-athentication is enforced
+                                            (e.g. if session has timed out with 401 error)
+        Returns:
+            dictionary: Cookie information. Also stores cookie information in self._cookie
         """
 
         # Already authenticated and session still valid?
         if self._cookie and not revalidate:
             return self._cookie
 
         otds_ticket = "NotSet"
 
-        logger.info("Requesting OTDS ticket from {}".format(self.credentialUrl()))
+        logger.info("Requesting OTDS ticket from -> {}".format(self.credentialUrl()))
 
         response = None
         try:
             response = requests.post(
                 self.credentialUrl(), json=self.credentials(), headers=requestHeaders
             )
         except Exception as e:
@@ -300,17 +302,15 @@
             if not authenticate_dict:
                 return None
             else:
                 otds_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otds_ticket))
         else:
             logger.error(
-                "Failed to request an OTDS ticket; error -> {}".format(
-                    response.text
-                )
+                "Failed to request an OTDS ticket; error -> {}".format(response.text)
             )
             return None
 
         self._cookie = {"OTDSTicket": otds_ticket}
         return self._cookie
 
     # end method definition
@@ -318,24 +318,25 @@
     def addLicenseToResource(
         self,
         path_to_license_file: str,
         product_name: str,
         product_description: str,
         resource_id: str,
         update: bool = True,
-    ):
-        """Adds a product license to OTDS.
+    ) -> dict:
+        """Add a product license to an OTDS resource.
 
         Args:
-            pathToLicenseFile (string): fully qualified filename of the license file
-            productName (string): product name
-            productDescription (string): product description
+            path_to_license_file (string): fully qualified filename of the license file
+            product_name (string): product name
+            product_description (string): product description
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
-            update (boolean): whether or not an existing license should be updated
-        Return: Request response (json) or None if the REST call fails
+            update (boolean, optional): whether or not an existing license should be updated (default = True)
+        Returns:
+            dictionary: Request response or None if the REST call fails
         """
 
         logger.info("Reading license file -> {}...".format(path_to_license_file))
         try:
             with open(path_to_license_file) as license_file:
                 license_content = license_file.read()
         except IOError as e:
@@ -415,15 +416,16 @@
     # end method definition
 
     def getLicensesForResource(self, resource_id: str):
         """Get a product license for a resource in OTDS.
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
-        Return: Licenses for a resource or None if the REST call fails
+        Returns:
+            Licenses for a resource or None if the REST call fails
         """
 
         request_url = (
             self.licenseUrl()
             + "/assignedlicenses?resourceID="
             + resource_id
             + "&validOnly=false"
@@ -456,21 +458,22 @@
                         resource_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def deleteLicenseFromResource(self, resource_id: str, license_id: str):
+    def deleteLicenseFromResource(self, resource_id: str, license_id: str) -> bool:
         """Delete a product license for a resource in OTDS.
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
-            licenseId (string): OTDS license ID (this is the ID not the license name!)
-        Return: True if successful or False if the REST call fails
+            license_id (string): OTDS license ID (this is the ID not the license name!)
+        Returns:
+            boolean: True if successful or False if the REST call fails
         """
 
         request_url = "{}/{}".format(self.licenseUrl(), license_id)
 
         logger.info(
             "Deleting product license -> {} from resource -> {}; calling -> {}".format(
                 license_id, resource_id, request_url
@@ -491,74 +494,75 @@
                 retries += 1
             else:
                 logger.error(
                     "Failed to delete license -> {} for resource -> {}; error -> {}".format(
                         license_id, resource_id, response.text
                     )
                 )
-                return None
+                return False
 
     # end method definition
 
     def assignUserToLicense(
         self,
         partition: str,
         user_id: str,
         resource_id: str,
         license_feature: str,
         license_name: str,
         license_type: str = "Full",
-    ):
-        """Assign a product license (feature) to a user in OTDS.
+    ) -> bool:
+        """Assign an OTDS user to a product license (feature) in OTDS.
 
         Args:
             partition (string): user partition in OTDS, e.g. "Content Server Members"
             user_id (string): ID of the user (= login name)
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             license_feature (string): name of the license feature
             license_name (string): name of the license to assign
             license_type (string, optional): deault is "Full", Extended ECM also has "Occasional"
-        Return: True if successful or False if the REST call fails
+        Returns:
+            boolean: True if successful or False if the REST call fails or the license is not found
         """
 
         licenses = self.getLicensesForResource(resource_id)
 
         for lic in licenses:
             if lic["_oTLicenseProduct"] == license_name:
-                licenseLocation = lic["id"]
+                license_location = lic["id"]
 
         try:
-            licenseLocation
+            license_location
         except UnboundLocalError:
             logger.error(
-                "Cannot find license for resource -> {} for {}".format(
+                "Cannot find license -> {} for resource -> {}".format(
                     license_name, resource_id
                 )
             )
-            return None
+            return False
 
         user = self.getUser(partition, user_id)
         if user:
             userLocation = user["location"]
         else:
             logger.error("Cannot find location for user -> {}".format(user_id))
-            return None
+            return False
 
         licensePostBodyJson = {
             "_oTLicenseType": license_type,
             "_oTLicenseProduct": "users",
             "name": userLocation,
             "values": [{"name": "counter", "values": [license_feature]}],
         }
 
-        request_url = self.licenseUrl() + "/object/" + licenseLocation
+        request_url = self.licenseUrl() + "/object/" + license_location
 
         logger.info(
             "Assign license feature -> {} of license -> {} associated with resource -> {} to user -> {}; calling -> {}".format(
-                license_feature, licenseLocation, resource_id, user_id, request_url
+                license_feature, license_location, resource_id, user_id, request_url
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
@@ -587,21 +591,105 @@
                         response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
-    def addPartition(self, name: str, description: str):
+    def assignPartitionToLicense(
+        self,
+        partition_name: str,
+        resource_id: str,
+        license_feature: str,
+        license_name: str,
+        license_type: str = "Full",
+    ) -> bool:
+        """Assign an OTDS partition to a product license (feature).
+
+        Args:
+            partition_name (string): user partition in OTDS, e.g. "Content Server Members"
+            resource_id (string): OTDS resource ID (this is ID not the resource name!)
+            license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
+            license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
+            license_type (string, optional): deault is "Full", Extended ECM also has "Occasional"
+        Returns:
+            boolean: True if successful or False if the REST call fails or the license is not found
+        """
+
+        licenses = self.getLicensesForResource(resource_id)
+
+        for lic in licenses:
+            if lic["_oTLicenseProduct"] == license_name:
+                license_location = lic["id"]
+
+        try:
+            license_location
+        except UnboundLocalError:
+            logger.error(
+                "Cannot find license -> {} for resource -> {}".format(
+                    license_name, resource_id
+                )
+            )
+            return False
+
+        licensePostBodyJson = {
+            "_oTLicenseType": license_type,
+            "_oTLicenseProduct": "partitions",
+            "name": partition_name,
+            "values": [{"name": "counter", "values": [license_feature]}],
+        }
+
+        request_url = self.licenseUrl() + "/object/" + license_location
+
+        logger.info(
+            "Assign license feature -> {} of license -> {} associated with resource -> {} to partition -> {}; calling -> {}".format(
+                license_feature, license_location, resource_id, partition_name, request_url
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.post(
+                request_url,
+                json=licensePostBodyJson,
+                headers=requestHeaders,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                logger.info(
+                    "Added license feature -> {} for partition -> {}".format(
+                        license_feature, partition_name
+                    )
+                )
+                return True
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to add license feature -> {} associated with resource -> {} for partition -> {}; status code -> {}".format(
+                        license_feature,
+                        resource_id,
+                        partition_name,
+                        response.status_code,
+                    )
+                )
+                return False
+
+    # end method definition
+
+    def addPartition(self, name: str, description: str) -> dict:
         """Add a new user partition to OTDS
 
         Args:
             name (string): name of the new partition
-        Return:
-            Request response (json) or None if the creation fails.
+        Returns:
+            dictionary: Request response or None if the creation fails.
         """
 
         partitionPostBodyJson = {"name": name, "description": description}
 
         request_url = self.partitionUrl()
 
         logger.info(
@@ -631,22 +719,22 @@
                         name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getPartition(self, name: str, show_error: bool = True):
+    def getPartition(self, name: str, show_error: bool = True) -> dict:
         """Get an existing user partition from OTDS
 
         Args:
             name (string): name of the partition to retrieve
-            show_error (boolean): whether or not we want to log an error if partion is not found
-        Return:
-            Request response (json) or None if the creation fails.
+            show_error (boolean, optional): whether or not we want to log an error if partion is not found
+        Returns:
+            dictionary: Request response or None if the creation fails.
         """
 
         request_url = "{}/{}".format(self.config()["partitionUrl"], name)
 
         logger.info(
             "Getting user partition -> {}; calling -> {}".format(name, request_url)
         )
@@ -678,26 +766,26 @@
         self,
         partition: str,
         name: str,
         description: str = "",
         first_name: str = "",
         last_name: str = "",
         email: str = "",
-    ):
+    ) -> dict:
         """Add a new user to a user partition in OTDS
 
         Args:
             partition (string): name of the OTDS user partition (needs to exist)
             name (string): login name of the new user
-            description (string): description of the new user
-            first_name (string): first name of the new user
-            last_name (string): last name of the new user
-            email (string): email address of the new user
-        Return:
-            Request response (json) or None if the creation fails.
+            description (string, optional): description of the new user
+            first_name (string, optional): first name of the new user
+            last_name (string, optional): last name of the new user
+            email (string, optional): email address of the new user
+        Returns:
+            dictionary: Request response or None if the creation fails.
         """
 
         userPostBodyJson = {
             "userPartitionID": partition,
             "values": [
                 {"name": "sn", "values": [last_name]},
                 {"name": "givenName", "values": [first_name]},
@@ -729,30 +817,28 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add user -> {}; error -> {}".format(
-                        name, response.text
-                    )
+                    "Failed to add user -> {}; error -> {}".format(name, response.text)
                 )
                 return None
 
     # end method definition
 
-    def getUser(self, partition: str, user_id: str):
+    def getUser(self, partition: str, user_id: str) -> dict:
         """Get a user by its partition and user ID
 
         Args:
             partition (string): name of the partition
             user_id (string): ID of the user (= login name)
-        Return:
-            Request response (json) or None if the creation fails.
+        Returns:
+            dictionary: Request response or None if the user was not found.
         """
 
         request_url = self.usersUrl() + "/" + user_id + "@" + partition
 
         logger.info(
             "Get user -> {} in partition -> {}; calling -> {}".format(
                 user_id, partition, request_url
@@ -779,24 +865,24 @@
                 )
                 return None
 
     # end method definition
 
     def updateUser(
         self, partition: str, user_id: str, attribute_name: str, attribute_value: str
-    ):
+    ) -> dict:
         """Update a user attribute with a new value
 
         Args:
             partition (string): name of the partition
             user_id (string): ID of the user (= login name)
             attribute_name (string): name of the attribute
-            attribute_value (string):new value of the attribute
+            attribute_value (string): new value of the attribute
         Return:
-            Request response (json) or None if the creation fails.
+            dictionary: Request response or None if the update fails.
         """
 
         userPatchBodyJson = {
             "userPartitionID": partition,
             "values": [{"name": attribute_name, "values": [attribute_value]}],
         }
 
@@ -829,22 +915,22 @@
                         user_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def deleteUser(self, partition: str, user_id: str):
+    def deleteUser(self, partition: str, user_id: str) -> bool:
         """Delete an existing user
 
         Args:
             partition (string): name of the partition
             user_id (string): Id (= login name) of the user
-        Return:
-            Request response (json) or None if the reset fails.
+        Returns:
+            Boolean: True = success, False = error
         """
 
         request_url = self.usersUrl() + "/" + user_id + "@" + partition
 
         logger.info(
             "Delete user -> {} in partition -> {}; calling -> {}".format(
                 user_id, partition, request_url
@@ -869,22 +955,22 @@
                         user_id, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def resetUserPassword(self, user_id: str, password: str):
+    def resetUserPassword(self, user_id: str, password: str) -> bool:
         """Reset a password of an existing user
 
         Args:
             user_id (string): Id (= login name) of the user
             password (string): new password of the user
-        Return:
-            Request response (json) or None if the reset fails.
+        Returns:
+            boolean: True = success, False = error.
         """
 
         userPostBodyJson = {"newPassword": password}
 
         request_url = "{}/{}/password".format(self.usersUrl(), user_id)
 
         logger.info(
@@ -898,39 +984,39 @@
             response = requests.put(
                 request_url,
                 json=userPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
             if response.ok:
-                return response.ok
+                return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to reset password for user -> {}; error -> {}".format(
                         user_id, response.text
                     )
                 )
-                return response.ok
+                return False
 
     # end method definition
 
-    def addGroup(self, partition: str, name: str, description: str):
+    def addGroup(self, partition: str, name: str, description: str) -> dict:
         """Add a new user group to a user partition in OTDS
 
         Args:
             partition (string): name of the OTDS user partition (needs to exist)
             name (string): name of the new group
             description (string): description of the new group
-        Return:
-            Request response (json) or None if the creation fails.
+        Returns:
+            dictionary: Request response (json) or None if the creation fails.
         """
 
         groupPostBodyJson = {
             "userPartitionID": partition,
             "name": name,
             "description": description,
         }
@@ -957,29 +1043,27 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add group -> {}; error -> {}".format(
-                        name, response.text
-                    )
+                    "Failed to add group -> {}; error -> {}".format(name, response.text)
                 )
                 return None
 
     # end method definition
 
-    def getGroup(self, group: str):
-        """Get a group by its group name
+    def getGroup(self, group: str) -> dict:
+        """Get a OTDS group by its group name
 
         Args:
-            group_id (string): ID of the group (= group name)
+            group (string): ID of the group (= group name)
         Return:
-            Request response (json) or None if the group was not found.
+            dictionary: Request response or None if the group was not found.
             Example values:
             {
                 'numMembers': 7,
                 'userPartitionID': 'Content Server Members',
                 'name': 'Sales',
                 'location': 'oTGroup=3f921294-b92a-4c9e-bf7c-b50df16bb937,orgunit=groups,partition=Content Server Members,dc=identity,dc=opentext,dc=net',
                 'id': 'Sales@Content Server Members',
@@ -1016,22 +1100,22 @@
                         group, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addUserToGroup(self, user: str, group: str):
+    def addUserToGroup(self, user: str, group: str) -> bool:
         """Add an existing user to an existing group in OTDS
 
         Args:
             user (string): name of the OTDS user (needs to exist)
             group (string): name of the OTDS group (needs to exist)
-        Return:
-            Request return code.
+        Returns:
+            boolean: Request return code.
         """
 
         userToGroupPostBodyJson = {"stringList": [group]}
 
         request_url = self.usersUrl() + "/" + user + "/memberof"
 
         logger.info(
@@ -1061,22 +1145,22 @@
                         user, group, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroupToParentGroup(self, group: str, parent_group: str):
+    def addGroupToParentGroup(self, group: str, parent_group: str) -> bool:
         """Add an existing group to an existing parent group in OTDS
 
         Args:
             group (string): name of the OTDS group (needs to exist)
             parent_group (string): name of the OTDS parent group (needs to exist)
-        Return:
-            Request return code.
+        Returns:
+            boolean: Request return code.
         """
 
         groupToParentGroupPostBodyJson = {"stringList": [parent_group]}
 
         request_url = self.groupsUrl() + "/" + group + "/memberof"
 
         logger.info(
@@ -1113,24 +1197,24 @@
 
     def addResource(
         self,
         name: str,
         description: str,
         display_name: str,
         additional_payload: dict = {},
-    ):
+    ) -> dict:
         """Add an OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
             description (string): description of the new OTDS resource
             display_name (string): display name of the OTDS resource
-            additional_payload (list): additional values for the json payload
-        Return:
-            Request response (json) or None if the REST call fails.
+            additional_payload (dictionary, optional): additional values for the json payload
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         resourcePostBodyJson = {
             "resourceName": name,
             "description": description,
             "displayName": display_name,
         }
@@ -1169,27 +1253,29 @@
                         name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getResource(self, name: str, show_error: bool = False):
+    def getResource(self, name: str, show_error: bool = False) -> dict:
         """Get an existing OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
-            show_error (boolean): treat as error if resource is not found
-        Return:
-            Request response (json) or None if the REST call fails.
+            show_error (boolean, optional): treat as error if resource is not found
+        Returns:
+            dictionary: Request response or None if the REST call fails.
         """
 
         request_url = "{}/{}".format(self.config()["resourceUrl"], name)
 
-        logger.info("Retrieving resource -> {}; calling -> {}".format(name, request_url))
+        logger.info(
+            "Retrieving resource -> {}; calling -> {}".format(name, request_url)
+        )
 
         retries = 0
         while True:
             response = requests.get(
                 request_url, headers=requestHeaders, cookies=self.cookie()
             )
             if response.ok:
@@ -1210,33 +1296,36 @@
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def updateResource(self, name: str, resource: object, show_error: bool = True):
+    def updateResource(self, name: str, resource: object, show_error: bool = True) -> dict:
         """Update an existing OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
             resource (object): updated resource object of getResource called before
-            show_error (boolean): treat as error if resource is not found
-        Return:
-            Request response (json) or None if the REST call fails.
+            show_error (boolean, optional): treat as error if resource is not found
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         request_url = "{}/{}".format(self.config()["resourceUrl"], name)
 
         logger.info("Updating resource -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
             response = requests.put(
-                request_url, json=resource, headers=requestHeaders, cookies=self.cookie()
+                request_url,
+                json=resource,
+                headers=requestHeaders,
+                cookies=self.cookie(),
             )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
@@ -1252,21 +1341,21 @@
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def activateResource(self, resource_id):
+    def activateResource(self, resource_id: str) -> dict:
         """Activate an OTDS resource
 
         Args:
             resource_id (string): ID of the OTDS resource
-        Return:
-            Request response (json) or None if the REST call fails.
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         resourcePostBodyJson = {}
 
         request_url = "{}/{}/activate".format(self.config()["resourceUrl"], resource_id)
 
         logger.info(
@@ -1294,20 +1383,20 @@
                         resource_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getAccessRoles(self):
+    def getAccessRoles(self) -> dict:
         """Get a list of all OTDS access roles
 
         Args: None
-        Return:
-            Request response (json) or None if the REST call fails.
+        Returns:
+            dictionary: Request response or None if the REST call fails.
         """
 
         request_url = self.config()["accessRoleUrl"]
 
         logger.info("Retrieving access roles; calling -> {}".format(request_url))
 
         retries = 0
@@ -1320,29 +1409,27 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to retrieve access roles; error -> {}".format(
-                        response.text
-                    )
+                    "Failed to retrieve access roles; error -> {}".format(response.text)
                 )
                 return None
 
     # end method definition
 
-    def getAccessRole(self, name: str):
+    def getAccessRole(self, name: str) -> dict:
         """Get an OTDS access role
 
         Args:
             name (string): name of the access role
-        Return:
-            Request response (json) or None if the REST call fails.
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         request_url = self.config()["accessRoleUrl"] + "/" + name
 
         logger.info(
             "Retrieving access role -> {}; calling -> {}".format(name, request_url)
         )
@@ -1367,31 +1454,34 @@
                 )
                 return None
 
     # end method definition
 
     def addPartitionToAccessRole(
         self, access_role: str, partition: str, location: str = ""
-    ):
+    ) -> bool:
         """Add an OTDS partition to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             partition (string): name of the partition
-            location (string): this is kind of a unique identifier DN (Distinguished Name)
-                               most of the times you will want to keep it to empty string ("")
-        Return:
-            Request response (json) or None if the REST call fails.
+            location (string, optional): this is kind of a unique identifier DN (Distinguished Name)
+                                         most of the times you will want to keep it to empty string ("")
+        Returns:
+            boolean: True if partition is in access role or has been successfully added.
+                     False if partition has been not been added (error)
         """
 
         accessRolePostBodyJson = {
             "userPartitions": [{"name": partition, "location": location}]
         }
 
-        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(
+            self.config()["accessRoleUrl"], access_role
+        )
 
         logger.info(
             "Add user partition -> {} to access role -> {}; calling -> {}".format(
                 partition, access_role, request_url
             )
         )
 
@@ -1415,24 +1505,25 @@
                         partition, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def addUserToAccessRole(self, access_role: str, user_id: str, location: str = ""):
+    def addUserToAccessRole(self, access_role: str, user_id: str, location: str = "") -> bool:
         """Add an OTDS user to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             user_id (string): ID of the user (= login name)
-            location (string): this is kind of a unique identifier DN (Distinguished Name)
-                               most of the times you will want to keep it to empty string ("")
-        Return:
-            Request response (json) or None if the REST call fails.
+            location (string, optional): this is kind of a unique identifier DN (Distinguished Name)
+                                         most of the times you will want to keep it to empty string ("")
+        Returns:
+            boolean: True if user is in access role or has been successfully added.
+                     False if user has been not been added (error)
         """
 
         # get existing members to check if user is already a member:
         accessRolesGetResponse = self.getAccessRole(access_role)
 
         if not accessRolesGetResponse:
             return False
@@ -1453,15 +1544,17 @@
                 user_id, access_role
             )
         )
 
         # create payload for REST call:
         accessRolePostBodyJson = {"users": [{"name": user_id, "location": location}]}
 
-        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(
+            self.config()["accessRoleUrl"], access_role
+        )
 
         logger.info(
             "Add user -> {} to access role -> {}; calling -> {}".format(
                 user_id, access_role, request_url
             )
         )
 
@@ -1485,29 +1578,29 @@
                         user_id, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroupToAccessRole(self, access_role: str, group: str, location: str = ""):
-        """Add an OTDS user to an OTDS access role
+    def addGroupToAccessRole(self, access_role: str, group: str, location: str = "") -> bool:
+        """Add an OTDS group to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             group (string): name of the group
-            location (string): this is kind of a unique identifier DN (Distinguished Name)
-                               most of the times you will want to keep it to empty string ("")
-        Return:
-            Request response (json) or None if the REST call fails.
+            location (string, optional): this is kind of a unique identifier DN (Distinguished Name)
+                                         most of the times you will want to keep it to empty string ("")
+        Returns:
+            boolean: True if group is in access role or has been successfully added.
+                     False if group has been not been added (error)
         """
 
         # get existing members to check if user is already a member:
         accessRolesGetResponse = self.getAccessRole(access_role)
-
         if not accessRolesGetResponse:
             return False
 
         # Checking if group already added to access role
         accessRoleGroups = accessRolesGetResponse["accessRoleMembers"]["groups"]
         for accessRoleGroup in accessRoleGroups:
             if accessRoleGroup["name"] == group:
@@ -1523,15 +1616,17 @@
                 group, access_role
             )
         )
 
         # create payload for REST call:
         accessRolePostBodyJson = {"groups": [{"name": group, "location": location}]}
 
-        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(
+            self.config()["accessRoleUrl"], access_role
+        )
 
         logger.info(
             "Add group -> {} to access role -> {}; calling -> {}".format(
                 group, access_role, request_url
             )
         )
 
@@ -1555,37 +1650,37 @@
                         group, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
-    def updateAccessRoleAttributes(self, name: str, attributeList: list):
+    def updateAccessRoleAttributes(self, name: str, attribute_list: list) -> dict:
         """Update some attributes of an existing OTDS Access Role
 
         Args:
             name (string): name of the existing access role
-            attributeList (list): list of attribute name and attribute value pairs
-                                  The values need to be a list as well. Example:
-                                  [{name: "pushAllGroups", values: ["True"]}]
-        Return:
-            Request response (json) or None if the REST call fails.
+            attribute_list (list): list of attribute name and attribute value pairs
+                                   The values need to be a list as well. Example:
+                                   [{name: "pushAllGroups", values: ["True"]}]
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         # Return if list is empty:
-        if not attributeList:
+        if not attribute_list:
             return None
 
         # create payload for REST call:
         access_role = self.getAccessRole(name)
         if not access_role:
             logger.error("Failed to get access role -> {}".format(name))
             return None
 
-        accessRolePutBodyJson = {"attributes": attributeList}
+        accessRolePutBodyJson = {"attributes": attribute_list}
 
         request_url = "{}/{}/attributes".format(self.config()["accessRoleUrl"], name)
 
         logger.info(
             "Update access role -> {} with attributes -> {}; calling -> {}".format(
                 name, accessRolePutBodyJson, request_url
             )
@@ -1612,23 +1707,23 @@
                         name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addSystemAttribute(self, name: str, value: str, description: str = ""):
+    def addSystemAttribute(self, name: str, value: str, description: str = "") -> dict:
         """Add a new system attribute to OTDS
 
         Args:
             name (string): name of the new system attribute
             value (string): value of the system attribute
-            description (string): optional description of the system attribute
-        Return:
-            Request response (json) or None if the REST call fails.
+            description (string, optional): optional description of the system attribute
+        Returns:
+            dictionary: Request response (json) or None if the REST call fails.
         """
 
         systemAttributePostBodyJson = {
             "name": name,
             "value": value,
             "friendlyName": description,
         }
@@ -1669,20 +1764,21 @@
                         name, value, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getTrustedSites(self):
-        """get all configured OTDS trusted sites
+    def getTrustedSites(self) -> dict:
+        """Get all configured OTDS trusted sites
 
-        Args: None
-        Return:
-            Request response (json) or None if the REST call fails.
+        Args:
+            None
+        Returns:
+            dictionary: Request response or None if the REST call fails.
         """
 
         request_url = "{}/whitelist".format(self.config()["systemConfigUrl"])
 
         logger.info("Retrieving trusted sites; calling -> {}".format(request_url))
 
         retries = 0
@@ -1703,21 +1799,21 @@
                         response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def addTrustedSite(self, trusted_site: str):
+    def addTrustedSite(self, trusted_site: str) -> dict:
         """Add a new OTDS trusted site
 
         Args:
-            trustedSite (string): name of the new trusted site
+            trusted_site (string): name of the new trusted site
         Return:
-            Request response (json) or None if the REST call fails.
+            dictionary: Request response or None if the REST call fails.
         """
 
         trustedSitePostBodyJson = {"stringList": [trusted_site]}
 
         # we need to first retrieve the existing sites and then
         # append the new one:
         existingTrustedSites = self.getTrustedSites()
@@ -1741,23 +1837,24 @@
         )
         if not response.ok:
             logger.error(
                 "Failed to add trusted site -> {}; error -> {}".format(
                     trusted_site, response.text
                 )
             )
-        return response
+            return None
+        return response # don't parse it!
 
     # end method definition
 
     def enableAudit(self):
         """enable Audit
 
         Args:
-            -
+            None
         Return:
             Request response (json) or None if the REST call fails.
         """
 
         auditPutBodyJson = {
             "daysToKeep": "7",
             "enabled": "true",
@@ -1820,45 +1917,43 @@
         response = requests.put(
             request_url,
             json=auditPutBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
         if not response.ok:
-            logger.error(
-                "Failed to enable audit; error -> {}".format(response.text)
-            )
+            logger.error("Failed to enable audit; error -> {}".format(response.text))
         return response
 
     # end method definition
 
     def addOauthClient(
         self,
         client_id: str,
         description: str,
         redirect_urls: list = [],
         allow_impersonation: bool = True,
         confidential: bool = True,
-        auth_scopes: list = [],  # empty string = "Global"
+        auth_scopes: list = [],  # empty list = "Global"
         allowed_scopes: list = [],  # in OTDS UI: Permissible scopes
         default_scopes: list = [],  # in OTDS UI: Default scopes
-    ):
+    ) -> dict:
         """Add a new OAuth client to OTDS
 
         Args:
             client_id (string): name of the new OAuth client (should not have blanks)
             description (string): description of the OAuth client
             redirect_urls (list): list of redirect URLs (strings)
-            allow_impersonation (boolean)
-            confidential (boolean)
-            auth_scope: str = "",  # empty string = "Global"
-            allowed_scopes: list = [],  # in OTDS UI: Permissible scopes
-            default_scopes: list = [],  # in OTDS UI: Default scopes
-        Return:
-            Request response (json) or None if the creation fails.
+            allow_impersonation (boolean, optional): allow impresonation
+            confidential (boolean, optional): is confidential
+            auth_scopes (list, optional): if empty then "Global"
+            allowed_scopes (list, optional): in OTDS UI this is called Permissible scopes
+            default_scopes (list, optional): in OTDS UI this is called Default scopes
+        Returns:
+            dictionary: Request response or None if the creation fails.
         """
 
         oauthClientPostBodyJson = {
             "id": client_id,
             "description": description,
             "redirectURLs": redirect_urls,
             "accessTokenLifeTime": 1000,
@@ -1902,21 +1997,21 @@
                         client_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
-    def getOauthClient(self, client_id, show_error: bool = True):
+    def getOauthClient(self, client_id: str, show_error: bool = True):
         """Get an existing OAuth client from OTDS
 
         Args:
             client_id (string): name (= ID) of the OAuth client to retrieve
             show_error (boolean): whether or not we want to log an error if partion is not found
-        Return:
+        Returns:
             Request response (json) or None if the client is not found.
         """
 
         request_url = "{}/{}".format(self.oauthClientUrl(), client_id)
 
         logger.info(
             "Get oauth client -> {}; calling -> {}".format(client_id, request_url)
@@ -1982,16 +2077,16 @@
     # end method definition
 
     def addOauthClientsToAccessRole(self, access_role_name: str):
         """Add Oauth clients user partion to an OTDS Access Role
 
         Args:
             access_role_name (string): name of the OTDS Access Role
-
-        Return: response of REST call or None in case of an error
+        Returns:
+            response of REST call or None in case of an error
         """
 
         accessRolesUrl = self.config()["accessRoleUrl"] + "/" + access_role_name
 
         logger.info(
             "Get access role -> {}; calling -> {}".format(
                 access_role_name, accessRolesUrl
@@ -2070,15 +2165,15 @@
             logger.info(
                 "OauthClients partition successfully added to access role -> {}".format(
                     access_role_name
                 )
             )
         else:
             logger.warning(
-                "Status code of {} returned attempting to add OAuthClients to access role {}: error -> {}".format(
+                "Status code of -> {} returned attempting to add OAuthClients to access role -> {}: error -> {}".format(
                     response.status_code,
                     access_role_name,
                     response.text,
                 )
             )
         return response
 
@@ -2123,15 +2218,15 @@
 
         Args:
             name (string): name of the new authentication handler
             description (string): description of the new authentication handler
             provider_name (string): description of the new authentication handler
             saml_url (string): SAML URL
             otds_url (string): the external(!) service provider URL of OTDS
-        Return:
+        Returns:
             Request response (json) or None if the REST call fails.
         """
 
         authHandlerPostBodyJson = {
             "_name": name,
             "_description": description,
             "_class": "com.opentext.otds.as.drivers.saml.SAML2Handler",
@@ -2251,15 +2346,15 @@
         """Add a new SAP authentication handler
 
         Args:
             name (string): name of the new authentication handler
             description (string): description of the new authentication handler
             certificate_file (string): fully qualified file name (with path) to the certificate file
             certificate_password (string): password of the certificate
-        Return:
+        Returns:
             Request response (json) or None if the REST call fails.
         """
 
         # 1. Prepare the body for the AuthHandler REST call:
         authHandlerPostBodyJson = {
             "_name": name,
             "_description": description,
@@ -2444,33 +2539,33 @@
         provider_name: str,
         client_id: str,
         client_secret: str,
         active_by_default: bool = False,
         authorization_endpoint: str = "",
         token_endpoint: str = "",
         scope_string: str = "",
-    ):
+    ) -> dict:
         """Add a new OAuth authentication handler
 
         Args:
             name (string): name of the new authentication handler
             description (string): description of the new authentication handler
             provider_name (string): the name of the authentication provider. This name is displayed on the login page.
             client_id (string): the client ID
             client_secret (string): the client secret
-            active_by_default (boolean): Whether to activate this handler for any request to the OTDS login page.
-                                         If true, any login request to the OTDS login page will be redirected to this OAuth provider.
-                                         If false, the user has to select the provider on the login page.
-            authorization_endpoint (string): The URL to redirect the browser to for authentication.
-                                             It is used to retrieve the authorization code or an OIDC id_token.
-            token_endpoint (string): The URL from which to retrieve the access token.
-                                     Not strictly required with OpenID Connect if using the implicit flow.
-            scope_string (string): Space delimited scope values to send. Include 'openid' to use OpenID Connect.
-        Return:
-            Request response (json) or None if the REST call fails.
+            active_by_default (boolean, optional): Whether to activate this handler for any request to the OTDS login page.
+                                                   If True, any login request to the OTDS login page will be redirected to this OAuth provider.
+                                                   If False, the user has to select the provider on the login page.
+            authorization_endpoint (string, optional): The URL to redirect the browser to for authentication.
+                                                       It is used to retrieve the authorization code or an OIDC id_token.
+            token_endpoint (string, optional): The URL from which to retrieve the access token.
+                                               Not strictly required with OpenID Connect if using the implicit flow.
+            scope_string (string, optional): Space delimited scope values to send. Include 'openid' to use OpenID Connect.
+        Returns:
+            dictionary: Request response or None if the REST call fails.
         """
 
         # 1. Prepare the body for the AuthHandler REST call:
         authHandlerPostBodyJson = {
             "_name": name,
             "_description": description,
             "_class": "com.opentext.otds.as.drivers.http.OAuth2Handler",
@@ -2836,21 +2931,21 @@
                         name, response.text
                     )
                 )
                 return None
 
         # end method definition
 
-    def consolidate(self, resource_name: str):
+    def consolidate(self, resource_name: str) -> bool:
         """Consolidate an OTDS resource
 
         Args:
             resource_name (string): resource to be consolidated
-        Return:
-            True if the consolidation succeeded or False if it failed.
+        Returns:
+            boolean: True if the consolidation succeeded or False if it failed.
         """
 
         resource = self.getResource(resource_name)
         if not resource:
             logger.error(
                 "Resource -> {} not found - cannot consolidate; error -> {}".format(
                     resource_name
@@ -2890,37 +2985,33 @@
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
-                logger.error(
-                    "Failed to consolidate; error -> {}".format(
-                        response.text
-                    )
-                )
+                logger.error("Failed to consolidate; error -> {}".format(response.text))
                 return False
 
     # end method definition
 
     def impersonateResource(
         self,
         resource_name: str,
         allow_impersonation: bool = True,
         impersonation_list: list = [],
-    ):
+    ) -> bool:
         """Configure impersonation for an OTDS resource
 
         Args:
             resource_name (string): resource to be configure impersonation for
-            allow_impersonation (boolean): optional; wether to turn on or off impersonation
-            impersonation_list (list): optional; list of users to restrict it to; empty list = all users
-        Return:
-            True if the impersonation setting succeeded or False if it failed.
+            allow_impersonation (boolean, optional): wether to turn on or off impersonation (default = True)
+            impersonation_list (list, optional): optional; list of users to restrict it to; (default = empty list = all users)
+        Returns:
+            boolean: True if the impersonation setting succeeded or False if it failed.
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
@@ -2958,23 +3049,23 @@
     # end method definition
 
     def impersonateOauthClient(
         self,
         client_id: str,
         allow_impersonation: bool = True,
         impersonation_list: list = [],
-    ):
+    ) -> bool:
         """Configure impersonation for an OTDS OAuth Client
 
         Args:
             client_id (string): OAuth Client to be configure impersonation for
-            allow_impersonation (boolean): optional; wether to turn on or off impersonation
-            impersonation_list (list): optional; list of users to restrict it to; empty list = all users
-        Return:
-            True if the impersonation setting succeeded or False if it failed.
+            allow_impersonation (boolean, optional): wether to turn on or off impersonation (default = True)
+            impersonation_list (list, optional): list of users to restrict it to; (default = empty list = all users)
+        Returns:
+            boolean: True if the impersonation setting succeeded or False if it failed.
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
@@ -3005,8 +3096,8 @@
                 logger.error(
                     "Failed to set impersonation for OAuth Client -> {}; error -> {}".format(
                         client_id, response.text
                     )
                 )
                 return False
 
-    # end method definition
+    # end method definition
```

### Comparing `pyxecm-0.0.16/pyxecm/otiv.py` & `pyxecm-0.0.17/pyxecm/otiv.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
 
 logger = logging.getLogger(os.path.basename(__file__))
 
+
 class OTIV(object):
     """Used to manage stettings for OpenText Intelligent Viewing."""
 
     _config = None
 
     def __init__(
-        self, resource_name: str, product_name: str, product_description: str, license_file: str, default_license: str = "FULLTIME_USERS_REGULAR"
+        self,
+        resource_name: str,
+        product_name: str,
+        product_description: str,
+        license_file: str,
+        default_license: str = "FULLTIME_USERS_REGULAR",
     ):
-        """ Initialize the OTIV class for Intelligent Viewing
+        """Initialize the OTIV class for Intelligent Viewing
 
         Args:
             resource_name (string): OTDS resource name
             product_name (string): OTDS product name for licensing
             license_file (string): path to license file
             default_license (string, optional): Defaults to "FULLTIME_USERS_REGULAR".
         """
```

### Comparing `pyxecm-0.0.16/pyxecm/otpd.py` & `pyxecm-0.0.17/pyxecm/otpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                 logger.warning(message)
             return None
         else:
             return dict_object
 
     # end method definition
 
-    def importDatabase(self, filename):
+    def importDatabase(self, filename: str):
         """Import PowerDocs database backup from a zip file"""
 
         file = filename.split("/")[-1]
         file_tup = (file, open(filename, "rb"), "application/zip")
 
         # fields attribute is set according to the other party's interface description
         m = MultipartEncoder(fields={"name": file, "zipfile": file_tup})
@@ -195,15 +195,14 @@
             )
             return None
 
     # end method definition
 
     # This method is currently not used and not working...
     def authenticate(self, revalidate: bool = False):
-
         # Already authenticated and session still valid?
         if self._jsessionid and not revalidate:
             return self._jsessionid
 
         auth_url = (
             self.baseUrl()
             + "/j_security_check?j_username="
@@ -219,54 +218,54 @@
 
         ##Fetching session id will be three step process
         # Step1: intiate a dummy request to tomcat
         # Step2: fetch session id from the response, and hit j_security_check with proper authentication
         # Step3: get session id from the response, add to self. It can be used for other transactions
         session = requests.Session()
         response = session.put(requestUrl, json=payLoad)
-        logger.info("Initiating dummy rest call to tomcat to get initial session id")
+        logger.info("Initiating dummy rest call to Tomcat to get initial session id")
         logger.info(response.text)
         if response.ok:
-            logger.info("Url to authenticate tomcate for Session id -> " + auth_url)
+            logger.info("Url to authenticate Tomcat for Session id -> " + auth_url)
             sessionResponse = session.post(auth_url)
             if sessionResponse.ok:
                 logger.info("Response for -> {}, {} ".format(auth_url, sessionResponse))
                 session_dict = session.cookies.get_dict()
                 logger.info(
                     "Session id to perform Rest api calls to Tomcat -> "
                     + session_dict["JSESSIONID"]
                 )
                 self._jsessionid = session_dict["JSESSIONID"]
                 requestHeaders["Cookie"] = "JSESSIONID=" + self._jsessionid
             else:
                 logger.info(
-                    "Fetching session id from -> {} failed with j_security_check. Response => {}".format(
+                    "Fetching session id from -> {} failed with j_security_check. Response -> {}".format(
                         auth_url, sessionResponse.text
                     )
                 )
         else:
             logger.info(
                 "Fetching session id from -> {} failed. Response => {}".format(
                     requestUrl, response.text
                 )
             )
 
     # end method definition
 
     def applySetting(
         self, setting_name: str, setting_value: str, tenant_name: str = ""
-    ):
+    ) -> dict:
         """Appy a setting to the PowerDocs Server Manager
 
         Args:
             setting_name (string): name of the setting
             setting_value (string): new value of the setting
             tenant_name (string): name of the PowerDocs tenant - this is optional as some settings are not tenant-specific!
         Return:
-            Request response (json) or None if the REST call fails.
+            dictionary: Request response or None if the REST call fails.
         """
 
         settingsPutBody = {
             "settingname": setting_name,
             "settingvalue": setting_value,
         }
```

### Comparing `pyxecm-0.0.16/pyxecm/payload.py` & `pyxecm-0.0.17/pyxecm/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,24 @@
 processGroupsM365: process M365 user groups
 processUsers: process Extended ECM users
 processUsersM365: process M365 users
 processAdminSettings: process Extended ECM administration settings (LLConfig)
 processExternalSystems: process Extended ECM external systems
 processTransportPackages: process Extended ECM transport packages
 processUserPhotos: process Extended ECM user photos (user profile)
+processUserPhotosM365: process user photos in payload and assign them to Microsoft 365 users.
 processWorkspaceTypes: process Extended ECM workspace types (needs to run after processTransportPackages)
 processWorkspaceTemplateRegistrations: register workspace templates as projects for Extended ECM for Engineering (deprecated)
 processWorkspaces: process Extended ECM workspace instances
 processWorkspaceRelationships: process Extended ECM workspace relationships
 processWorkspaceMembers: process Extended ECM workspace members (users and groups)
 processWebReports: process Extended ECM Web Reports (starts them with parameters)
 processCSApplications: process Extended ECM CS Applications
-processUserFavoritesAndSettings: process Extended ECM user favorites and user settings
+processUserSettings: Process user settings in payload and apply themin OTDS.
+processUserFavoritesAndProfile: Process user favorites in payload and create them in Extended ECM
 processSecurityClearances: process Security Clearance for users
 processSupplementalMarkings: process Supplemental Markings for users
 processUserSecurity: process Security Clearance and Supplemental Markings for users
 processRecordsManagementSettings: process Records Management settings by applying settings files
 processHolds: process Records Management Holds
 processAdditionalGroupMembers: process additional OTDS group memberships
 processAdditionalAccessRoleMembers: process additional OTDS group memberships
@@ -64,14 +66,15 @@
 processItems: process Extended ECM items (nodes) to create
 processPermissions: process permission changes for alist of Extended ECM items or volumes
 processAssignments: process assignments of workspaces / documents to users / groups
 processUserLicenses: process and apply licenses to all Extended ECM users (used for OTIV)
 processExecPodCommands: process Kubernetes pod commands
 initSAP: initalize SAP object for RFC communication
 processSAPRFCs: process SAP Remote Function Calls (RFC) to trigger automation in SAP S/4HANA
+processDocumentGenerators: Generate documents for a defined workspace type based on template
 
 getPayload: return the payload data structure
 getUsers: return list of users
 getGroups: return list of groups
 getWorkspaces: return list of workspaces
 getOTCSFrontend: return OTCS object for OTCS frontend
 getOTCSBackend: return OTCS object for OTCS backend
@@ -106,14 +109,15 @@
 
     # _debug controls whether or not transport processing is
     # stopped if one transport fails:
     _debug = False
     _otcs = None
     _otcs_backend = None
     _otcs_frontend = None
+    _otac = None
     _otds = None
     _otiv = None
     _k8s = None
     _web = None
     _m365 = None
     _custom_settings_dir = ""
 
@@ -145,14 +149,16 @@
     # "description", "external_system_name", "connection_type",
     # "as_url", "base_url", "username", and "password". Depending
     # on the connection type there may be additional dict values.
     _external_systems = []
     # transport_packages (list): List of transport packages systems. Each list element is a
     # dict with "url", "name", and "description" keys.
     _transport_packages = []
+    _content_transport_packages = []
+    _transport_packages_post = []
     _workspace_types = []
     _workspaces = []
     _sap_rfcs = []
     _web_reports = []
     _web_reports_post = []
     _cs_applications = []
     _admin_settings_post = []
@@ -166,15 +172,14 @@
     # is a dict with these keys:
     # - access_role (string)
     # - user_name (string)
     # - group_name (string)
     # - partition_name (string)
     _additional_access_role_members = []
     _renamings = []
-    _content_transport_packages = []
     _items = []
     _items_post = []
     _permissions = []
     _permissions_post = []
     # assignments: List of assignments. Each element is a dict with these keys:
     # - subject (string)
     # - instruction (string)
@@ -184,63 +189,70 @@
     # - users (list)
     _assignments = []
     _workspace_template_registrations = []
     _security_clearances = []
     _supplemental_markings = []
     _records_management_settings = []
     _holds = []
+    _doc_generators = []
 
     _placeholder_values = {}
 
-    def __init__(self, payload_source: str,
-                 custom_settings_dir: str,
-                 k8s_object: object,
-                 otds_object: object,
-                 otcs_backend_object: object,
-                 otcs_frontend_object: object,
-                 otiv_object: object,
-                 m365_object: object,
-                 placeholder_values: dict = {},
-                 stop_on_error: bool = False):
+    def __init__(
+        self,
+        payload_source: str,
+        custom_settings_dir: str,
+        k8s_object: object,
+        otds_object: object,
+        otac_object: object,
+        otcs_backend_object: object,
+        otcs_frontend_object: object,
+        otiv_object: object,
+        m365_object: object,
+        placeholder_values: dict = {},
+        stop_on_error: bool = False,
+    ):
         """Initialize the Payload object
 
         Args:
             payload_source (string): path or URL to payload source file
             k8s_object (object): Kubernetes object
             otds_object (object): OTDS object
+            otac_object (object): OTAC object
             otcs_backend_object (object): OTCS backend object
             otcs_frontend_object (object): OTCS frontend object
             otiv_object (object): OTIV object
             m365_object (object): M365 object to talk to Microsoft Graph API
             placeholder_values (dict): dictionary of placeholder values to be replaced in admin settings
             stop_on_error (bool): controls if transport deployment should stop if one transport fails
         """
 
         self._stop_on_error = stop_on_error
         self._payload_source = payload_source
         self._k8s = k8s_object
         self._otds = otds_object
+        self._otac = otac_object
         self._otcs = otcs_backend_object
         self._otcs_backend = otcs_backend_object
         self._otcs_frontend = otcs_frontend_object
         self._otiv = otiv_object
         self._m365 = m365_object
         self._custom_settings_dir = custom_settings_dir
         self._placeholder_values = placeholder_values
 
         self._http_object = web.HTTP()
 
-       # end method definition
+    # end method definition
 
     def replacePlaceholders(self, content: str):
-
         # https://stackoverflow.com/questions/63502218/replacing-placeholders-in-a-text-file-with-python
         return re.sub(
-            r"%%(\w+?)%%", lambda match: self._placeholder_values[match.group(
-                1)], content
+            r"%%(\w+?)%%",
+            lambda match: self._placeholder_values[match.group(1)],
+            content,
         )
 
         # end method definition
 
     def initPayload(self):
         """Read the YAML or Terraform HCL payload file.
 
@@ -248,36 +260,41 @@
         Return:
             payload as a Python dict. Elements are the different payload sections.
             None in case the file couldn't be found or read.
         """
 
         if not os.path.exists(self._payload_source):
             logger.error(
-                "Cannot access payload file -> {}".format(self._payload_source))
+                "Cannot access payload file -> {}".format(self._payload_source)
+            )
             return None
 
         # Is it a YAML file?
         if self._payload_source.endswith(".yaml"):
             logger.info(
-                "Open payload from YAML file -> {}".format(self._payload_source))
+                "Open payload from YAML file -> {}".format(self._payload_source)
+            )
             try:
                 with open(self._payload_source, "r") as stream:
                     payload_data = stream.read()
                 self._payload = yaml.safe_load(payload_data)
             except yaml.YAMLError as exc:
                 logger.error(
                     "Error while reading YAML payload file -> {}; error -> {}".format(
                         self._payload_source, exc
                     )
                 )
                 self._payload = None
         # Or is it a Terraform HCL file?
         elif self._payload_source.endswith(".tf"):
             logger.info(
-                "Open payload from Terraform HCL file -> {}".format(self._payload_source))
+                "Open payload from Terraform HCL file -> {}".format(
+                    self._payload_source
+                )
+            )
             try:
                 with open(self._payload_source, "r") as stream:
                     self._payload = hcl2.load(stream)
                 # If payload is wrapped into "external_payload" we unwrap it:
                 if self._payload.get("external_payload"):
                     self._payload = self._payload["external_payload"]
             except Exception as exc:
@@ -287,15 +304,16 @@
                     )
                 )
                 self._payload = None
         # If not, it is an unsupported type:
         else:
             logger.error(
                 "File -> {} has unsupported file type; error -> {}".format(
-                    self._payload_source)
+                    self._payload_source
+                )
             )
             self._payload = None
 
         self._payload_sections = self._payload["payloadSections"]
         if not self._payload_sections:
             logger.error(
                 "Sections for payload -> {} are undefined - skipping...".format(
@@ -313,85 +331,95 @@
         self._system_attributes = self.getPayloadSection("systemAttributes")
         self._groups = self.getPayloadSection("groups")
         self._users = self.getPayloadSection("users")
         self._admin_settings = self.getPayloadSection("adminSettings")
         self._exec_pod_commands = self.getPayloadSection("execPodCommands")
         self._external_systems = self.getPayloadSection("externalSystems")
         self._transport_packages = self.getPayloadSection("transportPackages")
+        self._content_transport_packages = self.getPayloadSection(
+            "contentTransportPackages"
+        )
+        self._transport_packages_post = self.getPayloadSection("transportPackagesPost")
         self._workspaces = self.getPayloadSection("workspaces")
         self._sap_rfcs = self.getPayloadSection("sapRFCs")
         self._web_reports = self.getPayloadSection("webReports")
         self._web_reports_post = self.getPayloadSection("webReportsPost")
         self._cs_applications = self.getPayloadSection("csApplications")
         self._admin_settings_post = self.getPayloadSection("adminSettingsPost")
         self._additional_group_members = self.getPayloadSection(
-            "additionalGroupMemberships")
+            "additionalGroupMemberships"
+        )
         self._additional_access_role_members = self.getPayloadSection(
-            "additionalAccessRoleMemberships")
+            "additionalAccessRoleMemberships"
+        )
         self._renamings = self.getPayloadSection("renamings")
-        self._content_transport_packages = self.getPayloadSection(
-            "contentTransportPackages")
         self._items = self.getPayloadSection("items")
         self._items_post = self.getPayloadSection("itemsPost")
         self._permissions = self.getPayloadSection("permissions")
         self._permissions_post = self.getPayloadSection("permissionsPost")
         self._assignments = self.getPayloadSection("assignments")
         self._workspace_template_registrations = self.getPayloadSection(
             "workspaceTemplateRegistrations",
         )
-        self._security_clearances = self.getPayloadSection(
-            "securityClearances")
-        self._supplemental_markings = self.getPayloadSection(
-            "supplementalMarkings")
+        self._security_clearances = self.getPayloadSection("securityClearances")
+        self._supplemental_markings = self.getPayloadSection("supplementalMarkings")
         self._records_management_settings = self.getPayloadSection(
-            "recordsManagementSettings")
+            "recordsManagementSettings"
+        )
         self._holds = self.getPayloadSection("holds")
+        self._doc_generators = self.getPayloadSection("documentGenerators")
 
         return self._payload
         # end method definition
 
-    def getPayloadSection(self, payload_section_name: str):
+    def getPayloadSection(self, payload_section_name: str) -> list:
         """Get a defined section of the payload. The section is delivered as a list of settings.
         It deliveres an empty list if this payload section is disabled by the corresponding
         payload switch (this is read from the payloadSections dictionary of the payload)
 
         Args:
-            payload (dict): payload data structure (converted to dict from YAML file)
             payload_section_name (string): name of the dict element in the payload structure
-        Return:
-            section of the payload as a Python list. Empty list if section does not exist
+        Returns:
+            list: section of the payload as a Python list. Empty list if section does not exist
             or section is disabled by the corresponding payload switch.
         """
 
         # if the secton is not in the payload we return an empty list:
         if not self._payload.get(payload_section_name):
             return []
 
         # Check if the payload section is either enabled
         # or the struct for payloadSection enabling is not in the payload:
         sections = self._payload.get("payloadSections")
         if sections:
             section = next(
-                (item for item in sections if item["name"]
-                 == payload_section_name),
+                (item for item in sections if item["name"] == payload_section_name),
                 None,
             )
             if not section or not section["enabled"]:
                 return []
 
         return self._payload[payload_section_name]
 
         # end method definition
 
+    def getAllGroupNames(self) -> list:
+        return [group.get("name") for group in self._groups]
+
     def processPayload(self):
         """Main method to process a payload file.
 
-        Returns: None
+        Args:
+            None
+        Returns:
+            None
         """
 
+        workspace_types = []
+
         if not self._payload_sections:
             return None
 
         for payload_section in self._payload_sections:
             match payload_section["name"]:
                 case "webHooks":
                     logger.info(
@@ -426,41 +454,55 @@
                 case "groups":
                     logger.info(
                         "========== Process OTCS Groups ========================="
                     )
                     self.processGroups()
                     if self._m365:
                         logger.info(
+                            "========== Cleanup existing MS Teams ==================="
+                        )
+                        self.cleanupAllTeamsM365()
+                        logger.info(
                             "========== Process M365 Groups ========================="
                         )
                         self.processGroupsM365()
                 case "users":
                     logger.info(
                         "========== Process OTCS Users =========================="
                     )
                     self.processUsers()
-                    logger.info("========== Assign OTCS Licenses to Users ===============")
+                    logger.info(
+                        "========== Assign OTCS Licenses to Users ==============="
+                    )
                     self.processUserLicenses(
                         self._otcs.config()["resource"],
                         self._otcs.config()["license"],
                         "EXTENDED_ECM",
-                        user_specific_payload_field="license"
+                        user_specific_payload_field="licenses",
+                    )
+                    logger.info(
+                        "========== Assign OTIV Licenses to Users ==============="
                     )
-                    logger.info("========== Assign OTIV Licenses to Users ===============")
                     self.processUserLicenses(
                         self._otiv.config()["resource"],
                         self._otiv.config()["license"],
                         "INTELLIGENT_VIEWING",
-                        user_specific_payload_field=""
+                        user_specific_payload_field="",
                     )
+                    logger.info(
+                        "========== Process User Settings ======================="
+                    )
+                    self.processUserSettings()
                     if self._m365:
                         logger.info(
                             "========== Process M365 Users =========================="
                         )
                         self.processUsersM365()
+                        # We need to do the MS Teams creation after the creation of
+                        # the M365 users as we require Group Owners to create teams
                         logger.info(
                             "========== Process M365 Teams =========================="
                         )
                         self.processTeamsM365()
                 case "adminSettings":
                     logger.info(
                         "========== Process OTCS LLConfig Settings (1) =========="
@@ -497,14 +539,29 @@
                     self.processTransportPackages(self._transport_packages)
                     # right after the transport that create the workspace types
                     # we extract them and put them in a generated payload list:
                     logger.info(
                         "========== Process Workspace Types ====================="
                     )
                     workspace_types = self.processWorkspaceTypes()
+                case "contentTransportPackages":
+                    logger.info(
+                        "========== Process Content Transport Packages =========="
+                    )
+                    self.processTransportPackages(self._content_transport_packages)
+                case "transportPackagesPost":
+                    # if self._m365:
+                    #     logger.info(
+                    #         "========== Cleanup stale MS Teams ======================"
+                    #     )
+                    #     self.cleanupStaleTeamsM365(workspace_types)
+                    logger.info(
+                        "========== Process Transport Packages (post) ==========="
+                    )
+                    self.processTransportPackages(self._transport_packages_post)
                 case "workspaceTemplateRegistrations":
                     logger.info(
                         "========== Register Workspace Templates ================"
                     )
                     self.processWorkspaceTemplateRegistrations()
                 case "workspaces":
                     logger.info(
@@ -570,20 +627,14 @@
                     )
                     self.processAdditionalAccessRoleMembers()
                 case "renamings":
                     logger.info(
                         "========== Process Custom Node Renamings ==============="
                     )
                     self.processRenamings()
-                case "contentTransportPackages":
-                    logger.info(
-                        "========== Process Content Transport Packages =========="
-                    )
-                    self.processTransportPackages(
-                        self._content_transport_packages)
                 case "items":
                     logger.info(
                         "========== Process Items ==============================="
                     )
                     self.processItems(self._items)
                 case "itemsPost":
                     logger.info(
@@ -621,93 +672,94 @@
                     )
                     self.processRecordsManagementSettings()
                 case "holds":
                     logger.info(
                         "========== Process Records Management Holds ============"
                     )
                     self.processHolds()
+                case "documentGenerators":
+                    logger.info(
+                        "========== Process Document Generators ================="
+                    )
+                    self.processDocumentGenerators()
                 case other:
                     logger.error(
                         "Illegal payload section name -> {} in payloadSections!".format(
                             payload_section["name"]
                         )
                     )
 
         if self._users:
-            logger.info(
-                "========== Process User Profile Photos =================")
+            logger.info("========== Process User Profile Photos =================")
             self.processUserPhotos()
             if self._m365:
-                logger.info(
-                    "========== Process M365 User Profile Photos ============")
+                logger.info("========== Process M365 User Profile Photos ============")
                 self.processUserPhotosM365()
-            logger.info(
-                "========== Process User Favorites and Settings =========")
-            self.processUserFavoritesAndSettings()
-            logger.info(
-                "========== Process User Security =======================")
+            logger.info("========== Process User Favorites and Profiles =========")
+            self.processUserFavoritesAndProfiles()
+            logger.info("========== Process User Security =======================")
             self.processUserSecurity()
 
         # end method definition
 
     def processWebHooks(self, webhooks: list):
         """Process Web Hooks in payload and do HTTP requests.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         if not webhooks:
             return None
 
         for webhook in webhooks:
-
             url = webhook.get("url")
             if not url:
                 logger.info("Web Hook does not have a url - skipping...")
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in webhook and not webhook["enabled"]:
                 logger.info(
-                    "Payload for Web Hook -> {} is disabled. Skipping...".format(
-                        url
-                    )
+                    "Payload for Web Hook -> {} is disabled. Skipping...".format(url)
                 )
                 continue
 
             description = webhook.get("description")
 
             method = webhook.get("method", "POST")
 
             payload = webhook.get("payload", {})
 
             headers = webhook.get("headers", {})
 
             if description:
                 logger.info(
-                    "Calling Web Hook -> {}: {} ({})".format(method, url, description))
+                    "Calling Web Hook -> {}: {} ({})".format(method, url, description)
+                )
             else:
-                logger.info(
-                    "Calling Web Hook -> {}: {}".format(method, url))
+                logger.info("Calling Web Hook -> {}: {}".format(method, url))
 
             self._http_object.httpRequest(url, method, payload, headers)
 
         # end method definition
 
     def processPartitions(self):
         """Process OTDS partitions in payload and create them in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         for partition in self._partitions:
-
             partition_name = partition.get("name")
             if not partition_name:
                 logger.error("Partition does not have a name - skipping...")
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
@@ -720,64 +772,106 @@
                 continue
 
             partition_description = partition.get("description")
 
             # Check if Partition does already exist
             # (in an attempt to make the code idem-potent)
             logger.info(
-                "Check if OTDS partition -> {} does already exist...".format(partition_name))
-            response = self._otds.getPartition(
-                partition_name, show_error=False)
+                "Check if OTDS partition -> {} does already exist...".format(
+                    partition_name
+                )
+            )
+            response = self._otds.getPartition(partition_name, show_error=False)
             if response:
                 logger.info(
-                    "Partition -> {} does already exist. Skipping...".format(partition_name))
+                    "Partition -> {} does already exist. Skipping...".format(
+                        partition_name
+                    )
+                )
                 continue
             else:
                 logger.info(
-                    "Partition -> {} does not exist. Creating...".format(partition_name))
+                    "Partition -> {} does not exist. Creating...".format(partition_name)
+                )
 
-            response = self._otds.addPartition(
-                partition_name, partition_description)
+            response = self._otds.addPartition(partition_name, partition_description)
             if response:
-                logger.info(
-                    "Added OTDS partition -> {}".format(partition_name))
+                logger.info("Added OTDS partition -> {}".format(partition_name))
             else:
                 logger.error(
-                    "Failed to add OTDS partition -> {}".format(partition_name))
+                    "Failed to add OTDS partition -> {}".format(partition_name)
+                )
                 continue
 
             access_role = partition.get("access_role")
             if access_role:
                 response = self._otds.addPartitionToAccessRole(
-                    access_role, partition_name)
+                    access_role, partition_name
+                )
                 if response:
                     logger.info(
                         "Added OTDS partition -> {} to access role -> {}".format(
                             partition_name, access_role
                         )
                     )
                 else:
                     logger.error(
                         "Failed to add OTDS partition -> {} to access role -> {}".format(
                             partition_name, access_role
                         )
                     )
                     continue
 
+            # Partions may have an optional list of licenses in
+            # the payload. Assign the partition to all these licenses:
+            partition_specific_licenses = partition.get("licenses")
+            if partition_specific_licenses:
+                # We assume these licenses are Extended ECM licenses!
+                otcs_resource_name = self._otcs.config()["resource"]
+                otcs_resource = self._otds.getResource(otcs_resource_name)
+                if not otcs_resource:
+                    logger.error(
+                        "Cannot find OTCS resource -> {}".format(otcs_resource_name)
+                    )
+                    continue
+                otcs_resource_id = otcs_resource["resourceID"]
+                license_name = "Extended ECM"
+                for license_feature in partition_specific_licenses:
+                    assigned_license = self._otds.assignPartitionToLicense(
+                        partition_name,
+                        otcs_resource_id,
+                        license_feature,
+                        license_name,
+                    )
+
+                    if not assigned_license:
+                        logger.error(
+                            "Failed to assign partition -> {} to license feature -> {} of license -> {}!".format(
+                                partition_name, license_feature, license_name
+                            )
+                        )
+                    else:
+                        logger.info(
+                            "Successfully assigned partition -> {} to license feature -> {} of license -> {}".format(
+                                partition_name, license_feature, license_name
+                            )
+                        )
+
         # end method definition
 
     def processOAuthClients(self):
         """Process OTDS OAuth clients in payload and create them in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         for oauth_client in self._oauth_clients:
-
             client_name = oauth_client.get("name")
             if not client_name:
                 logger.error("OAuth client does not have a name - skipping...")
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
@@ -793,54 +887,58 @@
             client_confidential = oauth_client.get("confidential")
             client_partition = oauth_client.get("partition")
             if client_partition == "Global":
                 client_partition = None
             client_redirect_urls = oauth_client.get("redirect_urls")
             client_permission_scopes = oauth_client.get("permission_scopes")
             client_default_scopes = oauth_client.get("default_scopes")
-            client_allow_impersonation = oauth_client.get(
-                "allow_impersonation")
+            client_allow_impersonation = oauth_client.get("allow_impersonation")
 
             # Check if OAuth client does already exist
             # (in an attempt to make the code idem-potent)
             logger.info(
-                "Check if OTDS OAuth Client -> {} does already exist...".format(client_name))
-            response = self._otds.getOauthClient(
-                client_name, show_error=False)
+                "Check if OTDS OAuth Client -> {} does already exist...".format(
+                    client_name
+                )
+            )
+            response = self._otds.getOauthClient(client_name, show_error=False)
             if response:
                 logger.info(
-                    "OAuth Client -> {} does already exist. Skipping...".format(client_name))
+                    "OAuth Client -> {} does already exist. Skipping...".format(
+                        client_name
+                    )
+                )
                 continue
             else:
                 logger.info(
-                    "OAuth Client -> {} does not exist. Creating...".format(client_name))
+                    "OAuth Client -> {} does not exist. Creating...".format(client_name)
+                )
 
             response = self._otds.addOauthClient(
                 client_id=client_name,
                 description=client_description,
                 redirect_urls=client_redirect_urls,
                 allow_impersonation=client_allow_impersonation,
                 confidential=client_confidential,
                 auth_scopes=client_partition,
                 allowed_scopes=client_permission_scopes,
                 default_scopes=client_default_scopes,
             )
             if response:
-                logger.info(
-                    "Added OTDS OAuth client -> {}".format(client_name))
+                logger.info("Added OTDS OAuth client -> {}".format(client_name))
             else:
                 logger.error(
-                    "Failed to add OTDS OAuth client -> {}".format(client_name))
+                    "Failed to add OTDS OAuth client -> {}".format(client_name)
+                )
                 continue
 
             client_secret = response.get("secret")
             if not client_secret:
                 logger.error(
-                    "OAuth client -> {} does not have a secret!".format(
-                        client_name)
+                    "OAuth client -> {} does not have a secret!".format(client_name)
                 )
                 continue
 
             client_description += " Client Secret Key: " + str(client_secret)
             response = self._otds.updateOauthClient(
                 client_name, {"description": client_description}
             )
@@ -848,29 +946,33 @@
     #        self._otds.addOauthClientsToAccessRole()
 
     # end method definition
 
     def processTrustedSites(self):
         """Process OTDS trusted sites in payload and create them in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         for trusted_site in self._trusted_sites:
             self._otds.addTrustedSite(trusted_site)
             logger.info("Added OTDS trusted site -> {}".format(trusted_site))
 
         # end method definition
 
     def processSystemAttributes(self):
         """Process OTDS system attributes in payload and create them in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         for system_attribute in self._system_attributes:
             # Check if there's a matching formal parameter defined on the Web Report node:
             if not system_attribute.get("name"):
                 logger.error("OTDS System Attribute needs a name. Skipping...")
                 continue
@@ -881,69 +983,76 @@
                     "Payload for OTDS System Attribute -> {} is disabled. Skipping...".format(
                         attribute_name
                     )
                 )
                 continue
 
             if not system_attribute.get("value"):
-                logger.error(
-                    "OTDS System Attribute needs a value. Skipping...")
+                logger.error("OTDS System Attribute needs a value. Skipping...")
                 continue
 
             attribute_value = system_attribute["value"]
             attribute_description = system_attribute.get("description")
             self._otds.addSystemAttribute(
-                attribute_name, attribute_value, attribute_description)
+                attribute_name, attribute_value, attribute_description
+            )
             logger.info(
                 "Added OTDS system attribute -> {} with value -> {}".format(
                     attribute_name, attribute_value
                 )
             )
 
         # end method definition
 
     def processGroups(self):
         """Process groups in payload and create them in Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         Side Effects:
             the group items are modified by adding an "id" dict element that
             includes the technical ID of the group in Extended ECM
         """
 
         # First run through groups: create all groups in payload
         # and store the IDs of the created groups:
         for group in self._groups:
-
             if not "name" in group:
                 logger.error("Group needs a name. Skipping...")
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
                     "Payload for Group -> {} is disabled. Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
 
             # Check if the group does already exist (e.g. if job is restarted)
             # as this is a pattern search it could return multiple groups:
             existing_groups = self._otcs.getGroup(group_name)
             if existing_groups and existing_groups["data"]:
                 logger.debug(
-                    "Found existing groups -> {}".format(existing_groups["data"]))
+                    "Found existing groups -> {}".format(existing_groups["data"])
+                )
                 # Get list of all matching groups:
                 existing_groups_list = existing_groups["data"]
                 # Find the group with the exact match of the name:
                 existing_group = next(
-                    (item for item in existing_groups_list if item["name"] == group_name),
+                    (
+                        item
+                        for item in existing_groups_list
+                        if item["name"] == group_name
+                    ),
                     None,
                 )
                 # Have we found an exact match?
                 if existing_group is not None:
                     logger.info(
                         "Found existing group -> {} ({}) - skipping to next group...".format(
                             existing_group["name"], existing_group["id"]
@@ -959,16 +1068,15 @@
                     ] = str(group["id"])
                     continue
                 else:
                     logger.info(
                         "Did not find an exact match for the group - creating a new group..."
                     )
             else:
-                logger.info(
-                    "Did not find any matching group - creating a new group...")
+                logger.info("Did not find any matching group - creating a new group...")
             # Now we know it is a new group...
             new_group = self._otcs.addGroup(group_name)
             if new_group is not None:
                 logger.debug("New group -> {}".format(new_group))
                 group["id"] = new_group["id"]
 
             # Add Group with its ID to the global dict with placeholder values:
@@ -978,37 +1086,40 @@
                 )
             ] = str(group["id"])
 
         logger.debug("Groups = {}".format(self._groups))
 
         logger.debug(
             "Placeholder values after group processing = {}".format(
-                self._placeholder_values)
+                self._placeholder_values
+            )
         )
 
         # Second run through groups: create all group memberships
         # (nested groups) based on the IDs created in first run:
         for group in self._groups:
             if not "id" in group:
-                logger.error(
-                    "Group -> {} does not have an ID.".format(group["name"]))
+                logger.error("Group -> {} does not have an ID.".format(group["name"]))
                 continue
             parent_group_names = group["parent_groups"]
             for parent_group_name in parent_group_names:
                 # First, try to find parent group in payload by parent group name:
                 parent_group = next(
-                    (item for item in self._groups if item["name"]
-                     == parent_group_name), None
+                    (
+                        item
+                        for item in self._groups
+                        if item["name"] == parent_group_name
+                    ),
+                    None,
                 )
                 if parent_group is None:
                     # If this didn't work, try to get the parent group from OTCS. This covers
                     # cases where the parent group is system generated or part
                     # of a former payload processing:
-                    parent_group = self._otcs.getGroup(
-                        parent_group_name)
+                    parent_group = self._otcs.getGroup(parent_group_name)
                     if not parent_group:
                         logger.error(
                             "Parent Group -> {} not found. Skipping...".format(
                                 parent_group_name
                             )
                         )
                         continue
@@ -1018,16 +1129,15 @@
                         "Parent Group -> {} does not have an ID. Skipping...".format(
                             parent_group["name"]
                         )
                     )
                     continue
 
                 # retrieve all members of the parent group (1 = get only groups)
-                members = self._otcs.getGroupMembers(
-                    parent_group["id"], 1)
+                members = self._otcs.getGroupMembers(parent_group["id"], 1)
                 if self._otcs.existResultItem(members, "id", group["id"]):
                     #                if existing_member:
                     logger.info(
                         "Group -> {} ({}) is already a member of parent group -> {} ({}) - skipping to next parent group...".format(
                             group["name"],
                             group["id"],
                             parent_group["name"],
@@ -1039,61 +1149,70 @@
                         "Add group -> {} ({}) to parent group -> {} ({})".format(
                             group["name"],
                             group["id"],
                             parent_group["name"],
                             parent_group["id"],
                         )
                     )
-                    self._otcs.addGroupMember(
-                        group["id"], parent_group["id"])
+                    self._otcs.addGroupMember(group["id"], parent_group["id"])
 
         # end method definition
 
     def processGroupsM365(self):
         """Process groups in payload and create them in Microsoft 365.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         # First run through groups: create all groups in payload
         # and store the IDs of the created groups:
         for group in self._groups:
-
             if not "name" in group:
                 logger.error("Group needs a name. Skipping...")
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
                     "Payload for Group -> {} is disabled. Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
             if not "enable_o365" in group or not group["enable_o365"]:
                 logger.info(
                     "Office 365 is not enabled in payload for Group -> {}. Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
 
             # Check if the group does already exist (e.g. if job is restarted)
             # as this is a pattern search it could return multiple groups:
             existing_groups = self._m365.getGroup(group_name)
             if existing_groups and existing_groups["value"]:
                 logger.debug(
-                    "Found existing Microsoft 365 groups -> {}".format(existing_groups["value"]))
+                    "Found existing Microsoft 365 groups -> {}".format(
+                        existing_groups["value"]
+                    )
+                )
                 # Get list of all matching groups:
                 existing_groups_list = existing_groups["value"]
                 # Find the group with the exact match of the name:
                 existing_group = next(
-                    (item for item in existing_groups_list if item["displayName"] == group_name),
+                    (
+                        item
+                        for item in existing_groups_list
+                        if item["displayName"] == group_name
+                    ),
                     None,
                 )
                 # Have we found an exact match?
                 if existing_group is not None:
                     logger.info(
                         "Found existing Microsoft 365 group -> {} ({}) - skip creation of group...".format(
                             existing_group["displayName"], existing_group["id"]
@@ -1103,15 +1222,16 @@
                     continue
                 else:
                     logger.info(
                         "Did not find an exact match for the group - creating a new Microsoft 365 group..."
                     )
             else:
                 logger.info(
-                    "Did not find any matching group - creating a new Microsoft 365 group...")
+                    "Did not find any matching group - creating a new Microsoft 365 group..."
+                )
 
             # Now we know it is a new group...
             new_group = self._m365.addGroup(group_name)
             if new_group is not None:
                 # Store the Microsoft 365 group ID in payload:
                 group["m365_id"] = new_group["id"]
                 logger.info(
@@ -1121,38 +1241,37 @@
                 )
 
         # end method definition
 
     def processUsers(self):
         """Process users in payload and create them in Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         Side Effects:
             the user items are modified by adding an "id" dict element that
             includes the technical ID of the user in Extended ECM
         """
 
         # Add all users in payload and establish membership in
         # specified groups:
         for user in self._users:
-
             # Sanity checks:
             if not "name" in user:
-                logger.error(
-                    "User is missing a login - skipping to next user...")
+                logger.error("User is missing a login - skipping to next user...")
                 continue
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
 
             # Sanity checks:
             if not "password" in user:
                 logger.error(
                     "User -> {} is missing a password - skipping to next user...".format(
@@ -1171,15 +1290,16 @@
                 user["base_group"] = "DefaultGroup"
 
             # Check if the user does already exist (e.g. if job is restarted)
             # As this is a pattern search it could return multiple users:
             existing_users = self._otcs.getUser(user_name)
             if existing_users and existing_users["data"]:
                 logger.debug(
-                    "Found existing users -> {}".format(existing_users["data"]))
+                    "Found existing users -> {}".format(existing_users["data"])
+                )
                 # Get list of all matching users:
                 existing_users_list = existing_users["data"]
                 # Find the user with the exact match of the name:
                 existing_user = next(
                     (item for item in existing_users_list if item["name"] == user_name),
                     None,
                 )
@@ -1193,21 +1313,23 @@
                     user["id"] = existing_user["id"]
                     continue
                 else:
                     logger.info(
                         "Did not find an exact match for the user - creating a new user..."
                     )
             else:
-                logger.info(
-                    "Did not find any matching user - creating a new user...")
+                logger.info("Did not find any matching user - creating a new user...")
 
             # Find the base group of the user. Assume 'Default Group' (= 1001) if not found:
             base_group = next(
-                (item["id"]
-                 for item in self._groups if item["name"] == user["base_group"]),
+                (
+                    item["id"]
+                    for item in self._groups
+                    if item["name"] == user["base_group"]
+                ),
                 1001,
             )
 
             # Now we know it is a new user...
             new_user = self._otcs.addUser(
                 name=user_name,
                 password=user["password"],
@@ -1228,25 +1350,24 @@
                     )
                 )
                 user["id"] = new_user["id"]
                 group_names = user["groups"]
                 for group_name in group_names:
                     # Find the group dictionary item to the parent group name:
                     group = next(
-                        (item for item in self._groups if item["name"]
-                         == group_name), None
+                        (item for item in self._groups if item["name"] == group_name),
+                        None,
                     )
                     if group is None:
                         # if group is not in payload try to find group in OTCS
                         # in case it is a pre-existing group:
                         group = self._otcs.getGroup(group_name)
                         if group is None:
                             logger.error(
-                                "Group -> {} not found. Skipping...".format(
-                                    group_name)
+                                "Group -> {} not found. Skipping...".format(group_name)
                             )
                             continue
                         group = group["data"][0]
 
                     if group["id"] is None:
                         logger.error(
                             "Group -> {} does not have an ID. Skipping...".format(
@@ -1259,16 +1380,15 @@
                         "Add user -> {} ({}) to group -> {} ({})".format(
                             user["name"], user["id"], group["name"], group["id"]
                         )
                     )
                     self._otcs.addGroupMember(user["id"], group["id"])
                 # for some unclear reason the user is not added to its base group in OTDS
                 # so we do this explicitly:
-                self._otds.addUserToGroup(
-                    user["name"], user["base_group"])
+                self._otds.addUserToGroup(user["name"], user["base_group"])
 
                 # Extra OTDS attributes for the user can be provided in "extra_attributes"
                 # as part of the user payload.
                 if "extra_attributes" in user:
                     extra_attributes = user["extra_attributes"]
                     for extra_attribute in extra_attributes:
                         attribute_name = extra_attribute.get("name")
@@ -1279,59 +1399,56 @@
                             )
                             continue
                         logger.info(
                             "Set user attribute -> {} to -> {}".format(
                                 attribute_name, attribute_value
                             )
                         )
-                        user_partition = self._otcs.config()[
-                            "partition"]
+                        user_partition = self._otcs.config()["partition"]
                         if not user_partition:
-                            logger.error(
-                                "User partition not found!"
-                            )
+                            logger.error("User partition not found!")
                         self._otds.updateUser(
                             user_partition,
                             user["name"],
                             attribute_name,
                             attribute_value,
                         )
 
         # end method definition
 
     def processUsersM365(self):
         """Process users in payload and create them in Microsoft 365 via MS Graph API.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         # Add all users in payload and establish membership in
         # specified groups:
         for user in self._users:
-
             # Sanity checks:
             if not "name" in user:
-                logger.error(
-                    "User is missing a login - skipping to next user...")
+                logger.error("User is missing a login - skipping to next user...")
                 continue
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
             if not "enable_o365" in user or not user["enable_o365"]:
                 logger.info(
                     "Office 365 is not enabled in payload for User -> {}. Skipping...".format(
-                        user_name)
+                        user_name
+                    )
                 )
                 continue
 
             # Sanity checks:
             if not "password" in user:
                 logger.error(
                     "User -> {} is missing a password - skipping to next user...".format(
@@ -1349,121 +1466,175 @@
             # Check if the user does already exist (e.g. if job is restarted)
             # As this is a pattern search it could return multiple users:
             user_name = user_name + "@" + self._m365.config()["domain"]
             existing_user = self._m365.getUser(user_name)
             if existing_user:
                 logger.info(
                     "Found existing Microsoft 365 user -> {} ({}) with ID -> {}".format(
-                        existing_user["displayName"], existing_user["userPrincipalName"], existing_user["id"]
+                        existing_user["displayName"],
+                        existing_user["userPrincipalName"],
+                        existing_user["id"],
                     )
                 )
                 user["m365_id"] = existing_user["id"]
             else:
                 logger.info(
-                    "Did not find existing user - creating a new Microsoft 365 user...")
+                    "Did not find existing user - creating a new Microsoft 365 user..."
+                )
 
                 # Now we know it is a new user...
-                new_user = self._m365.addUser(email=user_name,
-                                              password=user_password,
-                                              first_name=user_first_name,
-                                              last_name=user_last_name,
-                                              location=user_location,
-                                              department=user_department)
+                new_user = self._m365.addUser(
+                    email=user_name,
+                    password=user_password,
+                    first_name=user_first_name,
+                    last_name=user_last_name,
+                    location=user_location,
+                    department=user_department,
+                )
                 if new_user is not None:
                     # Store the Microsoft 365 user ID in payload:
                     user["m365_id"] = new_user["id"]
                     logger.info(
                         "New Microsoft 365 user -> {} with ID -> {} has been created".format(
                             user_name, user["m365_id"]
                         )
                     )
                 else:
                     logger.error(
-                        "Failed to create new Microsoft 365 user -> {}".format(user_name))
+                        "Failed to create new Microsoft 365 user -> {}. Skipping.".format(
+                            user_name
+                        )
+                    )
                     continue
 
             # Now we assign a license to the new M365 user.
-            # First we see if there's a specific M365 SKU in user
-            # payload - if not we use the default SKU configured
-            # for the m365 object:
-            sku_id = user.get("m365_sku", self._m365.config()["skuId"])
-            if sku_id:
+            # First we see if there's a M365 SKU list in user
+            # payload - if not we wrap the default SKU configured
+            # for the m365 object into a single item list:
+            existing_user_licenses = self._m365.getUserLicenses(user["m365_id"])
+            sku_list = user.get("m365_skus", [self._m365.config()["skuId"]])
+            for sku_id in sku_list:
                 # Check if the M365 user already has this license:
-                existing_user_licenses = self._m365.getUserLicenses(user["m365_id"])
-                if not self._m365.existResultItem(existing_user_licenses, "skuId", sku_id):
-                    response = self._m365.assignLicenseToUser(
-                        user["m365_id"], sku_id)
+                if not self._m365.existResultItem(
+                    existing_user_licenses, "skuId", sku_id
+                ):
+                    response = self._m365.assignLicenseToUser(user["m365_id"], sku_id)
                     if not response:
                         logger.error(
-                            "Failed to assign license -> {} to Microsoft 365 user -> {}".format(sku_id, user_name))
+                            "Failed to assign license -> {} to Microsoft 365 user -> {}".format(
+                                sku_id, user_name
+                            )
+                        )
                     else:
-                        user["m365_sku"] = sku_id
+                        if (
+                            not "m365_skus" in user
+                        ):  # this is only True if the default license from the m365 object is taken
+                            user["m365_skus"] = [sku_id]
                         logger.info(
-                            "License -> {} has been assigned to Microsoft 365 user -> {}".format(sku_id, user_name))
+                            "License -> {} has been assigned to Microsoft 365 user -> {}".format(
+                                sku_id, user_name
+                            )
+                        )
                 else:
                     logger.info(
-                        "Microsoft 365 user -> {} already has the license -> {}".format(user_name, sku_id))
+                        "Microsoft 365 user -> {} already has the license -> {}".format(
+                            user_name, sku_id
+                        )
+                    )
 
             # Now we assign the Extended ECM Teams App to the new M365 user.
             # First we check if the app is already assigned to the user.
             # If not we install / assign the app. If the user already has
             # the Extended ECM app we try to uprade it:
             app_name = self._m365.config()["teamsAppName"]
-            response = self._m365.getTeamsAppsOfUser(user["m365_id"], "contains(teamsAppDefinition/displayName, '{}')".format(app_name))
-            if self._m365.existResultItem(response, "displayName", app_name, sub_dict_name="teamsAppDefinition"):
+            response = self._m365.getTeamsAppsOfUser(
+                user["m365_id"],
+                "contains(teamsAppDefinition/displayName, '{}')".format(app_name),
+            )
+            if self._m365.existResultItem(
+                response, "displayName", app_name, sub_dict_name="teamsAppDefinition"
+            ):
                 logger.info(
-                    "Upgrade MS Teams app -> {} for user -> {}".format(app_name, user_name))
+                    "Upgrade MS Teams app -> {} for user -> {}".format(
+                        app_name, user_name
+                    )
+                )
                 response = self._m365.upgradeTeamsAppOfUser(user["m365_id"], app_name)
             else:
                 logger.info(
-                    "Install MS Teams app -> {} for user -> {}".format(app_name, user_name))
+                    "Install MS Teams app -> {} for user -> {}".format(
+                        app_name, user_name
+                    )
+                )
                 response = self._m365.assignTeamsAppToUser(user["m365_id"], app_name)
 
             # Process Microsoft 365 group memberships of new user:
             if "m365_id" in user:
                 user_id = user["m365_id"]
                 # don't forget the base group (department) !
                 group_names = user["groups"]
                 if user_department:
                     group_names.append(user_department)
                 logger.info(
-                    "User -> {} has these groups in payload -> {} (including base group -> {}). Checking if they are Microsoft 365 Groups...".format(user_name, group_names, user_department))
+                    "User -> {} has these groups in payload -> {} (including base group -> {}). Checking if they are Microsoft 365 Groups...".format(
+                        user_name, group_names, user_department
+                    )
+                )
+                # Go through all
                 for group_name in group_names:
-
-                    # Find the group dictionary item to the parent group name:
+                    # Find the group payload item to the parent group name:
                     group = next(
-                        (item for item in self._groups if item["name"]
-                         == group_name), None
+                        (item for item in self._groups if item["name"] == group_name),
+                        None,
                     )
-                    if group is None or not "enable_o365" in group or not group["enable_o365"]:
+                    if not group:
                         # if group is not in payload then this membership
-                        # is not relevant for Microsoft 365.
-                        # If Office 365 is not enabled for this group in
-                        # the payload we can also skip:
+                        # is not relevant for Microsoft 365. This could be system generated
+                        # groups like "PageEdit" or "Business Administrators".
+                        # In this case we do "continue" as we can't process parent groups
+                        # either:
+                        logger.info(
+                            "No payload found for Group -> {}. Skipping...".format(
+                                group_name
+                            )
+                        )
+                        continue
+                    elif not "enable_o365" in group or not group["enable_o365"]:
+                        # If Microsoft 365 is not enabled for this group in
+                        # the payload we don't create a M365 but we do NOT continue
+                        # as there may still be parent groups that are M365 enabled
+                        # we want to put the user in (see below):
                         logger.info(
-                            "Payload Group -> {} is not enabled for M365. Skipping...".format(
-                                group_name)
+                            "Payload Group -> {} is not enabled for M365.".format(
+                                group_name
+                            )
                         )
                     else:
                         response = self._m365.getGroup(group_name)
-                        if response is None or not "value" in response or not response["value"]:
+                        if (
+                            response is None
+                            or not "value" in response
+                            or not response["value"]
+                        ):
                             logger.error(
                                 "Microsoft 365 Group -> {} not found. Skipping...".format(
-                                    group_name)
+                                    group_name
+                                )
                             )
                         else:
                             group_id = response["value"][0]["id"]
 
                             # Check if user is already a member. We don't want
                             # to throw an error if the user is not found as a member:
                             if self._m365.isMember(group_id, user_id, show_error=False):
                                 logger.info(
                                     "Microsoft 365 user -> {} ({}) is already in Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
-                                    ))
+                                    )
+                                )
                             else:
                                 logger.info(
                                     "Add Microsoft 365 user -> {} ({}) to Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
                                     )
                                 )
                                 self._m365.addGroupMember(group_id, user_id)
@@ -1474,185 +1645,280 @@
                                     "Make Microsoft 365 user -> {} ({}) owner of Microsoft 365 group -> {} ({})".format(
                                         user["name"], user_id, group_name, group_id
                                     )
                                 )
                                 self._m365.addGroupOwner(group_id, user_id)
 
                     # As M365 groups are flat (not nested) we also add the
-                    # user as member to the parent groups of the current group:
+                    # user as member to the parent groups of the current group
+                    # if the parent group is enabled for M365:
                     parent_group_names = group.get("parent_groups")
-                    logger.info("Group -> {} has the following parent groups -> {}".format(group_name, parent_group_names))
+                    logger.info(
+                        "Group -> {} has the following parent groups -> {}".format(
+                            group_name, parent_group_names
+                        )
+                    )
                     for parent_group_name in parent_group_names:
                         # Find the group dictionary item to the parent group name:
                         parent_group = next(
-                            (item for item in self._groups if item["name"]
-                             == parent_group_name), None
+                            (
+                                item
+                                for item in self._groups
+                                if item["name"] == parent_group_name
+                            ),
+                            None,
                         )
-                        if parent_group is None or not "enable_o365" in parent_group or not parent_group["enable_o365"]:
+                        if (
+                            parent_group is None
+                            or not "enable_o365" in parent_group
+                            or not parent_group["enable_o365"]
+                        ):
                             # if parent group is not in payload then this membership
                             # is not relevant for Microsoft 365.
                             # If Office 365 is not enabled for this parent group in
                             # the payload we can also skip:
                             logger.info(
                                 "Parent Group -> {} is not enabled for M365. Skipping...".format(
-                                    group_name)
+                                    group_name
+                                )
                             )
                             continue
 
                         response = self._m365.getGroup(parent_group_name)
-                        if response is None or not "value" in response or not response["value"]:
+                        if (
+                            response is None
+                            or not "value" in response
+                            or not response["value"]
+                        ):
                             logger.error(
                                 "Microsoft 365 Group -> {} not found. Skipping...".format(
-                                    group_name)
+                                    group_name
+                                )
                             )
                             continue
                         parent_group_id = response["value"][0]["id"]
 
                         # Check if user is already a member. We don't want
                         # to throw an error if the user is not found as a member:
-                        if self._m365.isMember(parent_group_id, user_id, show_error=False):
+                        if self._m365.isMember(
+                            parent_group_id, user_id, show_error=False
+                        ):
                             logger.info(
                                 "Microsoft 365 user -> {} ({}) is already in Microsoft 365 group -> {} ({})".format(
-                                    user["name"], user_id, parent_group_name, parent_group_id
-                                ))
+                                    user["name"],
+                                    user_id,
+                                    parent_group_name,
+                                    parent_group_id,
+                                )
+                            )
                             continue
 
                         logger.info(
                             "Add Microsoft 365 user -> {} ({}) to Microsoft 365 group -> {} ({})".format(
-                                user["name"], user_id, parent_group_name, parent_group_id
+                                user["name"],
+                                user_id,
+                                parent_group_name,
+                                parent_group_id,
                             )
                         )
                         self._m365.addGroupMember(parent_group_id, user_id)
 
         # end method definition
 
     def processTeamsM365(self):
         """Process groups in payload and create matching Teams in Microsoft 365.
            We need to do this after the creation of the M365 users as wie require
            Group Owners to create teams.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         for group in self._groups:
-
             if not "name" in group:
                 logger.error("Team needs a name. Skipping...")
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
                     "Payload for Group -> {} is disabled. Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
             if not "enable_o365" in group or not group["enable_o365"]:
                 logger.info(
                     "Office 365 is not enabled in payload for Group -> {}. Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
 
             # Check if the M365 group does not exist (this should actually never happen at this point)
             if not "m365_id" in group:
                 # The "m365_id" value is set by the method processGroupsM365()
                 logger.error(
                     "No M365 Group exist for group -> {} (M365 Group creation may have failed). Skipping...".format(
-                        group_name)
+                        group_name
+                    )
                 )
                 continue
 
             if not self._m365.hasTeam(group_name):
                 logger.info(
-                    "Create M365 Team -> {} or existing M365 Group -> {}...".format(group_name, group_name))
+                    "Create M365 Team -> {} for existing M365 Group -> {}...".format(
+                        group_name, group_name
+                    )
+                )
                 # Now "upgrading" this group to a MS Team:
                 new_team = self._m365.addTeam(group_name)
             else:
                 logger.info(
-                    "M365 group -> {} already has an MS Team connected. Skipping...".format(group_name))
+                    "M365 group -> {} already has an MS Team connected. Skipping...".format(
+                        group_name
+                    )
+                )
+
+        # end method definition
+
+    def cleanupStaleTeamsM365(self, workspace_types: list):
+        """Delete Microsoft Teams that are left-overs from former deployments.
+           This method is currently not used.
+
+        Args:
+            workspace_types (list): list of all workspace types
+        """
+
+        if workspace_types == []:
+            logger.error("Empty workspace type list!")
+            return
+
+        for workspace_type in workspace_types:
+            if not "name" in workspace_type:
+                logger.error(
+                    "Workspace type -> {} does not have a name. Skipping...".format(
+                        workspace_type
+                    )
+                )
+                continue
+            response = self._otcs.getWorkspaceInstances(workspace_type["name"])
+            workspace_instances = response["results"]
+            if not workspace_instances:
+                logger.info(
+                    "Workspace type -> {} does not have any instances!".format(
+                        workspace_type["name"]
+                    )
+                )
+                continue
+            for workspace_instance in workspace_instances:
+                workspace_name = workspace_instance["data"]["properties"]["name"]
+                logger.info(
+                    "Check if stale Microsoft 365 Teams with name -> {} exist...".format(
+                        workspace_name
+                    )
+                )
+                response = self._m365.deleteTeams(workspace_name)
+
+        # end method definition
+
+    def cleanupAllTeamsM365(self) -> bool:
+        """Delete Microsoft Teams that are left-overs from former deployments
+
+        Args:
+            None
+        Returns:
+            boolean: True if teams have been deleted, False otherwise
+        """
+
+        exception_list = self.getAllGroupNames()
+        pattern_list = [r"\(\d+\)", r"\d+\s-\s"]
+
+        result = self._m365.deleteAllTeams(exception_list, pattern_list)
+
+        return result
 
         # end method definition
 
     def processAdminSettings(self, admin_settings: list) -> bool:
         """Process admin settings in payload and import them to Extended ECM.
 
         Args:
             admin_settings (list): list of admin settings. We need this parameter
                                    as we process two different lists.
-        Return:
-            True if a restart of the OTCS pods is required. False otherwise.
+        Returns:
+            boolean: True if a restart of the OTCS pods is required. False otherwise.
         """
 
         restart_required = False
 
         for admin_setting in admin_settings:
-
             # Sanity checks:
             if not "filename" in admin_setting:
-                logger.error(
-                    "Filename is missing - skipping to next admin setting...")
+                logger.error("Filename is missing - skipping to next admin setting...")
                 continue
             filename = admin_setting["filename"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in admin_setting and not admin_setting["enabled"]:
                 logger.info(
                     "Payload for setting file -> {} is disabled. Skipping...".format(
-                        filename)
+                        filename
+                    )
                 )
                 continue
 
             settings_file = self._custom_settings_dir + filename
             if os.path.exists(settings_file):
-
                 description = admin_setting.get("description")
                 if description:
                     logger.info(description)
 
                 # Read the config file:
                 with open(settings_file, "r") as file:
                     file_content = file.read()
 
                 logger.debug(
                     "Replace Placeholder -> {} in file -> {}".format(
                         self._placeholder_values, file_content
                     )
                 )
 
-                file_content = self.replacePlaceholders(
-                    file_content)
+                file_content = self.replacePlaceholders(file_content)
 
                 # Write the updated config file:
                 tmpfile = "/tmp/" + os.path.basename(settings_file)
                 with open(tmpfile, "w") as file:
                     file.write(file_content)
 
                 response = self._otcs.applyConfig(tmpfile)
                 if response and response["results"]["data"]["restart"]:
-                    logger.info(
-                        "A restart of Extended ECM service is required.")
+                    logger.info("A restart of Extended ECM service is required.")
                     restart_required = True
             else:
                 logger.error(
-                    "Admin settings file -> {} not found.".format(settings_file))
+                    "Admin settings file -> {} not found.".format(settings_file)
+                )
 
         return restart_required
 
         # end method definition
 
     def processExternalSystems(self):
         """Process external systems in payload and create them in Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         Side Effects:
             - based on system_type different other settings in the dict are set
             - reachability is tested and a flag is set in the dict are set
         """
 
         for external_system in self._external_systems:
             #
@@ -1679,16 +1945,17 @@
                     "Payload for External System -> {} ({}) is disabled. Skipping...".format(
                         system_name, system_type
                     )
                 )
                 continue
 
             description = (
-                external_system["description"] if external_system.get(
-                    "description") else ""
+                external_system["description"]
+                if external_system.get("description")
+                else ""
             )
 
             # Set the default settings for the different system types:
             match system_type:
                 # Check if we have a SuccessFactors system:
                 case "SuccessFactors":
                     connection_type = "SFInstance"
@@ -1730,20 +1997,23 @@
             as_url = external_system["as_url"]
 
             # Extract the hostname:
             external_system_hostname = urlparse(as_url).hostname
             # Write this information back into the data structure:
             external_system["external_system_hostname"] = external_system_hostname
             # Extract the port:
-            external_system_port = urlparse(
-                as_url).port if urlparse(as_url).port else 80
+            external_system_port = (
+                urlparse(as_url).port if urlparse(as_url).port else 80
+            )
             # Write this information back into the data structure:
             external_system["external_system_port"] = external_system_port
 
-            if self._http_object.checkHostReachable(external_system_hostname, external_system_port):
+            if self._http_object.checkHostReachable(
+                external_system_hostname, external_system_port
+            ):
                 logger.info(
                     "Mark external system -> {} as reachable for later workspace creation...".format(
                         system_name
                     )
                 )
                 external_system["reachable"] = True
             else:
@@ -1798,15 +2068,16 @@
                         else None
                     )
 
             # We do this existance test late in this function to make sure the payload
             # datastructure is properly updated for debugging purposes.
             logger.info(
                 "Test if external system -> {} does already exist...".format(
-                    system_name)
+                    system_name
+                )
             )
             if self._otcs.getExternalSystemConnection(system_name):
                 logger.info(
                     "External System connection -> {} already exists! Skipping to next external system...".format(
                         system_name
                     )
                 )
@@ -1835,16 +2106,15 @@
                 logger.error(
                     "Failed to create external system -> {}; type -> {}".format(
                         system_name, connection_type
                     )
                 )
             else:
                 logger.info(
-                    "Successfully created external system -> {}".format(
-                        system_name)
+                    "Successfully created external system -> {}".format(system_name)
                 )
 
             #
             # 3: Create Authentication Handler for external system:
             #
 
             match system_type:
@@ -1873,27 +2143,23 @@
                         name=system_name,
                         description=description,
                         provider_name=provider_name,
                         saml_url=saml_url,
                         otds_url=otds_sp_endpoint,
                     )
                     if response:
-                        logger.info(
-                            "Successfully added SAML authentication handler.")
+                        logger.info("Successfully added SAML authentication handler.")
                     else:
-                        logger.error(
-                            "Failed to add SAML authentication handler.")
+                        logger.error("Failed to add SAML authentication handler.")
                 case "SAP":
                     # Configure a certificate-based SAP authentication handler:
                     if not "certificate_file" in external_system:
                         logger.error(
-                            "External system -> {}; type -> {}; has a certificate file -> {} but it is missing the certificate password!".format(
-                                system_name,
-                                system_type,
-                                external_system["certificate_file"],
+                            "External system -> {}; type -> {}; is missing the certificate file!".format(
+                                system_name, system_type
                             )
                         )
                         continue
                     if not "certificate_password" in external_system:
                         logger.error(
                             "External system -> {}; type -> {}; has a certificate file -> {} but it is missing the certificate password!".format(
                                 system_name,
@@ -1908,19 +2174,46 @@
                     response = self._otds.addAuthHandlerSAP(
                         name=system_name,
                         description=certificate_description,
                         certificate_file=certificate_file,
                         certificate_password=certificate_password,
                     )
                     if response:
-                        logger.info(
-                            "Successfully added SAP authentication handler.")
+                        logger.info("Successfully added SAP authentication handler.")
                     else:
-                        logger.error(
-                            "Failed to add SAP authentication handler.")
+                        logger.error("Failed to add SAP authentication handler.")
+                    # Upload and enable certificate file for Archive Center that is required for SAP scenarios
+                    # we only do this if the necessary information is in payload and if OTAC is enabled:
+                    if (
+                        "archive_logical_name" in external_system
+                        and "archive_certificate_file" in external_system
+                        and self._otac
+                    ):
+                        logger.info(
+                            "Put certificate file -> {} for logical archive -> {} into Archive Center".format(
+                                external_system["archive_certificate_file"],
+                                external_system["archive_logical_name"],
+                            )
+                        )
+                        response = self._otac.putCert(
+                            external_system["external_system_name"],
+                            external_system["archive_logical_name"],
+                            external_system["archive_certificate_file"],
+                        )
+                        logger.info(
+                            "Enable certificate file -> {} for logical archive -> {}".format(
+                                external_system["archive_certificate_file"],
+                                external_system["archive_logical_name"],
+                            )
+                        )
+                        response = self._otac.enableCert(
+                            external_system["external_system_name"],
+                            external_system["archive_logical_name"],
+                            True,
+                        )
                 case "Salesforce":
                     # Configure an OAuth-based authentication handler:
                     if not "authorization_endpoint" in external_system:
                         logger.error(
                             "Salesforce system -> {} ({}) is missing the authorization endpoint!".format(
                                 system_name,
                                 connection_type,
@@ -1945,30 +2238,30 @@
                         client_secret=oauth_client_secret,
                         active_by_default=False,
                         authorization_endpoint=authorization_endpoint,
                         token_endpoint=token_endpoint,
                         scope_string="id",
                     )
                     if response:
-                        logger.info(
-                            "Successfully added OAuth authentication handler.")
+                        logger.info("Successfully added OAuth authentication handler.")
                     else:
-                        logger.error(
-                            "Failed to add OAuth authentication handler.")
+                        logger.error("Failed to add OAuth authentication handler.")
 
         # end method definition
 
     def processTransportPackages(self, transport_packages: list):
         """Process transport packages in payload and import them to Extended ECM.
 
         Args:
             transport_packages (list): list of transport packages. As we
-                                       have two different lists (transport and
-                                       content_transport) we need a parameter
-        Return: None
+                                       have three different lists (transport,
+                                       content_transport, transport_post) so
+                                       we need a parameter
+        Returns:
+            None
         """
 
         for transport_package in transport_packages:
             if not "name" in transport_package:
                 logger.error(
                     "Transport Package needs a name! Skipping to next transport..."
                 )
@@ -1988,112 +2281,115 @@
                     "Transport Package -> {} needs a URL! Skipping to next transport...".format(
                         name
                     )
                 )
                 continue
             if not "description" in transport_package:
                 logger.warning(
-                    "Transport Package -> {} is missing a description".format(
-                        name)
+                    "Transport Package -> {} is missing a description".format(name)
                 )
             url = transport_package["url"]
             description = transport_package["description"]
 
             # For some transports there can be string replacements
             # configured:
             if "replacements" in transport_package:
                 replacements = transport_package["replacements"]
                 logger.info(
-                    "Deploy transport -> {} with replacements -> {}; URL -> {}".format(description, url, replacements))
-                response = self._otcs.deployTransport(url, name, description, replacements)
-            else:            
+                    "Deploy transport -> {} with replacements -> {}; URL -> {}".format(
+                        description, url, replacements
+                    )
+                )
+                response = self._otcs.deployTransport(
+                    url, name, description, replacements
+                )
+            else:
                 logger.info(
-                    "Deploy transport -> {}; URL -> {}".format(description, url))
+                    "Deploy transport -> {}; URL -> {}".format(description, url)
+                )
                 response = self._otcs.deployTransport(url, name, description)
             if response == None:
                 logger.error(
-                    "Failed to deploy transport -> {}; URL -> {}".format(
-                        name, url)
+                    "Failed to deploy transport -> {}; URL -> {}".format(name, url)
                 )
                 if self._stop_on_error:
                     return
             else:
-                logger.info(
-                    "Successfully deployed transport -> {}".format(name))
+                logger.info("Successfully deployed transport -> {}".format(name))
 
         # end method definition
 
     def processUserPhotos(self):
         """Process user photos in payload and assign them to Extended ECM users.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         # we assume the nickname of the photo item equals the login name of the user
         # we also assume that the photos have been uploaded / transported into the target system
         for user in self._users:
             user_name = user["name"]
+
+            # Check if element has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in user and not user["enabled"]:
+                logger.info(
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
+                )
+                continue
+
             if not "id" in user:
                 logger.error(
                     "User -> {} does not have an ID. The user creation may have failed before. Skipping...".format(
                         user_name
                     )
                 )
                 continue
-            user_id = user["id"]
 
-            # Check if element has been disabled in payload (enabled = false).
-            # In this case we skip the element:
-            if "enabled" in user and not user["enabled"]:
-                logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
-                )
-                continue
+            user_id = user["id"]
 
             response = self._otcs.getNodeFromNickname(user_name)
             if response == None:
                 logger.warning(
                     "Missing photo for user -> {} - nickname not found. Skipping...".format(
                         user_name
                     )
                 )
                 continue
             photo_id = self._otcs.getResultValue(response, "id")
             response = self._otcs.updateUserPhoto(user_id, photo_id)
             if response == None:
-                logger.warning(
-                    "Failed to add photo for user -> {}".format(user_name))
+                logger.warning("Failed to add photo for user -> {}".format(user_name))
             else:
-                logger.info(
-                    "Successfully added photo for user -> {}".format(user_name))
+                logger.info("Successfully added photo for user -> {}".format(user_name))
 
         # Check if Admin has a photo as well (nickname needs to be "admin"):
         response = self._otcs.getNodeFromNickname("admin")
         if response == None:
-            logger.warning(
-                "Missing photo for admin - nickname not found. Skipping...")
+            logger.warning("Missing photo for admin - nickname not found. Skipping...")
             return
         photo_id = self._otcs.getResultValue(response, "id")
         response = self._otcs.updateUserPhoto(1000, photo_id)
         if response == None:
-            logger.warning(
-                "Failed to add photo for admin")
+            logger.warning("Failed to add photo for admin")
         else:
-            logger.info(
-                "Successfully added photo for admin")
+            logger.info("Successfully added photo for admin")
 
         # end method definition
 
     def processUserPhotosM365(self):
         """Process user photos in payload and assign them to Microsoft 365 users.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
         # we assume the nickname of the photo item equals the login name of the user
         # we also assume that the photos have been uploaded / transported into the target system
         for user in self._users:
             user_name = user["name"]
             if not "id" in user:
@@ -2104,36 +2400,47 @@
                 )
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
             if not "enable_o365" in user or not user["enable_o365"]:
                 logger.info(
                     "Office 365 is not enabled in payload for User -> {}. Skipping...".format(
-                        user_name)
+                        user_name
+                    )
                 )
                 continue
             if not "m365_id" in user:
                 logger.error(
                     "Office 365 user -> {} has not been created. Skipping...".format(
-                        user_name)
+                        user_name
+                    )
                 )
                 continue
 
             user_m365_id = user["m365_id"]
 
-            if self._m365.getUserPhoto(user_m365_id):
-                logger.info("User -> {} ({}) has already a photo in Microsoft 365. Skipping...".format(user_name, user_m365_id))
+            if self._m365.getUserPhoto(user_m365_id, show_error=False):
+                logger.info(
+                    "User -> {} ({}) has already a photo in Microsoft 365. Skipping...".format(
+                        user_name, user_m365_id
+                    )
+                )
                 continue
+            else:
+                logger.info(
+                    "User -> {} ({}) has not yet a photo in Microsoft 365. Uploading...".format(
+                        user_name, user_m365_id
+                    )
+                )
 
             response = self._otcs.getNodeFromNickname(user_name)
             if response == None:
                 logger.warning(
                     "Missing photo for user -> {} - nickname not found. Skipping...".format(
                         user_name
                     )
@@ -2141,35 +2448,49 @@
                 continue
             photo_id = self._otcs.getResultValue(response, "id")
             photo_name = self._otcs.getResultValue(response, "name")
             photo_path = "/tmp/" + photo_name
             response = self._otcs.downloadDocument(photo_id, photo_path)
             if response == None:
                 logger.warning(
-                    "Failed to download photo for user -> {} from Extended ECM".format(user_name))
+                    "Failed to download photo for user -> {} from Extended ECM".format(
+                        user_name
+                    )
+                )
             else:
                 logger.info(
-                    "Successfully downloaded photo for user -> {} from Extended ECM to file -> {}".format(user_name, photo_path))
+                    "Successfully downloaded photo for user -> {} from Extended ECM to file -> {}".format(
+                        user_name, photo_path
+                    )
+                )
 
             # Upload photo to M365:
             response = self._m365.updateUserPhoto(user_m365_id, photo_path)
             if response == None:
                 logger.error(
-                    "Failed to upload photo for user -> {} to Microsoft 365".format(user_name))
+                    "Failed to upload photo for user -> {} to Microsoft 365".format(
+                        user_name
+                    )
+                )
             else:
                 logger.info(
-                    "Successfully uploaded photo for user -> {} to Microsoft 365".format(user_name))
+                    "Successfully uploaded photo for user -> {} to Microsoft 365".format(
+                        user_name
+                    )
+                )
 
         # end method definition
 
-    def processWorkspaceTypes(self):
+    def processWorkspaceTypes(self) -> list:
         """Create a data structure for all workspace types in the Extended ECM system.
 
-        Args: None
-        Return: list of workspace types. Each list element is a dict with these values:
+        Args:
+            None
+        Returns:
+            list: list of workspace types. Each list element is a dict with these values:
                 - id (string)
                 - name (string)
                 - templates (list)
                     + name
                     + id
         """
 
@@ -2184,16 +2505,15 @@
         # now we enrich the workspace_type list elments (which are dicts)
         # with additional dict elements for further processing:
         for workspace_type in self._workspace_types:
             workspace_type_id = workspace_type["data"]["properties"]["wksp_type_id"]
             logger.info("Workspace Types ID -> {}".format(workspace_type_id))
             workspace_type["id"] = workspace_type_id
             workspace_type_name = workspace_type["data"]["properties"]["wksp_type_name"]
-            logger.info(
-                "Workspace Types Name -> {}".format(workspace_type_name))
+            logger.info("Workspace Types Name -> {}".format(workspace_type_name))
             workspace_type["name"] = workspace_type_name
             workspace_templates = workspace_type["data"]["properties"]["templates"]
             # Create empty lists of dicts with template names and node IDs:
             workspace_type["templates"] = []
             if workspace_templates:
                 # Determine available templates per workspace type (there can be multiple!)
                 for workspace_template in workspace_templates:
@@ -2209,26 +2529,26 @@
                         "id": workspace_template_id,
                     }
                     workspace_type["templates"].append(template)
 
                     # Workaround for problem with workspace role inheritance
                     # which may be related to Transport or REST API: to work-around this we
                     # push down the workspace roles to the workspace folders explicitly:
-                    response = self._otcs.getWorkspaceRoles(
-                        workspace_template_id)
+                    response = self._otcs.getWorkspaceRoles(workspace_template_id)
 
                     for roles in response["results"]:
                         role_name = roles["data"]["properties"]["name"]
                         role_id = roles["data"]["properties"]["id"]
                         permissions = roles["data"]["properties"]["perms"]
                         # as getWorkspaceRoles() delivers permissions as a value (bit encoded)
                         # we need to convert it to a permissions string list:
                         permission_string_list = (
                             self._otcs.convertPermissionValueToPermissionString(
-                                permissions)
+                                permissions
+                            )
                         )
 
                         logger.info(
                             "Inherit permissions of workspace template -> {} and role -> {} to workspace folders...".format(
                                 workspace_template_name, role_name
                             )
                         )
@@ -2292,34 +2612,38 @@
                 continue
             template_name = workspace_template_registration["workspace_template_name"]
 
             # now we have the template type name and the template name from the
             # payload. We can now proceed to find these items in the workspace types
             # data structure. First we lookup the workspace type:
             workspace_type = next(
-                (item for item in self._workspace_types if item["name"]
-                 == type_name), None
+                (item for item in self._workspace_types if item["name"] == type_name),
+                None,
             )
             if workspace_type is None:
                 logger.error(
-                    "Workspace Type with name -> {} not found.".format(type_name))
+                    "Workspace Type with name -> {} not found.".format(type_name)
+                )
                 continue
 
             # now we use the template list in the workspace type datastructure
             # to find the workspace template:
             workspace_template_list = workspace_type["templates"]
             if workspace_template_list is []:
                 logger.error(
-                    "Workspace Type with name -> {} has no templates.".format(
-                        type_name)
+                    "Workspace Type with name -> {} has no templates.".format(type_name)
                 )
                 continue
 
             workspace_template = next(
-                (item for item in workspace_template_list if item["name"] == template_name),
+                (
+                    item
+                    for item in workspace_template_list
+                    if item["name"] == template_name
+                ),
                 None,
             )
             if workspace_template is None:
                 logger.error(
                     "Workspace Type with name -> {} has no Template with name -> {}.".format(
                         type_name, template_name
                     )
@@ -2329,49 +2653,46 @@
 
             logger.info(
                 "Register workspace template -> {} ({}) with workspace type -> {}".format(
                     template_name, workspace_template_id, type_name
                 )
             )
 
-            response = self._otcs.registerWorkspaceTemplate(
-                workspace_template_id)
+            response = self._otcs.registerWorkspaceTemplate(workspace_template_id)
             if response == None:
                 logger.error(
                     "Failed to register workspace template -> {} with workspace type -> {}".format(
                         template_name, type_name
                     )
                 )
                 continue
 
         # end method definition
 
     def processWorkspaces(self):
         """Process workspaces in payload and create them in Extended ECM.
 
         Args: None
-        Return: None 
+        Return: None
         Side Effects:
             Set workspace["nodeId] to the node ID of the created workspace
         """
 
         for workspace in self._workspaces:
             # Read name from payload:
             if not "name" in workspace:
-                logger.error(
-                    "Workspace needs a name! Skipping to next workspace...")
+                logger.error("Workspace needs a name! Skipping to next workspace...")
                 continue
             name = workspace["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in workspace and not workspace["enabled"]:
                 logger.info(
-                    "Payload for Workspace -> {} is disabled. Skipping...".format(
-                        name)
+                    "Payload for Workspace -> {} is disabled. Skipping...".format(name)
                 )
                 continue
 
             # Read Type Name from payload:
             if not "type_name" in workspace:
                 logger.error(
                     "Workspace -> {} needs a type name! Skipping to next workspace...".format(
@@ -2383,18 +2704,18 @@
 
             # check if the workspace has been created before (effort to make the customizing code idem-potent)
             logger.info(
                 "Check if workspace -> {} of type -> {} does already exist...".format(
                     name, type_name
                 )
             )
-            response = self._otcs.getWorkspaceByNameAndType(
-                name, type_name)
+            response = self._otcs.getWorkspaceByTypeAndName(type_name, name)
             logger.debug(
-                "Search for existing workspace delivered -> {}".format(response))
+                "Search for existing workspace delivered -> {}".format(response)
+            )
             workspace_id = self._otcs.getResultValue(response, "id")
             if workspace_id:
                 # we still want to set the nodeId as other parts of the payload depend on it:
                 workspace["nodeId"] = workspace_id
                 logger.info(
                     "Workspace -> {} of type -> {} does already exist and has ID -> {}! Skipping to next workspace...".format(
                         name, type_name, workspace_id
@@ -2413,21 +2734,19 @@
                 description = ""
             else:
                 description = workspace["description"]
 
             # Parent ID is optional and only required if workspace type does not specify a create location.
             # This is typically the case if it is a nested workspace or workspaces of the same type can be created
             # in different locations in the Enterprise Workspace:
-            parent_id = workspace["parent_id"] if workspace.get(
-                "parent_id") else None
+            parent_id = workspace["parent_id"] if workspace.get("parent_id") else None
 
             if parent_id is not None:
                 parent_workspace = next(
-                    (item for item in self._workspaces if item["id"]
-                     == parent_id), None
+                    (item for item in self._workspaces if item["id"] == parent_id), None
                 )
                 if parent_workspace is None:
                     logger.error(
                         "Parent Workspace with logical ID -> {} not found.".format(
                             parent_id
                         )
                     )
@@ -2448,16 +2767,16 @@
             else:
                 # if no parent_id is specified the workspace location is determined by the workspace type definition
                 # and we pass None as parent ID to the getWorkspaceCreateForm and createWorkspace methods below:
                 parent_workspace_node_id = None
 
             # Find the workspace type with the name given in the payload:
             workspace_type = next(
-                (item for item in self._workspace_types if item["name"]
-                 == type_name), None
+                (item for item in self._workspace_types if item["name"] == type_name),
+                None,
             )
             if workspace_type is None:
                 logger.error(
                     "Workspace Type -> {} not found. Skipping to next workspace.".format(
                         type_name
                     )
                 )
@@ -2615,94 +2934,88 @@
                 # 1. Form for System Attributes (has no role name)
                 # 2. Form for Category Data (role name = "categories")
                 # 3. Form for Classifications (role name = "classifications")
                 # First we extract these 3 forms:
                 for form in forms:
                     if "role_name" in form and form["role_name"] == "categories":
                         categories_form = form
-                        logger.debug(
-                            "Found Categories form -> {}".format(form))
+                        logger.debug("Found Categories form -> {}".format(form))
                         continue
                     if "role_name" in form and form["role_name"] == "classifications":
                         classifications_form = form
-                        logger.debug(
-                            "Found Classification form -> {}".format(form))
+                        logger.debug("Found Classification form -> {}".format(form))
                         continue
                     # the remaining option is that this form is the system attributes form:
                     system_attributes_form = form
-                    logger.debug(
-                        "Found System Attributes form -> {}".format(form))
+                    logger.debug("Found System Attributes form -> {}".format(form))
 
                 # We are just interested in the single category data set (role_name = "categories"):
                 data = categories_form["data"]
                 logger.debug("Categories data found -> {}".format(data))
                 schema = categories_form["schema"]["properties"]
                 logger.debug("Categories schema found -> {}".format(schema))
                 # parallel loop over category data and schema
                 for cat_data, cat_schema in zip(data, schema):
                     logger.info("Category ID -> {}".format(cat_data))
                     data_attributes = data[cat_data]
-                    logger.debug(
-                        "Data Attributes -> {}".format(data_attributes))
+                    logger.debug("Data Attributes -> {}".format(data_attributes))
                     schema_attributes = schema[cat_schema]["properties"]
-                    logger.debug(
-                        "Schema Attributes -> {}".format(schema_attributes))
+                    logger.debug("Schema Attributes -> {}".format(schema_attributes))
                     cat_name = schema[cat_schema]["title"]
                     logger.info("Category name -> {}".format(cat_name))
                     # parallel loop over attribute data and schema
                     # Sets with one (fixed) row have type = object
                     # Multi-value Sets with (multiple) rows have type = array and "properties" in "items" schema
                     # Multi-value attributes have also type = array but NO "properties" in "items" schema
-                    for attr_data, attr_schema in zip(data_attributes, schema_attributes):
+                    for attr_data, attr_schema in zip(
+                        data_attributes, schema_attributes
+                    ):
                         logger.debug("Attribute ID -> {}".format(attr_data))
                         logger.debug(
-                            "Attribute Data -> {}".format(
-                                data_attributes[attr_data])
+                            "Attribute Data -> {}".format(data_attributes[attr_data])
                         )
                         logger.debug(
                             "Attribute Schema -> {}".format(
-                                schema_attributes[attr_schema])
+                                schema_attributes[attr_schema]
+                            )
                         )
                         attr_type = schema_attributes[attr_schema]["type"]
                         logger.debug("Attribute Type -> {}".format(attr_type))
                         if not "title" in schema_attributes[attr_schema]:
                             logger.debug("Attribute has no title - skipping")
                             continue
                         # Check if it is an multi-line set:
                         if attr_type == "array" and (
                             "properties" in schema_attributes[attr_schema]["items"]
                         ):
                             set_name = schema_attributes[attr_schema]["title"]
-                            logger.info(
-                                "Multi-line Set -> {}".format(set_name))
+                            logger.info("Multi-line Set -> {}".format(set_name))
                             set_data_attributes = data_attributes[
                                 attr_data
                             ]  # this is a list []
                             logger.debug(
-                                "Set Data Attributes -> {}".format(
-                                    set_data_attributes)
+                                "Set Data Attributes -> {}".format(set_data_attributes)
                             )
-                            set_schema_attributes = schema_attributes[attr_schema]["items"][
-                                "properties"
-                            ]
+                            set_schema_attributes = schema_attributes[attr_schema][
+                                "items"
+                            ]["properties"]
                             logger.debug(
                                 "Set Schema Attributes -> {}".format(
-                                    set_schema_attributes)
+                                    set_schema_attributes
+                                )
                             )
-                            set_schema_max_rows = schema_attributes[attr_schema]["items"][
-                                "maxItems"
-                            ]
+                            set_schema_max_rows = schema_attributes[attr_schema][
+                                "items"
+                            ]["maxItems"]
                             logger.debug(
-                                "Set Schema Max Rows -> {}".format(
-                                    set_schema_max_rows)
+                                "Set Schema Max Rows -> {}".format(set_schema_max_rows)
                             )
                             set_data_max_rows = len(set_data_attributes)
                             logger.debug(
-                                "Set Data Max Rows -> {}".format(
-                                    set_data_max_rows)
+                                "Set Data Max Rows -> {}".format(set_data_max_rows)
                             )
                             row = 1
                             # it can happen that the payload contains more rows than the
                             # initial rows in the set data structure. In this case we use
                             # a copy of the data structure from row 0 as template...
                             first_row = dict(set_data_attributes[0])
                             # We don't know upfront how many rows of data we will find in payload
@@ -2762,25 +3075,25 @@
                                         )
                                     )
                                     logger.debug(
                                         "Set Attribute Schema -> {} (row -> {})".format(
                                             set_schema_attributes[set_attr_schema], row
                                         )
                                     )
-                                    set_attr_type = set_schema_attributes[set_attr_schema][
-                                        "type"
-                                    ]
+                                    set_attr_type = set_schema_attributes[
+                                        set_attr_schema
+                                    ]["type"]
                                     logger.debug(
                                         "Set Attribute Type -> {} (row -> {})".format(
                                             set_attr_type, row
                                         )
                                     )
-                                    set_attr_name = set_schema_attributes[set_attr_schema][
-                                        "title"
-                                    ]
+                                    set_attr_name = set_schema_attributes[
+                                        set_attr_schema
+                                    ]["title"]
                                     logger.debug(
                                         "Set Attribute Name -> {} (row -> {})".format(
                                             set_attr_name, row
                                         )
                                     )
                                     # Lookup the attribute with the right category, set, attribute name, and row number in payload:
                                     attribute = next(
@@ -2800,16 +3113,17 @@
                                     if attribute is None:
                                         logger.warning(
                                             "Set -> {}, Attribute -> {}, Row -> {} not found in payload.".format(
                                                 set_name, set_attr_name, row
                                             )
                                         )
                                         # need to use row - 1 as index starts with 0 but payload rows start with 1
-                                        set_data_attributes[row -
-                                                            1][set_attr_schema] = ""
+                                        set_data_attributes[row - 1][
+                                            set_attr_schema
+                                        ] = ""
                                     else:
                                         logger.info(
                                             "Set -> {}, Attribute -> {}, Row -> {} found in payload, value -> {}".format(
                                                 set_name,
                                                 set_attr_name,
                                                 row,
                                                 attribute["value"],
@@ -2820,56 +3134,54 @@
                                         set_data_attributes[row - 1][
                                             set_attr_schema
                                         ] = attribute["value"]
                                 row += 1  # continue the while loop with the next row
                         # Check if it is single-line set:
                         elif attr_type == "object":
                             set_name = schema_attributes[attr_schema]["title"]
-                            logger.info(
-                                "Single-line Set -> {}".format(set_name))
+                            logger.info("Single-line Set -> {}".format(set_name))
                             set_data_attributes = data_attributes[attr_data]
                             logger.debug(
-                                "Set Data Attributes -> {}".format(
-                                    set_data_attributes)
+                                "Set Data Attributes -> {}".format(set_data_attributes)
                             )
                             set_schema_attributes = schema_attributes[attr_schema][
                                 "properties"
                             ]
                             logger.debug(
                                 "Set Schema Attributes -> {}".format(
-                                    set_schema_attributes)
+                                    set_schema_attributes
+                                )
                             )
                             for set_attr_data, set_attr_schema in zip(
                                 set_data_attributes, set_schema_attributes
                             ):
                                 logger.debug(
-                                    "Set Attribute ID -> {}".format(set_attr_data))
+                                    "Set Attribute ID -> {}".format(set_attr_data)
+                                )
                                 logger.debug(
                                     "Set Attribute Data -> {}".format(
                                         set_data_attributes[set_attr_data]
                                     )
                                 )
                                 logger.debug(
                                     "Set Attribute Schema -> {}".format(
                                         set_schema_attributes[set_attr_schema]
                                     )
                                 )
                                 set_attr_type = set_schema_attributes[set_attr_schema][
                                     "type"
                                 ]
                                 logger.debug(
-                                    "Set Attribute Type -> {}".format(
-                                        set_attr_type)
+                                    "Set Attribute Type -> {}".format(set_attr_type)
                                 )
                                 set_attr_name = set_schema_attributes[set_attr_schema][
                                     "title"
                                 ]
                                 logger.debug(
-                                    "Set Attribute Name -> {}".format(
-                                        set_attr_name)
+                                    "Set Attribute Name -> {}".format(set_attr_name)
                                 )
                                 # Lookup the attribute with the right category, set and attribute name in payload:
                                 attribute = next(
                                     (
                                         item
                                         for item in categories
                                         if (
@@ -2890,20 +3202,21 @@
                                 else:
                                     logger.info(
                                         "Set -> {}, Attribute -> {} found in payload, value -> {}".format(
                                             set_name, set_attr_name, attribute["value"]
                                         )
                                     )
                                     # Put the value from the payload into data structure
-                                    set_data_attributes[set_attr_data] = attribute["value"]
+                                    set_data_attributes[set_attr_data] = attribute[
+                                        "value"
+                                    ]
                         # It is a plain attribute (not inside a set) or it is a multi-value attribute (not inside a set):
                         else:
                             attr_name = schema_attributes[attr_schema]["title"]
-                            logger.debug(
-                                "Attribute Name -> {}".format(attr_name))
+                            logger.debug("Attribute Name -> {}".format(attr_name))
                             # Lookup the attribute with the right category and attribute name in payload:
                             attribute = next(
                                 (
                                     item
                                     for item in categories
                                     if (
                                         item["name"] == cat_name
@@ -2931,16 +3244,15 @@
                                 # to the data structure. This expects that the payload has the Group Name and not the Group ID
                                 if attr_type == str(11480):
                                     logger.info(
                                         "Attribute -> {} is is of type -> Organizational Unit ({}). Looking up group ID for group name -> {}".format(
                                             attr_name, attr_type, attribute["value"]
                                         )
                                     )
-                                    response = self._otcs.getGroup(
-                                        attribute["value"])
+                                    response = self._otcs.getGroup(attribute["value"])
                                     # retrieve the list of matching group names - should just be 1
                                     group_list = response["data"]
                                     # Make sure we have an exact match:
                                     group = next(
                                         (
                                             item
                                             for item in group_list
@@ -2953,16 +3265,15 @@
                                         group_id = group["id"]
                                         logger.info(
                                             "Group for Organizational Unit -> {} has ID -> {}".format(
                                                 attribute["value"], group_id
                                             )
                                         )
                                         # Put the group ID into data structure
-                                        data_attributes[attr_data] = str(
-                                            group_id)
+                                        data_attributes[attr_data] = str(group_id)
                                     else:
                                         logger.error(
                                             "Group for Organizational Unit -> {} does not exist!".format(
                                                 attribute["value"]
                                             )
                                         )
                                         # Clear the value to avoid workspace create failure
@@ -2973,16 +3284,15 @@
                                 # to lookup the real user ID here:
                                 elif attr_type == "otcs_user_picker":
                                     logger.info(
                                         "Attribute -> {} is is of type -> User Picker ({}). Looking up user ID for user login name -> {}".format(
                                             attr_name, attr_type, attribute["value"]
                                         )
                                     )
-                                    response = self._otcs.getUser(
-                                        attribute["value"])
+                                    response = self._otcs.getUser(attribute["value"])
                                     # retrieve the list of matching group names - should just be 1
                                     user_list = response["data"]
                                     # Make sure we have an exact match:
                                     user = next(
                                         (
                                             item
                                             for item in user_list
@@ -2995,32 +3305,30 @@
                                         user_id = user["id"]
                                         logger.info(
                                             "User -> {} has ID -> {}".format(
                                                 attribute["value"], user_id
                                             )
                                         )
                                         # Put the user ID into data structure
-                                        data_attributes[attr_data] = str(
-                                            user_id)
+                                        data_attributes[attr_data] = str(user_id)
                                     else:
                                         logger.error(
                                             "User with login name -> {} does not exist!".format(
                                                 attribute["value"]
                                             )
                                         )
                                         # Clear the value to avoid workspace create failure
                                         data_attributes[attr_data] = ""
 
                                 else:
                                     # Put the value from the payload into data structure
                                     data_attributes[attr_data] = attribute["value"]
                     category_create_data["categories"][cat_data] = data_attributes
 
-            logger.debug(
-                "Category Create Data -> {}".format(category_create_data))
+            logger.debug("Category Create Data -> {}".format(category_create_data))
 
             # Create the workspace with all provided information:
             response = self._otcs.createWorkspace(
                 template_id,
                 name,
                 description,
                 workspace_type_id,
@@ -3056,16 +3364,15 @@
             if (
                 "rm_classification_path" in workspace
                 and workspace["rm_classification_path"] != []
             ):
                 rm_class_node = self._otcs.getNodeByVolumeAndPath(
                     198, workspace["rm_classification_path"]
                 )
-                rm_class_node_id = self._otcs.getResultValue(
-                    rm_class_node, "id")
+                rm_class_node_id = self._otcs.getResultValue(rm_class_node, "id")
                 if rm_class_node_id:
                     response = self._otcs.assignRMClassification(
                         workspace["nodeId"], rm_class_node_id, False
                     )
                     if response == None:
                         logger.error(
                             "Failed to assign RM classification -> {} ({}) to workspace -> {}".format(
@@ -3084,15 +3391,16 @@
             # Classifications are specified as list of path elements (top-down)
             if (
                 "classification_pathes" in workspace
                 and workspace["classification_pathes"] != []
             ):
                 for classification_path in workspace["classification_pathes"]:
                     class_node = self._otcs.getNodeByVolumeAndPath(
-                        198, classification_path)
+                        198, classification_path
+                    )
                     class_node_id = self._otcs.getResultValue(class_node, "id")
                     if class_node_id:
                         response = self._otcs.assignClassification(
                             workspace["nodeId"], class_node_id, False
                         )
                         if response == None:
                             logger.error(
@@ -3128,16 +3436,15 @@
                 continue
             name = workspace["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in workspace and not workspace["enabled"]:
                 logger.info(
-                    "Payload for Workspace -> {} is disabled. Skipping...".format(
-                        name)
+                    "Payload for Workspace -> {} is disabled. Skipping...".format(name)
                 )
                 continue
 
             # Read relationships from payload:
             if not "relationships" in workspace:
                 logger.info(
                     "Workspace -> {} has no relationships - skipping to next workspace...".format(
@@ -3151,16 +3458,15 @@
             if not "id" in workspace:
                 logger.warning(
                     "Workspace without ID cannot have a relationship - skipping to next workspace..."
                 )
                 continue
 
             workspace_id = workspace["id"]
-            logger.info(
-                "Workspace -> {} has relationships - creating...".format(name))
+            logger.info("Workspace -> {} has relationships - creating...".format(name))
 
             if not "nodeId" in workspace:
                 logger.warning(
                     "Workspace without node ID cannot have a relationship (workspace creation may have failed) - skipping to next workspace..."
                 )
                 continue
             # now determine the actual node IDs of the workspaces (have been created above):
@@ -3170,16 +3476,19 @@
                     workspace_id, workspace_node_id
                 )
             )
 
             for related_workspace_id in workspace["relationships"]:
                 # Find the workspace type with the name given in the payload:
                 related_workspace = next(
-                    (item for item in self._workspaces if item["id"]
-                     == related_workspace_id),
+                    (
+                        item
+                        for item in self._workspaces
+                        if item["id"] == related_workspace_id
+                    ),
                     None,
                 )
                 if related_workspace is None:
                     logger.error(
                         "Related Workspace with logical ID -> {} not found.".format(
                             related_workspace_id
                         )
@@ -3210,22 +3519,25 @@
                 logger.info(
                     "Create Workspace Relationship between workspace node ID -> {} and workspace node ID -> {}".format(
                         workspace_node_id, related_workspace_node_id
                     )
                 )
 
                 # Check if relationship does already exists:
-                response = self._otcs.getWorkspaceRelationships(
-                    workspace_node_id)
+                response = self._otcs.getWorkspaceRelationships(workspace_node_id)
 
                 existing_workspace_relationship = self._otcs.existResultItem(
-                    response, "id", related_workspace_node_id)
+                    response, "id", related_workspace_node_id
+                )
                 if existing_workspace_relationship:
                     logger.info(
-                        "Workspace relationship between workspace ID -> {} and related workspace ID -> {} does already exist. Skipping...".format(workspace_node_id, related_workspace_node_id))
+                        "Workspace relationship between workspace ID -> {} and related workspace ID -> {} does already exist. Skipping...".format(
+                            workspace_node_id, related_workspace_node_id
+                        )
+                    )
                     continue
 
                 response = self._otcs.createWorkspaceRelationship(
                     workspace_node_id, related_workspace_node_id
                 )
                 if response == None:
                     logger.error("Failed to create workspace relationship.")
@@ -3278,30 +3590,60 @@
                 logger.warning(
                     "Workspace without node ID cannot have a members (workspaces creation may have failed) - skipping to next workspace..."
                 )
                 continue
 
             # now determine the actual node IDs of the workspaces (have been created by processWorkspaces()):
             workspace_node_id = workspace["nodeId"]
-            logger.info(
-                "Adding members to workspace with ID -> {} and node Id -> {}".format(
-                    workspace_id, workspace_node_id
-                )
+            workspace_node = self._otcs.getNode(workspace_node_id)
+            workspace_owner_id = self._otcs.getResultValue(
+                workspace_node, "owner_user_id"
             )
+            workspace_owner_name = self._otcs.getResultValue(workspace_node, "owner")
 
-            workspace_roles = self._otcs.getWorkspaceRoles(
-                workspace_node_id)
+            workspace_roles = self._otcs.getWorkspaceRoles(workspace_node_id)
             if workspace_roles == None:
                 logger.info(
                     "Workspace with ID -> {} and node Id -> {} has no roles - skipping to next workspace...".format(
                         workspace_id, workspace_node_id
                     )
                 )
                 continue
 
+            # We don't want the workspace creator to be in the leader role
+            # of automatically created workspaces - this can happen because the
+            # creator gets added to the leader role automatically:
+            leader_role_id = self._otcs.lookupResultValue(
+                workspace_roles, "leader", True, "id"
+            )
+
+            if leader_role_id:
+                leader_role_name = self._otcs.lookupResultValue(
+                    workspace_roles, "leader", True, "name"
+                )
+                response = self._otcs.removeMemberFromWorkspace(
+                    workspace_node_id, leader_role_id, workspace_owner_id, False
+                )
+                if response:
+                    logger.info(
+                        "Removed creator user -> {} ({}) from leader role -> {} ({}) of workspace -> {}".format(
+                            workspace_owner_name,
+                            workspace_owner_id,
+                            leader_role_name,
+                            leader_role_id,
+                            workspace_name,
+                        )
+                    )
+
+            logger.info(
+                "Adding members to workspace with ID -> {} and node ID -> {} defined in payload...".format(
+                    workspace_id, workspace_node_id
+                )
+            )
+
             for member in members:
                 # read user list and role name from payload:
                 member_users = (
                     member["users"] if member.get("users") else []
                 )  # be careful to avoid key errors as users are optional
                 member_groups = (
                     member["groups"] if member.get("groups") else []
@@ -3322,59 +3664,63 @@
                         "Role -> {} of workspace -> {} does not have any members (no users nor groups).".format(
                             member_role_name, workspace_name
                         )
                     )
                     continue
 
                 role_id = self._otcs.lookupResultValue(
-                    workspace_roles, "name", member_role_name, "id")
+                    workspace_roles, "name", member_role_name, "id"
+                )
                 if role_id is None:
                     #    if member_role is None:
                     logger.error(
                         "Workspace -> {} does not have a role with name -> {}".format(
                             workspace_name, member_role_name
                         )
                     )
                     continue
-                logger.info(
-                    "Role -> {} has ID -> {}".format(member_role_name, role_id))
+                logger.info("Role -> {} has ID -> {}".format(member_role_name, role_id))
 
                 # Process users as workspaces members:
                 for member_user in member_users:
                     # find member user in current payload:
                     member_user_id = next(
-                        (item for item in self._users if item["name"]
-                         == member_user), None
+                        (item for item in self._users if item["name"] == member_user),
+                        None,
                     )
                     if member_user_id:
                         user_id = member_user_id["id"]
                     else:
                         # If this didn't work, try to get the member user from OTCS. This covers
                         # cases where the user is system generated or part
                         # of a former payload processing (thus not in the current payload):
                         logger.info(
                             "Member -> {} not found in current payload - check if it exists in OTCS already...".format(
                                 member_user
                             )
                         )
                         existing_user = self._otcs.getUser(member_user)
-                        user_id = self._otcs.getResultValue(
-                            existing_user, "id")
-                        if not user_id:
+                        if (
+                            not existing_user or not existing_user["data"]
+                        ):  # we cannot use getResultValue() here - not a V2 call
                             logger.error(
                                 "Cannot find member user with login -> {}. Skipping...".format(
                                     member_user
                                 )
                             )
                             continue
+                        user_id = existing_user["data"][0][
+                            "id"
+                        ]  # we cannot use getResultValue()here!
 
                     # Add member if it does not yet exists - suppress warning
                     # message if user is already in role:
                     response = self._otcs.addMemberToWorkspace(
-                        workspace_node_id, role_id, user_id, False)
+                        workspace_node_id, role_id, user_id, False
+                    )
                     if response == None:
                         logger.error(
                             "Failed to add user -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_user_id["name"],
                                 user_id,
                                 member_role_name,
                                 workspace_name,
@@ -3389,27 +3735,27 @@
                                 workspace_name,
                             )
                         )
 
                 # Process groups as workspaces members:
                 for member_group in member_groups:
                     member_group_id = next(
-                        (item for item in self._groups if item["name"]
-                         == member_group), None
+                        (item for item in self._groups if item["name"] == member_group),
+                        None,
                     )
                     if member_group_id is None:
                         logger.error(
-                            "Cannot find group with name -> {}".format(
-                                member_group)
+                            "Cannot find group with name -> {}".format(member_group)
                         )
                         continue
                     group_id = member_group_id["id"]
 
                     response = self._otcs.addMemberToWorkspace(
-                        workspace_node_id, role_id, group_id)
+                        workspace_node_id, role_id, group_id
+                    )
                     if response == None:
                         logger.error(
                             "Failed to add group -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_group_id["name"],
                                 group_id,
                                 member_role_name,
                                 workspace_name,
@@ -3421,36 +3767,14 @@
                                 member_group_id["name"],
                                 group_id,
                                 member_role_name,
                                 workspace_name,
                             )
                         )
 
-                # We don't want Admin to be in the leader role
-                # of workspaces - this can happen because the admin
-                # user is the creator of the workspaces and the
-                # creator gets added to the leader role automatically:
-                leader_role_id = self._otcs.lookupResultValue(
-                    workspace_roles, "leader", True, "id")
-
-                if leader_role_id:
-                    leader_role_name = self._otcs.lookupResultValue(
-                        workspace_roles, "leader", True, "name")
-                    response = self._otcs.removeMemberFromWorkspace(
-                        workspace_node_id, leader_role_id, 1000, False
-                    )
-                    if response:
-                        logger.info(
-                            "Removed admin user (1000) from leader role -> {} ({}) of workspace -> {}".format(
-                                leader_role_name,
-                                leader_role_id,
-                                workspace_name,
-                            )
-                        )
-
         # end method definition
 
     def processWebReports(self, web_reports: list):
         """Process web reports in payload and run them in Extended ECM.
 
         Args:
             web_reports (list): list of web reports. As we have two different list (pre and post)
@@ -3470,20 +3794,25 @@
                     )
                 )
                 continue
 
             description = web_report["description"]
 
             if not self._otcs.getNodeFromNickname(nick_name):
-                logger.error("Web Report with nickname -> {} does not exist! Skipping...".format(nick_name))
+                logger.error(
+                    "Web Report with nickname -> {} does not exist! Skipping...".format(
+                        nick_name
+                    )
+                )
                 continue
-                    
+
             # be careful to avoid key errors as Web Report parameters are optional:
-            actual_params = web_report["parameters"] if web_report.get(
-                "parameters") else {}
+            actual_params = (
+                web_report["parameters"] if web_report.get("parameters") else {}
+            )
             formal_params = self._otcs.getWebReportParameters(nick_name)
             if actual_params:
                 logger.info(
                     "Running Web Report -> {} ({}) with parameters -> {} ...".format(
                         nick_name, description, actual_params
                     )
                 )
@@ -3498,15 +3827,16 @@
                     continue
                 lets_continue = False
                 # Check 2: Iterate through the actual parameters given in the payload
                 # and see if there's a matching formal parameter expected by the Web Report:
                 for key, value in actual_params.items():
                     # Check if there's a matching formal parameter defined on the Web Report node:
                     formal_param = next(
-                        (item for item in formal_params if item["parm_name"] == key), None
+                        (item for item in formal_params if item["parm_name"] == key),
+                        None,
                     )
                     if formal_param is None:
                         logger.error(
                             "Web Report -> {} is called with parameter -> {} that is not expected! Skipping...".format(
                                 nick_name, key
                             )
                         )
@@ -3526,30 +3856,30 @@
                             )
                         )
                         lets_continue = True  # we cannot do a "continue" here directly as we are in an inner loop
                 # Did any of the checks fail?
                 if lets_continue:
                     continue
                 # Actual parameters are validated, we can run the Web Report:
-                response = self._otcs.runWebReport(
-                    nick_name, actual_params)
+                response = self._otcs.runWebReport(nick_name, actual_params)
             else:
                 logger.info(
                     "Running Web Report -> {} ({}) without parameters...".format(
                         nick_name, description
                     )
                 )
                 # Check if there's a formal parameter that is mandatory but
                 # does not have a default value:
                 if formal_params:
                     required_param = next(
                         (
                             item
                             for item in formal_params
-                            if (item["mandatory"] == True) and (not item["default_value"])
+                            if (item["mandatory"] == True)
+                            and (not item["default_value"])
                         ),
                         None,
                     )
                     if required_param:
                         logger.error(
                             "Web Report -> {} is called without parameters but has a mandatory parameter -> {} without a default value! Skipping...".format(
                                 nick_name, required_param["parm_name"]
@@ -3560,16 +3890,15 @@
                         logger.debug(
                             "Web Report -> {} does not have a mandatory parameter without a default value!".format(
                                 nick_name
                             )
                         )
                 response = self._otcs.runWebReport(nick_name)
             if response == None:
-                logger.error(
-                    "Failed to run web report -> {}".format(nick_name))
+                logger.error("Failed to run web report -> {}".format(nick_name))
 
         # end method definition
 
     def processCSApplications(self, otcs_object: object = None):
         """Process CS applications in payload and install them in Extended ECM.
         The CS Applications need to be installed in all frontend and backends.
 
@@ -3602,143 +3931,173 @@
                 "Install CS Application -> {} ({})...".format(
                     application_name, application_description
                 )
             )
             response = otcs_object.installCSApplication(application_name)
             if response == None:
                 logger.error(
-                    "Failed to install CS Application -> {}!".format(
-                        application_name)
+                    "Failed to install CS Application -> {}!".format(application_name)
                 )
 
         # end method definition
 
-    def processUserFavoritesAndSettings(self):
-        """Process user favorites and settings in payload and create them in Extended ECM.
-
-        We can only set favorites if we impersonate / authenticate as the user.
-        We also want to make sure that the user is not forced to change the password.
-        The following code (for loop) will change the authenticated user - we need to
-        switch it back to admin user later so we safe the admin credentials for this:
+    def processUserSettings(self):
+        """Process user settings in payload and apply themin OTDS.
+           This includes password settings and user display settings.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Returns:
+            None
         """
 
-        if self._users:
-            # save admin credentials for later switch back to admin user:
-            admin_credentials = self._otcs.credentials()
-
         for user in self._users:
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
 
-            user_password = user["password"]
-
             user_partition = self._otcs.config()["partition"]
             if not user_partition:
-                logger.error(
-                    "User partition not found!"
-                )
+                logger.error("User partition not found!")
 
             # Set the OTDS display name. Extended ECM does not use this but
             # it makes AppWorks display users correctly (and it doesn't hurt)
             # We only set this if firstname _and_ last name are in the payload:
             if "firstname" in user and "lastname" in user:
                 user_display_name = user["firstname"] + " " + user["lastname"]
-                response = self._otds.updateUser(user_partition,
-                                                 user_name,
-                                                 "displayName",
-                                                 user_display_name)
+                response = self._otds.updateUser(
+                    user_partition, user_name, "displayName", user_display_name
+                )
                 if response:
                     logger.info(
                         "Display name for user -> {} has been updated to -> {}".format(
-                            user_name, user_display_name)
+                            user_name, user_display_name
+                        )
                     )
                 else:
                     logger.error(
                         "Display name for user -> {} could not be updated to -> {}".format(
-                            user_name, user_display_name)
+                            user_name, user_display_name
+                        )
                     )
 
             # Don't enforce the user to reset password at first login (settings in OTDS):
             logger.info(
-                "Don't enforce password change for user -> {}...".format(user_name))
-            response = self._otds.updateUser(user_partition,
-                                             user_name,
-                                             "UserMustChangePasswordAtNextSignIn",
-                                             "False")
+                "Don't enforce password change for user -> {}...".format(user_name)
+            )
+            response = self._otds.updateUser(
+                user_partition, user_name, "UserMustChangePasswordAtNextSignIn", "False"
+            )
+
+        # end method definition
+
+    def processUserFavoritesAndProfiles(self):
+        """Process user favorites in payload and create them in Extended ECM.
+           This method also simulates browsing the favorites to populate the
+           widgets on the landing pages and sets personal preferences.
+
+        Args:
+            None
+        Returns:
+            None
+        """
+
+        # We can only set favorites if we impersonate / authenticate as the user.
+        # The following code (for loop) will change the authenticated user - we need to
+        # switch it back to admin user later so we safe the admin credentials for this:
+
+        if self._users:
+            # save admin credentials for later switch back to admin user:
+            admin_credentials = self._otcs.credentials()
+
+        for user in self._users:
+            user_name = user["name"]
+
+            # Check if element has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in user and not user["enabled"]:
+                logger.info(
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
+                )
+                continue
+
+            user_password = user["password"]
 
             # we change the otcs credentials to the user:
             self._otcs.setCredentials(user_name, user_password)
 
             # we re-authenticate as the user:
             logger.info("Authenticate user -> {}...".format(user_name))
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
             if not cookie:
-                logger.error(
-                    "Couldn't authenticate user -> {}".format(user_name))
+                logger.error("Couldn't authenticate user -> {}".format(user_name))
                 continue
 
             # we update the user profile to activate navigation tree:
-            response = self._otcs.updateUserProfile(
-                "conwsNavigationTreeView", True)
+            response = self._otcs.updateUserProfile("conwsNavigationTreeView", True)
             if response is None:
                 logger.warning(
-                    "Profile for user -> {} couldn't be updated!".format(
-                        user_name)
+                    "Profile for user -> {} couldn't be updated!".format(user_name)
                 )
             else:
                 logger.info(
                     "Profile for user -> {} has been updated to enable Workspace Navigation Tree.".format(
                         user_name
                     )
                 )
 
             # we work through the list of favorites defined for the user:
             favorites = user["favorites"]
             for favorite in favorites:
                 # check if favorite is a logical workspace name
                 favorite_item = next(
-                    (item for item in self._workspaces if item["id"]
-                     == favorite), None
+                    (item for item in self._workspaces if item["id"] == favorite), None
                 )
                 is_workspace = False
                 if favorite_item is not None:
                     logger.info(
-                        "Found favorite item (workspace) -> {}".format(
+                        "Found favorite item (workspace) in payload -> {}".format(
                             favorite_item["name"]
                         )
                     )
                     if "nodeId" in favorite_item:
                         favorite_id = favorite_item["nodeId"]
                     else:
                         logger.info(
-                            "Favorite -> {} (workspace) does not have a nodeId - skipping to next favorite...".format(
+                            "Favorite -> {} (workspace) does not have a nodeId in payload - check if it was created by an external systems...".format(
                                 favorite
                             )
                         )
-                        continue
+                        response = self._otcs.getWorkspaceByTypeAndName(
+                            favorite_item["type_name"], favorite_item["name"]
+                        )
+                        favorite_id = self._otcs.getResultValue(response, "id")
+                        if not favorite_id:
+                            logger.warning(
+                                "Workspace of type -> {} and name -> {} does not exist. Cannot create favorite. Skipping...".format(
+                                    favorite_item["type_name"], favorite_item["name"]
+                                )
+                            )
+                            continue
+                        else:
+                            # store ID in payload in case it is used again
+                            favorite_item["nodeId"] = favorite_id
                     is_workspace = True
                 else:
                     # alternatively try to find the item as a nickname:
-                    favorite_item = self._otcs.getNodeFromNickname(
-                        favorite)
-                    favorite_id = self._otcs.getResultValue(
-                        favorite_item, "id")
-#                    if favorite_item is None:
+                    favorite_item = self._otcs.getNodeFromNickname(favorite)
+                    favorite_id = self._otcs.getResultValue(favorite_item, "id")
+                    #                    if favorite_item is None:
                     if favorite_id is None:
                         logger.warning(
                             "Favorite -> {} neither found as workspace ID nor as nickname - skipping to next favorite...".format(
                                 favorite
                             )
                         )
                         continue
@@ -3806,15 +4165,16 @@
             self._otcs.setCredentials(
                 admin_credentials["username"], admin_credentials["password"]
             )
 
             # we re-authenticate as the admin user:
             logger.info(
                 "Authenticate as admin user -> {}...".format(
-                    admin_credentials["username"])
+                    admin_credentials["username"]
+                )
             )
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
 
         # end method definition
 
     def processSecurityClearances(self):
@@ -3841,16 +4201,17 @@
                 clearance_description = ""
             if clearance_level and clearance_name:
                 logger.info(
                     "Creating Security Clearance -> {} : {}".format(
                         clearance_level, clearance_name
                     )
                 )
-                self._otcs.runWebReport("web_report_security_clearance",
-                                        security_clearance)
+                self._otcs.runWebReport(
+                    "web_report_security_clearance", security_clearance
+                )
             else:
                 logger.error(
                     "Cannot create Security Clearance - either level or name is missing!"
                 )
 
         # end method definition
 
@@ -3860,32 +4221,35 @@
         Args: None
         Return: None
         """
 
         for supplemental_marking in self._supplemental_markings:
             code = supplemental_marking.get("code")
 
-            if "enabled" in supplemental_marking and not supplemental_marking["enabled"]:
+            if (
+                "enabled" in supplemental_marking
+                and not supplemental_marking["enabled"]
+            ):
                 logger.info(
                     "Payload for Supplemental Marking -> {} is disabled. Skipping...".format(
                         code
                     )
                 )
                 continue
 
             description = supplemental_marking.get("description")
             if not description:
                 description = ""
             if code:
                 logger.info(
-                    "Creating Supplemental Marking -> {} : {}".format(
-                        code, description)
+                    "Creating Supplemental Marking -> {} : {}".format(code, description)
                 )
                 self._otcs.runWebReport(
-                    "web_report_supplemental_marking", supplemental_marking)
+                    "web_report_supplemental_marking", supplemental_marking
+                )
             else:
                 logger.error(
                     "Cannot create Supplemental Marking - either code or description is missing!"
                 )
 
         # end method definition
 
@@ -3900,24 +4264,24 @@
             user_id = user.get("id")
             user_name = user.get("name")
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name)
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
 
             # Read security clearance from user payload (it is optional!)
             user_security_clearance = user.get("security_clearance")
             if user_id and user_security_clearance:
                 response = self._otcs.assignUserSecurityClearance(
-                    user_id, user_security_clearance)
+                    user_id, user_security_clearance
+                )
 
             # Read supplemental markings from user payload (it is optional!)
             user_supplemental_markings = user.get("supplemental_markings")
             if user_id and user_supplemental_markings:
                 response = self._otcs.assignUserSupplementalMarkings(
                     user_id, user_supplemental_markings
                 )
@@ -3931,66 +4295,84 @@
 
         Args: None
         Return: None
         """
 
         if (
             "records_management_system_settings" in self._records_management_settings
-            and self._records_management_settings["records_management_system_settings"] != ""
+            and self._records_management_settings["records_management_system_settings"]
+            != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["records_management_system_settings"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings[
+                    "records_management_system_settings"
+                ]
+            )
             self._otcs.importRecordsManagementSettings(filename)
 
         if (
             "records_management_codes" in self._records_management_settings
             and self._records_management_settings["records_management_codes"] != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["records_management_codes"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["records_management_codes"]
+            )
             self._otcs.importRecordsManagementCodes(filename)
 
         if (
             "records_management_rsis" in self._records_management_settings
             and self._records_management_settings["records_management_rsis"] != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["records_management_rsis"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["records_management_rsis"]
+            )
             self._otcs.importRecordsManagementRSIs(filename)
 
         if (
             "physical_objects_system_settings" in self._records_management_settings
-            and self._records_management_settings["physical_objects_system_settings"] != ""
+            and self._records_management_settings["physical_objects_system_settings"]
+            != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["physical_objects_system_settings"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["physical_objects_system_settings"]
+            )
             self._otcs.importPhysicalObjectsSettings(filename)
 
         if (
             "physical_objects_codes" in self._records_management_settings
             and self._records_management_settings["physical_objects_codes"] != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["physical_objects_codes"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["physical_objects_codes"]
+            )
             self._otcs.importPhysicalObjectsCodes(filename)
 
         if (
             "physical_objects_locators" in self._records_management_settings
             and self._records_management_settings["physical_objects_locators"] != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["physical_objects_locators"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["physical_objects_locators"]
+            )
             self._otcs.importPhysicalObjectsLocators(filename)
 
         if (
             "security_clearance_codes" in self._records_management_settings
             and self._records_management_settings["security_clearance_codes"] != ""
         ):
-            filename = self._custom_settings_dir + \
-                self._records_management_settings["security_clearance_codes"]
+            filename = (
+                self._custom_settings_dir
+                + self._records_management_settings["security_clearance_codes"]
+            )
             self._otcs.importSecurityClearanceCodes(filename)
 
         # end method definition
 
     def processHolds(self):
         """Process Records Management Holds for Extended ECM users.
 
@@ -4003,57 +4385,58 @@
                 logger.error("Cannot create Hold without a name! Skipping...")
                 continue
             hold_name = hold["name"]
 
             if not "type" in hold:
                 logger.error(
                     "Cannot create Hold -> {} without a type! Skipping...".format(
-                        hold_name)
+                        hold_name
+                    )
                 )
                 continue
             hold_type = hold["type"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in hold and not hold["enabled"]:
                 logger.info(
-                    "Payload for Hold -> {} is disabled. Skipping...".format(
-                        hold_name)
+                    "Payload for Hold -> {} is disabled. Skipping...".format(hold_name)
                 )
                 continue
 
             hold_group = hold.get("group")
             hold_comment = hold.get("comment")
             hold_alternate_id = hold.get("alternate_id")
             hold_date_applied = hold.get("date_applied")
             hold_date_suspend = hold.get("date_to_remove")
 
             if hold_group:
                 # Check if the Hold Group (folder) does already exist.
                 # 2122 is the ID of the "Hold Maintenance" top level
                 # folder in Records Management area that (we hope) will remain
                 # stable:
-                response = self._otcs.getNodeByParentAndName(
-                    2122, hold_group)
+                response = self._otcs.getNodeByParentAndName(2122, hold_group)
                 parent_id = self._otcs.getResultValue(response, "id")
                 if not parent_id:
-                    response = self._otcs.createItem(
-                        2122, "833", hold_group)
+                    response = self._otcs.createItem(2122, "833", hold_group)
                     parent_id = self._otcs.getResultValue(response, "id")
             else:
                 parent_id = 2122
 
             # Holds are special - they ahve folders that cannot be traversed
             # in the normal way - we need to get the whole list of holds and use
             # specialparameters for the existResultItems() method as the REST
             # API calls delivers a results->data->holds structure (not properties)
             response = self._otcs.getRecordsManagementHolds()
-            if self._otcs.existResultItem(response, "HoldName", hold_name, property_name="holds"):
+            if self._otcs.existResultItem(
+                response, "HoldName", hold_name, property_name="holds"
+            ):
                 logger.info(
-                    "Hold -> {} does already exist. Skipping...".format(hold_name))
+                    "Hold -> {} does already exist. Skipping...".format(hold_name)
+                )
                 continue
 
             hold = self._otcs.createRecordsManagementHold(
                 hold_type,
                 hold_name,
                 hold_comment,
                 hold_alternate_id,
@@ -4105,31 +4488,29 @@
             if "group_name" in additional_group_member:
                 group_name = additional_group_member["group_name"]
                 logger.info(
                     "Adding group -> {} to parent group -> {} in OTDS.".format(
                         group_name, parent_group
                     )
                 )
-                response = self._otds.addGroupToParentGroup(
-                    group_name, parent_group)
+                response = self._otds.addGroupToParentGroup(group_name, parent_group)
                 if not response:
                     logger.error(
                         "Failed to add group -> {} to parent group -> {} in OTDS.".format(
                             group_name, parent_group
                         )
                     )
             elif "user_name" in additional_group_member:
                 user_name = additional_group_member["user_name"]
                 logger.info(
                     "Adding user -> {} to group -> {} in OTDS.".format(
                         user_name, parent_group
                     )
                 )
-                response = self._otds.addUserToGroup(
-                    user_name, parent_group)
+                response = self._otds.addUserToGroup(user_name, parent_group)
                 if not response:
                     logger.error(
                         "Failed to add user -> {} to group -> {} in OTDS.".format(
                             user_name, parent_group
                         )
                     )
 
@@ -4171,46 +4552,45 @@
             if "group_name" in additional_access_role_member:
                 group_name = additional_access_role_member["group_name"]
                 logger.info(
                     "Adding group -> {} to access role -> {} in OTDS.".format(
                         group_name, access_role
                     )
                 )
-                response = self._otds.addGroupToAccessRole(
-                    access_role, group_name)
+                response = self._otds.addGroupToAccessRole(access_role, group_name)
                 if not response:
                     logger.error(
                         "Failed to add group -> {} to access role -> {} in OTDS.".format(
                             group_name, access_role
                         )
                     )
             elif "user_name" in additional_access_role_member:
                 user_name = additional_access_role_member["user_name"]
                 logger.info(
                     "Adding user -> {} to access role -> {} in OTDS.".format(
                         user_name, access_role
                     )
                 )
-                response = self._otds.addUserToAccessRole(
-                    access_role, user_name)
+                response = self._otds.addUserToAccessRole(access_role, user_name)
                 if not response:
                     logger.error(
                         "Failed to add user -> {} to access role -> {} in OTDS.".format(
                             user_name, access_role
                         )
                     )
             elif "partition_name" in additional_access_role_member:
                 partition_name = additional_access_role_member["partition_name"]
                 logger.info(
                     "Adding partition -> {} to access role -> {} in OTDS.".format(
                         partition_name, access_role
                     )
                 )
                 response = self._otds.addPartitionToAccessRole(
-                    access_role, partition_name)
+                    access_role, partition_name
+                )
                 if not response:
                     logger.error(
                         "Failed to add partition -> {} to access role -> {} in OTDS.".format(
                             partition_name, access_role
                         )
                     )
 
@@ -4239,15 +4619,16 @@
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in renaming and not renaming["enabled"]:
                 logger.info("Payload for Renaming is disabled. Skipping...")
                 continue
 
             response = self._otcs.renameNode(
-                node_id, renaming["name"], renaming["description"])
+                node_id, renaming["name"], renaming["description"]
+            )
             if not response:
                 logger.error(
                     "Failed to rename node ID -> {} to new name -> {}.".format(
                         node_id, renaming["name"]
                     )
                 )
 
@@ -4260,95 +4641,88 @@
             otcs: OTCS object
             items: list of items to create (need this as parameter as we
                    have multiple lists)
         Return: None
         """
 
         for item in items:
-
             if not "name" in item:
                 logger.error("Item needs a name. Skipping...")
                 continue
             item_name = item["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in item and not item["enabled"]:
                 logger.info(
-                    "Payload for Item -> {} is disabled. Skipping...".format(
-                        item_name)
+                    "Payload for Item -> {} is disabled. Skipping...".format(item_name)
                 )
                 continue
 
             if not "description" in item:
                 item_description = ""
             else:
                 item_description = item["description"]
 
             parent_nickname = item.get("parent_nickname")
             parent_path = item.get("parent_path")
 
             if parent_nickname:
-                parent_node = self._otcs.getNodeFromNickname(
-                    parent_nickname)
+                parent_node = self._otcs.getNodeFromNickname(parent_nickname)
                 parent_id = self._otcs.getResultValue(parent_node, "id")
                 # if not parent_node:
                 if not parent_id:
                     logger.error(
                         "Item -> {} has a parent nickname -> {} that does not exist. Skipping...".format(
                             item_name, parent_nickname
                         )
                     )
                     continue
             else:  # use parent_path and Enterprise Volume
-                parent_node = self._otcs.getNodeByVolumeAndPath(
-                    141, parent_path)
+                parent_node = self._otcs.getNodeByVolumeAndPath(141, parent_path)
                 parent_id = self._otcs.getResultValue(parent_node, "id")
                 if not parent_id:
                     # if not parent_node:
                     logger.error(
                         "Item -> {} has a parent path that does not exist. Skipping...".format(
                             item_name
                         )
                     )
                     continue
 
             original_nickname = item.get("original_nickname")
             original_path = item.get("original_path")
 
             if original_nickname:
-                original_node = self._otcs.getNodeFromNickname(
-                    original_nickname)
+                original_node = self._otcs.getNodeFromNickname(original_nickname)
                 original_id = self._otcs.getResultValue(original_node, "id")
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> {} has a original nickname -> {} that does not exist. Skipping...".format(
                             item_name, original_nickname
                         )
                     )
                     continue
             elif original_path:
-                original_node = self._otcs.getNodeByVolumeAndPath(
-                    141, original_path)
+                original_node = self._otcs.getNodeByVolumeAndPath(141, original_path)
                 original_id = self._otcs.getResultValue(original_node, "id")
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> {} has a original path that does not exist. Skipping...".format(
                             item_name
                         )
                     )
                     continue
             else:
                 original_id = 0
 
             if not "type" in item:
-                logger.error(
-                    "Item -> {} needs a type. Skipping...".format(item_name))
+                logger.error("Item -> {} needs a type. Skipping...".format(item_name))
                 continue
 
             item_type = item.get("type")
             item_url = item.get("url")
 
             # check that we have the required information
             # for the given item type:
@@ -4369,16 +4743,15 @@
                             )
                         )
                         continue
 
             # Check if an item with the same name does already exist.
             # This can also be the case if the python container runs a 2nd time.
             # For this reason we are also not issuing an error but just an info (False):
-            response = self._otcs.getNodeByParentAndName(
-                parent_id, item_name, False)
+            response = self._otcs.getNodeByParentAndName(parent_id, item_name, False)
             if self._otcs.getResultValue(response, "name") == item_name:
                 logger.info(
                     "Item with name -> {} does already exist in parent folder with ID -> {}".format(
                         item_name, parent_id
                     )
                 )
                 continue
@@ -4418,22 +4791,20 @@
                                 apply_to = 2
                             }
 
         Return: None
         """
 
         for permission in permissions:
-
             if (
                 not "path" in permission
                 and not "volume" in permission
                 and not "nickname" in permission
             ):
-                logger.error(
-                    "Item to change permission is not specified. Skipping...")
+                logger.error("Item to change permission is not specified. Skipping...")
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in permission and not permission["enabled"]:
                 logger.info("Payload for Permission is disabled. Skipping...")
                 continue
@@ -4463,20 +4834,18 @@
             if "path" in permission and permission["path"]:
                 path = permission["path"]
                 logger.info(
                     "Found path -> {} in permission definition. Determine node ID...".format(
                         path
                     )
                 )
-                node = self._otcs.getNodeByVolumeAndPath(
-                    volume_type, path)
+                node = self._otcs.getNodeByVolumeAndPath(volume_type, path)
                 node_id = self._otcs.getResultValue(node, "id")
                 if not node_id:
-                    logger.error(
-                        "Path -> {} does not exist. Skipping...".format(path))
+                    logger.error("Path -> {} does not exist. Skipping...".format(path))
                     continue
 
             # Check if "nickname" is in payload and not empty string:
             if "nickname" in permission and permission["nickname"]:
                 nickname = permission["nickname"]
                 logger.info(
                     "Found nickname -> {} in permission definition. Determine node ID...".format(
@@ -4492,15 +4861,18 @@
             # Now we should have a value for node_id:
             if not node_id:
                 logger.error("No node ID found! Skipping permission...")
                 continue
             else:
                 node_name = self._otcs.getResultValue(node, "name")
                 logger.info(
-                    "Found node -> {} with ID -> {} to apply permission to.".format(node_name, node_id))
+                    "Found node -> {} with ID -> {} to apply permission to.".format(
+                        node_name, node_id
+                    )
+                )
 
             if "apply_to" in permission:
                 apply_to = permission["apply_to"]
             else:
                 apply_to = 2  # make item + sub-items the default
 
             # 1. Process Owner Permissions (list canbe empty!)
@@ -4508,47 +4880,52 @@
                 permissions = permission["owner_permissions"]
                 logger.info(
                     "Update owner permissions for item -> {} to -> {}".format(
                         node_id, permissions
                     )
                 )
                 response = self._otcs.assignPermission(
-                    node_id, "owner", 0, permissions, apply_to)
+                    node_id, "owner", 0, permissions, apply_to
+                )
                 if not response:
                     logger.error(
                         "Failed to update owner permissions for item -> {}.".format(
-                            node_id)
+                            node_id
+                        )
                     )
 
             # 2. Process Owner Group Permissions
             if "owner_group_permissions" in permission:
                 permissions = permission["owner_group_permissions"]
                 logger.info(
                     "Update owner group permissions for item -> {} to -> {}".format(
                         node_id, permissions
                     )
                 )
                 response = self._otcs.assignPermission(
-                    node_id, "group", 0, permissions, apply_to)
+                    node_id, "group", 0, permissions, apply_to
+                )
                 if not response:
                     logger.error(
                         "Failed to update group permissions for item -> {}.".format(
-                            node_id)
+                            node_id
+                        )
                     )
 
             # 3. Process Public Permissions
             if "public_permissions" in permission:
                 permissions = permission["public_permissions"]
                 logger.info(
                     "Update public permissions for item -> {} to -> {}".format(
                         node_id, permissions
                     )
                 )
                 response = self._otcs.assignPermission(
-                    node_id, "public", 0, permissions, apply_to)
+                    node_id, "public", 0, permissions, apply_to
+                )
                 if not response:
                     logger.error(
                         "Failed to update public permissions for item -> {}.".format(
                             node_id
                         )
                     )
                     continue
@@ -4632,33 +5009,32 @@
         Args: None
         Return: None
         """
 
         for assignment in self._assignments:
             # Sanity check: we need a subject - it's mandatory:
             if not "subject" in assignment:
-                logger.error(
-                    "Assignment needs a subject! Skipping assignment...")
+                logger.error("Assignment needs a subject! Skipping assignment...")
                 continue
             subject = assignment["subject"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in assignment and not assignment["enabled"]:
                 logger.info(
                     "Payload for Assignment -> {} is disabled. Skipping...".format(
-                        subject)
+                        subject
+                    )
                 )
                 continue
 
             # instruction is optional but we give a warning if they are missing:
             if not "instruction" in assignment:
                 logger.warning(
-                    "Assignment -> {} should have an instruction!".format(
-                        subject)
+                    "Assignment -> {} should have an instruction!".format(subject)
                 )
                 instruction = ""
             else:
                 instruction = assignment["instruction"]
             # Sanity check: we either need users or groups (or both):
             if not "groups" in assignment and not "users" in assignment:
                 logger.error(
@@ -4666,30 +5042,32 @@
                         subject
                     )
                 )
                 continue
             # Check if a workspace is specified for the assignment and check it does exist:
             if "workspace" in assignment and assignment["workspace"]:
                 workspace = next(
-                    (item for item in self._workspaces if item["id"]
-                     == assignment["workspace"]),
+                    (
+                        item
+                        for item in self._workspaces
+                        if item["id"] == assignment["workspace"]
+                    ),
                     None,
                 )
                 if not workspace or not "nodeId" in workspace:
                     logger.error(
                         "Assignment -> {} has specified a not existing workspace -> {}! Skipping assignment...".format(
                             subject, assignment["workspace"]
                         )
                     )
                     continue
                 node_id = workspace["nodeId"]
             # If we don't have a workspace then check if a nickname is specified for the assignment:
             elif "nickname" in assignment:
-                response = self._otcs.getNodeFromNickname(
-                    assignment["nickname"])
+                response = self._otcs.getNodeFromNickname(assignment["nickname"])
                 node_id = self._otcs.getResultValue(response, "id")
                 if not node_id:
                     # if response == None:
                     logger.error(
                         "Assignment item with nickname -> {} not found".format(
                             assignment["nickname"]
                         )
@@ -4706,16 +5084,19 @@
             assignees = []
 
             if "groups" in assignment:
                 group_assignees = assignment["groups"]
                 for group_assignee in group_assignees:
                     # find the group in the group list
                     group = next(
-                        (item for item in self._groups if item["name"]
-                         == group_assignee),
+                        (
+                            item
+                            for item in self._groups
+                            if item["name"] == group_assignee
+                        ),
                         None,
                     )
                     if not group:
                         logger.error(
                             "Assignment group -> {} does not exist! Skipping group...".format(
                                 group_assignee
                             )
@@ -4733,16 +5114,15 @@
                     assignees.append(group_id)
 
             if "users" in assignment:
                 user_assignees = assignment["users"]
                 for user_assignee in user_assignees:
                     # find the user in the user list
                     user = next(
-                        (item for item in self._users if item["name"]
-                         == user_assignee),
+                        (item for item in self._users if item["name"] == user_assignee),
                         None,
                     )
                     if not user:
                         logger.error(
                             "Assignment user -> {} does not exist! Skipping user...".format(
                                 user_assignee
                             )
@@ -4764,88 +5144,92 @@
                     "Cannot add assignment -> {} for node ID -> {} because no assignee was found.".format(
                         subject, node_id
                     )
                 )
                 return
 
             response = self._otcs.assignItemToUserGroup(
-                node_id, subject, instruction, assignees)
+                node_id, subject, instruction, assignees
+            )
             if not response:
                 logger.error(
                     "Failed to add assignment -> {} for node ID -> {} with assignees -> {}.".format(
                         subject, node_id, assignees
                     )
                 )
 
         # end method definition
 
-    def processUserLicenses(self, resource_name: str, license_feature: str, license_name: str ,user_specific_payload_field: str = "license"):
+    def processUserLicenses(
+        self,
+        resource_name: str,
+        license_feature: str,
+        license_name: str,
+        user_specific_payload_field: str = "licenses",
+    ):
         """Assign a specific OTDS license feature to all Extended ECM users.
+           This method is used for OTIV and Extended ECM licenses.
 
         Args:
             resource_name: name of the OTDS resource
             license_feature: license feature to assign to the user (product specific)
-            license_name: Name of the license Key
+            license_name: Name of the license Key (e.g. "EXTENDED_ECM" or "INTELLIGENT_VIEWING")
             user_specific_payload_field: name of the user specific field in payload
                                          (if empty it will be ignored)
         Return: None
         """
 
         otds_resource = self._otds.getResource(resource_name)
         if not otds_resource:
-            logger.error("OTDS Resource -> {} not found. Cannot assign licenses to users.")
+            logger.error(
+                "OTDS Resource -> {} not found. Cannot assign licenses to users."
+            )
             return
 
-        user_partition = self._otcs.config()[
-            "partition"]
+        user_partition = self._otcs.config()["partition"]
         if not user_partition:
-            logger.error(
-                "OTCS user partition not found in OTDS!"
-            )
+            logger.error("OTCS user partition not found in OTDS!")
             return
 
         for user in self._users:
-
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
-                    "Payload for User -> {} is disabled. Skipping...".format(
-                        user_name
-                    )
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
 
             if user_specific_payload_field and user_specific_payload_field in user:
                 logger.info(
                     "Found specific license feature -> {} for User -> {}. Overwriting default license feature -> {}".format(
                         user[user_specific_payload_field], user_name, license_feature
                     )
                 )
                 user_license_feature = user[user_specific_payload_field]
-            else: # use the default feature from the actual parameter
+            else:  # use the default feature from the actual parameter
                 user_license_feature = [license_feature]
 
             for lic_feature in user_license_feature:
                 assigned_license = self._otds.assignUserToLicense(
                     user_partition,
                     user_name,  # we want the plain login name here
                     otds_resource["resourceID"],
                     lic_feature,
-                    license_name
+                    license_name,
                 )
-                
-            if not assigned_license:
-                logger.error(
-                    "Failed to assign license feature -> {} to user -> {}!".format(
-                        license_feature, user["name"]
+
+                if not assigned_license:
+                    logger.error(
+                        "Failed to assign license feature -> {} to user -> {}!".format(
+                            lic_feature, user["name"]
+                        )
                     )
-                )
 
         # end method definition
 
     def processExecPodCommands(self):
         """Process commands that should be executed in the Kubernetes pods.
 
         Args: None
@@ -4859,44 +5243,55 @@
                 )
                 continue
             pod_name = exec_pod_command["pod_name"]
 
             if not "command" in exec_pod_command or not exec_pod_command.get("command"):
                 logger.error(
                     "Pod command is not specified for pod -> {}! It needs to be a non-empty list! Skipping to next pod command...".format(
-                        pod_name)
+                        pod_name
+                    )
                 )
                 continue
             command = exec_pod_command["command"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in exec_pod_command and not exec_pod_command["enabled"]:
                 logger.info(
-                    "Payload for Exec Pod Command in pod -> {} is disabled. Skipping...".format(pod_name))
+                    "Payload for Exec Pod Command in pod -> {} is disabled. Skipping...".format(
+                        pod_name
+                    )
+                )
                 continue
 
             if not "description" in exec_pod_command:
                 logger.info(
-                    "Executing command -> {} in pod -> {}".format(command, pod_name))
+                    "Executing command -> {} in pod -> {}".format(command, pod_name)
+                )
             else:
                 description = exec_pod_command["description"]
                 logger.info(
-                    "Executing command -> {} in pod -> {} ({})".format(command, pod_name, description))
+                    "Executing command -> {} in pod -> {} ({})".format(
+                        command, pod_name, description
+                    )
+                )
 
-            if not "interactive" in exec_pod_command or exec_pod_command["interactive"] == False:
+            if (
+                not "interactive" in exec_pod_command
+                or exec_pod_command["interactive"] == False
+            ):
                 result = self._k8s.execPodCommand(pod_name, command)
             else:
                 if not "timeout" in exec_pod_command:
-                    result = self._k8s.execPodCommandInteractive(
-                        pod_name, command)
+                    result = self._k8s.execPodCommandInteractive(pod_name, command)
                 else:
                     timeout = exec_pod_command["timeout"]
                     result = self._k8s.execPodCommandInteractive(
-                        pod_name, command, timeout)
+                        pod_name, command, timeout
+                    )
 
             if result:
                 logger.info(
                     "Execution of command -> {} in pod -> {} returned result -> {}".format(
                         command, pod_name, result
                     )
                 )
@@ -4907,20 +5302,272 @@
                     "Execution of command -> {} in pod -> {} did not return a result.".format(
                         command, pod_name, result
                     )
                 )
 
         # end method definition
 
-    def initSAP(self, sap_external_system: dict, direct_application_server_login: bool = True) -> object:
+    def processDocumentGenerators(self):
+        """Generate documents for a defined workspace type based on template
+
+        Args:
+            none
+        Returns:
+            none
+        """
+
+        # save admin credentials for later switch back to admin user:
+        admin_credentials = self._otcs.credentials()
+        authenticated_user = "admin"
+
+        for doc_generator in self._doc_generators:
+            if not "workspace_type" in doc_generator:
+                logger.error(
+                    "To generate documents for workspaces the workspace type needs to be specified in the payload! Skipping to next document generator..."
+                )
+                continue
+            workspace_type = doc_generator["workspace_type"]
+
+            if not "template_path" in doc_generator:
+                logger.error(
+                    "To generate documents for workspaces of type -> {} the path to the document template needs to be specified in the payload! Skipping to next document generator...".format(
+                        workspace_type
+                    )
+                )
+                continue
+            template_path = doc_generator["template_path"]
+
+            # Check if element has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in doc_generator and not doc_generator["enabled"]:
+                logger.info(
+                    "Payload for document generator of workspace type -> {} and template path -> {} is disabled. Skipping...".format(
+                        workspace_type, template_path
+                    )
+                )
+                continue
+
+            if not "classification_path" in doc_generator:
+                logger.error(
+                    "To generate documents for workspaces of type -> {} the path to the document classification needs to be specified in the payload! Skipping to next document generator...".format(
+                        workspace_type
+                    )
+                )
+                continue
+            classification_path = doc_generator["classification_path"]
+
+            if not "category_name" in doc_generator:
+                logger.error(
+                    "To generate documents for workspaces of type -> {} the category name needs to be specified in the payload! Skipping to next document generator...".format(
+                        workspace_type
+                    )
+                )
+                continue
+            category_name = doc_generator["category_name"]
+
+            if not "attributes" in doc_generator:
+                logger.error(
+                    "To generate documents for workspaces of type -> {} the attributes needs to be specified in the payload! Skipping to next document generator...".format(
+                        workspace_type
+                    )
+                )
+                continue
+            attributes = doc_generator["attributes"]
+
+            if not "workspace_folder_path" in doc_generator:
+                logger.info(
+                    "No workspace folder path defined for workspaces of type -> {}. Documents will be stored in workspace root.".format(
+                        workspace_type
+                    )
+                )
+                workspace_folder_path = []
+            else:
+                workspace_folder_path = doc_generator["workspace_folder_path"]
+
+            if "exec_as_user" in doc_generator:
+                exec_as_user = doc_generator["exec_as_user"]
+
+                # Find the user in the users payload:
+                exec_user = next(
+                    (item for item in self._users if item["name"] == exec_as_user),
+                    None,
+                )
+                # Have we found the user in the payload?
+                if exec_user is not None:
+                    logger.info(
+                        "Executing document generator with user -> {}".format(
+                            exec_as_user
+                        )
+                    )
+                    # we change the otcs credentials to the user:
+                    self._otcs.setCredentials(exec_user["name"], exec_user["password"])
+
+                    # we re-authenticate as the user:
+                    logger.info("Authenticate user -> {}...".format(exec_as_user))
+                    # True = force new login with new user
+                    cookie = self._otcs.authenticate(True)
+                    if not cookie:
+                        logger.error(
+                            "Couldn't authenticate user -> {}".format(exec_as_user)
+                        )
+                        continue
+                    admin_context = False
+                    authenticated_user = exec_as_user
+                else:
+                    logger.error(
+                        "Cannot find user with login name -> {} for executing. Executing as admin...".format(
+                            exec_as_user
+                        )
+                    )
+                    admin_context = True
+            else:
+                admin_context = True
+
+            if admin_context and authenticated_user != "admin":
+                # Set back admin credentials:
+                self._otcs.setCredentials(
+                    admin_credentials["username"], admin_credentials["password"]
+                )
+
+                # we re-authenticate as the admin user:
+                logger.info(
+                    "Authenticate as admin user -> {}...".format(
+                        admin_credentials["username"]
+                    )
+                )
+                # True = force new login with new user
+                cookie = self._otcs.authenticate(True)
+                authenticated_user = "admin"
+
+            template = self._otcs.getNodeByVolumeAndPath(20541, template_path)
+            template_id = self._otcs.getResultValue(template, "id")
+            template_name = self._otcs.getResultValue(template, "name")
+            classification = self._otcs.getNodeByVolumeAndPath(198, classification_path)
+            classification_id = self._otcs.getResultValue(classification, "id")
+
+            category_id, attribute_definitions = self._otcs.getNodeCategoryDefinition(
+                template_id, category_name
+            )
+            logger.info(
+                "Category ID -> {}, Attribute definitions -> {}".format(
+                    category_id, attribute_definitions
+                )
+            )
+
+            category_data = {str(category_id): {}}
+
+            for attribute in attributes:
+                attribute_name = attribute["name"]
+                attribute_value = attribute["value"]
+                attribute_type = attribute_definitions[attribute_name]["type"]
+                attribute_id = attribute_definitions[attribute_name]["id"]
+
+                # Special treatment for type user: determine the ID for the login name.
+                # the ID is the actual value we have to put in the attribute:
+                if attribute_type == "user":
+                    user = self._otcs.getUser(attribute_value, show_error=True)
+
+                    if not user or not user["data"]:
+                        logger.error(
+                            "Cannot find user with login name -> {}. Skipping...".format(
+                                attribute_value
+                            )
+                        )
+                        continue
+                    attribute_value = user["data"][0]["id"]
+
+                category_data[str(category_id)][attribute_id] = attribute_value
+
+            logger.info(
+                "Generate documents for workspace type -> {} based on template -> {} with metadata -> {}...".format(
+                    workspace_type, template_name, category_data
+                )
+            )
+
+            workspace_instances = self._otcs.getWorkspaceInstances(workspace_type)
+            for workspace_instance in workspace_instances["results"]:
+                workspace_id = workspace_instance["data"]["properties"]["id"]
+                workspace_name = workspace_instance["data"]["properties"]["name"]
+                if workspace_folder_path:
+                    workspace_folder = self._otcs.getNodeByWorkspaceAndPath(
+                        workspace_id, workspace_folder_path
+                    )
+                    if workspace_folder:
+                        workspace_folder_id = self._otcs.getResultValue(
+                            workspace_folder, "id"
+                        )
+                    else:
+                        # If the workspace template is not matching
+                        # the path we may have an error here. Then
+                        # we fall back to workspace root level.
+                        logger.info(
+                            "Folder path does not exist in workspace -> {}. Using workspace root level instead...".format(
+                                workspace_name
+                            )
+                        )
+                        workspace_folder_id = workspace_id
+                else:
+                    workspace_folder_id = workspace_id
+
+                document_name = workspace_name + " - " + template_name
+
+                response = self._otcs.checkNodeName(workspace_folder_id, document_name)
+                if response["results"]:
+                    logger.warning(
+                        "Node with name -> {} does already exist in workspace folder with ID -> {}".format(
+                            document_name, workspace_folder_id
+                        )
+                    )
+                    continue
+                response = self._otcs.createDocumentFromTemplate(
+                    template_id,
+                    workspace_folder_id,
+                    classification_id,
+                    category_data,
+                    document_name,
+                    "This document has been auto-generated by Terrarium",
+                )
+                if not response:
+                    logger.error(
+                        "Failed to generate document -> {} in workspace -> {}".format(
+                            document_name, workspace_name
+                        )
+                    )
+                else:
+                    logger.info(
+                        "Successfully generated document -> {} in workspace -> {}".format(
+                            document_name, workspace_name
+                        )
+                    )
+
+        if authenticated_user != "admin":
+            # Set back admin credentials:
+            self._otcs.setCredentials(
+                admin_credentials["username"], admin_credentials["password"]
+            )
+
+            # we authenticate back as the admin user:
+            logger.info(
+                "Authenticate as admin user -> {}...".format(
+                    admin_credentials["username"]
+                )
+            )
+            # True = force new login with new user
+            cookie = self._otcs.authenticate(True)
+
+        # end method definition
+
+    def initSAP(
+        self, sap_external_system: dict, direct_application_server_login: bool = True
+    ) -> object:
         """Initialize SAP object for RFC communication with SAP S/4HANA.
 
         Args:
             sap_external_system (dictionary): SAP external system created before
-            direct_application_server_login (boolean): flag to control wether we comminicate directly with 
+            direct_application_server_login (boolean): flag to control wether we comminicate directly with
                                                        SAP application server or via a load balancer
         Return: sap_object
         """
 
         if not sap_external_system:
             return None
 
@@ -4928,52 +5575,49 @@
         password = sap_external_system["password"]
         # "external_system_hostname" is extracted from as_url in processExternalSystems()
         host = sap_external_system["external_system_hostname"]
         client = sap_external_system.get("client", "100")
         system_number = sap_external_system.get("external_system_number", "00")
         system_id = sap_external_system["external_system_name"]
         group = sap_external_system.get("group", "PUBLIC")
-        destination = sap_external_system.get(
-            "destination", "")
+        destination = sap_external_system.get("destination", "")
 
         logger.info("Connection parameters SAP:")
         logger.info("SAP Hostname             = " + host)
         logger.info("SAP Client               = " + client)
         logger.info("SAP System Number        = " + system_number)
         logger.info("SAP System ID            = " + system_id)
         logger.info("SAP User Name            = " + username)
         if not direct_application_server_login:
             logger.info("SAP Group Name (for RFC) = " + group)
         if destination:
             logger.info("SAP Destination          = " + destination)
 
         if direct_application_server_login:
-            logger.info(
-                "SAP Login                = Direct Application Server (ashost)")
+            logger.info("SAP Login                = Direct Application Server (ashost)")
             sap_object = sap.SAP(
                 username=username,
                 password=password,
                 ashost=host,
                 client=client,
                 system_number=system_number,
                 system_id=system_id,
-                destination=destination
+                destination=destination,
             )
         else:
-            logger.info(
-                "SAP Login                = Logon with load balancing (mshost)")
+            logger.info("SAP Login                = Logon with load balancing (mshost)")
             sap_object = sap.SAP(
                 username=username,
                 password=password,
                 mshost=host,
                 group=group,
                 client=client,
                 system_number=system_number,
                 system_id=system_id,
-                destination=destination
+                destination=destination,
             )
 
         return sap_object
 
         # end method definition
 
     def processSAPRFCs(self, sap_object: object):
@@ -4988,54 +5632,53 @@
             rfc_name = sap_rfc["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in sap_rfc and not sap_rfc["enabled"]:
                 logger.info(
                     "Payload for SAP RFC -> {} is disabled. Skipping...".format(
-                        rfc_name)
+                        rfc_name
+                    )
                 )
                 continue
 
-            rfc_description = sap_rfc["description"] if sap_rfc.get(
-                "description") else ""
+            rfc_description = (
+                sap_rfc["description"] if sap_rfc.get("description") else ""
+            )
 
             # be careful to avoid key errors as SAP RFC parameters are optional:
-            rfc_params = sap_rfc["parameters"] if sap_rfc.get(
-                "parameters") else {}
+            rfc_params = sap_rfc["parameters"] if sap_rfc.get("parameters") else {}
             if rfc_params:
                 logger.info(
                     "Calling SAP RFC -> {} ({}) with parameters -> {} ...".format(
                         rfc_name, rfc_description, rfc_params
                     )
                 )
             else:
                 logger.info(
                     "Calling SAP RFC -> {} ({}) without parameters...".format(
                         rfc_name, rfc_description
                     )
                 )
 
             # be careful to avoid key errors as SAP RFC parameters are optional:
-            rfc_call_options = sap_rfc["call_options"] if sap_rfc.get(
-                "call_options") else {}
+            rfc_call_options = (
+                sap_rfc["call_options"] if sap_rfc.get("call_options") else {}
+            )
             if rfc_call_options:
-                logger.info(
-                    "Using call options -> {} ...".format(
-                        rfc_call_options
-                    )
-                )
+                logger.debug("Using call options -> {} ...".format(rfc_call_options))
 
             result = sap_object.call(rfc_name, rfc_call_options, rfc_params)
             if result == None:
                 logger.error("Failed to call SAP RFC -> {}".format(rfc_name))
             else:
                 logger.info(
                     "Successfully called RFC -> {}. Result -> {}".format(
-                        rfc_name, result)
+                        rfc_name, result
+                    )
                 )
 
         # end method definition
 
     def getPayload(self) -> dict:
         return self._payload
 
@@ -5057,8 +5700,8 @@
     def getOTDS(self) -> object:
         return self._otds
 
     def getK8S(self) -> object:
         return self._k8s
 
     def getM365(self) -> object:
-        return self._m365
+        return self._m365
```

### Comparing `pyxecm-0.0.16/pyxecm/sap.py` & `pyxecm-0.0.17/pyxecm/sap.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,22 @@
 
 import os
 import logging
 
 
 global rfc_available
 try:
-  import pyrfc
-  pyrfc_available=True
+    import pyrfc
+
+    pyrfc_available = True
 except ModuleNotFoundError:
-  logging.error("pyrfc could not be loaded, SAP integration impatcted")
-  pyrfc_available=False
-  pass
-  
+    logging.error("pyrfc could not be loaded, SAP integration impatcted")
+    pyrfc_available = False
+    pass
+
 from datetime import datetime
 
 # Configure Kubernetes API authentication to use pod serviceAccount
 # config.load_incluster_config()
 
 logger = logging.getLogger(os.path.basename(__file__))
 
@@ -88,16 +89,15 @@
             "client": client,
             "trace": trace,
             "lang": lang,
         }
 
         # see https://sap.github.io/PyRFC/pyrfc.html#connection
         if ashost:
-            logger.info(
-                "Logon with application server logon: requiring ashost, sysnr")
+            logger.info("Logon with application server logon: requiring ashost, sysnr")
             self._connection_parameters["ashost"] = ashost
             self._connection_parameters["sysnr"] = system_number
             self._connection_parameters["sysid"] = system_id
         elif mshost:
             logger.info(
                 "Logon with load balancing: requiring mshost, msserv, sysid, group"
             )
@@ -107,42 +107,42 @@
             self._connection_parameters["group"] = group
 
         if destination:
             self._connection_parameters["dest"] = destination
 
         # end method definition
 
-    def call(self, rfc_name: str, options: dict = {}, rfc_parameters: dict = {}) -> dict:
+    def call(
+        self, rfc_name: str, options: dict = {}, rfc_parameters: dict = {}
+    ) -> dict:
         """Do an RFC Call. See http://sap.github.io/PyRFC/pyrfc.html#pyrfc.Connection.call
 
         Args:
             rfc_name (string): this is the name of the RFC (typical in capital letters), e.g. SM02_ADD_MESSAGE
-            options (dict, optional) the call options for the RFC call. Defaults to {}.
+            options (dictionary, optional): the call options for the RFC call. Defaults to {}.
             * not_requested: Allows to deactivate certain parameters in the function module interface.
               This is particularly useful for BAPIs which have many large tables, the Python client is not interested in.
               Deactivate those, to reduce network traffic and memory consumption in your application considerably.
               This functionality can be used for input and output parameters. If the parameter is an input,
               no data for that parameter will be sent to the backend. If it’s an output, the backend will be
               informed not to return data for that parameter.
             * timeout: Cancel RFC connection if ongoing RFC call not completed within timeout seconds.
-              Timeout can be also set as client connection configuration option, in which case is valid for all RFC calls.            
-            rfc_parameters (dict, optional): the actual RFC parameters thatare specific for
-                                             the type of the call. Defaults to {}.
+              Timeout can be also set as client connection configuration option, in which case is valid for all RFC calls.
+            rfc_parameters (dictionary, optional): the actual RFC parameters thatare specific for
+                                                   the type of the call. Defaults to {}.
         Returns:
-            dict: Result of the RFC call or None if the call fails or timeouts.
+            dictionary: Result of the RFC call or None if the call fails or timeouts.
         """
 
         # Create the connection object and call the RFC function
         params = self._connection_parameters
-        logger.info("Connection Parameters -> {}".format(params))
+        logger.debug("Connection Parameters -> {}".format(params))
 
         try:
             with pyrfc.Connection(**params) as conn:
                 result = conn.call(rfc_name, options=options, **rfc_parameters)
                 return result
         except pyrfc.RFCError as e:
-            logger.error(
-                "Failed to call RFC -> {}; error -> {}".format(rfc_name, e))
+            logger.error("Failed to call RFC -> {}; error -> {}".format(rfc_name, e))
             return None
 
         # end method definition
-
```

### Comparing `pyxecm-0.0.16/pyxecm/translate.py` & `pyxecm-0.0.17/pyxecm/translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,87 @@
+__author__ = "Dr. Marc Diefenbruch"
+__copyright__ = "Copyright 2023, OpenText"
+__credits__ = ["Kai-Philip Gatzweiler"]
+__maintainer__ = "Dr. Marc Diefenbruch"
+__email__ = "mdiefenb@opentext.com"
+
 import requests
 import logging
-import os 
+import os
 
 logger = logging.getLogger(os.path.basename(__file__))
 
+
 class Translator:
     _config = None
     _headers = None
 
     def __init__(self, api_key: str, project_key: str = "", domain: str = ""):
-
         translateConfig = {}
 
         translateConfig["apiKey"] = api_key
-        translateConfig["translateUrlV2"] = "https://translation.googleapis.com/language/translate/v2"
-        translateConfig["translateUrlV3"] = "https://translation.googleapis.com/v3/projects/{}:translateText".format(project_key)
+        translateConfig[
+            "translateUrlV2"
+        ] = "https://translation.googleapis.com/language/translate/v2"
+        translateConfig[
+            "translateUrlV3"
+        ] = "https://translation.googleapis.com/v3/projects/{}:translateText".format(
+            project_key
+        )
         translateConfig["project"] = project_key
         translateConfig["parent"] = "projects/{}/locations/global".format(project_key)
         translateConfig["model"] = f'nmt{":{}".format(domain) if domain else ""}'
 
         self._headers = {
             "Authorization": f"Bearer {api_key}",
-            "Content-Type": "application/json; charset=utf-8"
+            "Content-Type": "application/json; charset=utf-8",
         }
 
         self._config = translateConfig
 
     def config(self):
         return self._config
 
     def translate(self, source_language: str, target_language: str, text: str) -> str:
         params = {
             "key": self.config()["apiKey"],
             "q": text,
             "source": source_language,
-            "target": target_language
+            "target": target_language,
         }
 
         request_url = self.config()["translateUrlV2"]
 
         response = requests.post(request_url, params=params)
 
         if response.status_code != 200:
             logger.error("Failed to translate text -> {}".format(response.content))
             return None
 
-        translated_text = response.json()['data']['translations'][0]['translatedText']
+        translated_text = response.json()["data"]["translations"][0]["translatedText"]
 
         return translated_text
-    
+
+    # end method definition
+
     def translateV3(self, source_language: str, target_language: str, text: str) -> str:
         data = {
             "source_language_code": source_language,
             "target_language_code": target_language,
             "contents": [text],
-#            "parent": self._parent
+            #            "parent": self._parent
         }
 
         request_header = self._headers
         request_url = self.config()["translateUrlV3"]
 
         response = requests.post(request_url, headers=request_header, json=data)
 
         if response.status_code != 200:
             logger.error("Failed to translate text -> {}".format(response.content))
             return None
 
-        translated_text = response.json()['data']['translations'][0]['translatedText']
+        translated_text = response.json()["data"]["translations"][0]["translatedText"]
 
         return translated_text
-    
+
+    # end method definition
```

### Comparing `pyxecm-0.0.16/pyxecm/web.py` & `pyxecm-0.0.17/pyxecm/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,22 +39,20 @@
 
     def checkHostReachable(self, hostname: str, port: int = 80) -> bool:
         """Check if a server / web address is reachable
 
         Args:
             hostname (string): endpoint hostname
             port (integer): endpoint port
-
-        Result: True is reachable, False otherwise
+        Results:
+            boolean: True is reachable, False otherwise
         """
 
         logger.info(
-            "Test if host -> {} is reachable on port -> {} ...".format(
-                hostname, port
-            )
+            "Test if host -> {} is reachable on port -> {} ...".format(hostname, port)
         )
         try:
             socket.getaddrinfo(hostname, port)
         except socket.gaierror as e:
             logger.warning(
                 "Address-related error - cannot reach host -> {}; error -> {}".format(
                     hostname, e
@@ -65,32 +63,34 @@
             logger.warning(
                 "Connection error - cannot reach host -> {}; error -> {}".format(
                     hostname, e
                 )
             )
             return False
         else:
-            logger.info(
-                "Host is reachable at -> {}:{}".format(hostname, port))
+            logger.info("Host is reachable at -> {}:{}".format(hostname, port))
             return True
 
+    # end method definition
 
-    def httpRequest(self, url: str, method: str = "POST", payload: dict = {}, headers: dict = {}):
-
+    def httpRequest(
+        self, url: str, method: str = "POST", payload: dict = {}, headers: dict = {}
+    ):
         if not headers:
             headers = requestHeaders
 
         logger.info(
             "Make HTTP Request to URL -> {} using -> {} method with payload -> {}".format(
                 url, method, payload
             )
         )
 
         httpRequestResponse = requests.request(
-            method=method, url=url, data=payload, headers=headers)
+            method=method, url=url, data=payload, headers=headers
+        )
 
         if not httpRequestResponse.ok:
             logger.error(
                 "HTTP request -> {} to url -> {} failed; error -> {}".format(
                     method, httpRequestResponse.text
                 )
             )
```

### Comparing `pyxecm-0.0.16/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.17/pyxecm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.16
-Summary: A library to connect to Opentext Extended ECM
+Version: 0.0.17
+Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYXECM
 
-A python library to connect to Opentext Extended ECM
+A python library to interact with Opentext Extended ECM REST API.
+API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

