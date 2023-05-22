# Comparing `tmp/py4web-1.20230521.1.tar.gz` & `tmp/py4web-1.20230521.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230521.1.tar", last modified: Mon May 22 05:36:20 2023, max compression
+gzip compressed data, was "py4web-1.20230521.2.tar", last modified: Mon May 22 06:14:22 2023, max compression
```

## Comparing `py4web-1.20230521.1.tar` & `py4web-1.20230521.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.286200 py4web-1.20230521.1/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230521.1/LICENSE.md
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 05:36:20.286200 py4web-1.20230521.1/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230521.1/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.266206 py4web-1.20230521.1/py4web/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-22 05:35:37.000000 py4web-1.20230521.1/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.278202 py4web-1.20230521.1/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995779 2023-05-22 05:36:07.000000 py4web-1.20230521.1/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-05-22 05:36:07.000000 py4web-1.20230521.1/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4356813 2023-05-22 05:36:08.000000 py4web-1.20230521.1/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-05-22 05:36:07.000000 py4web-1.20230521.1/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-05-22 05:36:07.000000 py4web-1.20230521.1/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1385465 2023-05-22 05:36:08.000000 py4web-1.20230521.1/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.282201 py4web-1.20230521.1/py4web/utils/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    69664 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.286200 py4web-1.20230521.1/py4web/utils/auth_plugins/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2github.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/pam.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/misc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/recaptcha.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230521.1/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.266206 py4web-1.20230521.1/py4web.egg-info/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1830 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/SOURCES.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/dependency_links.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/entry_points.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/requires.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-22 05:36:20.000000 py4web-1.20230521.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-22 05:35:24.000000 py4web-1.20230521.1/pyproject.toml
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-22 05:36:20.286200 py4web-1.20230521.1/setup.cfg
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:36:20.286200 py4web-1.20230521.1/tests/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_action.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_auth.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_cache.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_fixture.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_get_error_snapshot.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_json.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_main.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_session.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_template.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230521.1/tests/test_url.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230521.2/LICENSE.md
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 06:14:22.651144 py4web-1.20230521.2/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230521.2/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.631138 py4web-1.20230521.2/py4web/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-22 06:13:47.000000 py4web-1.20230521.2/py4web/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.643141 py4web-1.20230521.2/py4web/assets/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995779 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  4356813 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  1385465 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app.showcase.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.647143 py4web-1.20230521.2/py4web/utils/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    69608 2023-05-22 05:41:10.000000 py4web-1.20230521.2/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/py4web/utils/auth_plugins/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2discord.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2github.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/pam.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/misc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/recaptcha.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.631138 py4web-1.20230521.2/py4web.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1830 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/entry_points.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/requires.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/top_level.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-22 06:13:31.000000 py4web-1.20230521.2/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-22 06:14:22.655145 py4web-1.20230521.2/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/tests/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_action.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_auth.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_cache.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_fixture.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_get_error_snapshot.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_json.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_main.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_session.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_template.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_url.py
```

### Comparing `py4web-1.20230521.1/LICENSE.md` & `py4web-1.20230521.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/PKG-INFO` & `py4web-1.20230521.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230521.1
+Version: 1.20230521.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230521.1/README.rst` & `py4web-1.20230521.2/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/__init__.py` & `py4web-1.20230521.2/py4web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230521.1"
+__version__ = "1.20230521.2"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._documentation.zip`

 * *Format-specific differences are supported for ZIP archives but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Zip archive data, at least v2.0 to extract, compression method=deflate*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

 * *Files 0% similar despite different names*

```diff
@@ -5811,16 +5811,16 @@
 00016b20: 9439 5bd3 66fc fa0e 0bb3 f07d 431b e169  .9[.f......}C..i
 00016b30: 9eb6 da29 8e76 db97 5620 a9e7 3e13 c373  ...).v..V ..>..s
 00016b40: bb3d b08d d9dc 5f19 22a5 2449 7869 653e  .=...._.".$Ixie>
 00016b50: f907 504b 0304 1400 0000 0800 7595 a756  ..PK........u..V
 00016b60: 6b35 2548 0407 0000 6812 0000 2500 1c00  k5%H....h...%...
 00016b70: 7374 6174 6963 2f65 6e2f 5f73 7461 7469  static/en/_stati
 00016b80: 632f 7370 6869 6e78 5f68 6967 686c 6967  c/sphinx_highlig
-00016b90: 6874 2e6a 7355 5409 0003 ce53 5864 1923  ht.jsUT....SXd.#
-00016ba0: 6864 7578 0b00 0104 e803 0000 04e8 0300  hdux............
+00016b90: 6874 2e6a 7355 5409 0003 ce53 5864 47ff  ht.jsUT....SXdG.
+00016ba0: 6a64 7578 0b00 0104 e803 0000 04e8 0300  jdux............
 00016bb0: 009d 5859 93db 360c 7ef7 af60 d499 54de  ..XY..6.~..`..T.
 00016bc0: b8f2 b67d db8d b7b3 871b 6fe3 d899 95d3  ...}......o.....
 00016bd0: 63da 8e87 9668 8b89 4caa 22e5 63d2 fdef  c....h..L.".c...
 00016be0: 0548 1d94 f668 dacc ac6d 9120 0002 1f80  .H...h...m. ....
 00016bf0: 4f19 9e90 09df 2429 fc69 2e36 a4d0 3ce5  O.....$).i.6..<.
 00016c00: 9a33 45d6 3227 6196 7071 2093 c5bb 2989  .3E.2'a.pq ...).
 00016c10: 6554 6c99 d054 7329 0272 32ec 7985 6244  eTl..Ts).r2.y.bD
@@ -5929,15 +5929,15 @@
 00017280: 6ba6 5b79 36f9 0d6f c57f ffda 061a ce6d  k.[y6..o.......m
 00017290: b565 b9f9 be61 6b5a a4da ef52 ebaa c691  .e...akZ...R....
 000172a0: df2d 012d f1d1 7f68 e221 9d82 634f 483f  .-.-...h.!..cOH?
 000172b0: 442d c8fe 0350 4b03 0414 0000 0008 00aa  D-...PK.........
 000172c0: 99a7 560e c632 5d53 7800 009d 5d01 001b  ..V..2]Sx...]...
 000172d0: 001c 0073 7461 7469 632f 656e 2f5f 7374  ...static/en/_st
 000172e0: 6174 6963 2f6a 7175 6572 792e 6a73 5554  atic/jquery.jsUT
-000172f0: 0900 03bf 5a58 649f 2368 6475 780b 0001  ....ZXd.#hdux...
+000172f0: 0900 03bf 5a58 6447 ff6a 6475 780b 0001  ....ZXdG.jdux...
 00017300: 04e8 0300 0004 e803 0000 ac5b e976 db38  ...........[.v.8
 00017310: 96fe 3f4f 21b1 320a 61c1 b494 7432 27b4  ..?O!.2.a...t2'.
 00017320: 119d 94ed 54d2 9dad 2357 5577 4b4a 1d5a  ....T...#WUwKJ.Z
 00017330: 846c 2632 a990 9097 98aa 67ef ef02 dc45  .l&2......g....E
 00017340: 55aa 67c6 3931 492c 1777 c3dd 001f ec75  U.g.91I,.w.....u
 00017350: 3b9f ffbe 96f1 5de7 fab1 f3d4 1974 d28e  ;.....]......t..
 00017360: 3d67 9df7 2b19 fe75 dc79 19ad 43df 5341  =g..+..u.y..C.SA
@@ -19721,16 +19721,16 @@
 0004d080: f50d 3f84 85bd 9946 0cff ab23 8c59 a914  ..?....F...#.Y..
 0004d090: be66 37a1 0bae fae6 2abe e102 44fc 2f50  .f7.....*...D./P
 0004d0a0: 4b03 0414 0000 0008 00aa 99a7 566c 0ed5  K...........Vl..
 0004d0b0: 2cfd 0500 00c1 1000 0039 001c 0073 7461  ,........9...sta
 0004d0c0: 7469 632f 656e 2f5f 7374 6174 6963 2f5f  tic/en/_static/_
 0004d0d0: 7370 6869 6e78 5f6a 6176 6173 6372 6970  sphinx_javascrip
 0004d0e0: 745f 6672 616d 6577 6f72 6b73 5f63 6f6d  t_frameworks_com
-0004d0f0: 7061 742e 6a73 5554 0900 03bf 5a58 6412  pat.jsUT....ZXd.
-0004d100: 2368 6475 780b 0001 04e8 0300 0004 e803  #hdux...........
+0004d0f0: 7061 742e 6a73 5554 0900 03bf 5a58 6447  pat.jsUT....ZXdG
+0004d100: ff6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 0004d110: 0000 a557 6d6f db36 10fe ee5f 71f3 805a  ...Wmo.6..._q..Z
 0004d120: 4a3c 2a6d bfc5 cb8a 261d 8a0e 7dd9 e2b6  J<*m....&...}...
 0004d130: fbe0 0601 25d1 1653 59d4 48ca 2f6b f2df  ....%..SY.H./k..
 0004d140: 7747 4ab2 9c28 69d0 0941 2c91 f77e cf1d  wGJ..(i..A,..~..
 0004d150: 8fd1 019c a965 c92d 8f65 2eed 164c 2697  .....e.-.e...L&.
 0004d160: 3057 1aae feaa 84de 022f 52a8 8a54 6893  0W......./R..Th.
 0004d170: 282d 0cbb 326c 0007 f887 7ce5 56cb 4566  (-..2l....|.V.Ef
@@ -140722,15 +140722,15 @@
 00225b10: fcfa 0e0b b3f0 7d43 1be1 699e b6da 298e  ......}C..i...).
 00225b20: 76db 9756 20a9 e73e 13c3 73bb 3db0 8dd9  v..V ..>..s.=...
 00225b30: dc5f 1922 a524 4978 6965 3ef9 0750 4b03  ._.".$Ixie>..PK.
 00225b40: 0414 0000 0008 0075 95a7 566b 3525 4804  .......u..Vk5%H.
 00225b50: 0700 0068 1200 0025 001c 0073 7461 7469  ...h...%...stati
 00225b60: 632f 7074 2f5f 7374 6174 6963 2f73 7068  c/pt/_static/sph
 00225b70: 696e 785f 6869 6768 6c69 6768 742e 6a73  inx_highlight.js
-00225b80: 5554 0900 03ce 5358 6419 2368 6475 780b  UT....SXd.#hdux.
+00225b80: 5554 0900 03ce 5358 6447 ff6a 6475 780b  UT....SXdG.jdux.
 00225b90: 0001 04e8 0300 0004 e803 0000 9d58 5993  .............XY.
 00225ba0: db36 0c7e f7af 60d4 9954 deb8 f2b6 7ddb  .6.~..`..T....}.
 00225bb0: 8db7 b387 1b6f e3d8 9995 d363 da8e 8796  .....o.....c....
 00225bc0: 688b 894c aa22 e563 d2fd ef05 481d 94f6  h..L.".c....H...
 00225bd0: 68da ccac 6d91 2000 021f 804f 199e 9009  h...m. ....O....
 00225be0: df24 29fc 692e 36a4 d03c e59a 3345 d632  .$).i.6..<..3E.2
 00225bf0: 2761 9670 7120 93c5 bb29 8965 546c 99d0  'a.pq ...).eTl..
@@ -140840,15 +140840,15 @@
 00226270: f90d 6fc5 7fff da06 1ace 6db5 65b9 f9be  ..o.......m.e...
 00226280: 616b 5aa4 daef 52eb aac6 91df 2d01 2df1  akZ...R.....-.-.
 00226290: d17f 68e2 219d 8263 4f48 3f44 2dc8 fe03  ..h.!..cOH?D-...
 002262a0: 504b 0304 1400 0000 0800 ac99 a756 0ec6  PK...........V..
 002262b0: 325d 5378 0000 9d5d 0100 1b00 1c00 7374  2]Sx...]......st
 002262c0: 6174 6963 2f70 742f 5f73 7461 7469 632f  atic/pt/_static/
 002262d0: 6a71 7565 7279 2e6a 7355 5409 0003 c45a  jquery.jsUT....Z
-002262e0: 5864 a023 6864 7578 0b00 0104 e803 0000  Xd.#hdux........
+002262e0: 5864 47ff 6a64 7578 0b00 0104 e803 0000  XdG.jdux........
 002262f0: 04e8 0300 00ac 5be9 76db 3896 fe3f 4f21  ......[.v.8..?O!
 00226300: b132 0a61 c1b4 9474 3227 b411 9d94 ed54  .2.a...t2'.....T
 00226310: d29d ad23 5755 774b 4a1d 5a84 6c26 32a9  ...#WUwKJ.Z.l&2.
 00226320: 9090 9798 aa67 efef 02dc 4555 aa67 c639  .....g....EU.g.9
 00226330: 3149 2c17 77c3 dd00 1fec 753b 9fff be96  1I,.w.....u;....
 00226340: f15d e7fa b1f3 d419 74d2 8e3d 679d f72b  .]......t..=g..+
 00226350: 19fe 75dc 7919 ad43 df53 4114 76bc d0ef  ..u.y..C.SA.v...
@@ -154903,15 +154903,15 @@
 0025d160: 8485 bd99 460c ffab 238c 59a9 14be 6637  ....F...#.Y...f7
 0025d170: a10b aefa e62a bee1 0244 fc2f 504b 0304  .....*...D./PK..
 0025d180: 1400 0000 0800 ac99 a756 6c0e d52c fd05  .........Vl..,..
 0025d190: 0000 c110 0000 3900 1c00 7374 6174 6963  ......9...static
 0025d1a0: 2f70 742f 5f73 7461 7469 632f 5f73 7068  /pt/_static/_sph
 0025d1b0: 696e 785f 6a61 7661 7363 7269 7074 5f66  inx_javascript_f
 0025d1c0: 7261 6d65 776f 726b 735f 636f 6d70 6174  rameworks_compat
-0025d1d0: 2e6a 7355 5409 0003 c45a 5864 1223 6864  .jsUT....ZXd.#hd
+0025d1d0: 2e6a 7355 5409 0003 c45a 5864 47ff 6a64  .jsUT....ZXdG.jd
 0025d1e0: 7578 0b00 0104 e803 0000 04e8 0300 00a5  ux..............
 0025d1f0: 576d 6fdb 3610 feee 5f71 f380 5a4a 3c2a  Wmo.6..._q..ZJ<*
 0025d200: 6dbf c5cb 8a26 1d8a 0e7d d9e2 b6fb e006  m....&...}......
 0025d210: 0125 d116 5359 d448 ca2f 6bf2 df77 474a  .%..SY.H./k..wGJ
 0025d220: b29c 2869 d009 412c 91f7 7ecf 1d8f d101  ..(i..A,..~.....
 0025d230: 9ca9 65c9 2d8f 652e ed16 4c26 9730 571a  ..e.-.e...L&.0W.
 0025d240: aefe aa84 de02 2f52 a88a 5468 9328 2d0c  ....../R..Th.(-.
```

#### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._documentation.zip`

```diff
@@ -5811,16 +5811,16 @@
 00016b20: 9439 5bd3 66fc fa0e 0bb3 f07d 431b e169  .9[.f......}C..i
 00016b30: 9eb6 da29 8e76 db97 5620 a9e7 3e13 c373  ...).v..V ..>..s
 00016b40: bb3d b08d d9dc 5f19 22a5 2449 7869 653e  .=...._.".$Ixie>
 00016b50: f907 504b 0304 1400 0000 0800 7595 a756  ..PK........u..V
 00016b60: 6b35 2548 0407 0000 6812 0000 2500 1c00  k5%H....h...%...
 00016b70: 7374 6174 6963 2f65 6e2f 5f73 7461 7469  static/en/_stati
 00016b80: 632f 7370 6869 6e78 5f68 6967 686c 6967  c/sphinx_highlig
-00016b90: 6874 2e6a 7355 5409 0003 ce53 5864 1923  ht.jsUT....SXd.#
-00016ba0: 6864 7578 0b00 0104 e803 0000 04e8 0300  hdux............
+00016b90: 6874 2e6a 7355 5409 0003 ce53 5864 47ff  ht.jsUT....SXdG.
+00016ba0: 6a64 7578 0b00 0104 e803 0000 04e8 0300  jdux............
 00016bb0: 009d 5859 93db 360c 7ef7 af60 d499 54de  ..XY..6.~..`..T.
 00016bc0: b8f2 b67d db8d b7b3 871b 6fe3 d899 95d3  ...}......o.....
 00016bd0: 63da 8e87 9668 8b89 4caa 22e5 63d2 fdef  c....h..L.".c...
 00016be0: 0548 1d94 f668 dacc ac6d 9120 0002 1f80  .H...h...m. ....
 00016bf0: 4f19 9e90 09df 2429 fc69 2e36 a4d0 3ce5  O.....$).i.6..<.
 00016c00: 9a33 45d6 3227 6196 7071 2093 c5bb 2989  .3E.2'a.pq ...).
 00016c10: 6554 6c99 d054 7329 0272 32ec 7985 6244  eTl..Ts).r2.y.bD
@@ -5929,15 +5929,15 @@
 00017280: 6ba6 5b79 36f9 0d6f c57f ffda 061a ce6d  k.[y6..o.......m
 00017290: b565 b9f9 be61 6b5a a4da ef52 ebaa c691  .e...akZ...R....
 000172a0: df2d 012d f1d1 7f68 e221 9d82 634f 483f  .-.-...h.!..cOH?
 000172b0: 442d c8fe 0350 4b03 0414 0000 0008 00aa  D-...PK.........
 000172c0: 99a7 560e c632 5d53 7800 009d 5d01 001b  ..V..2]Sx...]...
 000172d0: 001c 0073 7461 7469 632f 656e 2f5f 7374  ...static/en/_st
 000172e0: 6174 6963 2f6a 7175 6572 792e 6a73 5554  atic/jquery.jsUT
-000172f0: 0900 03bf 5a58 649f 2368 6475 780b 0001  ....ZXd.#hdux...
+000172f0: 0900 03bf 5a58 6447 ff6a 6475 780b 0001  ....ZXdG.jdux...
 00017300: 04e8 0300 0004 e803 0000 ac5b e976 db38  ...........[.v.8
 00017310: 96fe 3f4f 21b1 320a 61c1 b494 7432 27b4  ..?O!.2.a...t2'.
 00017320: 119d 94ed 54d2 9dad 2357 5577 4b4a 1d5a  ....T...#WUwKJ.Z
 00017330: 846c 2632 a990 9097 98aa 67ef ef02 dc45  .l&2......g....E
 00017340: 55aa 67c6 3931 492c 1777 c3dd 001f ec75  U.g.91I,.w.....u
 00017350: 3b9f ffbe 96f1 5de7 fab1 f3d4 1974 d28e  ;.....]......t..
 00017360: 3d67 9df7 2b19 fe75 dc79 19ad 43df 5341  =g..+..u.y..C.SA
@@ -19721,16 +19721,16 @@
 0004d080: f50d 3f84 85bd 9946 0cff ab23 8c59 a914  ..?....F...#.Y..
 0004d090: be66 37a1 0bae fae6 2abe e102 44fc 2f50  .f7.....*...D./P
 0004d0a0: 4b03 0414 0000 0008 00aa 99a7 566c 0ed5  K...........Vl..
 0004d0b0: 2cfd 0500 00c1 1000 0039 001c 0073 7461  ,........9...sta
 0004d0c0: 7469 632f 656e 2f5f 7374 6174 6963 2f5f  tic/en/_static/_
 0004d0d0: 7370 6869 6e78 5f6a 6176 6173 6372 6970  sphinx_javascrip
 0004d0e0: 745f 6672 616d 6577 6f72 6b73 5f63 6f6d  t_frameworks_com
-0004d0f0: 7061 742e 6a73 5554 0900 03bf 5a58 6412  pat.jsUT....ZXd.
-0004d100: 2368 6475 780b 0001 04e8 0300 0004 e803  #hdux...........
+0004d0f0: 7061 742e 6a73 5554 0900 03bf 5a58 6447  pat.jsUT....ZXdG
+0004d100: ff6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 0004d110: 0000 a557 6d6f db36 10fe ee5f 71f3 805a  ...Wmo.6..._q..Z
 0004d120: 4a3c 2a6d bfc5 cb8a 261d 8a0e 7dd9 e2b6  J<*m....&...}...
 0004d130: fbe0 0601 25d1 1653 59d4 48ca 2f6b f2df  ....%..SY.H./k..
 0004d140: 7747 4ab2 9c28 69d0 0941 2c91 f77e cf1d  wGJ..(i..A,..~..
 0004d150: 8fd1 019c a965 c92d 8f65 2eed 164c 2697  .....e.-.e...L&.
 0004d160: 3057 1aae feaa 84de 022f 52a8 8a54 6893  0W......./R..Th.
 0004d170: 282d 0cbb 326c 0007 f887 7ce5 56cb 4566  (-..2l....|.V.Ef
@@ -140722,15 +140722,15 @@
 00225b10: fcfa 0e0b b3f0 7d43 1be1 699e b6da 298e  ......}C..i...).
 00225b20: 76db 9756 20a9 e73e 13c3 73bb 3db0 8dd9  v..V ..>..s.=...
 00225b30: dc5f 1922 a524 4978 6965 3ef9 0750 4b03  ._.".$Ixie>..PK.
 00225b40: 0414 0000 0008 0075 95a7 566b 3525 4804  .......u..Vk5%H.
 00225b50: 0700 0068 1200 0025 001c 0073 7461 7469  ...h...%...stati
 00225b60: 632f 7074 2f5f 7374 6174 6963 2f73 7068  c/pt/_static/sph
 00225b70: 696e 785f 6869 6768 6c69 6768 742e 6a73  inx_highlight.js
-00225b80: 5554 0900 03ce 5358 6419 2368 6475 780b  UT....SXd.#hdux.
+00225b80: 5554 0900 03ce 5358 6447 ff6a 6475 780b  UT....SXdG.jdux.
 00225b90: 0001 04e8 0300 0004 e803 0000 9d58 5993  .............XY.
 00225ba0: db36 0c7e f7af 60d4 9954 deb8 f2b6 7ddb  .6.~..`..T....}.
 00225bb0: 8db7 b387 1b6f e3d8 9995 d363 da8e 8796  .....o.....c....
 00225bc0: 688b 894c aa22 e563 d2fd ef05 481d 94f6  h..L.".c....H...
 00225bd0: 68da ccac 6d91 2000 021f 804f 199e 9009  h...m. ....O....
 00225be0: df24 29fc 692e 36a4 d03c e59a 3345 d632  .$).i.6..<..3E.2
 00225bf0: 2761 9670 7120 93c5 bb29 8965 546c 99d0  'a.pq ...).eTl..
@@ -140840,15 +140840,15 @@
 00226270: f90d 6fc5 7fff da06 1ace 6db5 65b9 f9be  ..o.......m.e...
 00226280: 616b 5aa4 daef 52eb aac6 91df 2d01 2df1  akZ...R.....-.-.
 00226290: d17f 68e2 219d 8263 4f48 3f44 2dc8 fe03  ..h.!..cOH?D-...
 002262a0: 504b 0304 1400 0000 0800 ac99 a756 0ec6  PK...........V..
 002262b0: 325d 5378 0000 9d5d 0100 1b00 1c00 7374  2]Sx...]......st
 002262c0: 6174 6963 2f70 742f 5f73 7461 7469 632f  atic/pt/_static/
 002262d0: 6a71 7565 7279 2e6a 7355 5409 0003 c45a  jquery.jsUT....Z
-002262e0: 5864 a023 6864 7578 0b00 0104 e803 0000  Xd.#hdux........
+002262e0: 5864 47ff 6a64 7578 0b00 0104 e803 0000  XdG.jdux........
 002262f0: 04e8 0300 00ac 5be9 76db 3896 fe3f 4f21  ......[.v.8..?O!
 00226300: b132 0a61 c1b4 9474 3227 b411 9d94 ed54  .2.a...t2'.....T
 00226310: d29d ad23 5755 774b 4a1d 5a84 6c26 32a9  ...#WUwKJ.Z.l&2.
 00226320: 9090 9798 aa67 efef 02dc 4555 aa67 c639  .....g....EU.g.9
 00226330: 3149 2c17 77c3 dd00 1fec 753b 9fff be96  1I,.w.....u;....
 00226340: f15d e7fa b1f3 d419 74d2 8e3d 679d f72b  .]......t..=g..+
 00226350: 19fe 75dc 7919 ad43 df53 4114 76bc d0ef  ..u.y..C.SA.v...
@@ -154903,15 +154903,15 @@
 0025d160: 8485 bd99 460c ffab 238c 59a9 14be 6637  ....F...#.Y...f7
 0025d170: a10b aefa e62a bee1 0244 fc2f 504b 0304  .....*...D./PK..
 0025d180: 1400 0000 0800 ac99 a756 6c0e d52c fd05  .........Vl..,..
 0025d190: 0000 c110 0000 3900 1c00 7374 6174 6963  ......9...static
 0025d1a0: 2f70 742f 5f73 7461 7469 632f 5f73 7068  /pt/_static/_sph
 0025d1b0: 696e 785f 6a61 7661 7363 7269 7074 5f66  inx_javascript_f
 0025d1c0: 7261 6d65 776f 726b 735f 636f 6d70 6174  rameworks_compat
-0025d1d0: 2e6a 7355 5409 0003 c45a 5864 1223 6864  .jsUT....ZXd.#hd
+0025d1d0: 2e6a 7355 5409 0003 c45a 5864 47ff 6a64  .jsUT....ZXdG.jd
 0025d1e0: 7578 0b00 0104 e803 0000 04e8 0300 00a5  ux..............
 0025d1f0: 576d 6fdb 3610 feee 5f71 f380 5a4a 3c2a  Wmo.6..._q..ZJ<*
 0025d200: 6dbf c5cb 8a26 1d8a 0e7d d9e2 b6fb e006  m....&...}......
 0025d210: 0125 d116 5359 d448 ca2f 6bf2 df77 474a  .%..SY.H./k..wGJ
 0025d220: b29c 2869 d009 412c 91f7 7ecf 1d8f d101  ..(i..A,..~.....
 0025d230: 9ca9 65c9 2d8f 652e ed16 4c26 9730 571a  ..e.-.e...L&.0W.
 0025d240: aefe aa84 de02 2f52 a88a 5468 9328 2d0c  ....../R..Th.(-.
```

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app.showcase.zip`

 * *Format-specific differences are supported for ZIP archives but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Zip archive data, at least v2.0 to extract, compression method=deflate*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

 * *Files 0% similar despite different names*

```diff
@@ -6278,15 +6278,15 @@
 00018850: e38d 6f55 9654 9fa8 7b6c 692c 8f97 fc53  ..oU.T..{li,...S
 00018860: e758 11d4 1eb6 3c3d 6fe3 1ade bda9 2d65  .X....<=o.....-e
 00018870: c30d 3b17 39fd ff05 504b 0304 0a00 0000  ..;.9...PK......
 00018880: 0000 f68c a756 0000 0000 0000 0000 0000  .....V..........
 00018890: 0000 2900 1c00 7374 6174 6963 2f63 6f6d  ..)...static/com
 000188a0: 706f 6e65 6e74 732f 7374 6172 7261 7465  ponents/starrate
 000188b0: 722f 7374 6172 7261 7465 722e 6373 7355  r/starrater.cssU
-000188c0: 5409 0003 d044 5864 07a5 5d64 7578 0b00  T....DXd..]dux..
+000188c0: 5409 0003 d044 5864 48ff 6a64 7578 0b00  T....DXdH.jdux..
 000188d0: 0104 e803 0000 04e8 0300 0050 4b03 0414  ...........PK...
 000188e0: 0000 0008 00f6 8ca7 564d ceb8 9b2e 0600  ........VM......
 000188f0: 0017 1d00 001d 001c 0073 7461 7469 632f  .........static/
 00018900: 636f 6d70 6f6e 656e 7473 2f6d 7461 626c  components/mtabl
 00018910: 652e 6874 6d6c 5554 0900 03d0 4458 64a4  e.htmlUT....DXd.
 00018920: fe6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 00018930: 0000 bd59 db6e e336 107d cf57 3002 766d  ...Y.n.6.}.W0.vm
@@ -26494,15 +26494,15 @@
 000677d0: 3c9e ab90 3a87 8aa0 79bf e5e9 911b 56ff  <...:...y.....V.
 000677e0: fa8d 6d29 1bee d9a9 c8e9 ff1f 504b 0304  ..m)........PK..
 000677f0: 0a00 0000 0000 f68c a756 0000 0000 0000  .........V......
 00067800: 0000 0000 0000 2f00 1c00 7374 6174 6963  ....../...static
 00067810: 2f63 6f6d 706f 6e65 6e74 732d 6275 6c6d  /components-bulm
 00067820: 612f 7374 6172 7261 7465 722f 7374 6172  a/starrater/star
 00067830: 7261 7465 722e 6373 7355 5409 0003 d044  rater.cssUT....D
-00067840: 5864 07a5 5d64 7578 0b00 0104 e803 0000  Xd..]dux........
+00067840: 5864 48ff 6a64 7578 0b00 0104 e803 0000  XdH.jdux........
 00067850: 04e8 0300 0050 4b03 0414 0000 0008 00f6  .....PK.........
 00067860: 8ca7 564d ceb8 9b2e 0600 0017 1d00 0023  ..VM...........#
 00067870: 001c 0073 7461 7469 632f 636f 6d70 6f6e  ...static/compon
 00067880: 656e 7473 2d62 756c 6d61 2f6d 7461 626c  ents-bulma/mtabl
 00067890: 652e 6874 6d6c 5554 0900 03d0 4458 64a4  e.htmlUT....DXd.
 000678a0: fe6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 000678b0: 0000 bd59 db6e e336 107d cf57 3002 766d  ...Y.n.6.}.W0.vm
```

#### Comparing `py4web-1.20230521.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230521.2/py4web/assets/py4web.app.showcase.zip`

```diff
@@ -6278,15 +6278,15 @@
 00018850: e38d 6f55 9654 9fa8 7b6c 692c 8f97 fc53  ..oU.T..{li,...S
 00018860: e758 11d4 1eb6 3c3d 6fe3 1ade bda9 2d65  .X....<=o.....-e
 00018870: c30d 3b17 39fd ff05 504b 0304 0a00 0000  ..;.9...PK......
 00018880: 0000 f68c a756 0000 0000 0000 0000 0000  .....V..........
 00018890: 0000 2900 1c00 7374 6174 6963 2f63 6f6d  ..)...static/com
 000188a0: 706f 6e65 6e74 732f 7374 6172 7261 7465  ponents/starrate
 000188b0: 722f 7374 6172 7261 7465 722e 6373 7355  r/starrater.cssU
-000188c0: 5409 0003 d044 5864 07a5 5d64 7578 0b00  T....DXd..]dux..
+000188c0: 5409 0003 d044 5864 48ff 6a64 7578 0b00  T....DXdH.jdux..
 000188d0: 0104 e803 0000 04e8 0300 0050 4b03 0414  ...........PK...
 000188e0: 0000 0008 00f6 8ca7 564d ceb8 9b2e 0600  ........VM......
 000188f0: 0017 1d00 001d 001c 0073 7461 7469 632f  .........static/
 00018900: 636f 6d70 6f6e 656e 7473 2f6d 7461 626c  components/mtabl
 00018910: 652e 6874 6d6c 5554 0900 03d0 4458 64a4  e.htmlUT....DXd.
 00018920: fe6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 00018930: 0000 bd59 db6e e336 107d cf57 3002 766d  ...Y.n.6.}.W0.vm
@@ -26494,15 +26494,15 @@
 000677d0: 3c9e ab90 3a87 8aa0 79bf e5e9 911b 56ff  <...:...y.....V.
 000677e0: fa8d 6d29 1bee d9a9 c8e9 ff1f 504b 0304  ..m)........PK..
 000677f0: 0a00 0000 0000 f68c a756 0000 0000 0000  .........V......
 00067800: 0000 0000 0000 2f00 1c00 7374 6174 6963  ....../...static
 00067810: 2f63 6f6d 706f 6e65 6e74 732d 6275 6c6d  /components-bulm
 00067820: 612f 7374 6172 7261 7465 722f 7374 6172  a/starrater/star
 00067830: 7261 7465 722e 6373 7355 5409 0003 d044  rater.cssUT....D
-00067840: 5864 07a5 5d64 7578 0b00 0104 e803 0000  Xd..]dux........
+00067840: 5864 48ff 6a64 7578 0b00 0104 e803 0000  XdH.jdux........
 00067850: 04e8 0300 0050 4b03 0414 0000 0008 00f6  .....PK.........
 00067860: 8ca7 564d ceb8 9b2e 0600 0017 1d00 0023  ..VM...........#
 00067870: 001c 0073 7461 7469 632f 636f 6d70 6f6e  ...static/compon
 00067880: 656e 7473 2d62 756c 6d61 2f6d 7461 626c  ents-bulma/mtabl
 00067890: 652e 6874 6d6c 5554 0900 03d0 4458 64a4  e.htmlUT....DXd.
 000678a0: fe6a 6475 780b 0001 04e8 0300 0004 e803  .jdux...........
 000678b0: 0000 bd59 db6e e336 107d cf57 3002 766d  ...Y.n.6.}.W0.vm
```

### Comparing `py4web-1.20230521.1/py4web/core.py` & `py4web-1.20230521.2/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/server_adapters.py` & `py4web-1.20230521.2/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth.py` & `py4web-1.20230521.2/py4web/utils/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,30 +729,28 @@
         if check and CRYPT()(password)[0] != user.get("password"):
             return {
                 "errors": {"password": self.param.messages["errors"].get("invalid")}
             }
         return (
             db(db.auth_user.id == user.get("id"))
             .validate_and_update(email=new_email)
-            .as_dict()
         )
 
     def update_profile(self, user, **fields):
         db = self.db
         errors = {
             k: self.param.messages["errors"].get("invalid")
             for k in fields
             if k not in db.auth_user.fields or not db.auth_user[k].writable
         }
         if errors:
             return {"errors": errors}
         return (
             db(db.auth_user.id == user.get("id"))
             .validate_and_update(**fields)
-            .as_dict()
         )
 
     def gdpr_unsubscribe(self, user, send=True):
         """GDPR unsubscribe means we delete first_name, last_name,
         then replace email with hash of the actual email and notify the user.
 
         Essentially we erase the user info yet retain the ability to verify
@@ -1150,15 +1148,15 @@
             return AuthAPI.get_model(defaultAuthFunction=auth.form_source.register)
 
         payload = request.POST if (request.json is None) else request.json
 
         if payload is None:
             return auth._error(auth.param.messages["errors"].get("no_post_payload"))
         auth.get_or_delete_existing_unverified_account(payload.get("email"))
-        return auth.register(payload, send=True).as_dict()
+        return auth.register(payload, send=True)
 
     @staticmethod
     @api_wrapper
     def login(auth):
         if AuthAPI.model_request("login"):
             return AuthAPI.get_model(defaultAuthFunction=auth.form_source.login)
```

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230521.2/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/cors.py` & `py4web-1.20230521.2/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/dbstore.py` & `py4web-1.20230521.2/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/downloader.py` & `py4web-1.20230521.2/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/factories.py` & `py4web-1.20230521.2/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/form.py` & `py4web-1.20230521.2/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/grid.py` & `py4web-1.20230521.2/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/jsonrpc.py` & `py4web-1.20230521.2/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/mailer.py` & `py4web-1.20230521.2/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/misc.py` & `py4web-1.20230521.2/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/populate.py` & `py4web-1.20230521.2/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/publisher.py` & `py4web-1.20230521.2/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/recaptcha.py` & `py4web-1.20230521.2/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/security.py` & `py4web-1.20230521.2/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web/utils/url_signer.py` & `py4web-1.20230521.2/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/py4web.egg-info/PKG-INFO` & `py4web-1.20230521.2/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230521.1
+Version: 1.20230521.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230521.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20230521.2/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/pyproject.toml` & `py4web-1.20230521.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20230521.1"
+version = "1.20230521.2"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
@@ -22,15 +22,15 @@
         "requests",
         "threadsafevariable >= 20230507.1",
         "pyjwt >= 2.0.1",
         "pycryptodome",
         "pluralize >= 20230507.1",
         "rocket3 >= 20230507.1",
         "yatl >= 20230507.3",
-        "pydal >= 20230511.1",
+        "pydal >= 20230521.1",
         "watchgod >= 0.6",
     ]
 
 [tool.setuptools]    
 packages = ["py4web", "py4web.utils", "py4web.utils.auth_plugins",]
 
 [tool.setuptools.package-data]
```

### Comparing `py4web-1.20230521.1/tests/test_action.py` & `py4web-1.20230521.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_auth.py` & `py4web-1.20230521.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_cache.py` & `py4web-1.20230521.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_fixture.py` & `py4web-1.20230521.2/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_form.py` & `py4web-1.20230521.2/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_get_error_snapshot.py` & `py4web-1.20230521.2/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_json.py` & `py4web-1.20230521.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_main.py` & `py4web-1.20230521.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_session.py` & `py4web-1.20230521.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.1/tests/test_tags.py` & `py4web-1.20230521.2/tests/test_tags.py`

 * *Files identical despite different names*

