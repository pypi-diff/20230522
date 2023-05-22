# Comparing `tmp/z0lib-2.0.4.tar.gz` & `tmp/z0lib-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z0lib-2.0.4.tar", last modified: Fri Apr 14 15:32:52 2023, max compression
+gzip compressed data, was "dist/z0lib-2.0.5.tar", last modified: Mon May 22 08:42:42 2023, max compression
```

## Comparing `z0lib-2.0.4.tar` & `z0lib-2.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1505 2023-04-14 15:32:52.842398 z0lib-2.0.4/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7402 2023-04-14 15:32:52.000000 z0lib-2.0.4/README.rst
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 15:32:52.842398 z0lib-2.0.4/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1936 2023-04-14 14:48:04.000000 z0lib-2.0.4/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/explore_env.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4999 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/optargs
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6393 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1936 2023-04-14 15:28:25.000000 z0lib-2.0.4/z0lib/scripts/setup.info
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib/tests/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4783 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/tests/test_runtraced.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/tests/test_z0lib.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/tmp.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.4/z0lib/tests/tmp1.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4118 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/xuname
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    58413 2023-04-14 14:48:04.000000 z0lib-2.0.4/z0lib/z0librc
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20882 2023-04-14 14:47:59.000000 z0lib-2.0.4/z0lib/z0librun.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 15:32:52.842398 z0lib-2.0.4/z0lib.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1505 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      531 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.4/z0lib.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-04-14 15:32:52.000000 z0lib-2.0.4/z0lib.egg-info/top_level.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/tests/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4853 2023-05-20 08:02:42.000000 z0lib-2.0.5/z0lib/tests/test_runtraced.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/tmp.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/tmp1.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-05-20 08:02:43.000000 z0lib-2.0.5/z0lib/tests/test_z0lib.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1952 2023-05-20 08:36:29.000000 z0lib-2.0.5/z0lib/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2023-05-20 08:02:43.000000 z0lib-2.0.5/z0lib/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4039 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/xuname
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    57347 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/z0librc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/explore_env.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4920 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/optargs
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20883 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/z0librun.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-22 08:42:42.000000 z0lib-2.0.5/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1650 2023-05-22 07:11:35.000000 z0lib-2.0.5/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.5/z0lib.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      531 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       20 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-22 08:42:42.000000 z0lib-2.0.5/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6379 2023-05-22 08:37:43.000000 z0lib-2.0.5/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `z0lib-2.0.4/README.rst` & `z0lib-2.0.5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
-===========
-z0lib 2.0.4
-===========
+======
+ 2.0.5
+======
 
 
 
-|Maturity| |Build Status| |Coverage Status| |license gpl|
+|Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -31,96 +31,86 @@
 |
 |
 
 Getting started
 ===============
 
 
-|
-
-Installation
-------------
-
 Installation
 ------------
 
 Zeroincombenze tools require:
 
-* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20
-* python 2.7, some tools require python 3.6+
+* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+* python 2.7+, some tools require python 3.6+
 * bash 5.0+
 
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    pip install z0lib
+::
+
+    pip install 
 
 |
 
 Current version via Git
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     git clone https://github.com/zeroincombenze/tools.git
     cd ./tools
     ./install_tools.sh -p
-    source /opt/odoo/devel/activate_tools
+    source $HOME/devel/activate_tools
 
 
 Upgrade
 -------
 
-Upgrade
--------
-
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    pip install z0lib -U
+::
+
+    pip install  -U
 
 |
 
-Current stable version
-~~~~~~~~~~~~~~~~~~~~~~
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     ./install_tools.sh -U
-    source /opt/odoo/devel/activate_tools
-
-Current development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -Ud
-    source /opt/odoo/devel/activate_tools
+    source $HOME/devel/activate_tools
 
 
 History
 -------
 
+2.0.5 (2023-05-14)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] Sometime configuration init fails
+* [IMP] Configuration name LOCAL_PKGS read real packages
+* [IMP] is_pypi function more precise
+
 2.0.4 (2023-04-10)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_traced: cd does not work w/o alias
 * [IMP] coveralls and codecov are not more dependencies
 
 2.0.3 (2022-12-22)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_traced: --switch sometime crashes
-
-2.0.2.1 (2022-12-15)
-~~~~~~~~~~~~~~~~~~~~
-
 * [FIX] run_traced: alias function
 
 2.0.2 (2022-12-07)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] best recognition of python version
 * [FIX] run_traced: fail with python 2
@@ -175,59 +165,41 @@
 
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
-* Antonio Maria Vigliotti <info@shs-av.com>
-Contributors
-------------
-
+* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 
 
 |
 
-This module is part of tools project.
+This module is part of  project.
 
-Last Update / Ultimo aggiornamento: 2023-04-14
+Last Update / Ultimo aggiornamento: 
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-    :target: https://travis-ci.com/zeroincombenze/tools
-    :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-    :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-    :alt: Codecov
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
     :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
     :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/2.0
-    :alt: Codecov
-.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-   :target: https://odoo-italia.org
-   :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
 .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
 .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
```

### Comparing `z0lib-2.0.4/setup.py` & `z0lib-2.0.5/z0lib/scripts/setup.info`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0lib',
-    version='2.0.4',
+    version='2.0.5',
     description='Bash zeroincombenze lib',
     long_description="""
 General purpose bash and python library for zeroincombenze(R) tools
 
 Features:
 
 * xuname: unix/linux platform recognizer (tested on various environments)
@@ -35,13 +35,13 @@
     project_urls={
         'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
         'Source': 'https://github.com/zeroincombenze/tools',
     },
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
-    install_requires=['future'],
+    install_requires=['configparser', 'future'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': ['scripts/setup.info', './optargs', './xuname', './z0librc']},
     entry_points={'console_scripts': ['z0lib-info = z0lib.scripts.main:main']},
     zip_safe=False,
 )
```

### Comparing `z0lib-2.0.4/z0lib/optargs` & `z0lib-2.0.5/z0lib/optargs`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,24 @@
     Z0LIBDIR=$(readlink -e $d)
     break
   fi
 done
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.4
+__version__=2.0.5
 
 if [ "$OPTARGS_TEST_1_2" ]; then
   test_1_2=$OPTARGS_TEST_1_2
 else
   test_1_2=1
 fi
 if [ $test_1_2 -eq 1 ]; then
```

### Comparing `z0lib-2.0.4/z0lib/scripts/main.py` & `z0lib-2.0.5/z0lib/scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 General purpose bash and python library for zeroincombenze(R) tools
 
 Features:
 
 * xuname: unix/linux platform recognizer (tested on various environments)
 * parseoptargs: line command parser;
@@ -17,15 +17,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -101,20 +101,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `z0lib-2.0.4/z0lib/scripts/setup.info` & `z0lib-2.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from setuptools import find_packages, setup
 
+author = "Antonio Maria Vigliotti"
+author_email = "<info@shs-av.com>"
+source_url = "https://github.com/zeroincombenze/tools"
+doc_url = "https://github.com/zeroincombenze/tools"
+changelog_url = "%s/blob/master/z0lib/egg-info/CHANGELOG.rst" % source_url
+
+
 setup(
-    name='z0lib',
-    version='2.0.4',
-    description='Bash zeroincombenze lib',
-    long_description="""
-General purpose bash and python library for zeroincombenze(R) tools
-
-Features:
-
-* xuname: unix/linux platform recognizer (tested on various environments)
-* parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
-* tracelog: manage tracelog (only bash)
-* findpkg: find package in file system (only bash)
-* run_traced: execute (or dry_run) shell command (only bash)
-* CFG: local dictionary values from config file like python ConfigParser (only bash)
-""",
+    name="z0lib",
+    version="2.0.5",
+    description="Bash zeroincombenze lib",
+    long_description=open("README.rst").read(),
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: GNU Affero General Public License v3',
-        'Operating System :: POSIX',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: System :: System Shells',
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Operating System :: POSIX",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: System :: System Shells",
     ],
-    keywords='bash, optargs',
-    url='https://zeroincombenze-tools.readthedocs.io',
+    keywords="bash, optargs",
+    url="https://zeroincombenze-tools.readthedocs.io",
     project_urls={
-        'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
-        'Source': 'https://github.com/zeroincombenze/tools',
+        "Documentation": doc_url,
+        "Source": source_url,
+        "Changelog": changelog_url,
     },
-    author='Antonio Maria Vigliotti',
-    author_email='antoniomaria.vigliotti@gmail.com',
-    license='Affero GPL',
-    install_requires=['future'],
-    packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
-    package_data={'': ['scripts/setup.info', './optargs', './xuname', './z0librc']},
-    entry_points={'console_scripts': ['z0lib-info = z0lib.scripts.main:main']},
+    author=author,
+    author_email=author_email,
+    license="Affero GPL",
+    install_requires=["configparser", "future"],
+    packages=find_packages(exclude=["docs", "examples", "tests", "junk"]),
+    package_data={"": ["scripts/setup.info", "./optargs", "./xuname", "./z0librc"]},
+    entry_points={"console_scripts": ["z0lib-info = z0lib.scripts.main:main"]},
     zip_safe=False,
 )
+
+
+
+
+
+
+
+
+
+
```

### Comparing `z0lib-2.0.4/z0lib/tests/test_runtraced.py` & `z0lib-2.0.5/z0lib/tests/test_runtraced.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from __future__ import print_function, unicode_literals
 import os
 import sys
 from zerobug import z0test
 from z0lib import z0lib
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
@@ -64,14 +64,16 @@
         sts += self.run_test_cmd(z0ctx, "rm -fR %s" % fn)
         sts += self.Z.test_result(
             z0ctx, 'dir %s removed' % fn, True, not os.path.isdir(fn))
         return sts
 
     def test_02(self, z0ctx):
         fn = os.path.expanduser("~/16.0")
+        if os.path.isdir(fn):
+            os.system("rm -fR %s" % fn)
         self.run_test_cmd(z0ctx, "mkdir %s" % fn)
         self.run_test_cmd(z0ctx, "mkdir %s" % os.path.join(fn, "addons"))
         self.run_test_cmd(z0ctx, "mkdir %s" % os.path.join(fn, "odoo"))
         self.run_test_cmd(z0ctx, "mkdir %s" % os.path.join(fn, "odoo", "addons"))
         self.run_test_cmd(z0ctx, "touch %s" % os.path.join(fn, "odoo", "release.py"))
         self.run_test_cmd(z0ctx, "mkdir %s" % os.path.join(fn, ".git"))
         self.run_test_cmd(z0ctx, "mkdir %s" % os.path.join(fn, "repo1"))
```

### Comparing `z0lib-2.0.4/z0lib/tests/test_z0lib.py` & `z0lib-2.0.5/z0lib/tests/test_z0lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # import pdb
 import os
 
 # import sys
 # from zerobug import Z0test
 from z0lib import z0lib
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `z0lib-2.0.4/z0lib/tests/tmp.py` & `z0lib-2.0.5/z0lib/tests/tmp.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.4/z0lib/tests/tmp1.py` & `z0lib-2.0.5/z0lib/tests/tmp1.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.4/z0lib/xuname` & `z0lib-2.0.5/z0lib/xuname`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,24 @@
     Z0LIBDIR=$(readlink -e $d)
     break
   fi
 done
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.4
+__version__=2.0.5
 
 
 # Main program
 OPTOPTS=(h        a       c       d       f        i       k       m       p       r       s       v       V           x)
 OPTDEST=(opt_help opt_prm opt_prm opt_prm opt_prm  opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_version opt_prm)
 OPTACTI=("+"      "*>"    "*>"    "*>"    "*>"     "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"        "*>")
 OPTDEFL=(1        ""      ""      ""      ""       ""      ""      ""      ""      ""      ""      ""      ""          "")
```

### Comparing `z0lib-2.0.4/z0lib/z0librc` & `z0lib-2.0.5/z0lib/z0librc`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) SHS-AV s.r.l. (<http://ww.zeroincombenze.it>)
 # This software is free software under GNU Affero GPL3
 # Bash general purpose library
-#__version__=2.0.4
+#__version__=2.0.5
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
 [ "${BASH_SOURCE-}" == "$0" ] && echo "You must source this script: \$ source $0" >&2 && exit 33
 STS_FAILED=1
 STS_SUCCESS=0
 
 ##############################################################################
 # Install this lib file in /etc if version is more recent
@@ -294,15 +294,14 @@
       elif [[ $oo =~ ^- ]]; then
         local jj=1
         while ((jj<${#oo})); do
           jy=0
           f=0
           while ((jy<${#OPTOPTS[*]})); do
             if [[ ${oo:jj:1} == ${OPTOPTS[jy]} ]]; then
-              # set -x
               f=1
               a=${OPTACTI[jy]}
               b=${a:1:1}
               if [ "$b" == ">" ]; then
                  export opt_help=0
                  export opt_version=""
               fi
@@ -669,56 +668,14 @@
     done
     echo "$result"
     $SETX
 }
 export -f findpkg
 
 
-## Deprecated: use CFG_init
-#a_new() {
-#    [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
-#    if [ "$1" == "0" -o "$1" == "1" -o "$1" == "2" -o "$1" == "3" ]; then
-#      local tid=$1
-#    else
-#      local tid="0"
-#    fi
-#    cmd="unset DEFDICT$tid DEFRULE$tid"
-#    echo $cmd
-#    $SETX
-#}
-#export -f a_new
-
-
-
-## Deprecated: use CFG_init
-#a_active() {
-#    [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
-#    if [ "$1" == "0" -o "$1" == "1" -o "$1" == "2" -o "$1" == "3" ]; then
-#      local tid=$1
-#    else
-#      local tid="0"
-#    fi
-#    if [ "$XU_FH" != "RHEL" -a "$XU_FH" != "Debian" ]; then
-#      XU_FH=$(xuname "-f")
-#      local x=$(xuname "-v")
-#      local v=$(echo $x|awk -F. '{print $1}')
-#      XU_DISTO=$(xuname "-d")$v
-#    elif [ -z "$XU_DISTO" ]; then
-#      local x=$(xuname "-v")
-#      XU_DISTO=$(xuname "-d")${x:0:1}
-#    fi
-#    # declare -g XU_FH=$XU_FH XU_DISTO=$XU_DISTO
-#    # declare -gA DEFDICT$tid DEFRULE$tid
-#    cmd="XU_FH=$XU_FH XU_DISTO=$XU_DISTO; declare -gA DEFDICT$tid DEFRULE$tid"
-#    echo $cmd
-#    $SETX
-#}
-#export -f a_active
-
-
 ##############################################################################
 # Add key and value to dictionary (associative array)
 # key may be regex to match multiple values
 # It's a ugly solution but currently works
 #
 # Global variables declared by CFG_init
 #   DEFDICT  global dictionary based on unique key (associative array)
@@ -747,38 +704,38 @@
       if [[ $4 == "-d" ]]; then
         SFX="__$XU_DISTO"
       elif [[ $4 == "-f" ]]; then
         SFX="__$XU_FH"
       elif [[ -n $4 ]]; then
         SFX="__$4"
       else
-        SFX=
+        SFX=""
       fi
       key=${1//-/_}
       [[ $5 =~ (-D|1) ]] && SFX="${SFX}__DEV"
-      if [[ "$tid" == "0" ]]; then
-        if [ "${key:0:1}" == "^" ]; then
+      if [[ $tid == "0" ]]; then
+        if [[ "${key:0:1}" == "^" ]]; then
           DEFRULE0[$key$SFX]="$2"
         else
           DEFDICT0[$key$SFX]="$2"
         fi
       elif [[ $tid == "1" ]]; then
-        if [ "${key:0:1}" == "^" ]; then
+        if [[ "${key:0:1}" == "^" ]]; then
           DEFRULE1[$key$SFX]="$2"
         else
           DEFDICT1[$key$SFX]="$2"
         fi
       elif [[ $tid == "2" ]]; then
-        if [ "${key:0:1}" == "^" ]; then
+        if [[ "${key:0:1}" == "^" ]]; then
           DEFRULE2[$key$SFX]="$2"
         else
           DEFDICT2[$key$SFX]="$2"
         fi
       elif [[ $tid == "3" ]]; then
-        if [ "${key:0:1}" == "^" ]; then
+        if [[ "${key:0:1}" == "^" ]]; then
           DEFRULE3[$key$SFX]="$2"
         else
           DEFDICT3[$key$SFX]="$2"
         fi
       fi
     fi
     $SETX
@@ -808,38 +765,38 @@
 #    dictionary value to stdout
 #    status
 CFG_find() {
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     local p=""
     local sts=1
     local x SFX key KK
-    if [ -n "$2" ]; then
+    if [[ -n "$2" ]]; then
       SFX=
       key=${2//-/_}
-      if [ "$1" == "0" ]; then
+      if [[ $1 == "0" ]]; then
         for SFX in __${XU_DISTO}__DEV __${XU_FH}__DEV __$XU_DISTO __$XU_FH ""; do
           KK=$key$SFX
           p=${DEFDICT0[$KK]}
-          if [ -n "$p" ]; then break; fi
+          [[ -n "$p" ]] && break
         done
         if [ -z "$p" ]; then
           local KK=(${!DEFRULE0[@]})
           local SFX=
           for SFX in __${XU_DISTO}__DEV __${XU_FH}__DEV __$XU_DISTO __$XU_FH ""; do
             local jy=0
             while ((jy<${#DEFRULE0[@]})); do
               local K=${KK[$jy]}
               if [[ "$K" =~ ^.*$SFX ]]; then
                 if [[ "${key}__$XU_DISTO" =~ $K ]]; then
                   p=${DEFRULE0[$K]}
-                  local sts=0
+                  sts=0
                   break
                 elif [[ "${key}__$XU_FH" =~ $K ]]; then
                   p=${DEFRULE0[$K]}
-                  local sts=0
+                  sts=0
                   break
                 fi
               fi
               ((jy++))
             done
             if [ $sts -eq $STS_SUCCESS ]; then break; fi
           done
@@ -856,19 +813,19 @@
           for SFX in __${XU_DISTO}__DEV __${XU_FH}__DEV __$XU_DISTO __$XU_FH ""; do
             local jy=0
             while ((jy<${#DEFRULE1[@]})); do
               local K=${KK[$jy]}
               if [[ "$K" =~ ^.*$SFX ]]; then
                 if [[ "${key}__$XU_DISTO" =~ $K ]]; then
                   p=${DEFRULE1[$K]}
-                  local sts=0
+                  sts=0
                   break
                 elif [[ "${key}__$XU_FH" =~ $K ]]; then
                   p=${DEFRULE1[$K]}
-                  local sts=0
+                  sts=0
                   break
                 fi
               fi
               ((jy++))
             done
             if [ $sts -eq $STS_SUCCESS ]; then break; fi
           done
@@ -885,19 +842,19 @@
           for SFX in __${XU_DISTO}__DEV __${XU_FH}__DEV __$XU_DISTO __$XU_FH ""; do
             local jy=0
             while ((jy<${#DEFRULE2[@]})); do
               local K=${KK[$jy]}
               if [[ "$K" =~ ^.*$SFX ]]; then
                 if [[ "${key}__$XU_DISTO" =~ $K ]]; then
                   p=${DEFRULE2[$K]}
-                  local sts=0
+                  sts=0
                   break
                 elif [[ "${key}__$XU_FH" =~ $K ]]; then
                   p=${DEFRULE2[$K]}
-                  local sts=0
+                  sts=0
                   break
                 fi
               fi
               ((jy++))
             done
             if [ $sts -eq $STS_SUCCESS ]; then break; fi
           done
@@ -914,42 +871,36 @@
           for SFX in __${XU_DISTO}__DEV __${XU_FH}__DEV __$XU_DISTO __$XU_FH ""; do
             local jy=0
             while ((jy<${#DEFRULE3[@]})); do
               local K=${KK[$jy]}
               if [[ "$K" =~ ^.*$SFX ]]; then
                 if [[ "${key}__$XU_DISTO" =~ $K ]]; then
                   p=${DEFRULE3[$K]}
-                  local sts=0
+                  sts=0
                   break
                 elif [[ "${key}__$XU_FH" =~ $K ]]; then
                   p=${DEFRULE3[$K]}
-                  local sts=0
+                  sts=0
                   break
                 fi
               fi
               ((jy++))
             done
             if [ $sts -eq $STS_SUCCESS ]; then break; fi
           done
         fi
       fi
-      if [ -n "$p" ]; then
-        local sts=0
-      fi
+      [[ -n "$p" ]] && sts=0
     fi
     echo "$p"
     $SETX
     return $sts
 }
 export -f CFG_find
 
-# Deprecated: use CFG_find
-#a_find() {
-#    CFG_find "$@"
-#}
 
 ##############################################################################
 # get value from config file
 # if file does not exist, or parameter does not exist, return default value
 #
 # Require CFG_find
 #   DEFDICT  global dictionary based on unique key (associative array)
@@ -961,26 +912,28 @@
 # Parameter $2:
 #    Parameter key to search
 # Return:
 #    parameter value
 get_cfg_value() {
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     local p tid t
-    if [ -z "$2" ]; then
+    if [[ -z "$2" ]]; then
       p=
       echo $p
       return
     else
       p=
     fi
     [[ $3 =~ [0123] ]] && tid=$3 || tid="0 1 2 3"
     for t in $tid; do
       p=$(CFG_find "$t" "$2")
       [[ -n "$p" && $p != "False" ]] && break
     done
+    # Workaround
+    [[ $2 =~ (LOCAL_PKGS|PKGS_LIST) ]] && p="clodoo lisa odoo_score os0 oerplib3 python_plus travis_emulator wok_code z0bug_odoo z0lib zar zerobug"
     [[ $p == "None" ]] && p=""
     echo "$p"
     $SETX
 }
 export -f get_cfg_value
 
 
@@ -1018,51 +971,26 @@
       declare -gA DEFDICT$tid DEFRULE$tid
     fi
     $SETX
 }
 export -f CFG_init
 
 
-# Deprecated: use CFG_init
-#init_cfg() {
-## Parameter $1: Id of table (may be 0..3)
-#    if [ "$1" == "0" -o "$1" == "1" -o "$1" == "2" -o "$1" == "3" ]; then
-#      local tid=$1
-#    else
-#      local tid="0"
-#    fi
-#    echo $(a_new "$tid")
-#    eval $(a_active "$tid")
-#}
-#export -f init_cfg
-
-# Deprecated: use CFG_init
-#active_cfg() {
-## Parameter $1: Id of table (may be 0..3)
-#    if [ "$1" == "0" -o "$1" == "1" -o "$1" == "2" -o "$1" == "3" ]; then
-#      local tid=$1
-#    else
-#      local tid="0"
-#    fi
-#    echo $(a_active "$tid")
-#}
-#export -f active_cfg
-
 set_cfg_def() {
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     # set_cfg_set(key value [id])
     # Deprecated: use CFG_set
     CFG_set "$1" "$2" "$3" "$4" "$5" "$6"
     $SETX
 }
 export -f set_cfg_def
 
 
 _read_cfg_file() {
-#read_cfg_file(file $tid [section] [-D|-d])    -D or -d means debug
+# read_cfg_file(file $tid [section] [-D|-d])    -D or -d means debug
     [[ ! -n "$1"  || ! -f "$1" ]] && return
     local key val lne x r t s d b dev
     if [[ "$(type -t store_cfg_param_value)" == "function" ]]; then
       store_param=store_cfg_param_value
     else
       store_param=CFG_set
     fi
@@ -1142,43 +1070,47 @@
         fi
       fi
     done < "$1"
 }
 
 link_cfg_def() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
-  local file_bckdel file_backup file_meta file_vcs file_bins
-  local file_media file_bindata
+  local fn_bckdel fn_backup fn_meta fn_vcs fn_bins
+  local fn_media fn_bindata LOCAL_PKGS
   [[ -n "$HOSTNAME_DEV" ]] && set_cfg_def "DEV_HOST" "$HOSTNAME_DEV" || set_cfg_def "DEV_HOST" "(pc[0-9]+)?shsde([a-z][0-9]+)?"
   [[ -n "$HOSTNAME_PRD" ]] && set_cfg_def "PRD_HOST" "$HOSTNAME_PRD" || set_cfg_def "PRD_HOST" "(shsp([a-z][0-9]+)?"
   CFG_set "CHAT_HOME" "https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b"
   CFG_set "ODOO_SETUPS" "__manifest__.py __openerp__.py"
-  file_bckdel=".bak *~ .tmp .log .out .tracehis .tracehistory ,cover .coverage test*.pdf tmp.* npm-debug.log.* .oca .z0i .oia .gitrepname"
-  file_backup=".orig .swp .tar .gz .zip __old_*"
-  file_meta=".DS_Store ._* .Spotlight-V100 .Trashes Thumbs.db Desktop.ini .cover/ .coverage/ .conf build/ dist/ conf/ filestore/ html/ .idea/ latex/ __pycache__/ .local/ .npm/ .gem/ Trash/ VME/ PycharmProjects pycharm*"
-  file_vcs="_MTN .bzr/ .svn/ .hg/ .fslckout _FOSSIL_ .fos CVS _darcs .git/ .osc"
-  file_bins=".pyc .a .obj .o .so .la .lib .dll .exe"
-  file_media=".jpg .gif .png .bmp .wav .mp3 .ogg .flac .avi .mpg .xcf .xpm"
-  file_bindata=".xls .xlsx .pickle"
-  CFG_set "filedel" "$file_bckdel"
-  CFG_set "file_backup" "$file_backup"
-  CFG_set "file_meta" "$file_meta"
-  CFG_set "file_vcs" "$file_vcs"
-  CFG_set "file_bins" "$file_bins"
-  CFG_set "file_media" "$file_media"
-  CFG_set "file_bindata" "$file_bindata"
-  CFG_set "fileignore" "$file_backup $file_meta $file_vcs $file_bins $file_media $file_bindata"
+  fn_bckdel=".bak '*~' .tmp .log .out .tracehis .tracehistory ,cover .coverage 'test*.pdf' 'tmp.*' 'npm-debug.log.*' .oca .z0i .oia .gitrepname"
+  fn_backup=".orig .swp .tar .gz .zip '__old_*'"
+  fn_meta=".DS_Store '._*' .Spotlight-V100 .Trashes Thumbs.db Desktop.ini .cover/ .coverage/ .conf build/ dist/ conf/ filestore/ html/ .idea/ latex/ __pycache__/ .local/ .npm/ .gem/ Trash/ VME/ PycharmProjects pycharm*"
+  fn_vcs="_MTN .bzr/ .svn/ .hg/ .fslckout _FOSSIL_ .fos CVS _darcs .git/ .osc"
+  fn_bins=".pyc .a .obj .o .so .la .lib .dll .exe"
+  fn_media=".jpg .gif .png .bmp .wav .mp3 .ogg .flac .avi .mpg .xcf .xpm"
+  fn_bindata=".xls .xlsx .pickle"
+  CFG_set "filedel" "$fn_bckdel"
+  CFG_set "file_backup" "$fn_backup"
+  CFG_set "file_meta" "$fn_meta"
+  CFG_set "file_vcs" "$fn_vcs"
+  CFG_set "file_bins" "$fn_bins"
+  CFG_set "file_media" "$fn_media"
+  CFG_set "fie_bindata" "$fn_bindata"
+  CFG_set "fileignore" "$fn_backup $fn_meta $fn_vcs $fn_bins $fn_media $fn_bindata"
   CFG_set "filediffignore" ".po .pot LICENSE README README.md* README.rst* /docs/"
   CFG_set "PS_TXT_COLOR" "0;97;40"
   CFG_set "PS_RUN_COLOR" "1;37;44"
   CFG_set "PS_NOP_COLOR" "34;107"
   CFG_set "PS_HDR1_COLOR" "97;42"
   CFG_set "PS_HDR2_COLOR" "30;43"
   CFG_set "PS_HDR3_COLOR" "30;45"
-  CFG_set "PKGS_LIST" "clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
+  LOCAL_PKGS="clodoo lisa odoo_score os0 python_plus travis_emulator wok_code z0bug_odoo z0lib zar zerobug"
+  [[ -d $HOME_DEVEL/../tools ]] && LOCAL_PKGS=$(find $HOME_DEVEL/../tools -maxdepth 1 -type d|grep -Ev "(/|.git|.idea|docs|egg-info|license_text|templates|tools|tests|z0tester)$"|sort|cut -d/ -f7|tr "\n" " ")
+  [[ -d $HOME_DEVEL/pypi ]] && LOCAL_PKGS=$(find $HOME_DEVEL/pypi -maxdepth 1 -type d|grep -Ev "(/|.git|.idea|docs|egg-info|license_text|templates|tools|tests|z0tester)$"|sort|cut -d/ -f6|tr "\n" " ")
+  LOCAL_PKGS=$(echo $LOCAL_PKGS)
+  CFG_set "LOCAL_PKGS" "$LOCAL_PKGS"
   CFG_set "HTML_SVG_DIR" "/var/www/html/wp-zi/wp-content/uploads/ci-ct"
   CFG_set "DEV_SVG" "$HOME_DEVEL/svg"
   CFG_set "HTML_DOCS_DIR" "/var/www/html/mw/html"
   CFG_set "HTML_DOWNLOAD_DIR" "/var/www/html/mw/download"
   CFG_set "PYTHON_MATRIX" "(2.7|3.6|3.7|3.8|3.9)"
   CFG_set "distpath" "$(readlink -f $HOME_DEVEL/..)/tools/\${pkgname}"
   [[ -z $DIST_CONF ]] && DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
@@ -1459,15 +1391,18 @@
     done
     return 1
 }
 
 is_pypi() {
     local x
     [[ -z $1 ]] && return 1
-    [[ -f $1/__main__.py && -f $1/__init__.py && -d $1/scripts && -d $1/egg-info ]] && return 0
+    [[ ( -f $1/setup.py || -f $1/../setup.py ) && -f $1/__init__.py && ( -d $1/egg-info || -f $1/oerp.py ) ]] && return 0
+    x=$(get_cfg_value "" "LOCAL_PKGS")
+    x="(${x// /|})"
+    [[ $(basename $1) =~ $x && $(basename $(dirname $1)) == "local" ]] && return 0
     return 1
 }
 
 get_value_from_setup() {
   # get_value_from_setup(file value)
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
   local n r s x=$(basename $1)
```

### Comparing `z0lib-2.0.4/z0lib/z0librun.py` & `z0lib-2.0.5/z0lib/z0librun.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Area managed:
 - parseoptargs: line command parser; expands python argparse and adds same
                 functionalities to bash scripts
 - xuname:       platform recognition (only bash); return info about host
 - tracelog:     manage tracelog (only bash)
 - run_traced:   execute (or dry_run) shell command
 - findpkg:      find package in file system (only bash)
-- CFG:          manage a dictionay value from config file
+- CFG:          manage a dictionary value from config file
                 like python ConfigParser (only bash)
 
 @author: Antonio M. Vigliotti antoniomaria.vigliotti@gmail.com
 """
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 from future import standard_library
@@ -46,15 +46,15 @@
     "/etc/openerp-server.conf",
     "/etc/odoo/openerp-server.conf",
     "/etc/openerp/odoo-server.conf",
 ]
 # Read Odoo configuration file (False or /etc/openerp-server.conf)
 OE_CONF = False
 DEFDCT = {}
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 
 def nakedname(path):
     return os.path.splitext(os.path.basename(path))[0]
 
 
 def run_traced(cmd, verbose=None, dry_run=None, disable_alias=None, is_alias=None):
```

### Comparing `z0lib-2.0.4/z0lib.egg-info/SOURCES.txt` & `z0lib-2.0.5/z0lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

