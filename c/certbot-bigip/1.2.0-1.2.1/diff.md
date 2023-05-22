# Comparing `tmp/certbot-bigip-1.2.0.tar.gz` & `tmp/certbot-bigip-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-bigip-1.2.0.tar", last modified: Thu Jan 26 12:57:36 2023, max compression
+gzip compressed data, was "certbot-bigip-1.2.1.tar", last modified: Mon May 22 13:20:16 2023, max compression
```

## Comparing `certbot-bigip-1.2.0.tar` & `certbot-bigip-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/certbot_bigip/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/certbot_bigip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/certbot_bigip/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/certbot_bigip/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/certbot_bigip/obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/certbot_bigip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-26 12:57:36.000000 certbot-bigip-1.2.0/certbot_bigip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 12:57:36.695255 certbot-bigip-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/tests/test_bigip_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-01-26 12:57:26.000000 certbot-bigip-1.2.0/tests/test_shellcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/certbot_bigip/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/certbot_bigip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/certbot_bigip/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/certbot_bigip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/certbot_bigip/obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/certbot_bigip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 13:20:16.000000 certbot-bigip-1.2.1/certbot_bigip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:20:16.219155 certbot-bigip-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/tests/test_bigip_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-22 13:20:01.000000 certbot-bigip-1.2.1/tests/test_shellcommands.py
```

### Comparing `certbot-bigip-1.2.0/PKG-INFO` & `certbot-bigip-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: certbot-bigip
-Version: 1.2.0
+Version: 1.2.1
 Summary: F5 BIG-IP plugin for Certbot
 Author: Certbot Team @ Open Networks
 Author-email: certbot@on.at
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # certbot-bigip
 
 ## Requirements
 
 see certbot rquirements: <https://certbot.eff.org/docs/install.html#system-requirements>
@@ -31,14 +36,18 @@
   * The LetsEncrypt Chain needs to be at /Common/chain_Letsencrypt and in every other partition that uses this plugin. ( f.e.: /Partition/chain_Letsencrypt)
       At the moment, the plugin checks if a corresponding certificate/chain is located in the same partition/folder as the clientssl profile that uses it.
   * clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
   * F5 SW version 14.x and higher
 
 ## Install
 
+`pip install certbot-bigip`
+
+by installing the plugin you will also install all missing dependencies including certbot.
+
 ## Supported Features
 
 * verifies the domain via HTTP01 (challenge verification implemented through an iRule)
 * Partitions and iApps
 * Standalone and HA setups (Active/Standby, Active/Active)
 * Creates the clientssl profile and attaches the certificate, key and chain
   * Does not modify the clientssl profile if it already exists
@@ -125,15 +134,15 @@
 fi
 ```
 
 The first call only validates and renews the certificate through ```certonly``` parameter and the ```cert-test.sh``` compares the local certificate to the certificate delivered by the F5. If these don't match the second certbot call will skip the validation (as the certificate got already renewed) and install the certificate onto the F5.
 
 ## Testing
 
-> :warning: Currently only integration tests are supported. Therefore a bigip is needed. to run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
+> :warning: Currently only integration tests are supported. Therefore a bigip is needed. To run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
 
 ### Prerequisites
 
 1. Connection to the bigip under test from the machine running the tests
 2. clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
 3. Configure the tests using the following environment variables:
```

### Comparing `certbot-bigip-1.2.0/README.md` & `certbot-bigip-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,18 @@
   * The LetsEncrypt Chain needs to be at /Common/chain_Letsencrypt and in every other partition that uses this plugin. ( f.e.: /Partition/chain_Letsencrypt)
       At the moment, the plugin checks if a corresponding certificate/chain is located in the same partition/folder as the clientssl profile that uses it.
   * clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
   * F5 SW version 14.x and higher
 
 ## Install
 
+`pip install certbot-bigip`
+
+by installing the plugin you will also install all missing dependencies including certbot.
+
 ## Supported Features
 
 * verifies the domain via HTTP01 (challenge verification implemented through an iRule)
 * Partitions and iApps
 * Standalone and HA setups (Active/Standby, Active/Active)
 * Creates the clientssl profile and attaches the certificate, key and chain
   * Does not modify the clientssl profile if it already exists
@@ -102,15 +106,15 @@
 fi
 ```
 
 The first call only validates and renews the certificate through ```certonly``` parameter and the ```cert-test.sh``` compares the local certificate to the certificate delivered by the F5. If these don't match the second certbot call will skip the validation (as the certificate got already renewed) and install the certificate onto the F5.
 
 ## Testing
 
-> :warning: Currently only integration tests are supported. Therefore a bigip is needed. to run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
+> :warning: Currently only integration tests are supported. Therefore a bigip is needed. To run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
 
 ### Prerequisites
 
 1. Connection to the bigip under test from the machine running the tests
 2. clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
 3. Configure the tests using the following environment variables:
```

### Comparing `certbot-bigip-1.2.0/certbot_bigip/configurator.py` & `certbot-bigip-1.2.1/certbot_bigip/configurator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,111 @@
-"""Certbot Bigip plugin."""
+'''Certbot Bigip plugin.'''
 import logging
 import os
 import sys
 import time
 from collections import defaultdict
 
-import zope.interface
 from acme import challenges
 
 from certbot import errors
 from certbot import interfaces
 from certbot.plugins import common
 
 from . import constants
 from . import obj
 
 # create a logging format
-formatter = logging.Formatter("[%(asctime)s] [%(levelname)8s] [%(name)30s] %(message)s")
+formatter = logging.Formatter('[%(asctime)s] [%(levelname)8s] [%(name)30s] %(message)s')
 
 streamhandler = logging.StreamHandler()
 streamhandler.setLevel(logging.DEBUG)
 
-logging.getLogger("certbot_bigip").addHandler(streamhandler)
+logging.getLogger('certbot_bigip').addHandler(streamhandler)
 logger = logging.getLogger(__name__)
 
 
-@zope.interface.implementer(interfaces.IAuthenticator, interfaces.IInstaller)
-@zope.interface.provider(interfaces.IPluginFactory)
-class BigipConfigurator(common.Plugin):
-    """Configurator for BigIP. Deploys certificates to ssl profiles in BigIp."""
+class BigipConfigurator(common.Configurator):
+    '''Configurator for BigIP. Deploys certificates to ssl profiles in BigIp.'''
 
-    description = "F5 BIG-IP - beta!"
+    description = 'F5 BIG-IP - beta!'
 
     @classmethod
     def add_parser_arguments(cls, add):
-        """Defines Commandline Arguments for the plugin.
+        '''Defines Commandline Arguments for the plugin.
         beware that the full name of the argument will be `--certbot-bigip:bigip-<ARGUMENT-NAME>`
         ie. `username` is set with `--certbot-bigip:bigip-username`
-        """
+        '''
         add(
-            "list",
-            metavar="bigip1,bigip2",
-            default=constants.CLI_DEFAULTS["bigip_list"],
-            help="CSV list of BIG-IP system hostnames or addresses, all have to be in the same cluster",
+            'list',
+            metavar='bigip1,bigip2',
+            default=constants.CLI_DEFAULTS['bigip_list'],
+            help='CSV list of BIG-IP system hostnames or addresses, all have to be in the same cluster',
         )
         add(
-            "username",
-            metavar="USERNAME",
-            default=constants.CLI_DEFAULTS["bigip_username"],
-            help="BIG-IP username (common to all listed BIG-IP systems)",
+            'username',
+            metavar='USERNAME',
+            default=constants.CLI_DEFAULTS['bigip_username'],
+            help='BIG-IP username (common to all listed BIG-IP systems)',
         )
         add(
-            "password",
-            metavar="PASSWORD",
-            default=constants.CLI_DEFAULTS["bigip_password"],
-            help="BIG-IP password (common to all listed BIG-IP systems)",
+            'password',
+            metavar='PASSWORD',
+            default=constants.CLI_DEFAULTS['bigip_password'],
+            help='BIG-IP password (common to all listed BIG-IP systems)',
         )
         add(
-            "partition",
-            metavar="PartitionName",
-            default=constants.CLI_DEFAULTS["bigip_partition"],
-            help="BIG-IP partition (common to all listed BIG-IP systems)",
+            'partition',
+            metavar='PartitionName',
+            default=constants.CLI_DEFAULTS['bigip_partition'],
+            help='BIG-IP partition (common to all listed BIG-IP systems)',
         )
         add(
-            "iapp",
-            metavar="Application Service Name",
-            default=constants.CLI_DEFAULTS["bigip_iapp"],
-            help="BIG-IP partition (common to all listed BIG-IP systems)",
+            'iapp',
+            metavar='Application Service Name',
+            default=constants.CLI_DEFAULTS['bigip_iapp'],
+            help='BIG-IP partition (common to all listed BIG-IP systems)',
         )
         add(
-            "vs-list",
-            metavar="vs1,vs2,vs3",
-            default=constants.CLI_DEFAULTS["virtual_server_list"],
-            help="CSV list of BIG-IP virtual server names, optionally including partition",
+            'vs-list',
+            metavar='vs1,vs2,vs3',
+            default=constants.CLI_DEFAULTS['virtual_server_list'],
+            help='CSV list of BIG-IP virtual server names, optionally including partition',
         )
         add(
-            "clientssl-parent",
-            metavar="/Partition/Profile",
-            default=constants.CLI_DEFAULTS["bigip_clientssl_parent"],
-            help="Client SSL parent profile to inherit default values from",
+            'clientssl-parent',
+            metavar='/Partition/Profile',
+            default=constants.CLI_DEFAULTS['bigip_clientssl_parent'],
+            help='Client SSL parent profile to inherit default values from',
         )
         add(
-            "device-group",
-            metavar="sync-failover",
-            default=constants.CLI_DEFAULTS["bigip_device_group"],
-            help="Device Group to syncronise configuration",
+            'device-group',
+            metavar='sync-failover',
+            default=constants.CLI_DEFAULTS['bigip_device_group'],
+            help='Device Group to syncronise configuration',
         )
         add(
-            "apm",
-            metavar="apm",
-            default=constants.CLI_DEFAULTS["bigip_apm"],
-            help="Is the VS APM enabled or not",
+            'apm',
+            metavar='apm',
+            default=constants.CLI_DEFAULTS['bigip_apm'],
+            help='Is the VS APM enabled or not',
         )
         add(
-            "verify-ssl",
-            metavar="verify-ssl",
-            default=constants.CLI_DEFAULTS["bigip_verify_ssl"],
-            help="enable or disable SSL verification of the BIG-IP management API",
+            'verify-ssl',
+            metavar='verify-ssl',
+            default=constants.CLI_DEFAULTS['bigip_verify_ssl'],
+            help='enable or disable SSL verification of the BIG-IP management API',
         )
 
     def __init__(self, *args, **kwargs):
-        """Membervariables are initialiyed as empty objects of the coressponding type.
+        '''Membervariables are initialiyed as empty objects of the coressponding type.
         The only exception is the version parameter which can be parsed.
-        """
+        '''
 
-        version = kwargs.pop("version", None)
+        version = kwargs.pop('version', None)
         super(BigipConfigurator, self).__init__(*args, **kwargs)
 
         # Add name_server association dict
         self.assoc = dict()
         # Outstanding challenges
         self._chall_out = set()
         # Maps enhancements to vhosts we've enabled the enhancement for
@@ -122,301 +119,301 @@
         self.vservers = None
         self._enhance_func = {}
 
         self._domain = None
         self.cert_chain_name = None
 
     def prepare(self):
-        """Prepare the authenticator/installer"""
+        '''Prepare the authenticator/installer'''
 
-        if self.conf("username") == "":
-            msg = "No username specified, please use --bigip-username"
+        if self.conf('username') == '':
+            msg = 'No username specified, please use --bigip-username'
             raise errors.MissingCommandlineFlag(msg)
 
-        if self.conf("password") == "":
-            msg = "No password specified, please use --bigip-password"
+        if self.conf('password') == '':
+            msg = 'No password specified, please use --bigip-password'
             raise errors.MissingCommandlineFlag(msg)
 
-        if self.conf("vs_list") != "" and self.conf("vs_list") is not None:
-            self.bigip_vs_list = self.conf("vs_list").split(",")
+        if self.conf('vs_list') != '' and self.conf('vs_list') is not None:
+            self.bigip_vs_list = self.conf('vs_list').split(',')
             for vs in self.bigip_vs_list:
-                logger.debug(f"Virtual server: {vs}")
+                logger.debug(f'Virtual server: {vs}')
         else:
-            msg = "--bigip-vs-list is required when using the F5 BIG-IP plugin"
+            msg = '--bigip-vs-list is required when using the F5 BIG-IP plugin'
             raise errors.MissingCommandlineFlag(msg)
 
-        self.iapp = ""
-        if self.conf("iapp") != "" and self.conf("iapp") is not None:
-            self.iapp = self.conf("iapp")
+        self.iapp = ''
+        if self.conf('iapp') != '' and self.conf('iapp') is not None:
+            self.iapp = self.conf('iapp')
 
-        if self.conf("list") != "":
-            self.bigip_host_list = self.conf("list").split(",")
+        if self.conf('list') != '':
+            self.bigip_host_list = self.conf('list').split(',')
         else:
-            msg = "--bigip-list is required when using the F5 BIG-IP plugin"
+            msg = '--bigip-list is required when using the F5 BIG-IP plugin'
             raise errors.MissingCommandlineFlag(msg)
 
-        if "--staging" in sys.argv or "--test-cert" in sys.argv:
-            self.cert_chain_name = "staging_chain"
-            logger.debug("certbot was called in staging mode")
+        if '--staging' in sys.argv or '--test-cert' in sys.argv:
+            self.cert_chain_name = 'staging_chain'
+            logger.debug('certbot was called in staging mode')
         else:
-            self.cert_chain_name = "chain"
+            self.cert_chain_name = 'chain'
 
-        if self.conf("apm"):
+        if self.conf('apm'):
             self.apm = True
 
         try:
             self.bigip = obj.Bigip(
                 self.bigip_host_list,
-                self.conf("username"),
-                self.conf("password"),
+                self.conf('username'),
+                self.conf('password'),
                 self.bigip_vs_list,
-                self.conf("device-group"),
-                self.conf("partition"),
-                self.conf("clientssl-parent"),
-                self.conf("verify-ssl"),
+                self.conf('device-group'),
+                self.conf('partition'),
+                self.conf('clientssl-parent'),
+                self.conf('verify-ssl'),
             )
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
-                "(You most probably need to ensure the username and "
-                "password is correct. Make sure you use the --bigip-username "
-                "and --bigip-password options)"
+                f'Connection to F5 BIG-IP iControl REST API failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
+                '(You most probably need to ensure the username and '
+                'password is correct. Make sure you use the --bigip-username '
+                'and --bigip-password options)'
             )
             raise errors.AuthorizationError(msg)
 
     def config_test(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
+        '''
 
-        logger.debug("in config_test()")
+        logger.debug('in config_test()')
 
         return
 
     def more_info(self):
-        """Human-readable string to help understand the module.
+        '''Human-readable string to help understand the module.
         Mandatory member function of parent class.
-        """
+        '''
 
         return (
-            "Configures F5 BIG-IP to authenticate and configure X.509"
-            "certificate/key use. Only one F5 Cluster addressable."
+            'Configures F5 BIG-IP to authenticate and configure X.509'
+            'certificate/key use. Only one F5 Cluster addressable.'
         )
 
     def get_chall_pref(self, domain):
-        """Return list of challenge preferences.
+        '''Return list of challenge preferences.
         Currently only HTTP01 is supported.
         Mandatory member function of parent class.
-        """
+        '''
 
         return [
             challenges.HTTP01
         ]  # support only HTTP01, DNS01 can be done with DNS module, not implemented now
 
     def perform(self, achalls):
-        """Perform the configuration related challenge.
+        '''Perform the configuration related challenge.
         This function currently assumes all challenges will be fulfilled.
         If this turns out not to be the case in the future. Cleanup and
         outstanding challenges will have to be designed better.
 
-        """
+        '''
 
         responses = [None] * len(achalls)
 
         for count, achall in enumerate(achalls):
             if isinstance(achall.chall, challenges.HTTP01):
                 response, validation = achall.response_and_validation()
-                token = achall.chall.encode("token")
+                token = achall.chall.encode('token')
                 responses[count] = response
 
                 bigip = self.bigip
-                if not bigip.exists_irule(f"Certbot-Letsencrypt-{token}"):
+                if not bigip.exists_irule(f'Certbot-Letsencrypt-{token}'):
                     bigip.create_irule_HTTP01(token, validation, self.apm)
 
-                logger.debug(f"DEBUG: VS-List: {self.bigip_vs_list}")
+                logger.debug(f'DEBUG: VS-List: {self.bigip_vs_list}')
                 for virtual_server in self.bigip_vs_list:
-                    logger.debug(f"DEBUG: VS: {virtual_server}")
+                    logger.debug(f'DEBUG: VS: {virtual_server}')
                     try:
                         if bigip.exists_virtual(virtual_server) and bigip.http_virtual(
                             virtual_server
                         ):
                             # virtual server exists and has a HTTP profile attached to it
                             # associate the iRule to it which will respond for HTTP01 validations
-                            logger.debug(f"Associating irule with {virtual_server}")
+                            logger.debug(f'Associating irule with {virtual_server}')
                             bigip.associate_irule_virtual(token, virtual_server)
                             time.sleep(10)
                         else:
                             logger.debug(
-                                f"VS {virtual_server} does not exist or has no HTTP profile attached."
+                                f'VS {virtual_server} does not exist or has no HTTP profile attached.'
                             )
-                            logger.debug("Skipping challenge on this VS")
+                            logger.debug('Skipping challenge on this VS')
                             logger.debug(
-                                f"exists_virtual: {bigip.exists_virtual(virtual_server)}"
+                                f'exists_virtual: {bigip.exists_virtual(virtual_server)}'
                             )
                             logger.debug(
-                                f"http_virtual: {bigip.http_virtual(virtual_server)}"
+                                f'http_virtual: {bigip.http_virtual(virtual_server)}'
                             )
                     except Exception as e:
                         msg = (
-                            f"Connection to F5 BIG-IP iControl REST API on {self.bigip_host_list[0]} failed."
-                            f"{os.linesep}Error raised was {os.linesep}{e}{os.linesep}"
+                            f'Connection to F5 BIG-IP iControl REST API on {self.bigip_host_list[0]} failed.'
+                            f'{os.linesep}Error raised was {os.linesep}{e}{os.linesep}'
                         )
                         raise errors.PluginError(msg)
 
         return responses
 
     def cleanup(self, achalls):
-        """Revert all challenges.
+        '''Revert all challenges.
 
         :param achalls: challanges
         :type achalls: [type]
         :raises errors.PluginError:
-        """
+        '''
 
         for achall in achalls:
             if isinstance(achall.chall, challenges.HTTP01):
-                token = achall.chall.encode("token")
+                token = achall.chall.encode('token')
                 for virtual_server in self.bigip_vs_list:
                     if self.bigip.exists_virtual(virtual_server):
                         if (
                             self.bigip.remove_irule_virtual(token, virtual_server)
                             is not True
                         ):
                             logger.error(
-                                f"iRule could not be removed from virtual server {virtual_server} you may need to do this manually"
+                                f'iRule could not be removed from virtual server {virtual_server} you may need to do this manually'
                             )
                     else:
                         logger.error(
-                            f"The virtual server {virtual_server} does not appear to exist on this BIG-IP"
+                            f'The virtual server {virtual_server} does not appear to exist on this BIG-IP'
                         )
                 try:
                     self.bigip.delete_irule(token)
                 except Exception as e:
                     msg = (
-                        f"Connection to F5 BIG-IP iControl REST API on {self.bigip_host_list[0]} failed.{os.linesep}"
-                        f"Error raised was {os.linesep}{e}{os.linesep}"
+                        f'Connection to F5 BIG-IP iControl REST API on {self.bigip_host_list[0]} failed.{os.linesep}'
+                        f'Error raised was {os.linesep}{e}{os.linesep}'
                     )
                     raise errors.PluginError(msg)
             elif isinstance(achall.chall, challenges.DNS01):
                 pass
 
         return
 
     def get_all_names(self):
-        """Cannot currently work for F5 BIG-IP due to the way in which Cerbot validates
+        '''Cannot currently work for F5 BIG-IP due to the way in which Cerbot validates
         returned strings as conforming to host/domain name format. e.g. F5 BIG-IP virtual
         server names are not always in pure host/domain name.
 
         :raises errors.PluginError: Always
 
-        """
+        '''
 
         msg = (
-            "Certbot can't be used to select domain names based on F5 "
-            f"BIG-IP Virtual Server names.{os.linesep}{os.linesep}Please use CLI arguments, "
-            "example: --bigip-vs-list virtual_name1,virtual_name2 --domain "
-            "domain.name"
+            'Certbot can\'t be used to select domain names based on F5 '
+            f'BIG-IP Virtual Server names.{os.linesep}{os.linesep}Please use CLI arguments, '
+            'example: --bigip-vs-list virtual_name1,virtual_name2 --domain '
+            'domain.name'
         )
 
         raise errors.PluginError(msg)
 
     def deploy_cert(
         self, domain, cert_path, key_path, chain_path=None, fullchain_path=None
     ):
-        """Deploys certificate and key to specified F5 BIG-IP, creates or updates
+        '''Deploys certificate and key to specified F5 BIG-IP, creates or updates
         client SSL profiles, and ensures they are associated with the specified
         virtual server.
 
         NOTE: This gets run for EVERY primary certificate name and every subjectAltName
               in a certificate. Need to improve efficiency within F5 BIG-IP config by
               not creating lots of duplicates of certs/keys.
 
         :raises errors.PluginError: When unable to deploy certificate due to
             a lack of directives
-        """
+        '''
 
-        logger.debug("Deploying on bigip")
+        logger.debug('Deploying on bigip')
         bigip = self.bigip
 
-        logger.debug("Uploading certificates to bigip")
+        logger.debug('Uploading certificates to bigip')
         bigip.upload_file(cert_path)
         bigip.upload_file(key_path)
         bigip.upload_file(chain_path)
 
-        logger.debug("deploying certs and keys on bigip")
+        logger.debug('deploying certs and keys on bigip')
         bigip.update_crypto(
-            domain.replace(".", "_").replace("*", "wildcard"),
+            domain.replace('.', '_').replace('*', 'wildcard'),
             cert_path,
             key_path,
             chain_path,
             self.cert_chain_name,
         )
-        logger.debug("Deployed Succesfully")
+        logger.debug('Deployed Succesfully')
 
-        logger.debug("Updating Client SSL Profile")
+        logger.debug('Updating Client SSL Profile')
 
         bigip.update_clientssl_profile(
-            domain.replace(".", "_").replace("*", "wildcard"),
+            domain.replace('.', '_').replace('*', 'wildcard'),
             self.bigip_vs_list[0],
             self.iapp,
         )
-        logger.debug("Successfully Updated Client SSL Profile")
+        logger.debug('Successfully Updated Client SSL Profile')
 
         return True
 
     def renew_deploy(self, lineage, *args, **kwargs): # pylint: disable=missing-docstring,no-self-use
-        """
+        '''
         Renew certificates when calling `certbot renew`
-        """
+        '''
 
         # Run deploy_cert with the lineage params
         self.deploy_cert(lineage.names()[0], lineage.cert_path, lineage.key_path, lineage.chain_path, lineage.fullchain_path)
 
         return
 
 
     def enhance(self, domain, enhancement, options=None):
-        """Enhance configuration.
+        '''Enhance configuration.
 
         :param str domain: domain to enhance
         :param str enhancement: enhancement type defined in
             :const:`~certbot.constants.ENHANCEMENTS`
         :param options: options for the enhancement
             See :const:`~certbot.constants.ENHANCEMENTS`
             documentation for appropriate parameter.
 
         :raises .errors.PluginError: If Enhancement is not supported, or if
             there is any other problem with the enhancement.
 
-        """
+        '''
 
         logger.debug(
-            f"DEBUG: enhance(domain={domain}, enhancement={enhancement}, options={options})"
+            f'DEBUG: enhance(domain={domain}, enhancement={enhancement}, options={options})'
         )
 
         return
 
     def supported_enhancements(self):  # pylint: disable=no-self-use
-        """Returns currently supported enhancements.
+        '''Returns currently supported enhancements.
         Mandatory member function of parent class.
-        """
+        '''
 
         # return ['ensure-http-header', 'redirect', 'staple-ocsp']
         return []
 
     def get_all_certs_keys(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
-        logger.debug("DEBUG: in get_all_certs_keys()")
+        '''
+        logger.debug('DEBUG: in get_all_certs_keys()')
         return []
 
     def save(self, title=None, temporary=False):
-        """Saves all changes to all F5 BIG-IP's, e.g. tmsh /sys save config.
+        '''Saves all changes to all F5 BIG-IP's, e.g. tmsh /sys save config.
 
         This function first checks for save errors, if none are found,
         all configuration changes made will be saved. According to the
         function parameters. If an exception is raised, a new checkpoint
         was not created.
 
         :param str title: The title of the save. If a title is given, a UCS
@@ -424,50 +421,50 @@
 
         :param bool temporary: Indicates whether the changes made will
             be quickly reversed in the future (ie. challenges)
 
         :raises .errors.PluginError: If there was an error in Augeas, in
             an attempt to save the configuration, or an error creating a
             checkpoint
-        """
+        '''
         bigip = self.bigip
 
         if temporary is False:
             bigip.save()
 
         return
 
     def revert_challenge_config(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
-        logger.debug("DEBUG: in revert_challenge_config()")
+        '''
+        logger.debug('DEBUG: in revert_challenge_config()')
         return
 
     def rollback_checkpoints(self, rollback=1):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
-        logger.debug("DEBUG: in rollback_checkpoints()")
+        '''
+        logger.debug('DEBUG: in rollback_checkpoints()')
         return
 
     def recovery_routine(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
-        logger.debug("DEBUG: in recovery_routine()")
+        '''
+        logger.debug('DEBUG: in recovery_routine()')
         return
 
     def view_config_changes(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
-        logger.debug("DEBUG: in view_config_changes()")
+        '''
+        logger.debug('DEBUG: in view_config_changes()')
         return
 
     def restart(self):
-        """Does nothing in context of F5 BIG-IP, but must be defined.
+        '''Does nothing in context of F5 BIG-IP, but must be defined.
         Mandatory member function of parent class.
-        """
+        '''
         return
 
 interfaces.RenewDeployer.register(BigipConfigurator)
```

### Comparing `certbot-bigip-1.2.0/certbot_bigip/obj.py` & `certbot-bigip-1.2.1/certbot_bigip/obj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module contains classes used by the F5 BIG-IP Configurator."""
+'''Module contains classes used by the F5 BIG-IP Configurator.'''
 
 import logging
 import os
 import requests
 from urllib3.exceptions import InsecureRequestWarning
 
 from certbot import errors
@@ -12,32 +12,32 @@
 from f5.multi_device.device_group import DeviceGroup
 
 
 logger = logging.getLogger(__name__)
 
 
 class Bigip(object):
-    """Object representing access to F5 BIG-IP system(s)
+    '''Object representing access to F5 BIG-IP system(s)
 
     :param object: [description]
     :type object: [type]
-    """
+    '''
 
     def __init__(
         self,
         bigips,
         username,
         password,
         vs_list,
         device_group,
         partition,
         clientssl_parent,
         verify_ssl,
     ):
-        """Initialize a BIG-IP.
+        '''Initialize a BIG-IP.
 
         :param hosts: CSV list of BIG-IP system hostnames or addresses, all have to be in the same cluster
         :type hosts: string
         :param username: BIG-IP username
         :type username: string
         :param password: BIG-IP password
         :type password: string
@@ -47,15 +47,15 @@
         :type partition: str, optional
         :param clientssl_parent: Client SSL parent profile to inherit default values from,
                                  defaults to '/Common/clientssl'
         :type clientssl_parent: str, optional
         :param verify_ssl: enable or disable SSL verification of the BIG-IP management API, defaults to False
         :type verify_ssl: bool, optional
         :raises errors.AuthorizationError: Connection to the BIG-IP failed
-        """
+        '''
 
         self.bigips = bigips
         self.bigip_map = {}
         self.username = username
         self.__password = password
         self.token = True
         self.partition = partition
@@ -65,773 +65,773 @@
         self.standalone = False
         self.verify_ssl = verify_ssl
 
         if not self.verify_ssl:
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
         self.bigip_map = self._get_bigip_map()
-        logger.debug(f"bigip map: {self.bigip_map}")
+        logger.debug(f'bigip map: {self.bigip_map}')
         self.active_device = self._get_active_bigip()
-        logger.debug(f"active device: {self.active_device}")
+        logger.debug(f'active device: {self.active_device}')
         if self.active_device:
             try:
                 self.mgmt = ManagementRoot(
                     self.active_device,
                     self.username,
                     self.__password,
                     token=True,
                     verify=self.verify_ssl,
                 )
             except Exception as e:
                 msg = (
-                    f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                    f"Error raised was {os.linesep}{e}{os.linesep}"
-                    "(You most probably need to ensure the username and"
-                    "password is correct. Make sure you use the --bigip-username"
-                    "and --bigip-password options)"
+                    f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                    f'Error raised was {os.linesep}{e}{os.linesep}'
+                    '(You most probably need to ensure the username and'
+                    'password is correct. Make sure you use the --bigip-username'
+                    'and --bigip-password options)'
                 )
                 raise errors.AuthorizationError(msg)
         else:
             msg = (
-                f"No active device found which is responsible for all "
-                "provided virtual servers or auto-sync is disabled. If you run an active/active setup "
-                f"please ensure that all virtual servers are in the same traffic group or auto-sync is enabled{os.linesep}"
+                f'No active device found which is responsible for all '
+                'provided virtual servers or auto-sync is disabled. If you run an active/active setup '
+                f'please ensure that all virtual servers are in the same traffic group or auto-sync is enabled{os.linesep}'
             )
             raise errors.PluginError(msg)
         self.standalone = self._get_cluster_state()
-        logger.debug(f"standalone: {self.standalone}")
+        logger.debug(f'standalone: {self.standalone}')
 
     def _split_fullpath(self, fullpath):
-        """Return partition, subpath and name from object.
+        '''Return partition, subpath and name from object.
 
         :return: splits object into its parts like: /partition/path/object -> ['partition', 'path', 'object']
         :rtype: list
-        """
+        '''
         try:
-            if len(fullpath.split("/")) == 4:
-                subpath = fullpath.split("/")[2]
-                partition = fullpath.split("/")[1]
-                name = fullpath.split("/")[3]
-            elif len(fullpath.split("/")) == 3:
-                subpath = ""
-                partition = fullpath.split("/")[1]
-                name = fullpath.split("/")[2]
-            elif len(fullpath.split("/")) == 2:
-                subpath = ""
-                partition = "Common"
-                name = fullpath.split("/")[2]
+            if len(fullpath.split('/')) == 4:
+                subpath = fullpath.split('/')[2]
+                partition = fullpath.split('/')[1]
+                name = fullpath.split('/')[3]
+            elif len(fullpath.split('/')) == 3:
+                subpath = ''
+                partition = fullpath.split('/')[1]
+                name = fullpath.split('/')[2]
+            elif len(fullpath.split('/')) == 2:
+                subpath = ''
+                partition = 'Common'
+                name = fullpath.split('/')[2]
 
             return [partition, subpath, name]
         except Exception as e:
             msg = (
-                f"Failure with {fullpath}.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Failure with {fullpath}.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.PluginError(msg)
 
     def get_version(self):
-        """Returns the BIG-IPs SW version, currently not implemented.
+        '''Returns the BIG-IPs SW version, currently not implemented.
 
         :return: running software version
         :rtype: string
-        """
-        return "N/A"
+        '''
+        return 'N/A'
 
     def _get_bigip_map(self):
-        """Map bigips from user input with true bigip hostnamess.
+        '''Map bigips from user input with true bigip hostnamess.
 
         :raises errors.AuthorizationError: Connection to the BIG-IP failed
         :return: Dict with mapping of given bigip from user cli to actual hostname
         :rtype: dict
-        """
+        '''
         bigip_map = {}
         for bigip in self.bigips:
             try:
                 mgmt = ManagementRoot(
                     bigip,
                     self.username,
                     self.__password,
                     token=True,
                     verify=self.verify_ssl,
                 )
                 device = mgmt.tm.sys.global_settings.load()
-                bigip_map[bigip] = device.raw["hostname"]
+                bigip_map[bigip] = device.raw['hostname']
             except Exception as e:
                 msg = (
-                    f"Connection to F5 BIG-IP iControl REST API on {bigip} failed.{os.linesep}"
-                    f"Error raised was {os.linesep}{e}{os.linesep}"
-                    "(You most probably need to ensure the username and "
-                    "password is correct. Make sure you use the --bigip-username "
-                    "and --bigip-password options)"
+                    f'Connection to F5 BIG-IP iControl REST API on {bigip} failed.{os.linesep}'
+                    f'Error raised was {os.linesep}{e}{os.linesep}'
+                    '(You most probably need to ensure the username and '
+                    'password is correct. Make sure you use the --bigip-username '
+                    'and --bigip-password options)'
                 )
                 raise errors.AuthorizationError(msg)
         return bigip_map
 
     def _get_active_bigip(self):
-        """sets the active bigip if one is the active unit for all given virtual servers.
+        '''sets the active bigip if one is the active unit for all given virtual servers.
         sets the first bigip if cluster is active/active and auto-sync is turned on.
         returns false if no bigip is active for all virtual servers (active/active without auto-sync)
 
         :raises errors.AuthorizationError: Connection to the BIG-IP failed
         :raises errors.PluginError: Connection to the BIG-IP failed
         :return: name of the active bigip
         :rtype: string
-        """
+        '''
         try:
             mgmt = ManagementRoot(
                 self.bigips[0],
                 self.username,
                 self.__password,
                 token=True,
                 verify=self.verify_ssl,
             )
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.bigips[0]} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
-                "(You most probably need to ensure the username and "
-                "password is correct. Make sure you use the --bigip-username "
-                "and --bigip-password options)"
+                f'Connection to F5 BIG-IP iControl REST API on {self.bigips[0]} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
+                '(You most probably need to ensure the username and '
+                'password is correct. Make sure you use the --bigip-username '
+                'and --bigip-password options)'
             )
             raise errors.AuthorizationError(msg)
         try:
             # first check for failover status
-            active_device = ""
+            active_device = ''
             active_devices = []
             devices = mgmt.tm.cm.devices.get_collection()
             for device in devices:
-                if device.raw["failoverState"] == "active":
-                    active_devices.append(device.raw["hostname"])
+                if device.raw['failoverState'] == 'active':
+                    active_devices.append(device.raw['hostname'])
             if len(active_devices) == 0:
-                logger.debug("No active device found")
+                logger.debug('No active device found')
                 return False
             if len(active_devices) == 1:
                 active_device = active_devices[0]
-                logger.debug(f"Active device found in A/S cluster: {active_device}")
+                logger.debug(f'Active device found in A/S cluster: {active_device}')
             else:
                 # active/active cluster, checking if auto-sync is enabled
                 device_groups = mgmt.tm.cm.device_groups.get_collection()
                 for dg in device_groups:
                     if (
-                        dg.raw["type"] == "sync-failover"
-                        and dg.raw["autoSync"] == "enabled"
+                        dg.raw['type'] == 'sync-failover'
+                        and dg.raw['autoSync'] == 'enabled'
                     ):
                         logger.debug(
-                            "sync-failover with autoSync enabled, returning first device from list."
+                            'sync-failover with autoSync enabled, returning first device from list.'
                         )
                         active_devices.append(self.bigips[0])
                 # active/active cluster, need to find active device for specified virtual servers
                 destinations = []
                 for vs in self.vs_list:
                     # get destination from vs
                     # extract IP from destination
                     # get virtual address with address=destination
                     # get tg from va
                     # check active device for tgs
                     r = self._split_fullpath(vs)
                     virtual = mgmt.tm.ltm.virtuals.virtual.load(
                         partition=r[0], subPath=r[1], name=r[2]
                     )
-                    dst = virtual.raw["destination"]
-                    dst = dst[dst.rfind("/") + 1 :]
-                    if dst.count(".") == 3:
+                    dst = virtual.raw['destination']
+                    dst = dst[dst.rfind('/') + 1 :]
+                    if dst.count('.') == 3:
                         # IPv4 address
-                        dst = dst.split(":")[0]
+                        dst = dst.split(':')[0]
                     else:
                         # IPv6 address
-                        dst = dst.split(".")[0]
+                        dst = dst.split('.')[0]
                     if dst not in destinations:
                         destinations.append(dst)
 
                 tgs = []
                 virtual_addresses = mgmt.tm.ltm.virtual_address_s.get_collection()
                 for va in virtual_addresses:
                     for dst in destinations:
-                        if va.raw["address"] == dst:
-                            if va.raw["trafficGroup"] not in tgs:
-                                tgs.append(va.raw["trafficGroup"])
+                        if va.raw['address'] == dst:
+                            if va.raw['trafficGroup'] not in tgs:
+                                tgs.append(va.raw['trafficGroup'])
 
                 active_devices = []
                 for tg in tgs:
                     traffic_group = mgmt.tm.cm.traffic_groups.traffic_group.load(
-                        partition=tg.split("/")[1], name=tg.split("/")[2]
+                        partition=tg.split('/')[1], name=tg.split('/')[2]
                     )
                     traffic_group_stats = traffic_group.stats.load()
                     for item in traffic_group_stats.entries:
                         if (
-                            traffic_group_stats.entries[item]["nestedStats"]["entries"][
-                                "failoverState"
-                            ]["description"]
-                            == "active"
+                            traffic_group_stats.entries[item]['nestedStats']['entries'][
+                                'failoverState'
+                            ]['description']
+                            == 'active'
                         ):
                             if (
-                                traffic_group_stats.entries[item]["nestedStats"][
-                                    "entries"
-                                ]["deviceName"]["description"]
+                                traffic_group_stats.entries[item]['nestedStats'][
+                                    'entries'
+                                ]['deviceName']['description']
                                 not in active_devices
                             ):
                                 active_devices.append(
-                                    traffic_group_stats.entries[item]["nestedStats"][
-                                        "entries"
-                                    ]["deviceName"]["description"]
+                                    traffic_group_stats.entries[item]['nestedStats'][
+                                        'entries'
+                                    ]['deviceName']['description']
                                 )
                 if len(active_devices) == 0:
-                    logger.debug("No active device found")
+                    logger.debug('No active device found')
                     return False
                 if len(active_devices) == 1:
-                    active_device = active_devices[0].split("/")[2]
+                    active_device = active_devices[0].split('/')[2]
                     logger.debug(
-                        f"Active device found in A/A cluster: {active_devices[0]}"
+                        f'Active device found in A/A cluster: {active_devices[0]}'
                     )
                 else:
-                    logger.debug("No active device found")
+                    logger.debug('No active device found')
                     return False
 
             for device in self.bigip_map:
                 if self.bigip_map[device] == active_device:
-                    logger.debug(f"Active device {active_device} mapped to {device}")
+                    logger.debug(f'Active device {active_device} mapped to {device}')
                     return device
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.PluginError(msg)
 
     def _get_cluster_state(self):
-        """gets current cluster state
+        '''gets current cluster state
 
         :return: True for cluster, False for Standalone
         :rtype: bool
-        """
+        '''
         ss = self.mgmt.tm.cm.sync_status.load()
         if (
-            ss.raw["entries"]["https://localhost/mgmt/tm/cm/sync-status/0"][
-                "nestedStats"
-            ]["entries"]["mode"]["description"]
-            == "standalone"
+            ss.raw['entries']['https://localhost/mgmt/tm/cm/sync-status/0'][
+                'nestedStats'
+            ]['entries']['mode']['description']
+            == 'standalone'
         ):
             return True
         else:
             return False
 
     def save(self):
-        """Saves the running configuration.
+        '''Saves the running configuration.
 
         :raises errors.PluginError: something went wrong connecting to the BIG-IP
-        """
+        '''
         try:
-            self.mgmt.tm.sys.config.exec_cmd("save")
+            self.mgmt.tm.sys.config.exec_cmd('save')
             if not self.standalone:
                 list_of_bigips = []
                 for bigip in self.bigips:
                     list_of_bigips.append(
                         ManagementRoot(bigip, self.username, self.__password)
                     )
 
                 device_group = DeviceGroup(
                     devices=list_of_bigips,
                     device_group_name=self.device_group,
-                    device_group_type="sync-failover",
-                    device_group_partition="Common",
+                    device_group_type='sync-failover',
+                    device_group_partition='Common',
                 )
                 device_group.ensure_all_devices_in_sync()
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.PluginError(msg)
 
     def save_ucs(self, ucs_name):
-        """Generate UCS backup file, currently not used. Might be relevant for checkpoint implementation.
+        '''Generate UCS backup file, currently not used. Might be relevant for checkpoint implementation.
 
         :param ucs_name: name of the UCS file
         :type ucs_name: string
         :raises errors.PluginError: something went wrong connecting to the BIG-IP
         :return: return True if UCS generation is successfull
         :rtype: bool
-        """
+        '''
         try:
-            self.mgmt.tm.sys.ucs.exec_cmd("save", name=ucs_name)
+            self.mgmt.tm.sys.ucs.exec_cmd('save', name=ucs_name)
             return True
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.PluginError(msg)
 
     def upload_file(self, local_file_name):
-        """Upload a file.
+        '''Upload a file.
 
         :param local_file_name: local file name
         :type local_file_name: string
         :raises errors.CertStorageError: something went wrong saving the file to the BIG-IP
         :return: return True if file upload is successfull
         :rtype: bool
-        """
+        '''
         try:
             self.mgmt.shared.file_transfer.uploads.upload_file(local_file_name)
             return True
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.CertStorageError(msg)
 
     def exists_crypto_cert(self, certificate):
-        """check if certificate already exists
+        '''check if certificate already exists
 
         :param certificate: name of the certificate
         :type certificate: string
         :raises errors.CertStorageError: something went wrong accessing the file to the BIG-IP
         :return: return true or false certificate exists or not
         :rtype: bool
-        """
+        '''
         try:
             return self.mgmt.tm.sys.file.ssl_certs.ssl_cert.exists(
-                name=f"{certificate}_Letsencrypt", partition=self.partition
+                name=f'{certificate}_Letsencrypt', partition=self.partition
             )
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.CertStorageError(msg)
 
     def exists_crypto_key(self, key):
-        """check if key already exists
+        '''check if key already exists
 
         :param key: name of the key
         :type key: string
         :raises errors.CertStorageError: something went wrong accessing the file to the BIG-IP
         :return: return true or false certificate exists or not
         :rtype: bool
-        """
+        '''
         try:
             return self.mgmt.tm.sys.file.ssl_keys.ssl_key.exists(
-                name=f"{key}_Letsencrypt", partition=self.partition
+                name=f'{key}_Letsencrypt', partition=self.partition
             )
 
         except Exception as e:
             raise BigIpCertStorageError(self.active_device, e)
 
     def update_crypto(self, name, cert, key, chain, cert_chain_name):
-        """updated certificate and key
+        '''updated certificate and key
 
         :param name: domain name
         :type name: string
         :param cert: certificate filename
         :type cert: string
         :param key: key filename
         :type key: string
         :param chain: chain filename
         :type chain: string
         :param cert_chain_name: chain name
         :type cert_chain_name: string
         :raises BigIpCertStorageError: something went wrong accessing the file to the BIG-IP
-        """
+        '''
         # Because they exist, we will modify them in a transaction
         try:
             tx = self.mgmt.tm.transactions.transaction
             with TransactionContextManager(tx) as api:
 
                 self._update_crypto_key(api, key, name)
                 self._update_crypto_cert(api, cert, name)
 
             self._update_crypto_cert(api, chain, cert_chain_name)
 
         except Exception as e:
             raise BigIpCertStorageError(self.active_device, e)
 
     def _update_crypto_cert(self, api, cert, name):
-        """upload certificate
+        '''upload certificate
 
         :param api: transaction object
         :type api: TransactionContextManager
         :param cert: certificate filename
         :type cert: string
         :param name: domain name
         :type name: string
-        """
+        '''
         if self.exists_crypto_cert(name):
-            logger.debug(f"updating cert for {name}")
+            logger.debug(f'updating cert for {name}')
             modcert = api.tm.sys.file.ssl_certs.ssl_cert.load(
-                name=f"{name}_Letsencrypt", partition=self.partition
+                name=f'{name}_Letsencrypt', partition=self.partition
             )
             modcert.sourcePath = (
-                f"file:/var/config/rest/downloads/{os.path.basename(cert)}"
+                f'file:/var/config/rest/downloads/{os.path.basename(cert)}'
             )
             modcert.update()
 
         else:
-            logger.debug(f"creating cert for {name}")
+            logger.debug(f'creating cert for {name}')
             modcert = self.mgmt.tm.sys.file.ssl_certs.ssl_cert.create(
-                name=f"{name}_Letsencrypt",
+                name=f'{name}_Letsencrypt',
                 partition=self.partition,
-                sourcePath=f"file:/var/config/rest/downloads/{os.path.basename(cert)}",
+                sourcePath=f'file:/var/config/rest/downloads/{os.path.basename(cert)}',
             )
 
     def _update_crypto_key(self, api, key, name):
-        """upload key
+        '''upload key
 
         :param api: transaction object
         :type api: TransactionContextManager
         :param key: key filename
         :type key: string
         :param name: domain name
         :type name: string
-        """
+        '''
         if self.exists_crypto_key(name):
-            logger.debug(f"updating key for {name}")
+            logger.debug(f'updating key for {name}')
             modkey = api.tm.sys.file.ssl_keys.ssl_key.load(
-                name=f"{name}_Letsencrypt", partition=self.partition
+                name=f'{name}_Letsencrypt', partition=self.partition
             )
-            modkey.sourcePath = f"file:/var/config/rest/downloads/{os.path.basename(key)}"
+            modkey.sourcePath = f'file:/var/config/rest/downloads/{os.path.basename(key)}'
             modkey.update()
         else:
-            logger.debug(f"creating key for {name}")
+            logger.debug(f'creating key for {name}')
             modkey = self.mgmt.tm.sys.file.ssl_keys.ssl_key.create(
-                name=f"{name}_Letsencrypt",
+                name=f'{name}_Letsencrypt',
                 partition=self.partition,
-                sourcePath=f"file:/var/config/rest/downloads/{os.path.basename(key)}",
+                sourcePath=f'file:/var/config/rest/downloads/{os.path.basename(key)}',
             )
 
     def exists_clientssl_profile(self, domain, virtual_name, iapp):
-        """check if clientssl profile already exists
+        '''check if clientssl profile already exists
 
         :param domain: domain name
         :type domain: [string
         :param virtual_name: virtual server name
         :type virtual_name: string
         :param iapp: iapp name
         :type iapp: string
         :raises errors.CertStorageError: something went wrong accessing the file to the BIG-IP
         :return: true if exists, false if not exists
         :rtype: bool
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
-            name = f"{domain}_clientssl"
-            if iapp != "":
+            name = f'{domain}_clientssl'
+            if iapp != '':
                 return self.mgmt.tm.ltm.profile.client_ssls.client_ssl.exists(
                     name=name, partition=self.partition, subPath=r[1]
                 )
             else:
                 return self.mgmt.tm.ltm.profile.client_ssls.client_ssl.exists(
                     name=name, partition=self.partition
                 )
 
         except Exception as e:
             msg = (
-                f"Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.CertStorageError(msg)
 
     def update_clientssl_profile(self, domain, virtual_name, iapp):
-        """update client ssl profile
+        '''update client ssl profile
 
         :param domain: domain name
         :type domain: string
         :param virtual_name: virtual server name
         :type virtual_name: string
         :param iapp: iapp name
         :type iapp: string
-        """
-        if "wildcard" not in domain:
+        '''
+        if 'wildcard' not in domain:
             wildcard = False
         else:
             wildcard = True
         if not self.exists_clientssl_profile(domain, virtual_name, iapp):
             self.create_clientssl_profile(domain, virtual_name, iapp, wildcard)
         else:
-            logger.debug("Nothing left to do")
+            logger.debug('Nothing left to do')
 
     def create_clientssl_profile(self, domain, virtual_name, iapp, wildcard):
-        """create new clientssl profile
+        '''create new clientssl profile
 
         :param domain: domain name
         :type domain: string
         :param virtual_name: virtual server name
         :type virtual_name: string
         :param iapp: iapp name
         :type iapp: string
         :param wildcard: if it's a wildcard of not
         :type wildcard: bool
         :raises errors.CertStorageError: something went wrong creating the profile to the BIG-IP
         :return: return true if it worked
         :rtype: bool
-        """
+        '''
 
         # if it's a wildcard, we use it as default profile for SNI
         sni_default = wildcard
 
         try:
             r = self._split_fullpath(virtual_name)
-            if iapp != "":
-                name = f"/{self.partition}/{r[1]}/{domain}_clientssl"
+            if iapp != '':
+                name = f'/{self.partition}/{r[1]}/{domain}_clientssl'
             else:
-                name = f"/{self.partition}/{domain}_clientssl"
+                name = f'/{self.partition}/{domain}_clientssl'
             cssl_profile = {
-                "name": name,
-                "cert-key-chain":{
-                    "default": {
-                        "cert": f"/{self.partition}/{domain}_Letsencrypt",
-                        "key": f"/{self.partition}/{domain}_Letsencrypt",
-                        "chain": f"/{self.partition}/chain_Letsencrypt",
+                'name': name,
+                'cert-key-chain':{
+                    'default': {
+                        'cert': f'/{self.partition}/{domain}_Letsencrypt',
+                        'key': f'/{self.partition}/{domain}_Letsencrypt',
+                        'chain': f'/{self.partition}/chain_Letsencrypt',
                     }
                 },
-                "defaultsFrom": self.clientssl_parent,
-                "app-service": iapp,
-                "sniDefault": sni_default,
+                'defaultsFrom': self.clientssl_parent,
+                'app-service': iapp,
+                'sniDefault': sni_default,
             }
             self.mgmt.tm.ltm.profile.client_ssls.client_ssl.create(**cssl_profile)
             return True
 
         except Exception as e:
             msg = (
-                f"Certificate creation on F5 Failed. Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}"
-                f"Error raised was {os.linesep}{e}{os.linesep}"
+                f'Certificate creation on F5 Failed. Connection to F5 BIG-IP iControl REST API on {self.active_device} failed.{os.linesep}'
+                f'Error raised was {os.linesep}{e}{os.linesep}'
             )
             raise errors.CertStorageError(msg)
 
     def exists_irule(self, irule_name):
-        """check if iRule already exists
+        '''check if iRule already exists
 
         :param irule_name: iRule name
         :type irule_name: string
         :raises errors.ConfigurationError: check failed
         :return: True or False if iRule exists or not
         :rtype: bool
-        """
+        '''
         try:
             return self.mgmt.tm.ltm.rules.rule.exists(
                 partition=self.partition, name=irule_name
             )
 
         except Exception as e:
-            msg = f"iRule creation on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'iRule creation on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def create_irule_HTTP01(self, token, http_response_content, apm):
-        """create iRule for verification
+        '''create iRule for verification
 
         :param token: challenge token
         :type token: string
         :param http_response_content: challenge response value
         :type http_response_content: string
         :param apm: Flag if APM is enabled on this virtual server
         :type apm: bool
         :raises errors.ConfigurationError: creation failed
         :return: True iRule creation succeeded
         :rtype: bool
-        """
+        '''
         try:
-            irule_name = f"Certbot-Letsencrypt-{token}"
+            irule_name = f'Certbot-Letsencrypt-{token}'
             if apm is True:
                 irule_text = f'when CLIENT_ACCEPTED {{\n  catch {{\n    ACCESS::restrict_irule_events disable\n  }}\n}}\nwhen HTTP_REQUEST priority 100 {{\n  if {{[HTTP::has_responded]}}{{return}}\n  if {{[HTTP::uri] equals "/.well-known/acme-challenge/{token}"}} {{\n    HTTP::respond 200 -version auto content "{http_response_content}" noserver \n  event disable\n  }}\n}}'
             else:
                 irule_text = f'when HTTP_REQUEST priority 100 {{\n  if {{[HTTP::has_responded]}}{{return}}\n  if {{[HTTP::uri] equals "/.well-known/acme-challenge/{token}"}} {{\n    HTTP::respond 200 -version auto content "{http_response_content}" noserver \n  event disable\n  }}\n}}'
 
             self.mgmt.tm.ltm.rules.rule.create(
                 name=irule_name, partition=self.partition, apiAnonymous=irule_text
             )
             return True
 
         except Exception as e:
-            msg = f"iRule creation on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'iRule creation on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def delete_irule(self, token):
-        """delete iRule
+        '''delete iRule
 
         :param token: challenge token
         :type token: string
         :raises errors.ConfigurationError: deletion failed
         :return: True if deletion succeeded
         :rtype: bool
-        """
+        '''
         try:
-            irule_name = f"Certbot-Letsencrypt-{token}"
+            irule_name = f'Certbot-Letsencrypt-{token}'
 
             rule = self.mgmt.tm.ltm.rules.rule.load(
                 name=irule_name, partition=self.partition
             )
             rule.delete()
             return True
 
         except Exception as e:
-            msg = f"iRule deletion from {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'iRule deletion from {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def exists_virtual(self, virtual_name):
-        """check if virtual server exists
+        '''check if virtual server exists
 
         :param virtual_name: name of virtual server
         :type virtual_name: string
         :raises errors.ConfigurationError: check failed
         :return: True or False if VS exists or not
         :rtype: bool
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
             return self.mgmt.tm.ltm.virtuals.virtual.exists(
                 partition=r[0], subPath=r[1], name=r[2]
             )
 
         except Exception as e:
-            msg = f"Virtual server {virtual_name} check on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'Virtual server {virtual_name} check on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def profile_on_virtual(self, virtual_name, profile_type):
-        """check for profiles which are attached to the virtual server
+        '''check for profiles which are attached to the virtual server
 
         :param virtual_name: virtual server name
         :type virtual_name: string
         :param profile_type: type of profile to look for
         :type profile_type: string
         :raises errors.ConfigurationError: check failed
         :return: True or False if profile of specified type exists
         :rtype: bool
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
             virtual = self.mgmt.tm.ltm.virtuals.virtual.load(
                 partition=r[0], subPath=r[1], name=r[2]
             )
 
-            if virtual != "":
+            if virtual != '':
                 for profile in virtual.profiles_s.get_collection():
                     r = self._split_fullpath(profile.fullPath)
                     try:
                         getattr(
                             getattr(
-                                getattr(self.mgmt.tm.ltm.profile, f"{profile_type}s"),
-                                f"{profile_type}",
+                                getattr(self.mgmt.tm.ltm.profile, f'{profile_type}s'),
+                                f'{profile_type}',
                             ),
-                            "load",
+                            'load',
                         )(partition=r[0], subPath=r[1], name=r[2])
                         return True
                     except Exception:
                         pass
                 return False
             else:
                 return False
 
         except Exception as e:
-            msg = f"Test for HTTP profile on virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'Test for HTTP profile on virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def http_virtual(self, virtual_name):
-        """checks for http profile on virtual server
+        '''checks for http profile on virtual server
 
         :param virtual_name: virtual server name
         :type virtual_name: string
         :return: True or False
         :rtype: bool
-        """
-        return self.profile_on_virtual(virtual_name, "http")
+        '''
+        return self.profile_on_virtual(virtual_name, 'http')
 
     def client_ssl_virtual(self, virtual_name):
-        """checks for clientssl profile on virtual server
+        '''checks for clientssl profile on virtual server
 
         :param virtual_name: virtual server name
         :type virtual_name: string
         :return: True or False
         :rtype: bool
-        """
-        return self.profile_on_virtual(virtual_name, "client_ssl")
+        '''
+        return self.profile_on_virtual(virtual_name, 'client_ssl')
 
     def irules_on_virtual(self, virtual_name):
-        """[summary]
+        '''[summary]
 
         :param virtual_name: virtual server name
         :type virtual_name: string
         :raises errors.ConfigurationError: check failed
         :return: Dictionary with keys result and list of attached iRules
         :rtype: dict
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
             virtual = self.mgmt.tm.ltm.virtuals.virtual.load(
                 partition=r[0], subPath=r[1], name=r[2]
             )
 
-            if virtual != "" and "rules" in virtual.raw:
-                return {"result": True, "rules": virtual.rules}
+            if virtual != '' and 'rules' in virtual.raw:
+                return {'result': True, 'rules': virtual.rules}
             else:
-                return {"result": False, "rules": []}
+                return {'result': False, 'rules': []}
 
         except Exception as e:
-            msg = f"Retrieval of iRules for virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'Retrieval of iRules for virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def associate_irule_virtual(self, token, virtual_name):
-        """attach iRule to virtual server
+        '''attach iRule to virtual server
 
         :param token: challenge token
         :type token: string
         :param virtual_name: virtual server name
         :type virtual_name: string
         :raises errors.ConfigurationError: attach failed
         :return: True if successfull
         :rtype: bool
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
             irules = self.irules_on_virtual(virtual_name)
             virtual = self.mgmt.tm.ltm.virtuals.virtual.load(
                 partition=r[0], subPath=r[1], name=r[2]
             )
-            if irules["result"] is True:
-                virtual.rules.append(f"/{self.partition}/Certbot-Letsencrypt-{token}")
+            if irules['result'] is True:
+                virtual.rules.append(f'/{self.partition}/Certbot-Letsencrypt-{token}')
             else:
-                virtual.rules = [f"/{self.partition}/Certbot-Letsencrypt-{token}"]
+                virtual.rules = [f'/{self.partition}/Certbot-Letsencrypt-{token}']
             virtual.update()
             return True
 
         except Exception as e:
-            msg = f"iRule association to virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'iRule association to virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
     def remove_irule_virtual(self, token, virtual_name):
-        """remove iRule from virtual server
+        '''remove iRule from virtual server
 
         :param token: challenge token
         :type token: string
         :param virtual_name: virtual server name
         :type virtual_name: string
         :raises errors.ConfigurationError: removal failed
         :return: True if successfull
         :rtype: bool
-        """
+        '''
         try:
             r = self._split_fullpath(virtual_name)
             irules = self.irules_on_virtual(virtual_name)
-            if irules["result"] is True:
+            if irules['result'] is True:
                 virtual = self.mgmt.tm.ltm.virtuals.virtual.load(
                     partition=r[0], subPath=r[1], name=r[2]
                 )
-                if f"/{self.partition}/Certbot-Letsencrypt-{token}" in virtual.rules:
-                    virtual.rules.remove(f"/{self.partition}/Certbot-Letsencrypt-{token}")
+                if f'/{self.partition}/Certbot-Letsencrypt-{token}' in virtual.rules:
+                    virtual.rules.remove(f'/{self.partition}/Certbot-Letsencrypt-{token}')
                     virtual.update()
             return True
 
         except Exception as e:
-            msg = f"iRule removal from virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}"
+            msg = f'iRule removal from virtual server on {self.active_device} failed. {os.linesep}{e}{os.linesep}'
             raise errors.ConfigurationError(msg)
 
 
 class BigIpCertStorageError(errors.CertStorageError):
     def __init__(self, host: str, e: Exception):
         self.msg = (
-            f"Connection to F5 BIG-IP iControl REST API on {host} failed.{os.linesep}"
-            f"Error raised was {os.linesep}{e}{os.linesep}"
+            f'Connection to F5 BIG-IP iControl REST API on {host} failed.{os.linesep}'
+            f'Error raised was {os.linesep}{e}{os.linesep}'
         )
```

### Comparing `certbot-bigip-1.2.0/certbot_bigip.egg-info/PKG-INFO` & `certbot-bigip-1.2.1/certbot_bigip.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: certbot-bigip
-Version: 1.2.0
+Version: 1.2.1
 Summary: F5 BIG-IP plugin for Certbot
 Author: Certbot Team @ Open Networks
 Author-email: certbot@on.at
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # certbot-bigip
 
 ## Requirements
 
 see certbot rquirements: <https://certbot.eff.org/docs/install.html#system-requirements>
@@ -31,14 +36,18 @@
   * The LetsEncrypt Chain needs to be at /Common/chain_Letsencrypt and in every other partition that uses this plugin. ( f.e.: /Partition/chain_Letsencrypt)
       At the moment, the plugin checks if a corresponding certificate/chain is located in the same partition/folder as the clientssl profile that uses it.
   * clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
   * F5 SW version 14.x and higher
 
 ## Install
 
+`pip install certbot-bigip`
+
+by installing the plugin you will also install all missing dependencies including certbot.
+
 ## Supported Features
 
 * verifies the domain via HTTP01 (challenge verification implemented through an iRule)
 * Partitions and iApps
 * Standalone and HA setups (Active/Standby, Active/Active)
 * Creates the clientssl profile and attaches the certificate, key and chain
   * Does not modify the clientssl profile if it already exists
@@ -125,15 +134,15 @@
 fi
 ```
 
 The first call only validates and renews the certificate through ```certonly``` parameter and the ```cert-test.sh``` compares the local certificate to the certificate delivered by the F5. If these don't match the second certbot call will skip the validation (as the certificate got already renewed) and install the certificate onto the F5.
 
 ## Testing
 
-> :warning: Currently only integration tests are supported. Therefore a bigip is needed. to run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
+> :warning: Currently only integration tests are supported. Therefore a bigip is needed. To run integrations tests with other plugins for example the bluecat plugin you also need a bluecat in place.
 
 ### Prerequisites
 
 1. Connection to the bigip under test from the machine running the tests
 2. clientssl profile needs to be attached to the virtual server manually(DOMAIN_clientssl). At the moment, the plugin only updates the client profile but does not attach it to the virtual server.
 3. Configure the tests using the following environment variables:
```

### Comparing `certbot-bigip-1.2.0/tests/test_bigip_configurator.py` & `certbot-bigip-1.2.1/tests/test_bigip_configurator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import logging
 import os
 
 from certbot_bigip.configurator import BigipConfigurator
 
+from OpenSSL import crypto
+
 logging.basicConfig(level=logging.DEBUG)
 mylogger = logging.getLogger(__name__)
 
-email = os.getenv("BIGIP_EMAIL", "test@test.test")
-user = os.getenv("BIGIP_USERNAME")
-password = os.getenv("BIGIP_PASSWORD")
-bigip_list = os.getenv("BIGIP_LIST")
-partition = os.getenv("BIGIP_PARTITION", "Intern")
-clientssl_parent = os.getenv("BIGIP_CLIENTSSL_PARENT")
-vs_list = os.getenv("BIGIP_VS_LIST")
-device_group = os.getenv("BIGIP_DEVICE_GROUP", "fail-sync")
-iapp = os.getenv("BIGIP_IAPP")
-custom_partition = os.getenv("BIGIP_CUSTOM_PARTITION", "Common")
-custom_vs_list = os.getenv("BIGIP_CUSTOM_VS_LIST")
-
-from OpenSSL import crypto, SSL
+email = os.getenv('BIGIP_EMAIL', 'test@test.test')
+user = os.getenv('BIGIP_USERNAME')
+password = os.getenv('BIGIP_PASSWORD')
+bigip_list = os.getenv('BIGIP_LIST')
+partition = os.getenv('BIGIP_PARTITION', 'Intern')
+clientssl_parent = os.getenv('BIGIP_CLIENTSSL_PARENT')
+vs_list = os.getenv('BIGIP_VS_LIST')
+device_group = os.getenv('BIGIP_DEVICE_GROUP', 'fail-sync')
+iapp = os.getenv('BIGIP_IAPP')
+custom_partition = os.getenv('BIGIP_CUSTOM_PARTITION', 'Common')
+custom_vs_list = os.getenv('BIGIP_CUSTOM_VS_LIST')
 
 
 def cert_gen(
-    emailAddress="emailAddress",
-    commonName="commonName",
-    countryName="NT",
-    localityName="localityName",
-    stateOrProvinceName="stateOrProvinceName",
-    organizationName="organizationName",
-    organizationUnitName="organizationUnitName",
+    emailAddress='emailAddress',
+    commonName='commonName',
+    countryName='NT',
+    localityName='localityName',
+    stateOrProvinceName='stateOrProvinceName',
+    organizationName='organizationName',
+    organizationUnitName='organizationUnitName',
     serialNumber=0,
     validityStartInSeconds=0,
     validityEndInSeconds=10 * 365 * 24 * 60 * 60,
-    KEY_FILE="private.key",
-    CERT_FILE="selfsigned.crt",
+    KEY_FILE='private.key',
+    CERT_FILE='selfsigned.crt',
 ):
     # can look at generated file using openssl:
     # openssl x509 -inform pem -in selfsigned.crt -noout -text
     # create a key pair
     k = crypto.PKey()
     k.generate_key(crypto.TYPE_RSA, 4096)
     # create a self-signed cert
@@ -50,19 +50,19 @@
     cert.get_subject().CN = commonName
     cert.get_subject().emailAddress = emailAddress
     cert.set_serial_number(serialNumber)
     cert.gmtime_adj_notBefore(0)
     cert.gmtime_adj_notAfter(validityEndInSeconds)
     cert.set_issuer(cert.get_subject())
     cert.set_pubkey(k)
-    cert.sign(k, "sha512")
-    with open(CERT_FILE, "wt") as f:
-        f.write(crypto.dump_certificate(crypto.FILETYPE_PEM, cert).decode("utf-8"))
-    with open(KEY_FILE, "wt") as f:
-        f.write(crypto.dump_privatekey(crypto.FILETYPE_PEM, k).decode("utf-8"))
+    cert.sign(k, 'sha512')
+    with open(CERT_FILE, 'wt') as f:
+        f.write(crypto.dump_certificate(crypto.FILETYPE_PEM, cert).decode('utf-8'))
+    with open(KEY_FILE, 'wt') as f:
+        f.write(crypto.dump_privatekey(crypto.FILETYPE_PEM, k).decode('utf-8'))
 
 
 #########################################################
 # Instanciating an object without using the certbot-CLI #
 #########################################################
 
 
@@ -74,36 +74,36 @@
         self.certbot_bigip_partition = partition
         self.certbot_bigip_iapp = iapp
         self.certbot_bigip_clientssl_parent = clientssl_parent
         self.certbot_bigip_vs_list = vs_list
         self.certbot_bigip_device_group = device_group
         self.certbot_bigip_apm = False
         self.certbot_bigip_verify_ssl = False
-        self.backup_dir = "/tests/backup"
+        self.backup_dir = '/tests/backup'
         self.strict_permissions = False
-        self.temp_checkpoint_dir = "/tests/backup"
-        self.in_progress_dir = "/tests/backup"
+        self.temp_checkpoint_dir = '/tests/backup'
+        self.in_progress_dir = '/tests/backup'
 
 
 def test_upload_cert_to_bigip():
     config = Config()
 
-    configurator = BigipConfigurator(config, "certbot_bigip")
+    configurator = BigipConfigurator(config, 'certbot_bigip')
     configurator.prepare()
-    configurator.cert_chain_name = "test_chain"
+    configurator.cert_chain_name = 'test_chain'
 
-    domain = "test01.certbot.on.at"
+    domain = 'test01.certbot.on.at'
 
     from pathlib import Path
 
-    Path("tests/test_certificates").mkdir(parents=True, exist_ok=True)
+    Path('tests/test_certificates').mkdir(parents=True, exist_ok=True)
 
-    cert_path = "tests/test_certificates/test_certbot_ong_at.pem"
-    key_path = "tests/test_certificates/test_certbot_ong_at_key.pem"
-    chain_path = "tests/test_certificates/test_chain.pem"
+    cert_path = 'tests/test_certificates/test_certbot_ong_at.pem'
+    key_path = 'tests/test_certificates/test_certbot_ong_at_key.pem'
+    chain_path = 'tests/test_certificates/test_chain.pem'
 
     cert_gen(CERT_FILE=cert_path, KEY_FILE=key_path)
 
     if configurator.deploy_cert(
         domain,
         cert_path,
         key_path,
```

### Comparing `certbot-bigip-1.2.0/tests/test_shellcommands.py` & `certbot-bigip-1.2.1/tests/test_shellcommands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,241 +1,244 @@
-"""
+'''
 This test the deployment of several integration test
-"""
+'''
 
 import subprocess
 import re
 import logging
 import ssl
 import socket
 import os
 import pytest
 
+from os import system
+
+
 logging.basicConfig(level=logging.DEBUG)
 mylogger = logging.getLogger(__name__)
 
-email = os.getenv("BIGIP_EMAIL", "test@test.test")
-user = os.getenv("BIGIP_USERNAME")
-password = os.getenv("BIGIP_PASSWORD")
-bigip_list = os.getenv("BIGIP_LIST")
-partition = os.getenv("BIGIP_PARTITION")
-clientssl_parent = os.getenv("BIGIP_CLIENTSSL_PARENT")
-vs_list = os.getenv("BIGIP_VS_LIST")
-device_group = os.getenv("BIGIP_DEVICE_GROUP", "fail-sync")
-iapp = os.getenv("BIGIP_IAPP")
-custom_partition = os.getenv("BIGIP_CUSTOM_PARTITION", "Common")
-custom_vs_list = os.getenv("BIGIP_CUSTOM_VS_LIST")
+email = os.getenv('BIGIP_EMAIL', 'test@test.test')
+user = os.getenv('BIGIP_USERNAME')
+password = os.getenv('BIGIP_PASSWORD')
+bigip_list = os.getenv('BIGIP_LIST')
+partition = os.getenv('BIGIP_PARTITION')
+clientssl_parent = os.getenv('BIGIP_CLIENTSSL_PARENT')
+vs_list = os.getenv('BIGIP_VS_LIST')
+device_group = os.getenv('BIGIP_DEVICE_GROUP', 'fail-sync')
+iapp = os.getenv('BIGIP_IAPP')
+custom_partition = os.getenv('BIGIP_CUSTOM_PARTITION', 'Common')
+custom_vs_list = os.getenv('BIGIP_CUSTOM_VS_LIST')
 
 
 def validate_certbot_certificate_delivery(stdout: str, stderr: str):
     # from https://www.regextester.com/96683
-    regex_date = r"([12]\d{3}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01]))"
-    regex_cert_expire_indicator = "(?<=certificate expires on )"
+    regex_date = r'([12]\d{3}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01]))'
+    regex_cert_expire_indicator = '(?<=certificate expires on )'
     regex_check_result = regex_cert_expire_indicator + regex_date
     match = re.search(regex_check_result, stdout)
     if match is not None:
-        mylogger.info("New Certificate was created. Expiration Date: " + match.group(1))
+        mylogger.info('New Certificate was created. Expiration Date: ' + match.group(1))
         return True
     else:
         mylogger.error(
-            "Certificate aquirement failed: \n stdout:\n"
+            'Certificate aquirement failed: \n stdout:\n'
             + stdout
-            + "\n sterr:\n"
+            + '\n stderr:\n'
             + stderr
         )
+        mylogger.debug(system('cat /var/log/letsencrypt/letsencrypt.log'))
         return False
 
 
 def validate_certbot_certificate_delivery_renew(stdout: str, stderr: str):
     # from https://www.regextester.com/96683
-    regex_check_result = "(?<=Congratulations, all renewals succeeded)"
+    regex_check_result = '(?<=Congratulations, all renewals succeeded)'
     match = re.search(regex_check_result, stdout)
     if match is not None:
-        mylogger.info("Renewal succeded")
+        mylogger.info('Renewal succeded')
         return True
     else:
         mylogger.error(
-            "Certificate aquirement failed: \n stdout:\n"
+            'Certificate aquirement failed: \n stdout:\n'
             + stdout
-            + "\n sterr:\n"
+            + '\n stderr:\n'
             + stderr
         )
+        mylogger.debug(system('cat /var/log/letsencrypt/letsencrypt.log'))
         return False
 
 def get_certbot_certificate(domain: str):
-    file_path = f"/etc/letsencrypt/live/{domain}/cert.pem"
+    file_path = f'/etc/letsencrypt/live/{domain}/cert.pem'
 
-    with open(file_path, "r") as cert_file:
+    with open(file_path, 'r') as cert_file:
         return cert_file.read()
 
 
 def is_delivered_cert_equal_deployed_cert(domain):
     # check if certificate has been deployed
     delivered_cert = get_certbot_certificate(domain)
     socket.setdefaulttimeout(
         5
     )  # set the timeout low to fail quickly if no certificate is served by the server
 
     # use sni in ssl communication
     port = 443
     conn = ssl.create_connection((domain, port))
-    context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
     sock = context.wrap_socket(conn, server_hostname=domain)
     deployed_cert = ssl.DER_cert_to_PEM_cert(sock.getpeercert(True))
-    mylogger.debug(f"delivered_cert: \n {delivered_cert}")
-    mylogger.debug(f"deployed_cert: \n {deployed_cert}")
+    mylogger.debug(f'delivered_cert: \n {delivered_cert}')
+    mylogger.debug(f'deployed_cert: \n {deployed_cert}')
     return delivered_cert == deployed_cert
 
 
 def test_response_evaluation():
     stdout_sample = 'Successfully received certificate.\nCertificate is saved at: /etc/letsencrypt/live/example.on.at/fullchain.pem\nKey is saved at:         /etc/letsencrypt/live/example.on.at/privkey.pem\nThis certificate expires on 2023-04-25.\nThese files will be updated when the certificate renews.'
-    stderr_sample = ""
+    stderr_sample = ''
     validate_certbot_certificate_delivery(stdout_sample, stderr_sample)
 
 
 def test_certbot_bigip_server_cert():
-    domain = "test01.certbot.on.at"
+    domain = 'test01.certbot.on.at'
     response = subprocess.run(
         (
-            f"certbot --non-interactive --expand --email '{email}' --agree-tos"
-            " -a bigip -i bigip"
-            f" --bigip-list '{bigip_list}'"
-            f" --bigip-username '{user}'"
-            f" --bigip-password '{password}'"
-            f" --bigip-partition '{partition}'"
-            f" --bigip-clientssl-parent '{clientssl_parent}'"
-            f" --bigip-vs-list '{vs_list}'"
-            f" --bigip-device-group '{device_group}'"
-            f" --bigip-iapp '{iapp}'"
-            f" -d {domain}"
-            " -v --staging --debug --force-renewal"
+            f'certbot --non-interactive --expand --email \'{email}\' --agree-tos'
+            ' -a bigip -i bigip'
+            f' --bigip-list \'{bigip_list}\''
+            f' --bigip-username \'{user}\''
+            f' --bigip-password \'{password}\''
+            f' --bigip-partition \'{partition}\''
+            f' --bigip-clientssl-parent \'{clientssl_parent}\''
+            f' --bigip-vs-list \'{vs_list}\''
+            f' --bigip-device-group \'{device_group}\''
+            f' --bigip-iapp \'{iapp}\''
+            f' -d {domain}'
+            ' -v --staging --debug --force-renewal'
         ),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
     )
 
-    mylogger.debug(response.stdout.decode("utf-8"))
+    mylogger.debug(response.stdout.decode('utf-8'))
 
     # check if new certificate was created
     if not validate_certbot_certificate_delivery(
-        response.stdout.decode("utf-8"), response.stderr.decode("utf-8")
+        response.stdout.decode('utf-8'), response.stderr.decode('utf-8')
     ):
         assert False
     # check if process has finished correctly
     response.check_returncode()
 
     # check if certificate has been deployed
     assert is_delivered_cert_equal_deployed_cert(
         domain
-    ), "did you assign the ssl profile to the virtualserver? this step is not automated."
+    ), 'did you assign the ssl profile to the virtualserver? this step is not automated.'
 
 
 def test_certbot_bigip_server_cert_renew():
-    domain = "test01.certbot.on.at"
+    domain = 'test01.certbot.on.at'
     response = subprocess.run(
         (
-            f"certbot renew --force-renewal"
+            f'certbot renew --force-renewal'
         ),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
     )
 
-    mylogger.debug(response.stdout.decode("utf-8"))
-
     # check if new certificate was created
     if not validate_certbot_certificate_delivery_renew(
-        response.stdout.decode("utf-8"), response.stderr.decode("utf-8")
+        response.stdout.decode('utf-8'), response.stderr.decode('utf-8')
     ):
         assert False
     # check if process has finished correctly
     response.check_returncode()
 
     # check if certificate has been deployed
     assert is_delivered_cert_equal_deployed_cert(
         domain
-    ), "did you assign the ssl profile to the virtualserver? this step is not automated."
+    ), 'did you assign the ssl profile to the virtualserver? this step is not automated.'
 
 
 def test_certbot_bigip_deployment_in_custompartition_and_folders():
-    domain = "test02.certbot.on.at"
+    domain = 'test02.certbot.on.at'
     response = subprocess.run(
         (
-            f"certbot --non-interactive --expand --email '{email}' --agree-tos"
-            " -a bigip -i bigip"
-            f" --bigip-list '{bigip_list}'"
-            f" --bigip-username '{user}'"
-            f" --bigip-password '{password}'"
-            f" --bigip-partition '{custom_partition}'"
-            f" --bigip-clientssl-parent '{clientssl_parent}'"
-            f" --bigip-vs-list '{custom_vs_list}'"
-            f" --bigip-device-group '{device_group}'"
-            f" -d {domain}"
-            " -v --staging --debug --force-renewal"
+            f'certbot --non-interactive --expand --email \'{email}\' --agree-tos'
+            ' -a bigip -i bigip'
+            f' --bigip-list \'{bigip_list}\''
+            f' --bigip-username \'{user}\''
+            f' --bigip-password \'{password}\''
+            f' --bigip-partition \'{custom_partition}\''
+            f' --bigip-clientssl-parent \'{clientssl_parent}\''
+            f' --bigip-vs-list \'{custom_vs_list}\''
+            f' --bigip-device-group \'{device_group}\''
+            f' -d {domain}'
+            ' -v --staging --debug --force-renewal'
         ),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
     )
 
     # check if new certificate was created
     if not validate_certbot_certificate_delivery(
-        response.stdout.decode("utf-8"), response.stderr.decode("utf-8")
+        response.stdout.decode('utf-8'), response.stderr.decode('utf-8')
     ):
         assert False
 
     # check if process has finished correctly
     response.check_returncode()
 
     # check if certificate has been deployed
     assert is_delivered_cert_equal_deployed_cert(
         domain
-    ), "did you assign the ssl profile to the virtualserver? this step is not automated."
+    ), 'did you assign the ssl profile to the virtualserver? this step is not automated.'
 
 
-@pytest.mark.skip(reason="no way of currently testing this")
+@pytest.mark.skip(reason='no way of currently testing this')
 def test_wildcard_deployment_with_bluecat_validation():
-    domain = "*.certbot.on.at"
+    domain = '*.certbot.on.at'
     response = subprocess.run(
         (
-            "certbot"
-            " --non-interactive"
-            f" -d {domain}"
-            " --staging"
-            " --expand"
-            f" --email '{email}'"
-            " --agree-tos"
-            " --no-eff-email"
-            " -v"
-            " --debug"
-            " --force-renewal"
+            'certbot'
+            ' --non-interactive'
+            f' -d {domain}'
+            ' --staging'
+            ' --expand'
+            f' --email \'{email}\''
+            ' --agree-tos'
+            ' --no-eff-email'
+            ' -v'
+            ' --debug'
+            ' --force-renewal'
             # authentication
-            " -a bluecat"
-            " -i bigip"
-            f" --bigip-list '{bigip_list}'"
-            f" --bigip-username '{user}'"
-            f" --bigip-password '{password}'"
-            f" --bigip-partition '{partition}'"
-            f" --bigip-clientssl-parent '{clientssl_parent}'"
-            f" --bigip-vs-list '{vs_list}'"
-            f" --bigip-device-group '{device_group}'"
-            f" --bigip-iapp '{iapp}'"
+            ' -a bluecat'
+            ' -i bigip'
+            f' --bigip-list \'{bigip_list}\''
+            f' --bigip-username \'{user}\''
+            f' --bigip-password \'{password}\''
+            f' --bigip-partition \'{partition}\''
+            f' --bigip-clientssl-parent \'{clientssl_parent}\''
+            f' --bigip-vs-list \'{vs_list}\''
+            f' --bigip-device-group \'{device_group}\''
+            f' --bigip-iapp \'{iapp}\''
         ),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         shell=True,
     )
 
     # check if new certificate was created
     if not validate_certbot_certificate_delivery(
-        response.stdout.decode("utf-8"), response.stderr.decode("utf-8")
+        response.stdout.decode('utf-8'), response.stderr.decode('utf-8')
     ):
         assert False
 
     # check if process has finished correctly
     response.check_returncode()
 
     # check if certificate has been deployed
     assert is_delivered_cert_equal_deployed_cert(
-        domain.strip("*.")
-    ), "did you assign the ssl profile to the virtualserver? this step is not automated."
+        domain.strip('*.')
+    ), 'did you assign the ssl profile to the virtualserver? this step is not automated.'
```

