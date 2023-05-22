# Comparing `tmp/lockss_turtles-0.4.0.dev4.tar.gz` & `tmp/lockss_turtles-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_turtles-0.4.0.dev4.tar", max compression
+gzip compressed data, was "lockss_turtles-0.4.0.post1.tar", max compression
```

## Comparing `lockss_turtles-0.4.0.dev4.tar` & `lockss_turtles-0.4.0.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3158 2023-04-06 06:42:02.921705 lockss_turtles-0.4.0.dev4/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/LICENSE
--rw-r--r--   0        0        0    38149 2023-05-03 16:15:30.831989 lockss_turtles-0.4.0.dev4/README.rst
--rw-r--r--   0        0        0     1001 2023-05-03 16:15:37.332061 lockss_turtles-0.4.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     3201 2023-05-03 16:15:42.118780 lockss_turtles-0.4.0.dev4/src/lockss/turtles/__init__.py
--rw-r--r--   0        0        0     1633 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/__main__.py
--rw-r--r--   0        0        0     9074 2023-04-06 06:32:04.687811 lockss_turtles-0.4.0.dev4/src/lockss/turtles/app.py
--rw-r--r--   0        0        0    22476 2023-05-03 15:57:35.377335 lockss_turtles-0.4.0.dev4/src/lockss/turtles/cli.py
--rw-r--r--   0        0        0     4312 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin.py
--rw-r--r--   0        0        0     9441 2023-05-03 16:13:11.827075 lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin_registry.py
--rw-r--r--   0        0        0    10486 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin_set.py
--rw-r--r--   0        0        0     1579 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/__init__.py
--rw-r--r--   0        0        0      685 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
--rw-r--r--   0        0        0     2766 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-registry-schema.json
--rw-r--r--   0        0        0      650 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-set-catalog-schema.json
--rw-r--r--   0        0        0     2338 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-set-schema.json
--rw-r--r--   0        0        0      753 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
--rw-r--r--   0        0        0     2430 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev4/src/lockss/turtles/util.py
--rw-r--r--   0        0        0    39406 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     3271 2023-05-22 19:46:41.642669 lockss_turtles-0.4.0.post1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-05-18 06:19:10.992337 lockss_turtles-0.4.0.post1/LICENSE
+-rw-r--r--   0        0        0    38455 2023-05-22 19:46:41.642669 lockss_turtles-0.4.0.post1/README.rst
+-rw-r--r--   0        0        0     1002 2023-05-22 19:46:41.642669 lockss_turtles-0.4.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     3202 2023-05-22 19:46:41.642669 lockss_turtles-0.4.0.post1/src/lockss/turtles/__init__.py
+-rw-r--r--   0        0        0     1633 2023-05-18 06:19:10.992337 lockss_turtles-0.4.0.post1/src/lockss/turtles/__main__.py
+-rw-r--r--   0        0        0     9074 2023-05-18 06:19:45.689493 lockss_turtles-0.4.0.post1/src/lockss/turtles/app.py
+-rw-r--r--   0        0        0    22476 2023-05-18 06:19:45.692826 lockss_turtles-0.4.0.post1/src/lockss/turtles/cli.py
+-rw-r--r--   0        0        0     4312 2023-05-18 06:19:45.692826 lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin.py
+-rw-r--r--   0        0        0     9441 2023-05-18 06:19:45.692826 lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin_registry.py
+-rw-r--r--   0        0        0    10486 2023-05-18 06:19:45.692826 lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin_set.py
+-rw-r--r--   0        0        0     1579 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/__init__.py
+-rw-r--r--   0        0        0      685 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
+-rw-r--r--   0        0        0     2766 2023-05-18 06:19:45.692826 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-registry-schema.json
+-rw-r--r--   0        0        0      650 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-set-catalog-schema.json
+-rw-r--r--   0        0        0     2338 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-set-schema.json
+-rw-r--r--   0        0        0      753 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
+-rw-r--r--   0        0        0     2430 2023-05-18 06:19:10.995670 lockss_turtles-0.4.0.post1/src/lockss/turtles/util.py
+-rw-r--r--   0        0        0    39713 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.post1/PKG-INFO
```

### Comparing `lockss_turtles-0.4.0.dev4/CHANGELOG.rst` & `lockss_turtles-0.4.0.post1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 =============
 Release Notes
 =============
 
+-----------
+0.4.0-post1
+-----------
+
+Released: 2023-05-22
+
+*  **Bugfixes**
+
+   *  Documentation fixes.
+
 -----
 0.4.0
 -----
 
-Released: ?
+Released: 2023-05-17
 
 *  **Features**
 
    *  ``directory`` plugin registry layout now has the same file naming convention option as ``rcs``.
 
    *  New ``directory``/``rcs`` file naming convention ``underscore``: replace ``.`` in the plugin identifier by ``_`` and add ``.jar``.
```

### Comparing `lockss_turtles-0.4.0.dev4/LICENSE` & `lockss_turtles-0.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/README.rst` & `lockss_turtles-0.4.0.post1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 =======
 Turtles
 =======
 
-.. |RELEASE| replace:: 0.4.0-dev4
-.. |RELEASE_DATE| replace:: ?
+.. |RELEASE| replace:: 0.4.0-post1
+.. |RELEASE_DATE| replace:: 2023-05-22
 
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
 .. |LAYER| replace:: ``--layer/-l``
 .. |LAYERS| replace:: ``--layers/-L``
 .. |PLUGIN_REGISTRY_CATALOG| replace:: ``--plugin-registry-catalog/-r``
 .. |PLUGIN_SET_CATALOG| replace:: ``--plugin-set-catalog/-s``
 .. |PLUGIN_SIGNING_CREDENTIALS| replace:: ``--plugin-signing-credentials/-c``
 .. |PRODUCTION| replace:: ``--production/-p``
 .. |TESTING| replace:: ``--testing/-t``
 
+.. image:: https://assets.lockss.org/images/logos/turtles/turtles_128x128.png
+   :alt: Turtles logo
+   :align: right
+
 Turtles is a tool to manage LOCKSS plugin sets and LOCKSS plugin registries.
 
 **Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
@@ -397,14 +401,16 @@
    *Required.* Non-empty list of the plugin identifiers in this plugin registry.
 
 ``suppressed-plugin-identifiers``
    *Optional.* Non-empty list of plugin identifiers that are excluded from this plugin registry.
 
    Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
 
+   Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
+
 Plugin Registry Layouts
 =======================
 
 Turtles supports two kinds of plugin registry layouts:
 
 *  `Directory Plugin Registry Layout`_
 
@@ -795,15 +801,15 @@
                             add the layers in FILE to the list of plugin registry
                             layers to process
 
 The command needs:
 
 *  A `Plugin Registry Catalog`_, either from the |PLUGIN_REGISTRY_CATALOG| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
-*  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|IDENTIFIER| options, |IDENTIFIERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
+*  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|LAYER| options, |LAYERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
 
 *  One or more JAR paths. The list of JAR paths to process is derived from:
 
    *  The JAR paths listed as bare arguments to the command.
 
    *  The JAR paths listed as |JAR| options.
 
@@ -845,15 +851,15 @@
 The ``license`` command displays the license terms for Turtles and exits.
 
 .. _release-plugin:
 
 ``release-plugin`` (``rp``)
 ---------------------------
 
-The ``release-plugin`` command is used for `Building Plugins`_ and `Deploying Plugins`, being essentially `build-plugin`_ followed by `deploy-plugin`_. It has its own |HELP| option::
+The ``release-plugin`` command is used for `Building Plugins`_ and `Deploying Plugins`_, being essentially `build-plugin`_ followed by `deploy-plugin`_. It has its own |HELP| option::
 
     usage: turtles release-plugin [-h] [--output-format FMT] [--password PASS]
                                   [--plugin-registry-catalog FILE]
                                   [--plugin-set-catalog FILE]
                                   [--plugin-signing-credentials FILE]
                                   [--production] [--testing] [--identifier PLUGID]
                                   [--identifiers FILE] [--layer LAYER]
@@ -985,17 +991,17 @@
 *  The plugin identifiers found in the files listed as |IDENTIFIERS| options.
 
 Plugin Registry Layer Options
 -----------------------------
 
 Commands that are `Deploying Plugins`_ expect one or more plugin registry layer IDs. The list of plugin registry layer IDs to target is derived from:
 
-*  The plugin registry layer IDs listed as |JAR| options.
+*  The plugin registry layer IDs listed as |LAYER| options.
 
-*  The plugin registry layer IDs found in the files listed as |JARS| options.
+*  The plugin registry layer IDs found in the files listed as |LAYERS| options.
 
 As a convenience, the following synonyms also exist:
 
 *  |TESTING| is a synonym for ``--layer=testing``
 
 *  |PRODUCTION| is a synonym for ``--layer=production``
```

### Comparing `lockss_turtles-0.4.0.dev4/pyproject.toml` & `lockss_turtles-0.4.0.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-turtles"
-version = "0.4.0-dev4"
+version = "0.4.0-post1"
 description = "Tool to manage LOCKSS plugin sets and LOCKSS plugin registries"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
```

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/__init__.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.4.0-dev4'
+__version__ = '0.4.0-post1'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/__main__.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/__main__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/app.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/app.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/cli.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/cli.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin_registry.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/plugin_set.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/plugin_set.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/__init__.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-registry-catalog-schema.json` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-registry-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-registry-schema.json` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-registry-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-set-catalog-schema.json` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-set-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-set-schema.json` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-set-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/resources/plugin-signing-credentials-schema.json` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/resources/plugin-signing-credentials-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/src/lockss/turtles/util.py` & `lockss_turtles-0.4.0.post1/src/lockss/turtles/util.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev4/PKG-INFO` & `lockss_turtles-0.4.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-turtles
-Version: 0.4.0.dev4
+Version: 0.4.0.post1
 Summary: Tool to manage LOCKSS plugin sets and LOCKSS plugin registries
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,30 +29,34 @@
 Project-URL: Repository, https://github.com/lockss/lockss-turtles
 Description-Content-Type: text/x-rst
 
 =======
 Turtles
 =======
 
-.. |RELEASE| replace:: 0.4.0-dev4
-.. |RELEASE_DATE| replace:: ?
+.. |RELEASE| replace:: 0.4.0-post1
+.. |RELEASE_DATE| replace:: 2023-05-22
 
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
 .. |LAYER| replace:: ``--layer/-l``
 .. |LAYERS| replace:: ``--layers/-L``
 .. |PLUGIN_REGISTRY_CATALOG| replace:: ``--plugin-registry-catalog/-r``
 .. |PLUGIN_SET_CATALOG| replace:: ``--plugin-set-catalog/-s``
 .. |PLUGIN_SIGNING_CREDENTIALS| replace:: ``--plugin-signing-credentials/-c``
 .. |PRODUCTION| replace:: ``--production/-p``
 .. |TESTING| replace:: ``--testing/-t``
 
+.. image:: https://assets.lockss.org/images/logos/turtles/turtles_128x128.png
+   :alt: Turtles logo
+   :align: right
+
 Turtles is a tool to manage LOCKSS plugin sets and LOCKSS plugin registries.
 
 **Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
@@ -428,14 +432,16 @@
    *Required.* Non-empty list of the plugin identifiers in this plugin registry.
 
 ``suppressed-plugin-identifiers``
    *Optional.* Non-empty list of plugin identifiers that are excluded from this plugin registry.
 
    Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
 
+   Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
+
 Plugin Registry Layouts
 =======================
 
 Turtles supports two kinds of plugin registry layouts:
 
 *  `Directory Plugin Registry Layout`_
 
@@ -826,15 +832,15 @@
                             add the layers in FILE to the list of plugin registry
                             layers to process
 
 The command needs:
 
 *  A `Plugin Registry Catalog`_, either from the |PLUGIN_REGISTRY_CATALOG| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
-*  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|IDENTIFIER| options, |IDENTIFIERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
+*  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|LAYER| options, |LAYERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
 
 *  One or more JAR paths. The list of JAR paths to process is derived from:
 
    *  The JAR paths listed as bare arguments to the command.
 
    *  The JAR paths listed as |JAR| options.
 
@@ -876,15 +882,15 @@
 The ``license`` command displays the license terms for Turtles and exits.
 
 .. _release-plugin:
 
 ``release-plugin`` (``rp``)
 ---------------------------
 
-The ``release-plugin`` command is used for `Building Plugins`_ and `Deploying Plugins`, being essentially `build-plugin`_ followed by `deploy-plugin`_. It has its own |HELP| option::
+The ``release-plugin`` command is used for `Building Plugins`_ and `Deploying Plugins`_, being essentially `build-plugin`_ followed by `deploy-plugin`_. It has its own |HELP| option::
 
     usage: turtles release-plugin [-h] [--output-format FMT] [--password PASS]
                                   [--plugin-registry-catalog FILE]
                                   [--plugin-set-catalog FILE]
                                   [--plugin-signing-credentials FILE]
                                   [--production] [--testing] [--identifier PLUGID]
                                   [--identifiers FILE] [--layer LAYER]
@@ -1016,17 +1022,17 @@
 *  The plugin identifiers found in the files listed as |IDENTIFIERS| options.
 
 Plugin Registry Layer Options
 -----------------------------
 
 Commands that are `Deploying Plugins`_ expect one or more plugin registry layer IDs. The list of plugin registry layer IDs to target is derived from:
 
-*  The plugin registry layer IDs listed as |JAR| options.
+*  The plugin registry layer IDs listed as |LAYER| options.
 
-*  The plugin registry layer IDs found in the files listed as |JARS| options.
+*  The plugin registry layer IDs found in the files listed as |LAYERS| options.
 
 As a convenience, the following synonyms also exist:
 
 *  |TESTING| is a synonym for ``--layer=testing``
 
 *  |PRODUCTION| is a synonym for ``--layer=production``
```

