# Comparing `tmp/jupyterhub-nativeauthenticator-1.0.5.tar.gz` & `tmp/jupyterhub-nativeauthenticator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-nativeauthenticator-1.0.5.tar", last modified: Tue Oct 19 17:25:36 2021, max compression
+gzip compressed data, was "jupyterhub-nativeauthenticator-1.1.0.tar", last modified: Fri Sep  9 11:31:46 2022, max compression
```

## Comparing `jupyterhub-nativeauthenticator-1.0.5.tar` & `jupyterhub-nativeauthenticator-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.378932 jupyterhub-nativeauthenticator-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.382932 jupyterhub-nativeauthenticator-1.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    46492 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/authorization_area.png
--rw-r--r--   0 runner    (1001) docker     (121)  2487640 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/block_user_failed_logins.png
--rw-r--r--   0 runner    (1001) docker     (121)    43125 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/change-password.png
--rw-r--r--   0 runner    (1001) docker     (121)    85574 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/login-two-factor-auth.png
--rw-r--r--   0 runner    (1001) docker     (121)  1355938 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/native_auth_flow.png
--rw-r--r--   0 runner    (1001) docker     (121)    91790 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/signup-two-factor-auth.png
--rw-r--r--   0 runner    (1001) docker     (121)    78767 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/_static/wrong_signup.png
--rw-r--r--   0 runner    (1001) docker     (121)     5272 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)    10562 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/docs/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.382932 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2021-10-19 17:25:36.000000 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-10-19 17:25:36.000000 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-19 17:25:36.000000 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-19 17:25:36.000000 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-10-19 17:25:36.000000 jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.382932 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    76508 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/common-credentials.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     8048 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/signing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12459 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13897 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/nativeauthenticator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/autorization-area.html
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/change-password.html
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/my_message.html
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/native-login.html
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11324 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/tests/test_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/tests/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-19 17:25:36.386932 jupyterhub-nativeauthenticator-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-10-19 17:25:25.000000 jupyterhub-nativeauthenticator-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.145786 jupyterhub-nativeauthenticator-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.145786 jupyterhub-nativeauthenticator-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.149786 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)    62232 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/authorization_area.png
+-rw-r--r--   0 runner    (1001) docker     (121)  2487640 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/block_user_failed_logins.png
+-rw-r--r--   0 runner    (1001) docker     (121)    59939 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/change_password_self.png
+-rw-r--r--   0 runner    (1001) docker     (121)    52206 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/change_password_user.png
+-rw-r--r--   0 runner    (1001) docker     (121)    85574 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/login-two-factor-auth.png
+-rw-r--r--   0 runner    (1001) docker     (121)  1355938 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/native_auth_flow.png
+-rw-r--r--   0 runner    (1001) docker     (121)    91790 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/signup-two-factor-auth.png
+-rw-r--r--   0 runner    (1001) docker     (121)    78767 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/wrong_signup.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)     9963 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/options.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/docs/source/troubleshooting.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-09-09 11:31:46.000000 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-09-09 11:31:46.000000 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 11:31:46.000000 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-09 11:31:46.000000 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-09 11:31:46.000000 jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76508 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/common-credentials.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/signing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20094 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14554 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/nativeauthenticator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4350 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/authorization-area.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/change-password-admin.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/change-password.html
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/my_message.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/native-login.html
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4731 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12442 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/tests/test_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 11:31:46.153786 jupyterhub-nativeauthenticator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-09-09 11:31:35.000000 jupyterhub-nativeauthenticator-1.1.0/setup.py
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/LICENSE` & `jupyterhub-nativeauthenticator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/PKG-INFO` & `jupyterhub-nativeauthenticator-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyterhub-nativeauthenticator
-Version: 1.0.5
+Version: 1.1.0
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/jupyterhub/nativeauthenticator
 Author: Leticia Portella
 Author-email: leportella@protonmail.com
 License: 3 Clause BSD
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Native Authenticator
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/jupyterhub-nativeauthenticator?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/jupyterhub-nativeauthenticator)
 [![Documentation build status](https://img.shields.io/readthedocs/native-authenticator?logo=read-the-docs&logoColor=white)](https://native-authenticator.readthedocs.org/en/latest/)
@@ -22,33 +21,34 @@
 [![Gitter](https://img.shields.io/badge/social_chat-gitter-blue?logo=gitter)](https://gitter.im/jupyterhub/jupyterhub)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://github.com/jupyterhub/nativeauthenticator/blob/master/CONTRIBUTING.md)
 
 This is a relatively simple authenticator for small or medium-sized [JupyterHub](http://github.com/jupyter/jupyterhub/) applications. Signup and authentication are implemented as native to JupyterHub without relying on external services.
 
 NativeAuthenticator provides the following features:
 
-* New users can signup on the system;
-* New users can be blocked from accessing the system awaiting admin authorization;
-* Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
-* Option to block users after a set number of failed login attempts;
-* Option of open signup without need for initial authorization;
-* Option of asking more information about users on signup (e-mail).
-* Option of requiring users to agree with given Terms of Service;
-* Option of protection against scripting attacks via reCAPTCHA;
-* Option for users with an org-internal e-mail address to self-approve via secure link;
+- New users can signup on the system;
+- New users can be blocked from accessing the system awaiting admin authorization;
+- Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
+- Option to block users after a set number of failed login attempts;
+- Option of open signup without need for initial authorization;
+- Option of asking more information about users on signup (e-mail).
+- Option of requiring users to agree with given Terms of Service;
+- Option of protection against scripting attacks via reCAPTCHA;
+- Option for users with an org-internal e-mail address to self-approve via secure link;
 
 ## Documentation
 
 The latest documentation is always on readTheDocs, available [here](https://native-authenticator.readthedocs.io).
 
 ## Running tests
 
 To run the tests locally, you can install the development dependencies like so:
 
-`$ pip install -r dev-requirements.txt`
+```shell
+pip install -r dev-requirements.txt
+```
 
 Then run tests with pytest:
 
-`$ pytest`
-
-
-
+```
+pytest
+```
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/README.md` & `jupyterhub-nativeauthenticator-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 [![Gitter](https://img.shields.io/badge/social_chat-gitter-blue?logo=gitter)](https://gitter.im/jupyterhub/jupyterhub)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://github.com/jupyterhub/nativeauthenticator/blob/master/CONTRIBUTING.md)
 
 This is a relatively simple authenticator for small or medium-sized [JupyterHub](http://github.com/jupyter/jupyterhub/) applications. Signup and authentication are implemented as native to JupyterHub without relying on external services.
 
 NativeAuthenticator provides the following features:
 
-* New users can signup on the system;
-* New users can be blocked from accessing the system awaiting admin authorization;
-* Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
-* Option to block users after a set number of failed login attempts;
-* Option of open signup without need for initial authorization;
-* Option of asking more information about users on signup (e-mail).
-* Option of requiring users to agree with given Terms of Service;
-* Option of protection against scripting attacks via reCAPTCHA;
-* Option for users with an org-internal e-mail address to self-approve via secure link;
+- New users can signup on the system;
+- New users can be blocked from accessing the system awaiting admin authorization;
+- Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
+- Option to block users after a set number of failed login attempts;
+- Option of open signup without need for initial authorization;
+- Option of asking more information about users on signup (e-mail).
+- Option of requiring users to agree with given Terms of Service;
+- Option of protection against scripting attacks via reCAPTCHA;
+- Option for users with an org-internal e-mail address to self-approve via secure link;
 
 ## Documentation
 
 The latest documentation is always on readTheDocs, available [here](https://native-authenticator.readthedocs.io).
 
 ## Running tests
 
 To run the tests locally, you can install the development dependencies like so:
 
-`$ pip install -r dev-requirements.txt`
+```shell
+pip install -r dev-requirements.txt
+```
 
 Then run tests with pytest:
 
-`$ pytest`
-
+```
+pytest
+```
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/_static/block_user_failed_logins.png` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/_static/login-two-factor-auth.png` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/_static/native_auth_flow.png` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/_static/signup-two-factor-auth.png` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/_static/wrong_signup.png` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/index.rst` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/index.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-.. Native Authenticator documentation master file, created by
-   sphinx-quickstart on Wed Dec  5 10:28:37 2018.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
+# Welcome to Native Authenticator's documentation!
 
-Welcome to Native Authenticator's documentation!
-================================================
-
-This is a relatively simple authenticator for small or medium-sized `JupyterHub <https://github.com/jupyterhub/>`_ applications. Signup and authentication are implemented as native to JupyterHub without relying on external services.
+This is a relatively simple authenticator for small or medium-sized [JupyterHub](https://github.com/jupyterhub/) applications. Signup and authentication are implemented as native to JupyterHub without relying on external services.
 
 NativeAuthenticator provides the following features:
 
-* New users can signup on the system;
-* New users can be blocked from accessing the system awaiting admin authorization;
-* Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
-* Option to block users after a set number of failed login attempts;
-* Option of open signup without need for initial authorization;
-* Option of asking more information about users on signup (e-mail).
-* Option of requiring users to agree with given Terms of Service;
-* Option of protection against scripting attacks via reCAPTCHA;
-* Option for users with an org-internal e-mail address to self-approve via secure link;
-
-
-Indices and tables
-==================
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   quickstart
-   options
-   troubleshooting
+- New users can signup on the system;
+- New users can be blocked from accessing the system awaiting admin authorization;
+- Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
+- Option to block users after a set number of failed login attempts;
+- Option of open signup without need for initial authorization;
+- Option of asking more information about users on signup (e-mail).
+- Option of requiring users to agree with given Terms of Service;
+- Option of protection against scripting attacks via reCAPTCHA;
+- Option for users with an org-internal e-mail address to self-approve via secure link;
+
+# Indices and tables
+
+```{toctree}
+:caption: 'Contents:'
+:maxdepth: 2
+
+quickstart
+options
+troubleshooting
+```
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/options.rst` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/options.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,227 +1,202 @@
-Optional Configuration
-======================
+# Optional Configuration
 
+## Password Strength
 
-Password Strength
------------------
-
-By default, when a user signs up through Native Authenticator there is no password strength verification, so any type of password is valid. There are two methods that you can add to increase password strength: a verification for commmon passowords and a minimum length of password. 
+By default, when a user signs up through Native Authenticator there is no password strength verification, so any type of password is valid. There are two methods that you can add to increase password strength: a verification for commmon passowords and a minimum length of password.
 
 To verify if the password is not common (such as 'qwerty' or '1234'), you can add the following line to your config file:
 
-.. code-block:: python
-
-    c.Authenticator.check_common_password = True
-
-The Authenticator will verify if the password is a common password and the user won't be able to sign up if it is. The list of the common passwords that are in our verification is available `on this link <https://github.com/danielmiessler/SecLists/blob/master/Passwords/Common-Credentials/10-million-password-list-top-10000.txt>`_.
+```python
+c.NativeAuthenticator.check_common_password = True
+```
 
+The Authenticator will verify if the password is a common password and the user won't be able to sign up if it is. The list of the common passwords that are in our verification is available [on this link](https://github.com/danielmiessler/SecLists/blob/master/Passwords/Common-Credentials/10-million-password-list-top-10000.txt).
 
 You can also add a minimum password length that the user must have. To do this add the following line on the config file with an integer as a value:
 
-.. code-block:: python
-
-    c.Authenticator.minimum_password_length = 10
+```python
+c.NativeAuthenticator.minimum_password_length = 10
+```
 
 If any of this configuration is available, the user will receive this message on SignUp:
 
-.. image:: _static/wrong_signup.png
+![](_static/wrong_signup.png)
 
-
-Block users after failed logins
--------------------------------
+## Block users after failed logins
 
 One thing that can make systems more safe is to block users after a number of failed logins. With Native Authenticator you can add this feature by adding `allowed_failed_logins` on the config file. The default is 0, which means that the system will not block users ever.
 
-.. code-block:: python
-
-    c.Authenticator.allowed_failed_logins = 3
+```python
+c.NativeAuthenticator.allowed_failed_logins = 3
+```
 
 You can also define the number of seconds a user must wait before trying again. The default value is 600 seconds.
 
-.. code-block:: python
-
-    c.Authenticator.seconds_before_next_try = 1200
-
+```python
+c.NativeAuthenticator.seconds_before_next_try = 1200
+```
 
-.. image:: _static/block_user_failed_logins.png
+![](_static/block_user_failed_logins.png)
 
-Disable SignUp
---------------
+## Disable SignUp
 
 By default Native Authenticator allows everyone to register user accounts. But you can add a option to disable signup. To do so, just add the following line to the config file:
 
-.. code-block:: python
+```python
+c.NativeAuthenticator.enable_signup = False
+```
 
-    c.Authenticator.enable_signup = False
+## Open SignUp
 
-
-Open SignUp
------------
-
-By default all users that make sign up on Native Authenticator need an admin approval so 
-they can actually log in the system. You can change this behavior by adding an option of 
+By default all users that make sign up on Native Authenticator need an admin approval so
+they can actually log in the system. You can change this behavior by adding an option of
 open signup, where all users that do sign up can already log in the system. To do so, just add this line to the config file:
 
-.. code-block:: python
-
-    c.Authenticator.open_signup = True
-
+```python
+c.NativeAuthenticator.open_signup = True
+```
 
-Ask for extra information on SignUp
------------------------------------
+## Ask for extra information on SignUp
 
 Native Authenticator is based on username and password only. But if you need extra information about the users, you can add them on the sign up.
 For now, the only extra information you can ask is email. To do so, you can add the following line to the config file:
 
-.. code-block:: python
+```python
+c.NativeAuthenticator.ask_email_on_signup = True
+```
 
-    c.Authenticator.ask_email_on_signup = True
-
-
-Use reCaptcha to prevent scripted SignUp attacks
-------------------------------------------------
+## Use reCaptcha to prevent scripted SignUp attacks
 
 Since by default, anybody can sign up to the system, you may want to use the lightweight
 single-click "I am not a robot" checkbox provided by Google's reCAPTCHA v2 to reduce your
 risk from scripting attacks.
-To use this feature, you will need to `register with reCaptcha <https://www.google.com/recaptcha/admin/create>`_ (you will need a Google account to do so).
+To use this feature, you will need to [register with reCaptcha](https://www.google.com/recaptcha/admin/create) (you will need a Google account to do so).
 
-You can learn more about reCAPTCHA `here <https://developers.google.com/recaptcha/intro>`_.
+You can learn more about reCAPTCHA [here](https://developers.google.com/recaptcha/intro).
 If you would like to simply test this functionality without creating an account, you can do
-so as explained `here <https://developers.google.com/recaptcha/docs/faq#id-like-to-run-automated-tests-with-recaptcha.-what-should-i-do>`_.
+so as explained [here](https://developers.google.com/recaptcha/docs/faq#id-like-to-run-automated-tests-with-recaptcha.-what-should-i-do).
 Note that this test in itself does not provide actual security so please do **NOT** use
 these test credentials for your actual production system.
 
 To enable reCAPTCHA on signup, add the following two lines to the configuration file and
 substitute your own credentials.
 
-.. code-block:: python
-
-    c.Authenticator.recaptcha_key = "your key"
-    c.Authenticator.recaptcha_secret = "your secret"
-
+```python
+c.NativeAuthenticator.recaptcha_key = "your key"
+c.NativeAuthenticator.recaptcha_secret = "your secret"
+```
 
-Allow self-serve approval
--------------------------
+## Allow self-serve approval
 
 By default, all users who sign up on NativeAuthenticator need a manual admin approval so they can actually log in the system. Or you can allow anybody without approval as described above with `open_signup`.
-Alternatively, depending on your situation, you may want something *like* `open_signup` but only for users in your own organization. This is what this option permits.
+Alternatively, depending on your situation, you may want something _like_ `open_signup` but only for users in your own organization. This is what this option permits.
 
-New users are still created as non-authorized, but they can self-authorize by navigating to a (cryptographically verified) URL which will be e-mailed to them *only* if the provided email address matches the specified regular expression.
+New users are still created as non-authorized, but they can self-authorize by navigating to a (cryptographically verified) URL which will be e-mailed to them _only_ if the provided email address matches the specified regular expression.
 
 For example, to allow any users who have an `example.com` email address to self-approve, you add the following to your configuration file:
 
-.. code-block:: python
-
-    import re
-    c.Authenticator.allow_self_approval_for = re.compile('[^@]+@example\.com$')
+```python
+c.NativeAuthenticator.allow_self_approval_for = '[^@]+@example\.com$'
+```
 
 Please note that activating this setting automatically also enables `ask_email_on_signup`.
 
 To use the code, you must also provide a secret key (i.e. an arbitrary string, not too short) to cryptographically sign the URL. To prevents attacks, it is crucial that this key stays secret.
 
-.. code-block:: python
-
-    c.Authenticator.secret_key = "your-arbitrary-key"
+```python
+c.NativeAuthenticator.secret_key = "your-arbitrary-key"
+```
 
 You should also customize the email sent to users with something as follows:
 
-.. code-block:: python
-
-    c.Authenticator.self_approval_email = ("from", "subject", "email body, including https://example.com{approval_url}")
+```python
+c.NativeAuthenticator.self_approval_email = ("from", "subject", "email body, including https://example.com{approval_url}")
+```
 
 Note that you need to specify the domain where JupyterHub is running (`example.com` in the code block above) as well as the port, if you are using a non-standard one (e.g. `8000`).
 Also the protocol must be the correct one you are serving your connections from (`https` in the example).
 
 Furthermore, you may specify the SMTP server to use for sending the email. You can do that with
 
-.. code-block:: python
-
-    c.Authenticator.self_approval_server = {'url': 'smtp.gmail.com', 'usr': 'myself', 'pwd': 'mypassword'}
+```python
+c.NativeAuthenticator.self_approval_server = {'url': 'smtp.gmail.com', 'usr': 'myself', 'pwd': 'mypassword'}
+```
 
 If you do not specify a `self_approval_server`, it will attempt to use `localhost` without authentication.
 
-Using GMail (as in the example above) is entirely optional, any other SMTP server accepting password authentication also works. However, if you *do* wish to use GMail as your SMTP server, you must also allow "less secure apps" for this to work, as described at `this link <https://support.google.com/accounts/answer/6010255>`_. 
-If you have 2FA enabled (with GMail, not NativeAuthenticator) you should disable it for JupyterHub to be able to send emails, as described `over here <https://support.google.com/accounts/answer/185833>`_.
-Also see `this helpful StackExchange post <https://stackoverflow.com/questions/16512592/login-credentials-not-working-with-gmail-smtp>`_ for additional GMail-specific SMTP details.
+Using GMail (as in the example above) is entirely optional, any other SMTP server accepting password authentication also works. However, if you _do_ wish to use GMail as your SMTP server, you must also allow "less secure apps" for this to work, as described at [this link](https://support.google.com/accounts/answer/6010255).
+If you have 2FA enabled (with GMail, not NativeAuthenticator) you should disable it for JupyterHub to be able to send emails, as described [over here](https://support.google.com/accounts/answer/185833).
+Also see [this helpful StackExchange post](https://stackoverflow.com/questions/16512592/login-credentials-not-working-with-gmail-smtp) for additional GMail-specific SMTP details.
 
 Finally, the entire procedure so far will only correctly create and enable JupyterHub users.
 However, the people wishing to login as this users, will **also** need to have accounts on the system that is running Jupyterhub. If the system is one of the more common Linux distributions, adding the following to the configuration file will automatically create their Linux account the first time they log in JupyterHub.
 If the system where JupyterHub is running is another OS, such as BSD or Windows, the corresponding user creation command must be invoked instead of useradd with the appropriate arguments.
 
-.. code-block:: python
+```python
+def pre_spawn_hook(spawner):
+    username = spawner.user.name
+    try:
+        import pwd
+        pwd.getpwnam(username)
+    except KeyError:
+        import subprocess
+        subprocess.check_call(['useradd', '-ms', '/bin/bash', username])
 
-    def pre_spawn_hook(spawner):
-        username = spawner.user.name
-        try:
-            import pwd
-            pwd.getpwnam(username)
-        except KeyError:
-            import subprocess
-            subprocess.check_call(['useradd', '-ms', '/bin/bash', username])
-    
-    c.Spawner.pre_spawn_hook = pre_spawn_hook
+c.Spawner.pre_spawn_hook = pre_spawn_hook
+```
 
-
-Mandatory acceptance of Terms of Service before SignUp
-------------------------------------------------------
+## Mandatory acceptance of Terms of Service before SignUp
 
 You may require that users to click a checkbox agreeing to your TOS before they can sign up. This might be legally binding in some jurisditions.
 To do so, you only need to add the following line to your config file and provide a link the where users can find your TOS.
 
-.. code-block:: python
-
-    c.Authenticator.tos = 'I agree to the <a href="your-url" target="_blank">TOS</a>'
+```python
+c.NativeAuthenticator.tos = 'I agree to the <a href="your-url" target="_blank">TOS</a>'
+```
 
+## Import users from FirstUse Authenticator
 
-Import users from FirstUse Authenticator
-----------------------------------------
-
-If you are using `FirstUse Authenticator <https://github.com/jupyterhub/firstuseauthenticator>`_ and wish to change to Native Authenticator, you can import users from that authenticator to Native authenticator with minimum work!
+If you are using [FirstUse Authenticator](https://github.com/jupyterhub/firstuseauthenticator) and wish to change to Native Authenticator, you can import users from that authenticator to Native authenticator with minimum work!
 
 To do so, you have to add the following line on the configuration file:
 
-.. code-block:: python
-
-    c.Authenticator.import_from_firstuse = True
+```python
+c.NativeAuthenticator.import_from_firstuse = True
+```
 
 **Remark: unless you have configured the open signup configuration, the users will be created but they will not be able to login, because they don't have authorization by default.**
 
-
 By default, Native Authenticator assumes that the path for the database is the same directory. If that's not the case, you can change the path the file through this variables:
 
-.. code-block:: python
-
-    c.Authenticator.firstuse_dbm_path = '/home/user/passwords.dbm'
-
-Native Authenticator ensures that usernames are sanitized, so they won't have commas 
-or white spaces. Additionaly, you can add password verification such as 
-avoiding common passwords. If usernames or passwords imported from the 
-FirstUse Authenticator don't comply with these verifications, the importating will raise an 
+```python
+c.NativeAuthenticator.firstuse_dbm_path = '/home/user/passwords.dbm'
+```
+
+Native Authenticator ensures that usernames are sanitized, so they won't have commas
+or white spaces. Additionaly, you can add password verification such as
+avoiding common passwords. If usernames or passwords imported from the
+FirstUse Authenticator don't comply with these verifications, the importating will raise an
 error.
 
 You can also remove FirstUse's database file after the importation to Native Authenticator, to avoid leaving unused files on the system. To do so, you must add the following line to the configuration file:
 
+```python
+c.NativeAuthenticator.delete_firstuse_db_after_import = True
+```
 
-.. code-block:: python
-
-    c.Authenticator.delete_firstuse_db_after_import = True
-
-
-Add two factor authentication obligatory for users
---------------------------------------------------
+## Add two factor authentication obligatory for users
 
 You can increase security making two factor authentication obligatory for all users.
 To do so, add the following line on the config file:
 
-.. code-block:: python
-
-    c.Authenticator.allow_2fa = True
+```python
+c.NativeAuthenticator.allow_2fa = True
+```
 
-Users will receive a message after signup with the two factor authentication code:  
+Users will receive a message after signup with the two factor authentication code:
 
-.. image:: _static/signup-two-factor-auth.png
+![](_static/signup-two-factor-auth.png)
 
 And login will now require the two factor authentication code as well:
 
-.. image:: _static/login-two-factor-auth.png
+![](_static/login-two-factor-auth.png)
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/docs/quickstart.rst` & `jupyterhub-nativeauthenticator-1.1.0/docs/source/quickstart.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-Quickstart
-==========
+# Quickstart
 
-Installation
-------------
+## Installation
 
-NativeAuthenticator is a authenticator plugin for `JupyterHub <https://github.com/jupyterhub/>`_. 
+NativeAuthenticator is a authenticator plugin for [JupyterHub](https://github.com/jupyterhub/).
 
-It is available on `Pypi <https://pypi.org/project/jupyterhub-nativeauthenticator/>`_. The easiest way to install it is via pip:
+It is available on [PyPI](https://pypi.org/project/jupyterhub-nativeauthenticator/). The easiest way to install it is via pip:
 
-.. code-block:: bash
+```shell
+pip install jupyterhub-nativeauthenticator
+```
 
-   $ pip install jupyterhub-nativeauthenticator
-
-
-Alternatively, you can install this authenticator through the project's gitHub repository:
-
-.. code-block:: bash
-
-   $ git clone https://github.com/jupyterhub/nativeauthenticator.git
-   $ cd nativeauthenticator
-   $ pip install -e .
+Alternatively, you can install this authenticator through the project's GitHub repository:
 
+```shell
+git clone https://github.com/jupyterhub/nativeauthenticator.git
+cd nativeauthenticator
+pip install -e .
+```
 
 After running the installation method of your choice, you must create the configuration file for JupyterHub:
 
-.. code-block:: bash
-
-    $ jupyterhub --generate-config -f /etc/jupyterhub/jupyterhub_config.py
-
+```shell
+jupyterhub --generate-config -f /etc/jupyterhub/jupyterhub_config.py
+```
 
 Also, change the default authenticator class to NativeAuthenticator:
 
-.. code-block:: python
-
-    c.JupyterHub.authenticator_class = 'nativeauthenticator.NativeAuthenticator'
-
+```python
+c.JupyterHub.authenticator_class = 'nativeauthenticator.NativeAuthenticator'
+```
 
 Lastly, you need to add the following to the configuration file as well:
 
-.. code-block:: python
-
-    import os, nativeauthenticator
-    c.JupyterHub.template_paths = ["{}/templates/".format(os.path.dirname(nativeauthenticator.__file__))]
-
+```python
+import os, nativeauthenticator
+c.JupyterHub.template_paths = [f"{os.path.dirname(nativeauthenticator.__file__)}/templates/"]
+```
 
 Now you can run JupyterHub using the updated configuration file and start using JupyterHub with NativeAuthenticator:
 
+```shell
+jupyterhub -f /etc/jupyterhub/jupyterhub_config.py
+```
 
-.. code-block:: bash
-
-    $ jupyterhub -f /etc/jupyterhub/jupyterhub_config.py
-
-
-Default workflow
-----------------
+## Default workflow
 
-A new user that wants access to a system running NativeAuthenticator must first visit the signup page and create a new account with a username and password. By default, this user will not have access to the system, they will need the authorization of an admin to actually be able to login the system. Thus, after executing the signup, the user will receive a message letting them know that their information was sent to an admin. 
-
-
-.. image:: _static/native_auth_flow.png
+A new user that wants access to a system running NativeAuthenticator must first visit the signup page and create a new account with a username and password. By default, this user will not have access to the system, they will need the authorization of an admin to actually be able to login the system. Thus, after executing the signup, the user will receive a message letting them know that their information was sent to an admin.
 
+![](_static/native_auth_flow.png)
 
 The admin must access the authorization panel and authorize the user so they be able to login:
 
-.. image:: _static/authorization_area.png
+![](_static/authorization_area.png)
 
+## Adding new users
 
-Adding new users
-----------------
+To create a new user one must go to `/hub/signup` and sign up with a username and a password. The information asked for on signup can change depending on admin configuration, but all fields are obligatory. By default, when a new user is created on the system they will need an administrator authorization to access the system.
 
-To create a new user one must go to `/hub/signup` and sign up with a username and a password. The information asked for on signup can change depending on admin configuration, but all fields are obligatory. By default, when a new user is created on the system they will need an administrator authorization to access the system. 
+It is important to note that **admin accounts must also be created through signup**. However, usernames listed in the config file as admins (see below) will automatically have authorization to enter the system.
 
-It is important to note that **admin accounts must also be created through signup**. However, usernames listed in the config file as admins (see below) will automatically have authorization to enter the system. 
+```python
+c.Authenticator.admin_users = {'username'}
+```
 
-.. code-block:: python
+## Username restrictions
 
-    c.Authenticator.admin_users = {'username'}
+Usernames cannot be empty or contain commas, spaces or slashes. If any of these apply, the user will receive an error and will not be able to sign up.
 
+## Authorize, un-authorize or discard users
 
-Username restrictions
----------------------
+To authorize new users to enter the system or to manage those that already have access to the system you can go to `/hub/authorize` while logged in as an admin user. Alternatively, you can click the "Authorize Users" element on your home page. Authorized users will have a green background with a button to un-authorize them while un-authorized users will have a white background and an authorization button.
 
-Usernames cannot be empty or contain commas, spaces or slashes. If any of these apply, the user will receive an error and will not be able to sign up. 
+![](_static/authorization_area.png)
 
+From here, you can also discard users that attempted to sign up but whom you do not want to authorize. Users that are discarded will not be notified.
 
-Authorize or un-authorize users
--------------------------------
+To delete existing (authorized) users, first un-authorize and then discard them. Note that while discarding users will delete them from the database for both JupyterHub and NativeAuthenticator, **it will not delete data for accounts on the machine that is running JupyterHub!**  
+Make sure to delete these separately, otherwise someone else could sign up with the same username later and inadvertently gain access to data that is not theirs.
 
-To authorize new users to enter the system or to manage those that already have access to the system you can go to `/hub/authorize` while logged in as an admin user. Alternatively, you can click the "Authorize Users" element on your home page. Authorized users will have a green background with a button to unauthorize them while unauthorized users will have a white background and an authorization button. From here, you can also discard users that attempted to sign up but whom you do not want to authorize (they will not be notified). 
+## Changing your own password
 
-.. image:: _static/authorization_area.png
+Users that are logged in the system can easily change their password by going to: `/hub/change-password` or clicking the "Change Password" element on their home page.
 
+![](_static/change_password_self.png)
 
-Change password
----------------
+## Changing a user's password as admin
 
-Users that are logged in the system can easily change their password by going to: `/hub/change-password` or clicking the "Change Password" element on their home page.
+In case any user forgets or misplaces their account password, admins can reset it to a password of their choosing. Simply navigate to `/hub/change-password/SomeUserName` or click the "Change Password" element of that user in the authorization area.
 
-.. image:: _static/change-password.png
+![](_static/change_password_user.png)
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/PKG-INFO` & `jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyterhub-nativeauthenticator
-Version: 1.0.5
+Version: 1.1.0
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/jupyterhub/nativeauthenticator
 Author: Leticia Portella
 Author-email: leportella@protonmail.com
 License: 3 Clause BSD
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Native Authenticator
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/jupyterhub-nativeauthenticator?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/jupyterhub-nativeauthenticator)
 [![Documentation build status](https://img.shields.io/readthedocs/native-authenticator?logo=read-the-docs&logoColor=white)](https://native-authenticator.readthedocs.org/en/latest/)
@@ -22,33 +21,34 @@
 [![Gitter](https://img.shields.io/badge/social_chat-gitter-blue?logo=gitter)](https://gitter.im/jupyterhub/jupyterhub)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://github.com/jupyterhub/nativeauthenticator/blob/master/CONTRIBUTING.md)
 
 This is a relatively simple authenticator for small or medium-sized [JupyterHub](http://github.com/jupyter/jupyterhub/) applications. Signup and authentication are implemented as native to JupyterHub without relying on external services.
 
 NativeAuthenticator provides the following features:
 
-* New users can signup on the system;
-* New users can be blocked from accessing the system awaiting admin authorization;
-* Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
-* Option to block users after a set number of failed login attempts;
-* Option of open signup without need for initial authorization;
-* Option of asking more information about users on signup (e-mail).
-* Option of requiring users to agree with given Terms of Service;
-* Option of protection against scripting attacks via reCAPTCHA;
-* Option for users with an org-internal e-mail address to self-approve via secure link;
+- New users can signup on the system;
+- New users can be blocked from accessing the system awaiting admin authorization;
+- Option of enforcing password security by disallowing common passwords or requiring a minimum password length;
+- Option to block users after a set number of failed login attempts;
+- Option of open signup without need for initial authorization;
+- Option of asking more information about users on signup (e-mail).
+- Option of requiring users to agree with given Terms of Service;
+- Option of protection against scripting attacks via reCAPTCHA;
+- Option for users with an org-internal e-mail address to self-approve via secure link;
 
 ## Documentation
 
 The latest documentation is always on readTheDocs, available [here](https://native-authenticator.readthedocs.io).
 
 ## Running tests
 
 To run the tests locally, you can install the development dependencies like so:
 
-`$ pip install -r dev-requirements.txt`
+```shell
+pip install -r dev-requirements.txt
+```
 
 Then run tests with pytest:
 
-`$ pytest`
-
-
-
+```
+pytest
+```
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/jupyterhub_nativeauthenticator.egg-info/SOURCES.txt` & `jupyterhub-nativeauthenticator-1.1.0/jupyterhub_nativeauthenticator.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 LICENSE
 MANIFEST.in
 README.md
 dev-requirements.txt
 setup.py
 docs/Makefile
-docs/conf.py
-docs/index.rst
 docs/make.bat
-docs/options.rst
-docs/quickstart.rst
-docs/troubleshooting.rst
-docs/_static/authorization_area.png
-docs/_static/block_user_failed_logins.png
-docs/_static/change-password.png
-docs/_static/login-two-factor-auth.png
-docs/_static/native_auth_flow.png
-docs/_static/signup-two-factor-auth.png
-docs/_static/wrong_signup.png
+docs/requirements.txt
+docs/source/conf.py
+docs/source/index.md
+docs/source/options.md
+docs/source/quickstart.md
+docs/source/troubleshooting.md
+docs/source/_static/authorization_area.png
+docs/source/_static/block_user_failed_logins.png
+docs/source/_static/change_password_self.png
+docs/source/_static/change_password_user.png
+docs/source/_static/login-two-factor-auth.png
+docs/source/_static/native_auth_flow.png
+docs/source/_static/signup-two-factor-auth.png
+docs/source/_static/wrong_signup.png
 jupyterhub_nativeauthenticator.egg-info/PKG-INFO
 jupyterhub_nativeauthenticator.egg-info/SOURCES.txt
 jupyterhub_nativeauthenticator.egg-info/dependency_links.txt
 jupyterhub_nativeauthenticator.egg-info/requires.txt
 jupyterhub_nativeauthenticator.egg-info/top_level.txt
 nativeauthenticator/__init__.py
 nativeauthenticator/common-credentials.txt
 nativeauthenticator/handlers.py
 nativeauthenticator/nativeauthenticator.py
 nativeauthenticator/orm.py
 nativeauthenticator/crypto/__init__.py
 nativeauthenticator/crypto/crypto.py
 nativeauthenticator/crypto/encoding.py
 nativeauthenticator/crypto/signing.py
-nativeauthenticator/templates/autorization-area.html
+nativeauthenticator/templates/authorization-area.html
+nativeauthenticator/templates/change-password-admin.html
 nativeauthenticator/templates/change-password.html
 nativeauthenticator/templates/my_message.html
 nativeauthenticator/templates/native-login.html
 nativeauthenticator/templates/page.html
 nativeauthenticator/templates/signup.html
 nativeauthenticator/tests/__init__.py
 nativeauthenticator/tests/test_authenticator.py
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/common-credentials.txt` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/crypto.py` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,73 +6,68 @@
 import secrets
 
 from .encoding import force_bytes
 
 
 class InvalidAlgorithm(ValueError):
     """Algorithm is not supported by hashlib."""
+
     pass
 
 
-def salted_hmac(key_salt, value, secret, *, algorithm='sha1'):
+def salted_hmac(key_salt, value, secret, *, algorithm="sha1"):
     """
     Return the HMAC of 'value', using a key generated from key_salt and a
     secret. Default algorithm is SHA1,
     but any algorithm name supported by hashlib can be passed.
 
     A different key_salt should be passed in for every application of HMAC.
     """
 
     key_salt = force_bytes(key_salt)
     secret = force_bytes(secret)
     try:
         hasher = getattr(hashlib, algorithm)
     except AttributeError as e:
         raise InvalidAlgorithm(
-            '%r is not an algorithm accepted by the hashlib module.'
-            % algorithm
+            "%r is not an algorithm accepted by the hashlib module." % algorithm
         ) from e
     # We need to generate a derived key from our base key.  We can do this by
     # passing the key_salt and our base key through a pseudo-random function.
     key = hasher(key_salt + secret).digest()
     # If len(key_salt + secret) > block size of the hash algorithm, the above
     # line is redundant and could be replaced by key = key_salt + secret, since
     # the hmac module does the same thing for keys longer than the block size.
     # However, we need to ensure that we *always* do this.
     return hmac.new(key, msg=force_bytes(value), digestmod=hasher)
 
 
-RANDOM_STRING_CHARS = \
-        'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'
+RANDOM_STRING_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
 
 
 def get_random_string(length, allowed_chars=RANDOM_STRING_CHARS):
     """
     Return a securely generated random string.
 
     The bit length of the returned value can be calculated with the formula:
         log_2(len(allowed_chars)^length)
 
     For example, with default `allowed_chars` (26+26+10), this gives:
       * length: 12, bit length =~ 71 bits
       * length: 22, bit length =~ 131 bits
     """
-    return ''.join(secrets.choice(allowed_chars) for i in range(length))
+    return "".join(secrets.choice(allowed_chars) for i in range(length))
 
 
 def constant_time_compare(val1, val2):
     """Return True if the two strings are equal, False otherwise."""
     return secrets.compare_digest(force_bytes(val1), force_bytes(val2))
 
 
 def pbkdf2(password, salt, iterations, dklen=0, digest=None):
     """Return the hash of password using pbkdf2."""
     if digest is None:
         digest = hashlib.sha256
     dklen = dklen or None
     password = force_bytes(password)
     salt = force_bytes(salt)
-    return hashlib.pbkdf2_hmac(digest().name,
-                               password,
-                               salt,
-                               iterations,
-                               dklen)
+    return hashlib.pbkdf2_hmac(digest().name, password, salt, iterations, dklen)
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/encoding.py` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 
 class DjangoUnicodeDecodeError(UnicodeDecodeError):
     def __init__(self, obj, *args):
         self.obj = obj
         super().__init__(*args)
 
     def __str__(self):
-        return '%s. You passed in %r (%s)' % (
-                super().__str__(),
-                self.obj,
-                type(self.obj))
+        return f"{super().__str__()}. You passed in {self.obj!r} ({type(self.obj)})"
 
 
 _PROTECTED_TYPES = (
     type(None),
-    int, float, Decimal,
+    int,
+    float,
+    Decimal,
     datetime.datetime,
     datetime.date,
     datetime.time,
 )
 
 
 def is_protected_type(obj):
@@ -31,15 +30,15 @@
 
     Objects of protected types are preserved as-is when passed to
     force_str(strings_only=True).
     """
     return isinstance(obj, _PROTECTED_TYPES)
 
 
-def force_str(s, encoding='utf-8', strings_only=False, errors='strict'):
+def force_str(s, encoding="utf-8", strings_only=False, errors="strict"):
     """
     Similar to smart_str(), except that lazy instances are resolved to
     strings, rather than kept as lazy objects.
 
     If strings_only is True, don't convert (some) non-string-like objects.
     """
     # Handle the common case first for performance reasons.
@@ -53,50 +52,49 @@
         else:
             s = str(s)
     except UnicodeDecodeError as e:
         raise DjangoUnicodeDecodeError(s, *e.args)
     return s
 
 
-def force_bytes(s, encoding='utf-8', strings_only=False, errors='strict'):
+def force_bytes(s, encoding="utf-8", strings_only=False, errors="strict"):
     """
     Similar to smart_bytes, except that lazy instances are resolved to
     strings, rather than kept as lazy objects.
 
     If strings_only is True, don't convert (some) non-string-like objects.
     """
     # Handle the common case first for performance reasons.
     if isinstance(s, bytes):
-        if encoding == 'utf-8':
+        if encoding == "utf-8":
             return s
         else:
-            return s.decode('utf-8', errors).encode(encoding, errors)
+            return s.decode("utf-8", errors).encode(encoding, errors)
     if strings_only and is_protected_type(s):
         return s
     if isinstance(s, memoryview):
         return bytes(s)
     return str(s).encode(encoding, errors)
 
 
 # List of byte values that uri_to_iri() decodes from percent encoding.
 # First, the unreserved characters from RFC 3986:
 _ascii_ranges = [[45, 46, 95, 126], range(65, 91), range(97, 123)]
 _hextobyte = {
     (fmt % char).encode(): bytes((char,))
     for ascii_range in _ascii_ranges
     for char in ascii_range
-    for fmt in ['%02x', '%02X']
+    for fmt in ["%02x", "%02X"]
 }
 # And then everything above 128, because bytes ≥ 128 are part of multibyte
 # Unicode characters.
-_hexdig = '0123456789ABCDEFabcdef'
-_hextobyte.update({
-    (a + b).encode(): bytes.fromhex(a + b)
-    for a in _hexdig[8:] for b in _hexdig
-})
+_hexdig = "0123456789ABCDEFabcdef"
+_hextobyte.update(
+    {(a + b).encode(): bytes.fromhex(a + b) for a in _hexdig[8:] for b in _hexdig}
+)
 
 
 def uri_to_iri(uri):
     """
     Convert a Uniform Resource Identifier(URI) into an Internationalized
     Resource Identifier(IRI).
 
@@ -108,30 +106,30 @@
     if uri is None:
         return uri
     uri = force_bytes(uri)
     # Fast selective unquote: First, split on '%' and then starting with the
     # second block, decode the first 2 bytes if they represent a hex code to
     # decode. The rest of the block is the part after '%AB', not containing
     # any '%'. Add that to the output without further processing.
-    bits = uri.split(b'%')
+    bits = uri.split(b"%")
     if len(bits) == 1:
         iri = uri
     else:
         parts = [bits[0]]
         append = parts.append
         hextobyte = _hextobyte
         for item in bits[1:]:
             hex = item[:2]
             if hex in hextobyte:
                 append(hextobyte[item[:2]])
                 append(item[2:])
             else:
-                append(b'%')
+                append(b"%")
                 append(item)
-        iri = b''.join(parts)
+        iri = b"".join(parts)
     return repercent_broken_unicode(iri).decode()
 
 
 def escape_uri_path(path):
     """
     Escape the unsafe characters from the path portion of a Uniform Resource
     Identifier (URI).
@@ -146,32 +144,31 @@
     # The reason for not subtracting and escaping "/" is that we are escaping
     # the entire path, not a path segment.
     return quote(path, safe="/:@&+$,-_.!~*'()")
 
 
 def punycode(domain):
     """Return the Punycode of the given domain if it's non-ASCII."""
-    return domain.encode('idna').decode('ascii')
+    return domain.encode("idna").decode("ascii")
 
 
 def repercent_broken_unicode(path):
     """
     As per section 3.2 of RFC 3987, step three of converting a URI into an IRI,
     repercent-encode any octet produced that is not part of a strictly legal
     UTF-8 octet sequence.
     """
     while True:
         try:
             path.decode()
         except UnicodeDecodeError as e:
             # CVE-2019-14235: A recursion shouldn't be used since the exception
             # handling uses massive amounts of memory
-            repercent = quote(path[e.start:e.end],
-                              safe=b"/#%[]=:;$&()+,!?*@'~")
-            path = path[:e.start] + repercent.encode() + path[e.end:]
+            repercent = quote(path[e.start : e.end], safe=b"/#%[]=:;$&()+,!?*@'~")
+            path = path[: e.start] + repercent.encode() + path[e.end :]
         else:
             return path
 
 
 def filepath_to_uri(path):
     """Convert a file system path to a URI portion that is suitable for
     inclusion in a URL.
@@ -190,15 +187,15 @@
 def get_system_encoding():
     """
     The encoding of the default system locale. Fallback to 'ascii' if the
     #encoding is unsupported by Python or could not be determined. See tickets
     #10335 and #5846.
     """
     try:
-        encoding = locale.getdefaultlocale()[1] or 'ascii'
+        encoding = locale.getdefaultlocale()[1] or "ascii"
         codecs.lookup(encoding)
     except Exception:
-        encoding = 'ascii'
+        encoding = "ascii"
     return encoding
 
 
 DEFAULT_LOCALE_ENCODING = get_system_encoding()
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/crypto/signing.py` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/crypto/signing.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,96 +28,96 @@
 
 The fact that the string is compressed is signalled by the prefixed '.' at the
 start of the base64 JSON.
 
 There are 65 url-safe characters: the 64 used by url-safe base64 and the ':'.
 These functions make use of all of them.
 """
-
 import base64
 import datetime
-import re
 import json
+import re
 import time
 import zlib
 
-from .crypto import constant_time_compare, salted_hmac
+from .crypto import constant_time_compare
+from .crypto import salted_hmac
 
-_SEP_UNSAFE = re.compile(r'^[A-z0-9-_=]*$')
-BASE62_ALPHABET = \
-  '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
+_SEP_UNSAFE = re.compile(r"^[A-z0-9-_=]*$")
+BASE62_ALPHABET = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
 
 
 class BadSignature(Exception):
     """Signature does not match."""
+
     pass
 
 
 class SignatureExpired(BadSignature):
     """Signature timestamp is older than required max_age."""
+
     pass
 
 
 def b62_encode(s):
     if s == 0:
-        return '0'
-    sign = '-' if s < 0 else ''
+        return "0"
+    sign = "-" if s < 0 else ""
     s = abs(s)
-    encoded = ''
+    encoded = ""
     while s > 0:
         s, remainder = divmod(s, 62)
         encoded = BASE62_ALPHABET[remainder] + encoded
     return sign + encoded
 
 
 def b62_decode(s):
-    if s == '0':
+    if s == "0":
         return 0
     sign = 1
-    if s[0] == '-':
+    if s[0] == "-":
         s = s[1:]
         sign = -1
     decoded = 0
     for digit in s:
         decoded = decoded * 62 + BASE62_ALPHABET.index(digit)
     return sign * decoded
 
 
 def b64_encode(s):
-    return base64.urlsafe_b64encode(s).strip(b'=')
+    return base64.urlsafe_b64encode(s).strip(b"=")
 
 
 def b64_decode(s):
-    pad = b'=' * (-len(s) % 4)
+    pad = b"=" * (-len(s) % 4)
     return base64.urlsafe_b64decode(s + pad)
 
 
-def base64_hmac(salt, value, key, algorithm='sha1'):
+def base64_hmac(salt, value, key, algorithm="sha1"):
     return b64_encode(
-            salted_hmac(salt, value, key, algorithm=algorithm).digest()
-            ).decode()
+        salted_hmac(salt, value, key, algorithm=algorithm).digest()
+    ).decode()
 
 
 class JSONSerializer:
     """
     Simple wrapper around json to be used in signing.dumps and
     signing.loads.
     """
+
     def dumps(self, obj):
-        return json.dumps(obj, separators=(',', ':')).encode('latin-1')
+        return json.dumps(obj, separators=(",", ":")).encode("latin-1")
 
     def loads(self, data):
-        return json.loads(data.decode('latin-1'))
+        return json.loads(data.decode("latin-1"))
 
 
-def dumps(obj,
-          key=None,
-          salt='django.core.signing',
-          serializer=JSONSerializer,
-          compress=False):
+def dumps(
+    obj, key=None, salt="django.core.signing", serializer=JSONSerializer, compress=False
+):
     """
     Return URL-safe, hmac signed base64 compressed JSON string. If key is
     None, raises Exception. The hmac algorithm is the default
     Signer algorithm.
 
     If compress is True (not the default), check if compressing using zlib can
     save some space. Prepend a '.' to signify compression. This is included
@@ -126,55 +126,53 @@
     Salt can be used to namespace the hash, so that a signed string is
     only valid for a given namespace. Leaving this at the default
     value or re-using a salt value across different parts of your
     application without good cause is a security risk.
 
     The serializer is expected to return a bytestring.
     """
-    return TimestampSigner(key, salt=salt).sign_object(obj,
-                                                       serializer=serializer,
-                                                       compress=compress)
+    return TimestampSigner(key, salt=salt).sign_object(
+        obj, serializer=serializer, compress=compress
+    )
 
 
-def loads(s,
-          key=None,
-          salt='django.core.signing',
-          serializer=JSONSerializer,
-          max_age=None):
+def loads(
+    s, key=None, salt="django.core.signing", serializer=JSONSerializer, max_age=None
+):
     """
     Reverse of dumps(), raise BadSignature if signature fails.
 
     The serializer is expected to accept a bytestring.
     """
-    return TimestampSigner(key, salt=salt).unsign_object(s,
-                                                         serializer=serializer,
-                                                         max_age=max_age)
+    return TimestampSigner(key, salt=salt).unsign_object(
+        s, serializer=serializer, max_age=max_age
+    )
 
 
 class Signer:
-    def __init__(self, key, sep=':', salt=None, algorithm=None):
+    def __init__(self, key, sep=":", salt=None, algorithm=None):
         self.key = key
         self.sep = sep
         if _SEP_UNSAFE.match(self.sep):
             raise ValueError(
-                'Unsafe Signer separator: %r (cannot be empty or consist of '
-                'only A-z0-9-_=)' % sep,
+                "Unsafe Signer separator: %r (cannot be empty or consist of "
+                "only A-z0-9-_=)" % sep,
             )
-        self.salt = salt or '%s.%s' % (
-                self.__class__.__module__, self.__class__.__name__
-                )
-        self.algorithm = algorithm or 'sha256'
+        self.salt = salt or "{}.{}".format(
+            self.__class__.__module__, self.__class__.__name__
+        )
+        self.algorithm = algorithm or "sha256"
 
     def signature(self, value):
-        return base64_hmac(self.salt + 'signer',
-                           value, self.key,
-                           algorithm=self.algorithm)
+        return base64_hmac(
+            self.salt + "signer", value, self.key, algorithm=self.algorithm
+        )
 
     def sign(self, value):
-        return '%s%s%s' % (value, self.sep, self.signature(value))
+        return f"{value}{self.sep}{self.signature(value)}"
 
     def unsign(self, signed_value):
         if self.sep not in signed_value:
             raise BadSignature('No "%s" found in value' % self.sep)
         value, sig = signed_value.rsplit(self.sep, 1)
         if constant_time_compare(sig, self.signature(value)):
             return value
@@ -198,38 +196,37 @@
             # Avoid zlib dependency unless compress is being used.
             compressed = zlib.compress(data)
             if len(compressed) < (len(data) - 1):
                 data = compressed
                 is_compressed = True
         base64d = b64_encode(data).decode()
         if is_compressed:
-            base64d = '.' + base64d
+            base64d = "." + base64d
         return self.sign(base64d)
 
     def unsign_object(self, signed_obj, serializer=JSONSerializer, **kwargs):
         # Signer.unsign() returns str but base64 and zlib compression operate
         # on bytes.
         base64d = self.unsign(signed_obj, **kwargs).encode()
-        decompress = base64d[:1] == b'.'
+        decompress = base64d[:1] == b"."
         if decompress:
             # It's compressed; uncompress it first.
             base64d = base64d[1:]
         data = b64_decode(base64d)
         if decompress:
             data = zlib.decompress(data)
         return serializer().loads(data)
 
 
 class TimestampSigner(Signer):
-
     def timestamp(self):
         return b62_encode(int(time.time()))
 
     def sign(self, value):
-        value = '%s%s%s' % (value, self.sep, self.timestamp())
+        value = f"{value}{self.sep}{self.timestamp()}"
         return super().sign(value)
 
     def unsign(self, value, max_age=None):
         """
         Retrieve original value and check it wasn't signed more
         than max_age seconds ago.
         """
@@ -238,10 +235,9 @@
         timestamp = b62_decode(timestamp)
         if max_age is not None:
             if isinstance(max_age, datetime.timedelta):
                 max_age = max_age.total_seconds()
             # Check timestamp is not older than max_age
             age = time.time() - timestamp
             if age > max_age:
-                raise SignatureExpired(
-                    'Signature age %s > %s seconds' % (age, max_age))
+                raise SignatureExpired(f"Signature age {age} > {max_age} seconds")
         return value
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/nativeauthenticator.py` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/nativeauthenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,159 +1,178 @@
-import bcrypt
 import dbm
 import os
 import re
 import smtplib
-from email.message import EmailMessage
-from datetime import datetime, timedelta
+from datetime import datetime
+from datetime import timedelta
 from datetime import timezone as tz
-from jupyterhub.auth import Authenticator
+from email.message import EmailMessage
 from pathlib import Path
 
+import bcrypt
+from jupyterhub.auth import Authenticator
 from sqlalchemy import inspect
-from tornado import gen, web
-from traitlets import Bool, Integer, Unicode, Tuple, Dict
+from tornado import web
+from traitlets import Bool
+from traitlets import Dict
+from traitlets import Integer
+from traitlets import Tuple
+from traitlets import Unicode
 
-from .handlers import (
-    AuthorizeHandler,
-    AuthorizationHandler, ChangeAuthorizationHandler, ChangePasswordHandler,
-    ChangePasswordAdminHandler, LoginHandler, SignUpHandler, DiscardHandler,
-)
-from .orm import UserInfo
 from .crypto.signing import Signer
+from .handlers import AuthorizationAreaHandler
+from .handlers import ChangePasswordAdminHandler
+from .handlers import ChangePasswordHandler
+from .handlers import DiscardHandler
+from .handlers import EmailAuthorizationHandler
+from .handlers import LoginHandler
+from .handlers import SignUpHandler
+from .handlers import ToggleAuthorizationHandler
+from .orm import UserInfo
 
 
 class NativeAuthenticator(Authenticator):
 
     COMMON_PASSWORDS = None
     recaptcha_key = Unicode(
         config=True,
-        help=("Your key to enable reCAPTCHA as described at "
-              "https://developers.google.com/recaptcha/intro")
+        help=(
+            "Your key to enable reCAPTCHA as described at "
+            "https://developers.google.com/recaptcha/intro"
+        ),
     ).tag(default=None)
 
     recaptcha_secret = Unicode(
         config=True,
-        help=("Your secret to enable reCAPTCHA as described at "
-              "https://developers.google.com/recaptcha/intro")
+        help=(
+            "Your secret to enable reCAPTCHA as described at "
+            "https://developers.google.com/recaptcha/intro"
+        ),
     ).tag(default=None)
 
     tos = Unicode(
         config=True,
-        help=("The HTML to present next to the Term of Service "
-              "checkbox")
+        help=("The HTML to present next to the Term of Service " "checkbox"),
     ).tag(default=None)
 
     self_approval_server = Dict(
         config=True,
-        help=("SMTP server information as a dictionary of 'url', 'usr'"
-              "and 'pwd' to use for sending email, e.g."
-              "self_approval_server={'url': 'smtp.gmail.com', 'usr': 'myself'"
-              "'pwd': 'mypassword'}")
+        help=(
+            "SMTP server information as a dictionary of 'url', 'usr'"
+            "and 'pwd' to use for sending email, e.g."
+            "self_approval_server={'url': 'smtp.gmail.com', 'usr': 'myself'"
+            "'pwd': 'mypassword'}"
+        ),
     ).tag(default=None)
 
     secret_key = Unicode(
         config=True,
-        help=("Secret key to cryptographically sign the "
-              "self-approved URL (if allow_self_approval is utilized)")
+        help=(
+            "Secret key to cryptographically sign the "
+            "self-approved URL (if allow_self_approval is utilized)"
+        ),
     ).tag(default="")
 
     allow_self_approval_for = Unicode(
         allow_none=True,
         config=True,
-        help=("Use self-service authentication (rather than "
-              "admin-based authentication) for users whose "
-              "email match this patter. Note that this forces "
-              "ask_email_on_signup to be True.")
+        help=(
+            "Use self-service authentication (rather than "
+            "admin-based authentication) for users whose "
+            "email match this patter. Note that this forces "
+            "ask_email_on_signup to be True."
+        ),
     ).tag(default=None)
 
     self_approval_email = Tuple(
-        Unicode(), Unicode(), Unicode(),
-        config=True,
-        default_value=("do-not-reply@my-domain.com",
-                       "Welcome to JupyterHub on my-domain",
-                       ("Your JupyterHub account on my-domain has been "
-                        "created, but it's inactive.\n"
-                        "If you did not create the account yourself, "
-                        "IGNORE this message:\n"
-                        "somebody is trying to use your email to get an "
-                        "unathorized account!\n"
-                        "If you did create the account yourself, navigate "
-                        "to {approval_url} to activate it.\n"))
-
+        Unicode(),
+        Unicode(),
+        Unicode(),
+        config=True,
+        default_value=(
+            "do-not-reply@my-domain.com",
+            "Welcome to JupyterHub on my-domain",
+            (
+                "Your JupyterHub account on my-domain has been "
+                "created, but it's inactive.\n"
+                "If you did not create the account yourself, "
+                "IGNORE this message:\n"
+                "somebody is trying to use your email to get an "
+                "unathorized account!\n"
+                "If you did create the account yourself, navigate "
+                "to {approval_url} to activate it.\n"
+            ),
+        ),
     )
 
     check_common_password = Bool(
         config=True,
-        help=("Creates a verification of password strength "
-              "when a new user makes signup")
+        help=(
+            "Creates a verification of password strength "
+            "when a new user makes signup"
+        ),
     ).tag(default=False)
 
     minimum_password_length = Integer(
         config=True,
-        help=("Check if the length of the password is at least this size on "
-              "signup")
+        help=("Check if the length of the password is at least this size on " "signup"),
     ).tag(default=1)
 
     allowed_failed_logins = Integer(
         config=True,
-        help=("Configures the number of failed attempts a user can have "
-              "before being blocked.")
+        help=(
+            "Configures the number of failed attempts a user can have "
+            "before being blocked."
+        ),
     ).tag(default=0)
 
     seconds_before_next_try = Integer(
         config=True,
-        help=("Configures the number of seconds a user has to wait "
-              "after being blocked. Default is 600.")
+        help=(
+            "Configures the number of seconds a user has to wait "
+            "after being blocked. Default is 600."
+        ),
     ).tag(default=600)
 
     enable_signup = Bool(
         config=True,
         default_value=True,
-        help=("Allows every user to registry a new account")
+        help=("Allows every user to registry a new account"),
     )
 
     open_signup = Bool(
         config=True,
         default_value=False,
-        help=("Allows every user that made sign up to automatically log in "
-              "the system without needing admin authorization")
+        help=(
+            "Allows every user that made sign up to automatically log in "
+            "the system without needing admin authorization"
+        ),
     )
 
-    ask_email_on_signup = Bool(
-        False,
-        config=True,
-        help="Asks for email on signup"
-    )
+    ask_email_on_signup = Bool(False, config=True, help="Asks for email on signup")
 
     import_from_firstuse = Bool(
-        False,
-        config=True,
-        help="Import users from FirstUse Authenticator database"
+        False, config=True, help="Import users from FirstUse Authenticator database"
     )
 
     firstuse_db_path = Unicode(
-        'passwords.dbm',
+        "passwords.dbm",
         config=True,
         help="""
         Path to store the db file of FirstUse with username / pwd hash in
-        """
+        """,
     )
 
     delete_firstuse_db_after_import = Bool(
         config=True,
         default_value=False,
-        help="Deletes FirstUse Authenticator database after the import"
+        help="Deletes FirstUse Authenticator database after the import",
     )
 
-    allow_2fa = Bool(
-        False,
-        config=True,
-        help=""
-    )
+    allow_2fa = Bool(False, config=True, help="")
 
     def __init__(self, add_new_table=True, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.login_attempts = dict()
         if add_new_table:
             self.add_new_table()
@@ -165,85 +184,81 @@
 
     def setup_self_approval(self):
         if self.allow_self_approval_for:
             if self.open_signup:
                 self.log.error("self_approval and open_signup are conflicts!")
             self.ask_email_on_signup = True
             if len(self.secret_key) < 8:
-                raise ValueError("Secret_key must be a random string of "
-                                 "len > 8 when using self_approval")
+                raise ValueError(
+                    "Secret_key must be a random string of "
+                    "len > 8 when using self_approval"
+                )
 
     def add_new_table(self):
         inspector = inspect(self.db.bind)
-        if 'users_info' not in inspector.get_table_names():
+        if "users_info" not in inspector.get_table_names():
             UserInfo.__table__.create(self.db.bind)
 
     def add_login_attempt(self, username):
         if not self.login_attempts.get(username):
-            self.login_attempts[username] = {'count': 1,
-                                             'time': datetime.now()}
+            self.login_attempts[username] = {"count": 1, "time": datetime.now()}
         else:
-            self.login_attempts[username]['count'] += 1
-            self.login_attempts[username]['time'] = datetime.now()
+            self.login_attempts[username]["count"] += 1
+            self.login_attempts[username]["time"] = datetime.now()
 
     def can_try_to_login_again(self, username):
         login_attempts = self.login_attempts.get(username)
         if not login_attempts:
             return True
 
-        time_last_attempt = datetime.now() - login_attempts['time']
+        time_last_attempt = datetime.now() - login_attempts["time"]
         if time_last_attempt.seconds > self.seconds_before_next_try:
             return True
 
         return False
 
     def is_blocked(self, username):
         logins = self.login_attempts.get(username)
 
-        if not logins or logins['count'] < self.allowed_failed_logins:
+        if not logins or logins["count"] < self.allowed_failed_logins:
             return False
 
         if self.can_try_to_login_again(username):
             return False
         return True
 
     def successful_login(self, username):
         if self.login_attempts.get(username):
             self.login_attempts.pop(username)
 
-    @gen.coroutine
-    def authenticate(self, handler, data):
-        username = self.normalize_username(data['username'])
-        password = data['password']
+    async def authenticate(self, handler, data):
+        username = self.normalize_username(data["username"])
+        password = data["password"]
 
         user = self.get_user(username)
         if not user:
             return
 
         if self.allowed_failed_logins:
             if self.is_blocked(username):
                 return
 
-        validations = [
-            user.is_authorized,
-            user.is_valid_password(password)
-        ]
+        validations = [user.is_authorized, user.is_valid_password(password)]
         if user.has_2fa:
-            validations.append(user.is_valid_token(data.get('2fa')))
+            validations.append(user.is_valid_token(data.get("2fa")))
 
         if all(validations):
             self.successful_login(username)
             return username
 
         self.add_login_attempt(username)
 
     def is_password_common(self, password):
         common_credentials_file = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)),
-            'common-credentials.txt'
+            os.path.dirname(os.path.abspath(__file__)), "common-credentials.txt"
         )
         if not self.COMMON_PASSWORDS:
             with open(common_credentials_file) as f:
                 self.COMMON_PASSWORDS = set(f.read().splitlines())
         return password in self.COMMON_PASSWORDS
 
     def is_password_strong(self, password):
@@ -276,112 +291,126 @@
                     authed.update(set({info.username}))
 
         return authed.union(allowed.union(self.admin_users))
 
     def user_exists(self, username):
         return self.get_user(username) is not None
 
-    def create_user(self, username, pw, **kwargs):
+    def create_user(self, username, password, **kwargs):
         username = self.normalize_username(username)
 
-        if self.user_exists(username):
+        if self.user_exists(username) or not self.validate_username(username):
             return
 
-        if not self.is_password_strong(pw) or \
-           not self.validate_username(username):
+        if not self.is_password_strong(password):
             return
 
         if not self.enable_signup:
             return
 
-        encoded_pw = bcrypt.hashpw(pw.encode(), bcrypt.gensalt())
-        infos = {'username': username, 'password': encoded_pw}
+        encoded_password = bcrypt.hashpw(password.encode(), bcrypt.gensalt())
+        infos = {"username": username, "password": encoded_password}
         infos.update(kwargs)
 
-        if self.open_signup or username in self.get_authed_users():
-            infos.update({'is_authorized': True})
+        # Pre-authorized users (admins, or any users during open signup)
+        pre_authorized = self.open_signup or username in self.get_authed_users()
+
+        if pre_authorized:
+            infos.update({"is_authorized": True})
 
         try:
             user_info = UserInfo(**infos)
         except AssertionError:
             return
 
-        if self.allow_self_approval_for:
+        # Don't send authorization emails to pre-authorized users.
+        if self.allow_self_approval_for and not pre_authorized:
             match = re.match(self.allow_self_approval_for, user_info.email)
             if match:
                 url = self.generate_approval_url(username)
                 self.send_approval_email(user_info.email, url)
                 user_info.login_email_sent = True
 
         self.db.add(user_info)
         self.db.commit()
         return user_info
 
     def generate_approval_url(self, username, when=None):
         if when is None:
             when = datetime.now(tz.utc) + timedelta(minutes=15)
         s = Signer(self.secret_key)
-        u = s.sign_object({"username": username,
-                           "expire": when.isoformat()})
+        u = s.sign_object({"username": username, "expire": when.isoformat()})
         return "/confirm/" + u
 
     def send_approval_email(self, dest, url):
         msg = EmailMessage()
-        msg['From'] = self.self_approval_email[0]
-        msg['Subject'] = self.self_approval_email[1]
+        msg["From"] = self.self_approval_email[0]
+        msg["Subject"] = self.self_approval_email[1]
         msg.set_content(self.self_approval_email[2].format(approval_url=url))
-        msg['To'] = dest
+        msg["To"] = dest
         try:
             if self.self_approval_server:
-                s = smtplib.SMTP_SSL(self.self_approval_server['url'])
-                s.login(self.self_approval_server['usr'],
-                        self.self_approval_server['pwd'])
+                s = smtplib.SMTP_SSL(self.self_approval_server["url"])
+                s.login(
+                    self.self_approval_server["usr"], self.self_approval_server["pwd"]
+                )
             else:
-                s = smtplib.SMTP('localhost')
+                s = smtplib.SMTP("localhost")
             s.send_message(msg)
             s.quit()
         except Exception as e:
             self.log.error(e)
-            raise web.HTTPError(503,
-                                reason="Self-authorization email could not " +
-                                "be sent. Please contact the jupyterhub " +
-                                "admin about this.")
+            raise web.HTTPError(
+                503,
+                reason="Self-authorization email could not "
+                + "be sent. Please contact the JupyterHub "
+                + "admin about this.",
+            )
 
     def get_unauthed_amount(self):
         unauthed = 0
         for info in UserInfo.all_users(self.db):
             user = self.get_user(info.username)
             if user is not None:
                 if info.username not in self.get_authed_users():
                     unauthed += 1
 
         return unauthed
 
     def change_password(self, username, new_password):
         user = self.get_user(username)
+
+        criteria = [
+            user is not None,
+            self.is_password_strong(new_password),
+        ]
+        if not all(criteria):
+            return
+
         user.password = bcrypt.hashpw(new_password.encode(), bcrypt.gensalt())
         self.db.commit()
+        return True
 
     def validate_username(self, username):
-        invalid_chars = [',', ' ']
+        invalid_chars = [",", " ", "/"]
         if any((char in username) for char in invalid_chars):
             return False
         return super().validate_username(username)
 
     def get_handlers(self, app):
         native_handlers = [
-            (r'/login', LoginHandler),
-            (r'/signup', SignUpHandler),
-            (r'/discard/([^/]*)', DiscardHandler),
-            (r'/authorize', AuthorizationHandler),
-            (r'/authorize/([^/]*)', ChangeAuthorizationHandler),
+            (r"/login", LoginHandler),
+            (r"/signup", SignUpHandler),
+            (r"/discard/([^/]*)", DiscardHandler),
+            (r"/authorize", AuthorizationAreaHandler),
+            (r"/authorize/([^/]*)", ToggleAuthorizationHandler),
             # the following /confirm/ must be like in generate_approval_url()
-            (r'/confirm/([^/]*)', AuthorizeHandler),
-            (r'/change-password', ChangePasswordHandler),
-            (r'/change-password/([^/]+)', ChangePasswordAdminHandler),
+            (r"/confirm/([^/]*)", EmailAuthorizationHandler),
+            (r"/change-password", ChangePasswordHandler),
+            (r"/change-password/([^/]+)", ChangePasswordAdminHandler),
         ]
         return native_handlers
 
     def delete_user(self, user):
         user_info = self.get_user(user.name)
         if user_info is not None:
             self.db.delete(user_info)
@@ -391,25 +420,27 @@
     def delete_dbm_db(self):
         db_path = Path(self.firstuse_db_path)
         db_dir = db_path.cwd()
         db_name = db_path.name
         db_complete_path = str(db_path.absolute())
 
         # necessary for BSD implementation of dbm lib
-        if os.path.exists(os.path.join(db_dir, db_name + '.db')):
-            os.remove(db_complete_path + '.db')
+        if os.path.exists(os.path.join(db_dir, db_name + ".db")):
+            os.remove(db_complete_path + ".db")
         else:
             os.remove(db_complete_path)
 
     def add_data_from_firstuse(self):
-        with dbm.open(self.firstuse_db_path, 'c', 0o600) as db:
+        with dbm.open(self.firstuse_db_path, "c", 0o600) as db:
             for user in db.keys():
                 password = db[user].decode()
                 new_user = self.create_user(user.decode(), password)
                 if not new_user:
-                    error = '''User {} was not created. Check password
-                               restrictions or username problems before trying
-                               again'''.format(user)
+                    error = (
+                        f"User {user} was not created. Check password "
+                        "restrictions or username problems before trying "
+                        "again."
+                    )
                     raise ValueError(error)
 
         if self.delete_firstuse_db_after_import:
             self.delete_dbm_db()
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/autorization-area.html` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/authorization-area.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 {% extends "page.html" %}
+
 {% block main %}
 <div class="container">
-    <h1>Authorization Area</h1>
+    <h1>Authorization area</h1>
+
     <table class="table">
         <thead>
             <tr>
                 <th>Username</th>
-                {% if ask_email %}
-                <th>Email</th>
-                {% endif %}
-                <th>Has 2fa?</th>
-                <th>Is Authorized?</th>
+                {% if ask_email %}<th>Email</th>{% endif %}
+                <th>Has 2FA?</th>
+                <th>Is authorized?</th>
+                <th></th>
+                <th></th>
+                <th></th>
             </tr>
         </thead>
         <tbody>
             {% for user in users %}
             {% if user.is_authorized %}
             <tr class="success" id={{ user.username }}>
                 <td>{{ user.username }}</td>
-                {% if ask_email %}
-                <td>{{ user.email }}</td>
-                {% endif %}
+                {% if ask_email %}<td>{{ user.email }}</td>{% endif %}
                 <td>{{ user.has_2fa }}</td>
                 <td>Yes</td>
-                <td>
-                    <a class="btn btn-default" href="{{ base_url }}authorize/{{ user.username }}" role="button">Unauthorize</a>
-                </td>
+                <td><a class="btn btn-default" href="{{ base_url }}authorize/{{ user.username }}" role="button">Unauthorize</a></td>
+                <td><a class="btn btn-jupyter" href="{{ base_url }}change-password/{{ user.username }}" role="button">Change password</a></td>
                 <td></td>
-                {% else %}
+            </tr>
+            {% else %}
             <tr id={{ user.username }}>
                 <td>{{ user.username }}</td>
-                {% if ask_email %}
-                <td>{{ user.email }}</td>
-                {% endif %}
+                {% if ask_email %}<td>{{ user.email }}</td>{% endif %}
                 <td>{{ user.has_2fa }}</td>
                 <td>No</td>
-                <td>
-                    <a class="btn btn-jupyter" href="{{ base_url }}authorize/{{ user.username }}" role="button">Authorize</a>
-                </td>
-                <td>
-                    <a class="btn btn-jupyter" href="{{ base_url }}discard/{{ user.username }}" role="button">Discard</a>
-                </td>
-                {% endif %}
+                <td><a class="btn btn-jupyter" href="{{ base_url }}authorize/{{ user.username }}" role="button">Authorize</a></td>
+                <td><a class="btn btn-jupyter" href="{{ base_url }}change-password/{{ user.username }}" role="button">Change password</a></td>
+                <td><a class="btn btn-jupyter" href="{{ base_url }}discard/{{ user.username }}" role="button">Discard</a></td>
             </tr>
+            {% endif %}
             {% endfor %}
         </tbody>
     </table>
 </div>
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% extends "page.html" %} {% block main %}
-****** Authorization Area ******
-Username Email Has 2fa? Is Authorized?
+****** Authorization area ******
+Username Email Has 2FA? Is authorized?
 {% endblock %}
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/change-password.html` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/change-password.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 {% extends "page.html" %}
-{% block main %}
 
+{% block script %}
+{{ super() }}
 <script type="text/javascript">
-document.addEventListener('DOMContentLoaded', function() {
-    let button = document.getElementById('eye');
-    button.addEventListener("click", function(e){
-        let pwd = document.getElementById("pwd");
-        if(pwd.getAttribute("type") === "password"){
-            pwd.setAttribute("type","text");
-            button.textContent = "🔑";
-        } else {
-            pwd.setAttribute("type","password");
-            button.textContent = "👁";
-        }
+    document.addEventListener('DOMContentLoaded', function() {
+        let button = document.getElementById('eye');
+        button.addEventListener("click", function(e) {
+            let opwd = document.getElementById("old_password_input");
+            let npwd = document.getElementById("new_password_input");
+            let cpwd = document.getElementById("new_password_confirmation_input");
+            if (opwd.getAttribute("type") === "password") {
+                opwd.setAttribute("type", "text");
+                npwd.setAttribute("type", "text");
+                cpwd.setAttribute("type", "text");
+                button.textContent = "🔑";
+            } else {
+                opwd.setAttribute("type", "password");
+                npwd.setAttribute("type", "password");
+                cpwd.setAttribute("type", "password");
+                button.textContent = "👁";
+            }
+        });
     });
-});
 </script>
+{% endblock script %}
 
-  <div class="container">
+{% block main %}
+<div class="container">
     <form action="{{post_url}}" method="post" role="form">
-      <h2>
-      Change Password For {{user_name}}
-      </h2>
-      <div>
-        <div class="form-group">
-          <label for="pwd">New password:</label>
-          <div class="input-group">
-            <input
-            type="password"
-            class="form-control"
-            name="password"
-            id="pwd"
-            tabindex="2"
-            />
-            <span class="input-group-addon">
-              <button style="border:0;" type="button" id="eye">
-                👁
-              </button>
-            </span>
-          </div>
-          </div>
+        <h1>
+            Change password for {{user_name}}
+        </h1>
+        
+        <p>Please enter your current password and the new password you want to set it to. If you have forgotten your password, an admin can reset it for you.</p>
+
         <div class="form-group">
-          <input
-          type="submit"
-          id="signup_submit"
-          class='btn btn-jupyter'
-          value='Change Password'
-          tabindex="3"
-          />
+            <label for="old_password_input">Old password:</label>
+            <div class="input-group col-xs-6">
+                <input id="old_password_input" type="password" name="old_password" val="" autocapitalize="off" autocorrect="off" class="form-control" />
+                <span class="input-group-addon">
+                    <button id="eye" type="button" style="border:0;">👁</button>
+                </span>
+            </div>
+            <p></p>
+            
+            <label for="new_password_input">New password:</label>
+            <div class="input-group col-xs-6">
+                <input id="new_password_input" type="password" name="new_password" val="" autocapitalize="off" autocorrect="off" class="form-control" />
+            </div>
+            <p></p>
+            
+            <label for="new_password_confirmation_input">Confirm new password:</label>
+            <div class="input-group col-xs-6">
+                <input id="new_password_confirmation_input" type="password" name="new_password_confirmation" val="" autocapitalize="off" autocorrect="off" class="form-control" />
+                <span></span>
+            </div>
+            <p></p>
+
+            <input id="signup_submit" type="submit" value='Change Password' class='btn btn-jupyter' />
         </div>
-      </div>
     </form>
 
     {% if result_message %}
-      <div class="alert alert-success" role="alert">{{result_message}}</div>
+        <div class="alert {{alert}} col-xs-6" role="alert">{{result_message}}</div>
     {% endif %}
-    
-  </div>
-
-
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-{% extends "page.html" %} {% block main %}
-***** Change Password For {{user_name}} *****
+{% extends "page.html" %} {% block script %} {{ super() }}
+ {% endblock script %} {% block main %}
+****** Change password for {{user_name}} ******
+Please enter your current password and the new password you want to set it to.
+If you have forgotten your password, an admin can reset it for you.
+Old password:
+[********************]  ð
 New password:
-[********************]   ð
+[********************]
+Confirm new password:
+[********************]
 [Change Password]
 {% if result_message %}
 {{result_message}}
 {% endif %}
 {% endblock %}
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/templates/native-login.html` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/templates/native-login.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,84 @@
 {% extends "page.html" %}
+
 {% if announcement_login %}
   {% set announcement = announcement_login %}
 {% endif %}
-{% block main %}
+
+{% block script %}
+{{ super() }}
 <script type="text/javascript">
-document.addEventListener('DOMContentLoaded', function() {
-    let button = document.getElementById('eye');
-    button.addEventListener("click", function(e) {
-        let pwd = document.getElementById("password_input");
-        if (pwd.getAttribute("type") === "password") {
-            pwd.setAttribute("type", "text");
-            button.textContent = "🔑";
-        } else {
-            pwd.setAttribute("type", "password");
-            button.textContent = "👁";
-        }
+    document.addEventListener('DOMContentLoaded', function() {
+        let button = document.getElementById('eye');
+        button.addEventListener("click", function(e) {
+            let pwd = document.getElementById("password_input");
+            if (pwd.getAttribute("type") === "password") {
+                pwd.setAttribute("type", "text");
+                button.textContent = "🔑";
+            } else {
+                pwd.setAttribute("type", "password");
+                button.textContent = "👁";
+            }
+        });
     });
-});
+
+    if (window.location.protocol === "http:") {
+        // unhide http warning
+        let warning = document.getElementById('insecure-login-warning');
+        warning.className = warning.className.replace(/\bhidden\b/, '');
+    }
 </script>
+{% endblock script %}
+
+{% block main %}
 {% block login %}
 <div id="login-main" class="container">
     <form action="{{login_url}}?next={{next}}" method="post" role="form">
         <div class="auth-form-header">
             Sign In
         </div>
+
         <div class='auth-form-body'>
             <p id='insecure-login-warning' class='hidden'>
                 Warning: JupyterHub seems to be served over an unsecured HTTP connection.
                 We strongly recommend enabling HTTPS for JupyterHub.
             </p>
+
             {% if login_error %}
             <p class="login_error">
                 {{login_error}}
             </p>
             {% endif %}
+
             <label for="username_input">Username:</label>
-            <input id="username_input" type="text" autocapitalize="off" autocorrect="off" class="form-control" name="username" val="{{username}}" tabindex="1" autofocus="autofocus" />
+            <input id="username_input" type="text" name="username" val="{{username}}" autocapitalize="off" autocorrect="off" class="form-control" autofocus="autofocus" required />
             <p></p>
+
             <label for='password_input'>Password:</label>
             <div class="input-group">
-                <input type="password" class="form-control" name="password" id="password_input" tabindex="2" />
+                <input id="password_input" type="password" name="password" val="" autocapitalize="off" autocorrect="off" class="form-control" />
                 <span class="input-group-addon">
-                    <button style="border:0;" type="button" id="eye">
-                        👁
-                    </button>
+                    <button id="eye" type="button" style="border:0;">👁</button>
                 </span>
             </div>
+            <p></p>
+
             {% if two_factor_auth %}
+            <label for="2fa_input">2FA code:</label>
+            <input id="2fa_input" type="text" autocapitalize="off" autocorrect="off" class="form-control" name="2fa" placeholder="If you don't have 2FA, leave empty" />
             <p></p>
-            <label for="2fa_input">Two Factor Authentication:</label>
-            <input id="2fa_input" type="text" autocapitalize="off" autocorrect="off" class="form-control" name="2fa" tabindex="1" autofocus="autofocus" placeholder="If you don't have 2FA, leave empty" />
             {% endif %}
-            <input type="submit" id="login_submit" class='btn btn-jupyter' value='Sign In' tabindex="3" />
+
+            <input type="submit" id="login_submit" class='btn btn-jupyter' value='Sign In' />
+            <p></p>
+
             {% if enable_signup %}
-            <div style="padding-top: 25px;">
-                <p>Don't have an account? <a href="{{ base_url }}signup">Signup!</a></p>
-            </div>
+            <hr />
+            <p>
+                <a href="{{ base_url }}signup"> Sign up</a> to create a new user.
+            </p>
             {% endif %}
         </div>
     </form>
 </div>
 {% endblock login %}
-{% endblock %}
-{% block script %}
-{{ super() }}
-<script>
-if (window.location.protocol === "http:") {
-    // unhide http warning
-    let warning = document.getElementById('insecure-login-warning');
-    warning.className = warning.className.replace(/\bhidden\b/, '');
-}
-</script>
-{% endblock %}
+{% endblock main %}
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% extends "page.html" %} {% if announcement_login %} {% set announcement =
-announcement_login %} {% endif %} {% block main %}
- {% block login %}
+announcement_login %} {% endif %} {% block script %} {{ super() }}
+ {% endblock script %} {% block main %} {% block login %}
 Sign In
 Warning: JupyterHub seems to be served over an unsecured HTTP connection. We
 strongly recommend enabling HTTPS for JupyterHub.
 {% if login_error %}
 {{login_error}}
 {% endif %} Username: [username            ]
 Password:
-[********************]   ð
-{% if two_factor_auth %}
-Two Factor Authentication: [2fa                 ] {% endif %} [Sign In] {% if
-enable_signup %}
-Don't have an account? Signup!
+[********************]  ð
+{% if two_factor_auth %} 2FA code: [2fa                 ]
+{% endif %} [Sign In]
+{% if enable_signup %}
+===============================================================================
+Sign_up to create a new user.
 {% endif %}
-{% endblock login %} {% endblock %} {% block script %} {{ super() }}
- {% endblock %}
+{% endblock login %} {% endblock main %}
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/nativeauthenticator/tests/test_authenticator.py` & `jupyterhub-nativeauthenticator-1.1.0/nativeauthenticator/tests/test_authenticator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import datetime
 import dbm
 import os
-import pytest
-import datetime
-from datetime import timezone as tz
 import time
+from datetime import timezone as tz
+
+import pytest
 from jupyterhub.tests.mocking import MockHub
 
-from nativeauthenticator import NativeAuthenticator
+from ..handlers import EmailAuthorizationHandler
 from ..orm import UserInfo
-from ..handlers import AuthorizeHandler
+from nativeauthenticator import NativeAuthenticator
 
 
 @pytest.fixture
 def tmpcwd(tmpdir):
     tmpdir.chdir()
 
 
@@ -25,321 +26,361 @@
 
 # use pytest-asyncio
 pytestmark = pytest.mark.asyncio
 # run each test in a temporary working directory
 pytestmark = pytestmark(pytest.mark.usefixtures("tmpcwd"))
 
 
-@pytest.mark.parametrize("is_admin,open_signup,expected_authorization", [
-    (False, False, False),
-    (True, False, True),
-    (False, True, True),
-    (True, True, True)
-])
-async def test_create_user(is_admin, open_signup, expected_authorization,
-                           tmpcwd, app):
-    '''Test method create_user for new user and authorization '''
+@pytest.mark.parametrize(
+    "is_admin,open_signup,expected_authorization",
+    [
+        (False, False, False),
+        (True, False, True),
+        (False, True, True),
+        (True, True, True),
+    ],
+)
+async def test_create_user(is_admin, open_signup, expected_authorization, tmpcwd, app):
+    """Test method create_user for new user and authorization"""
     auth = NativeAuthenticator(db=app.db)
 
     if is_admin:
-        auth.admin_users = ({'johnsnow'})
+        auth.admin_users = {"johnsnow"}
     if open_signup:
         auth.open_signup = True
 
-    auth.create_user('johnsnow', 'password')
-    user_info = UserInfo.find(app.db, 'johnsnow')
-    assert user_info.username == 'johnsnow'
+    auth.create_user("johnsnow", "password")
+    user_info = UserInfo.find(app.db, "johnsnow")
+    assert user_info.username == "johnsnow"
     assert user_info.is_authorized == expected_authorization
 
 
 async def test_create_user_bad_characters(tmpcwd, app):
-    '''Test method create_user with bad characters on username'''
+    """Test method create_user with bad characters on username"""
     auth = NativeAuthenticator(db=app.db)
-    assert not auth.create_user('john snow', 'password')
-    assert not auth.create_user('john,snow', 'password')
+    assert not auth.create_user("john snow", "password")
+    assert not auth.create_user("john,snow", "password")
 
 
 async def test_create_user_twice(tmpcwd, app):
-    '''Test if creating users with an existing handle errors.'''
+    """Test if creating users with an existing handle errors."""
     auth = NativeAuthenticator(db=app.db)
 
     # First creation should succeed.
-    assert auth.create_user('johnsnow', 'password')
+    assert auth.create_user("johnsnow", "password")
 
     # Creating the same account again should fail.
-    assert not auth.create_user('johnsnow', 'password')
+    assert not auth.create_user("johnsnow", "password")
 
     # Creating a user with same handle but different pw should also fail.
-    assert not auth.create_user('johnsnow', 'adifferentpassword')
+    assert not auth.create_user("johnsnow", "adifferentpassword")
 
 
 async def test_get_authed_users(tmpcwd, app):
-    '''Test if get_authed_users returns the proper set of users.'''
+    """Test if get_authed_users returns the proper set of users."""
     auth = NativeAuthenticator(db=app.db)
 
     auth.admin_users = set()
     assert auth.get_authed_users() == set()
 
-    auth.create_user('johnsnow', 'password')
+    auth.create_user("johnsnow", "password")
     assert auth.get_authed_users() == set()
 
-    UserInfo.change_authorization(app.db, 'johnsnow')
-    assert auth.get_authed_users() == set({'johnsnow'})
+    UserInfo.change_authorization(app.db, "johnsnow")
+    assert auth.get_authed_users() == set({"johnsnow"})
 
-    auth.create_user('daenerystargaryen', 'anotherpassword')
-    assert auth.get_authed_users() == set({'johnsnow'})
+    auth.create_user("daenerystargaryen", "anotherpassword")
+    assert auth.get_authed_users() == set({"johnsnow"})
 
-    auth.admin_users = set({'daenerystargaryen'})
-    assert 'johnsnow' in auth.get_authed_users()
-    assert 'daenerystargaryen' in auth.get_authed_users()
+    auth.admin_users = set({"daenerystargaryen"})
+    assert "johnsnow" in auth.get_authed_users()
+    assert "daenerystargaryen" in auth.get_authed_users()
 
 
 async def test_get_unauthed_amount(tmpcwd, app):
-    '''Test if get_unauthed_amount returns the proper amount.'''
+    """Test if get_unauthed_amount returns the proper amount."""
     auth = NativeAuthenticator(db=app.db)
 
     auth.admin_users = set()
     assert auth.get_unauthed_amount() == 0
 
-    auth.create_user('johnsnow', 'password')
+    auth.create_user("johnsnow", "password")
     assert auth.get_unauthed_amount() == 1
 
-    UserInfo.change_authorization(app.db, 'johnsnow')
+    UserInfo.change_authorization(app.db, "johnsnow")
     assert auth.get_unauthed_amount() == 0
 
-    auth.create_user('daenerystargaryen', 'anotherpassword')
+    auth.create_user("daenerystargaryen", "anotherpassword")
     assert auth.get_unauthed_amount() == 1
 
-    auth.create_user('tyrionlannister', 'yetanotherpassword')
+    auth.create_user("tyrionlannister", "yetanotherpassword")
     assert auth.get_unauthed_amount() == 2
 
-    auth.admin_users = set({'daenerystargaryen'})
+    auth.admin_users = set({"daenerystargaryen"})
     assert auth.get_unauthed_amount() == 1
 
 
-@pytest.mark.parametrize("password,min_len,expected", [
-    ("qwerty", 1, False),
-    ("agameofthrones", 1, True),
-    ("agameofthrones", 15, False),
-    ("averyveryverylongpassword", 15, True),
-])
-async def test_create_user_with_strong_passwords(password, min_len, expected,
-                                                 tmpcwd, app):
-    '''Test if method create_user and strong passwords mesh'''
+@pytest.mark.parametrize(
+    "password,min_len,expected",
+    [
+        ("qwerty", 1, False),
+        ("agameofthrones", 1, True),
+        ("agameofthrones", 15, False),
+        ("averyveryverylongpassword", 15, True),
+    ],
+)
+async def test_create_user_with_strong_passwords(
+    password, min_len, expected, tmpcwd, app
+):
+    """Test if method create_user and strong passwords mesh"""
     auth = NativeAuthenticator(db=app.db)
     auth.check_common_password = True
     auth.minimum_password_length = min_len
-    user = auth.create_user('johnsnow', password)
+    user = auth.create_user("johnsnow", password)
     assert bool(user) == expected
 
 
-@pytest.mark.parametrize("enable_signup,expected_success", [
-    (True, True),
-    (False, False),
-])
-async def test_create_user_disable(enable_signup, expected_success,
-                                   tmpcwd, app):
-    '''Test method get_or_create_user not create user if signup is disabled'''
+async def test_change_password(tmpcwd, app):
+    auth = NativeAuthenticator(db=app.db)
+    user = auth.create_user("johnsnow", "password")
+    assert user.is_valid_password("password")
+    auth.change_password("johnsnow", "newpassword")
+    assert not user.is_valid_password("password")
+    assert user.is_valid_password("newpassword")
+
+
+async def test_no_change_to_bad_password(tmpcwd, app):
+    """Test that changing password doesn't bypass password requirements"""
+    auth = NativeAuthenticator(db=app.db)
+    auth.check_common_password = True
+    auth.minimum_password_length = 8
+
+    auth.create_user("johnsnow", "ironwood")
+
+    # Can't change password of nonexistent users.
+    assert auth.change_password("samwelltarly", "palanquin") is None
+    assert auth.get_user("johnsnow").is_valid_password("ironwood")
+
+    # Can't change password to something too short.
+    assert auth.change_password("johnsnow", "mummer") is None
+    assert auth.get_user("johnsnow").is_valid_password("ironwood")
+
+    # Can't change password to something too common.
+    assert auth.change_password("johnsnow", "dragon") is None
+    assert auth.get_user("johnsnow").is_valid_password("ironwood")
+
+    # CAN change password to something fulfilling criteria.
+    assert auth.change_password("johnsnow", "Daenerys") is not None
+    assert not auth.get_user("johnsnow").is_valid_password("ironwood")
+    assert auth.get_user("johnsnow").is_valid_password("Daenerys")
+
+
+@pytest.mark.parametrize(
+    "enable_signup,expected_success",
+    [
+        (True, True),
+        (False, False),
+    ],
+)
+async def test_create_user_disable(enable_signup, expected_success, tmpcwd, app):
+    """Test method get_or_create_user not create user if signup is disabled"""
     auth = NativeAuthenticator(db=app.db)
     auth.enable_signup = enable_signup
 
-    user = auth.create_user('johnsnow', 'password')
+    user = auth.create_user("johnsnow", "password")
 
     if expected_success:
-        assert user.username == 'johnsnow'
+        assert user.username == "johnsnow"
     else:
         assert not user
 
 
-@pytest.mark.parametrize("username,password,authorized,expected", [
-    ("name", '123', False, False),
-    ("johnsnow", '123', True, False),
-    ("Snow", 'password', True, False),
-    ("johnsnow", 'password', False, False),
-    ("johnsnow", 'password', True, True),
-])
-async def test_authentication(username, password, authorized, expected,
-                              tmpcwd, app):
-    '''Test if authentication fails with a unexistent user'''
+@pytest.mark.parametrize(
+    "username,password,authorized,expected",
+    [
+        ("name", "123", False, False),
+        ("johnsnow", "123", True, False),
+        ("Snow", "password", True, False),
+        ("johnsnow", "password", False, False),
+        ("johnsnow", "password", True, True),
+    ],
+)
+async def test_authentication(username, password, authorized, expected, tmpcwd, app):
+    """Test if authentication fails with a unexistent user"""
     auth = NativeAuthenticator(db=app.db)
-    auth.create_user('johnsnow', 'password')
+    auth.create_user("johnsnow", "password")
     if authorized:
-        UserInfo.change_authorization(app.db, 'johnsnow')
-    response = await auth.authenticate(app, {'username': username,
-                                             'password': password})
+        UserInfo.change_authorization(app.db, "johnsnow")
+    response = await auth.authenticate(
+        app, {"username": username, "password": password}
+    )
     assert bool(response) == expected
 
 
 async def test_handlers(app):
-    '''Test if all handlers are available on the Authenticator'''
+    """Test if all handlers are available on the Authenticator"""
     auth = NativeAuthenticator(db=app.db)
     handlers = auth.get_handlers(app)
-    assert handlers[0][0] == '/login'
-    assert handlers[1][0] == '/signup'
-    assert handlers[2][0] == '/discard/([^/]*)'
-    assert handlers[3][0] == '/authorize'
-    assert handlers[4][0] == '/authorize/([^/]*)'
-    assert handlers[5][0] == '/confirm/([^/]*)'
-    assert handlers[6][0] == '/change-password'
-    assert handlers[7][0] == '/change-password/([^/]+)'
+    assert handlers[0][0] == "/login"
+    assert handlers[1][0] == "/signup"
+    assert handlers[2][0] == "/discard/([^/]*)"
+    assert handlers[3][0] == "/authorize"
+    assert handlers[4][0] == "/authorize/([^/]*)"
+    assert handlers[5][0] == "/confirm/([^/]*)"
+    assert handlers[6][0] == "/change-password"
+    assert handlers[7][0] == "/change-password/([^/]+)"
 
 
 async def test_add_new_attempt_of_login(tmpcwd, app):
     auth = NativeAuthenticator(db=app.db)
 
     assert not auth.login_attempts
-    auth.add_login_attempt('username')
-    assert auth.login_attempts['username']['count'] == 1
-    auth.add_login_attempt('username')
-    assert auth.login_attempts['username']['count'] == 2
+    auth.add_login_attempt("username")
+    assert auth.login_attempts["username"]["count"] == 1
+    auth.add_login_attempt("username")
+    assert auth.login_attempts["username"]["count"] == 2
 
 
 async def test_authentication_login_count(tmpcwd, app):
     auth = NativeAuthenticator(db=app.db)
-    infos = {'username': 'johnsnow', 'password': 'password'}
-    wrong_infos = {'username': 'johnsnow', 'password': 'wrong_password'}
-    auth.create_user(infos['username'], infos['password'])
-    UserInfo.change_authorization(app.db, 'johnsnow')
+    infos = {"username": "johnsnow", "password": "password"}
+    wrong_infos = {"username": "johnsnow", "password": "wrong_password"}
+    auth.create_user(infos["username"], infos["password"])
+    UserInfo.change_authorization(app.db, "johnsnow")
 
     assert not auth.login_attempts
 
     await auth.authenticate(app, wrong_infos)
-    assert auth.login_attempts['johnsnow']['count'] == 1
+    assert auth.login_attempts["johnsnow"]["count"] == 1
 
     await auth.authenticate(app, wrong_infos)
-    assert auth.login_attempts['johnsnow']['count'] == 2
+    assert auth.login_attempts["johnsnow"]["count"] == 2
 
     await auth.authenticate(app, infos)
-    assert not auth.login_attempts.get('johnsnow')
+    assert not auth.login_attempts.get("johnsnow")
 
 
 async def test_authentication_with_exceed_atempts_of_login(tmpcwd, app):
     auth = NativeAuthenticator(db=app.db)
     auth.allowed_failed_logins = 3
     auth.secs_before_next_try = 10
 
-    infos = {'username': 'johnsnow', 'password': 'wrongpassword'}
-    auth.create_user(infos['username'], 'password')
-    UserInfo.change_authorization(app.db, 'johnsnow')
+    infos = {"username": "johnsnow", "password": "wrongpassword"}
+    auth.create_user(infos["username"], "password")
+    UserInfo.change_authorization(app.db, "johnsnow")
 
     for i in range(3):
         response = await auth.authenticate(app, infos)
         assert not response
 
-    infos['password'] = 'password'
+    infos["password"] = "password"
     response = await auth.authenticate(app, infos)
     assert not response
 
     time.sleep(12)
     response = await auth.authenticate(app, infos)
     assert response
 
 
-async def test_change_password(tmpcwd, app):
-    auth = NativeAuthenticator(db=app.db)
-    user = auth.create_user('johnsnow', 'password')
-    assert user.is_valid_password('password')
-    auth.change_password('johnsnow', 'newpassword')
-    assert not user.is_valid_password('password')
-    assert user.is_valid_password('newpassword')
-
-
 async def test_get_user(tmpcwd, app):
     auth = NativeAuthenticator(db=app.db)
-    auth.create_user('johnsnow', 'password')
+    auth.create_user("johnsnow", "password")
 
     # Getting existing user is successful.
-    assert auth.get_user('johnsnow') is not None
+    assert auth.get_user("johnsnow") is not None
 
     # Getting non-existing user fails.
-    assert auth.get_user('samwelltarly') is None
+    assert auth.get_user("samwelltarly") is None
 
 
 async def test_delete_user(tmpcwd, app):
     auth = NativeAuthenticator(db=app.db)
-    auth.create_user('johnsnow', 'password')
+    auth.create_user("johnsnow", "password")
 
-    user = type('User', (), {'name': 'johnsnow'})
+    user = type("User", (), {"name": "johnsnow"})
     auth.delete_user(user)
 
-    user_info = UserInfo.find(app.db, 'johnsnow')
+    user_info = UserInfo.find(app.db, "johnsnow")
     assert not user_info
 
 
 async def test_import_from_firstuse_dont_delete_db_after(tmpcwd, app):
-    with dbm.open('passwords.dbm', 'c', 0o600) as db:
-        db['user1'] = 'password'
+    with dbm.open("passwords.dbm", "c", 0o600) as db:
+        db["user1"] = "password"
 
     auth = NativeAuthenticator(db=app.db)
     auth.add_data_from_firstuse()
 
     files = os.listdir()
-    assert UserInfo.find(app.db, 'user1')
-    assert ('passwords.dbm' in files) or ('passwords.dbm.db' in files)
+    assert UserInfo.find(app.db, "user1")
+    assert ("passwords.dbm" in files) or ("passwords.dbm.db" in files)
 
 
 async def test_import_from_firstuse_delete_db_after(tmpcwd, app):
-    with dbm.open('passwords.dbm', 'c', 0o600) as db:
-        db['user1'] = 'password'
+    with dbm.open("passwords.dbm", "c", 0o600) as db:
+        db["user1"] = "password"
 
     auth = NativeAuthenticator(db=app.db)
     auth.delete_firstuse_db_after_import = True
 
     auth.add_data_from_firstuse()
     files = os.listdir()
-    assert UserInfo.find(app.db, 'user1')
-    assert ('passwords.dbm' not in files) and ('passwords.dbm.db' not in files)
+    assert UserInfo.find(app.db, "user1")
+    assert ("passwords.dbm" not in files) and ("passwords.dbm.db" not in files)
 
 
-@pytest.mark.parametrize("user,pwd", [
-    ('user1', 'password'),
-    ('user 1', 'somethingelsereallysecure'),
-])
+@pytest.mark.parametrize(
+    "user,pwd",
+    [
+        ("user1", "password"),
+        ("user 1", "somethingelsereallysecure"),
+    ],
+)
 async def test_import_from_firstuse_invalid_password(user, pwd, tmpcwd, app):
-    with dbm.open('passwords.dbm', 'c', 0o600) as db:
+    with dbm.open("passwords.dbm", "c", 0o600) as db:
         db[user] = pwd
 
     auth = NativeAuthenticator(db=app.db)
     auth.check_common_password = True
     with pytest.raises(ValueError):
         auth.add_data_from_firstuse()
 
 
 async def test_secret_key(app):
     auth = NativeAuthenticator(db=app.db)
     auth.ask_email_on_signup = False
-    auth.allow_self_approval_for = '.*@some-domain.com$'
+    auth.allow_self_approval_for = ".*@example.com$"
     auth.secret_key = "short"
 
     with pytest.raises(ValueError):
         auth.setup_self_approval()
 
     auth.secret_key = "very long and kind-of random asdgaisgfjbafksdgasg"
 
     auth.setup_self_approval()
     assert auth.ask_email_on_signup is True
 
 
 async def test_approval_url(app):
     auth = NativeAuthenticator(db=app.db)
-    auth.allow_self_approval_for = '.*@some-domain.com$'
+    auth.allow_self_approval_for = ".*@example.com$"
     auth.secret_key = "very long and kind-of random asdgaisgfjbafksdgasg"
     auth.setup_self_approval()
 
     # confirm that a forged slug cannot be used
     with pytest.raises(ValueError):
-        AuthorizeHandler.validate_slug("foo", auth.secret_key)
+        EmailAuthorizationHandler.validate_slug("foo", auth.secret_key)
 
     # confirm that an expired URL cannot be used
     expiration = datetime.datetime.now(tz.utc) - datetime.timedelta(days=2)
     url = auth.generate_approval_url("somebody", when=expiration)
     slug = url.split("/")[-1]
     with pytest.raises(ValueError):
-        AuthorizeHandler.validate_slug(slug, auth.secret_key)
+        EmailAuthorizationHandler.validate_slug(slug, auth.secret_key)
 
     # confirm that a non-expired, correctly signed URL can be used
     expiration = datetime.datetime.now(tz.utc) + datetime.timedelta(days=2)
     url = auth.generate_approval_url("somebody", when=expiration)
     slug = url.split("/")[-1]
-    out = AuthorizeHandler.validate_slug(slug, auth.secret_key)
+    out = EmailAuthorizationHandler.validate_slug(slug, auth.secret_key)
     assert out["username"] == "somebody"
     assert out["expire"] == expiration
```

### Comparing `jupyterhub-nativeauthenticator-1.0.5/setup.py` & `jupyterhub-nativeauthenticator-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-with open("README.md", "r") as fh:
+with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
-    name='jupyterhub-nativeauthenticator',
-    version='1.0.5',
-    description='JupyterHub Native Authenticator',
+    name="jupyterhub-nativeauthenticator",
+    version="1.1.0",
+    description="JupyterHub Native Authenticator",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/jupyterhub/nativeauthenticator',
-    author='Leticia Portella',
-    author_email='leportella@protonmail.com',
-    license='3 Clause BSD',
+    url="https://github.com/jupyterhub/nativeauthenticator",
+    author="Leticia Portella",
+    author_email="leportella@protonmail.com",
+    license="3 Clause BSD",
     packages=find_packages(),
-    install_requires=['jupyterhub>=1.3', 'bcrypt', 'onetimepass'],
+    install_requires=["jupyterhub>=1.3", "bcrypt", "onetimepass"],
     include_package_data=True,
 )
```

