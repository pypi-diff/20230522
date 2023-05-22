# Comparing `tmp/pytest_httpserver-1.0.7.tar.gz` & `tmp/pytest_httpserver-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httpserver-1.0.7.tar", max compression
+gzip compressed data, was "pytest_httpserver-1.0.8.tar", max compression
```

## Comparing `pytest_httpserver-1.0.7.tar` & `pytest_httpserver-1.0.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11390 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/CHANGES.rst
--rw-r--r--   0        0        0     3225 2023-05-16 18:58:37.762110 pytest_httpserver-1.0.7/CONTRIBUTION.md
--rw-r--r--   0        0        0     1069 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/LICENSE
--rw-r--r--   0        0        0     4780 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/README.md
--rw-r--r--   0        0        0      615 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/doc/Makefile
--rw-r--r--   0        0        0        0 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/doc/_static/.placeholder
--rw-r--r--   0        0        0     1689 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/doc/api.rst
--rw-r--r--   0        0        0     8752 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/doc/background.rst
--rw-r--r--   0        0        0       42 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.7/doc/changes.rst
--rw-r--r--   0        0        0     5856 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/doc/conf.py
--rw-r--r--   0        0        0     2420 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/doc/fixtures.rst
--rw-r--r--   0        0        0      107 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/doc/guide.rst
--rw-r--r--   0        0        0    18202 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.7/doc/howto.rst
--rw-r--r--   0        0        0     1312 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.7/doc/index.rst
--rw-r--r--   0        0        0    17789 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.7/doc/tutorial.rst
--rw-r--r--   0        0        0     2229 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.7/doc/upgrade.rst
--rwxr-xr-x   0        0        0      391 2023-02-03 07:55:52.748134 pytest_httpserver-1.0.7/example.py
--rw-r--r--   0        0        0     1331 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.7/example_pytest.py
--rw-r--r--   0        0        0     2127 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      835 2023-01-18 22:01:30.861852 pytest_httpserver-1.0.7/pytest_httpserver/__init__.py
--rw-r--r--   0        0        0     7214 2023-02-03 07:55:52.829130 pytest_httpserver-1.0.7/pytest_httpserver/blocking_httpserver.py
--rw-r--r--   0        0        0    49366 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/pytest_httpserver/httpserver.py
--rw-r--r--   0        0        0        0 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.7/pytest_httpserver/py.typed
--rw-r--r--   0        0        0     2333 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/pytest_httpserver/pytest_plugin.py
--rw-r--r--   0        0        0      603 2023-01-18 22:01:30.863852 pytest_httpserver-1.0.7/tests/assets/Makefile
--rw-r--r--   0        0        0      179 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/README
--rw-r--r--   0        0        0      194 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.cnf
--rw-r--r--   0        0        0     1350 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.crt
--rw-r--r--   0        0        0     1679 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.key
--rw-r--r--   0        0        0       17 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.srl
--rw-r--r--   0        0        0      198 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.cnf
--rw-r--r--   0        0        0     1688 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.crt
--rw-r--r--   0        0        0     1078 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.csr
--rw-r--r--   0        0        0     1704 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.key
--rw-r--r--   0        0        0      200 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/v3.ext
--rw-r--r--   0        0        0      593 2023-02-03 07:55:52.757134 pytest_httpserver-1.0.7/tests/conftest.py
--rw-r--r--   0        0        0     1849 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_blocking_httpserver.py
--rw-r--r--   0        0        0      129 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_query_params1.py
--rw-r--r--   0        0        0      165 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_query_params2.py
--rw-r--r--   0        0        0     1495 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_authorization_headers.py
--rw-r--r--   0        0        0      750 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_case_insensitive_matcher.py
--rw-r--r--   0        0        0      369 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_check.py
--rw-r--r--   0        0        0     1160 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_check_handler_errors.py
--rw-r--r--   0        0        0      360 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_custom_handler.py
--rw-r--r--   0        0        0      780 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_header_value_matcher.py
--rw-r--r--   0        0        0      347 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_json_matcher.py
--rw-r--r--   0        0        0      357 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_dict.py
--rw-r--r--   0        0        0       99 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_never_do_this.py
--rw-r--r--   0        0        0       98 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_proper_use.py
--rw-r--r--   0        0        0      187 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_regexp.py
--rw-r--r--   0        0        0      235 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_timeout_requests.py
--rw-r--r--   0        0        0      390 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_url_matcher.py
--rw-r--r--   0        0        0      788 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_wait_success.py
--rw-r--r--   0        0        0     3481 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_blocking_httpserver.py
--rw-r--r--   0        0        0     2557 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.7/tests/test_handler_errors.py
--rw-r--r--   0        0        0     4280 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_headers.py
--rw-r--r--   0        0        0      567 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_ip_protocols.py
--rw-r--r--   0        0        0     1864 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.7/tests/test_json_matcher.py
--rw-r--r--   0        0        0     3309 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_mixed.py
--rw-r--r--   0        0        0     1817 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.7/tests/test_oneshot.py
--rw-r--r--   0        0        0     1675 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.7/tests/test_ordered.py
--rw-r--r--   0        0        0     1077 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_parse_qs.py
--rw-r--r--   0        0        0     4122 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_permanent.py
--rw-r--r--   0        0        0     1194 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.7/tests/test_port_changing.py
--rw-r--r--   0        0        0     1488 2023-01-18 22:01:30.866852 pytest_httpserver-1.0.7/tests/test_querymatcher.py
--rw-r--r--   0        0        0     1355 2023-02-03 07:55:52.798132 pytest_httpserver-1.0.7/tests/test_querystring.py
--rw-r--r--   0        0        0     6401 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_release.py
--rw-r--r--   0        0        0     1202 2023-02-03 07:55:52.799132 pytest_httpserver-1.0.7/tests/test_ssl.py
--rw-r--r--   0        0        0     1875 2023-02-03 07:55:52.818131 pytest_httpserver-1.0.7/tests/test_urimatch.py
--rw-r--r--   0        0        0     3122 2023-02-03 07:55:52.851129 pytest_httpserver-1.0.7/tests/test_wait.py
--rw-r--r--   0        0        0      122 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/test_with_statement.py
--rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.7/setup.py
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11570 2023-05-22 18:35:22.853064 pytest_httpserver-1.0.8/CHANGES.rst
+-rw-r--r--   0        0        0     3225 2023-05-16 18:58:37.762110 pytest_httpserver-1.0.8/CONTRIBUTION.md
+-rw-r--r--   0        0        0     1069 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.8/LICENSE
+-rw-r--r--   0        0        0     4780 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.8/README.md
+-rw-r--r--   0        0        0      615 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.8/doc/Makefile
+-rw-r--r--   0        0        0        0 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/doc/_static/.placeholder
+-rw-r--r--   0        0        0     1689 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.8/doc/api.rst
+-rw-r--r--   0        0        0     8752 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.8/doc/background.rst
+-rw-r--r--   0        0        0       42 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.8/doc/changes.rst
+-rw-r--r--   0        0        0     5856 2023-05-22 18:35:22.853064 pytest_httpserver-1.0.8/doc/conf.py
+-rw-r--r--   0        0        0     2420 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.8/doc/fixtures.rst
+-rw-r--r--   0        0        0      107 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.8/doc/guide.rst
+-rw-r--r--   0        0        0    18202 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.8/doc/howto.rst
+-rw-r--r--   0        0        0     1312 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.8/doc/index.rst
+-rw-r--r--   0        0        0    17789 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.8/doc/tutorial.rst
+-rw-r--r--   0        0        0     2229 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.8/doc/upgrade.rst
+-rwxr-xr-x   0        0        0      391 2023-02-03 07:55:52.748134 pytest_httpserver-1.0.8/example.py
+-rw-r--r--   0        0        0     1331 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.8/example_pytest.py
+-rw-r--r--   0        0        0     2127 2023-05-22 18:35:22.853064 pytest_httpserver-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      835 2023-01-18 22:01:30.861852 pytest_httpserver-1.0.8/pytest_httpserver/__init__.py
+-rw-r--r--   0        0        0     7214 2023-02-03 07:55:52.829130 pytest_httpserver-1.0.8/pytest_httpserver/blocking_httpserver.py
+-rw-r--r--   0        0        0    49366 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/pytest_httpserver/httpserver.py
+-rw-r--r--   0        0        0        0 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.8/pytest_httpserver/py.typed
+-rw-r--r--   0        0        0     2333 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/pytest_httpserver/pytest_plugin.py
+-rw-r--r--   0        0        0      603 2023-01-18 22:01:30.863852 pytest_httpserver-1.0.8/tests/assets/Makefile
+-rw-r--r--   0        0        0      179 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/README
+-rw-r--r--   0        0        0      194 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/rootCA.cnf
+-rw-r--r--   0        0        0     1350 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/rootCA.crt
+-rw-r--r--   0        0        0     1679 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/rootCA.key
+-rw-r--r--   0        0        0       17 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/rootCA.srl
+-rw-r--r--   0        0        0      198 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/server.cnf
+-rw-r--r--   0        0        0     1688 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/server.crt
+-rw-r--r--   0        0        0     1078 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/server.csr
+-rw-r--r--   0        0        0     1704 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/server.key
+-rw-r--r--   0        0        0      200 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/assets/v3.ext
+-rw-r--r--   0        0        0      593 2023-02-03 07:55:52.757134 pytest_httpserver-1.0.8/tests/conftest.py
+-rw-r--r--   0        0        0     1849 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_example_blocking_httpserver.py
+-rw-r--r--   0        0        0      129 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_example_query_params1.py
+-rw-r--r--   0        0        0      165 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_example_query_params2.py
+-rw-r--r--   0        0        0     1495 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_authorization_headers.py
+-rw-r--r--   0        0        0      750 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_case_insensitive_matcher.py
+-rw-r--r--   0        0        0      369 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_check.py
+-rw-r--r--   0        0        0     1160 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_check_handler_errors.py
+-rw-r--r--   0        0        0      360 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_custom_handler.py
+-rw-r--r--   0        0        0      780 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_header_value_matcher.py
+-rw-r--r--   0        0        0      347 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_json_matcher.py
+-rw-r--r--   0        0        0      357 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_query_params_dict.py
+-rw-r--r--   0        0        0       99 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_query_params_never_do_this.py
+-rw-r--r--   0        0        0       98 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_query_params_proper_use.py
+-rw-r--r--   0        0        0      187 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_regexp.py
+-rw-r--r--   0        0        0      235 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_timeout_requests.py
+-rw-r--r--   0        0        0      390 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_url_matcher.py
+-rw-r--r--   0        0        0      788 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.8/tests/examples/test_howto_wait_success.py
+-rw-r--r--   0        0        0     3481 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_blocking_httpserver.py
+-rw-r--r--   0        0        0     2557 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.8/tests/test_handler_errors.py
+-rw-r--r--   0        0        0     4280 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_headers.py
+-rw-r--r--   0        0        0      567 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_ip_protocols.py
+-rw-r--r--   0        0        0     1864 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.8/tests/test_json_matcher.py
+-rw-r--r--   0        0        0     3309 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_mixed.py
+-rw-r--r--   0        0        0     1817 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.8/tests/test_oneshot.py
+-rw-r--r--   0        0        0     1675 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.8/tests/test_ordered.py
+-rw-r--r--   0        0        0     1077 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_parse_qs.py
+-rw-r--r--   0        0        0     4122 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_permanent.py
+-rw-r--r--   0        0        0     1194 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.8/tests/test_port_changing.py
+-rw-r--r--   0        0        0     1488 2023-01-18 22:01:30.866852 pytest_httpserver-1.0.8/tests/test_querymatcher.py
+-rw-r--r--   0        0        0     1355 2023-02-03 07:55:52.798132 pytest_httpserver-1.0.8/tests/test_querystring.py
+-rw-r--r--   0        0        0     6401 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.8/tests/test_release.py
+-rw-r--r--   0        0        0     1202 2023-02-03 07:55:52.799132 pytest_httpserver-1.0.8/tests/test_ssl.py
+-rw-r--r--   0        0        0     1875 2023-02-03 07:55:52.818131 pytest_httpserver-1.0.8/tests/test_urimatch.py
+-rw-r--r--   0        0        0     3122 2023-02-03 07:55:52.851129 pytest_httpserver-1.0.8/tests/test_wait.py
+-rw-r--r--   0        0        0      122 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.8/tests/test_with_statement.py
+-rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.8/setup.py
+-rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.8/PKG-INFO
```

### Comparing `pytest_httpserver-1.0.7/CHANGES.rst` & `pytest_httpserver-1.0.8/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 =============
 Release Notes
 =============
 
+.. _Release Notes_1.0.8:
+
+1.0.8
+=====
+
+.. _Release Notes_1.0.8_Bug Fixes:
+
+Bug Fixes
+---------
+
+- Version 1.0.7 has been released with incorrect dependencies. This is fixed now.
+
+
 .. _Release Notes_1.0.7:
 
 1.0.7
 =====
 
 .. _Release Notes_1.0.7_Upgrade Notes:
```

### Comparing `pytest_httpserver-1.0.7/CONTRIBUTION.md` & `pytest_httpserver-1.0.8/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/LICENSE` & `pytest_httpserver-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/README.md` & `pytest_httpserver-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/Makefile` & `pytest_httpserver-1.0.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/api.rst` & `pytest_httpserver-1.0.8/doc/api.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/background.rst` & `pytest_httpserver-1.0.8/doc/background.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/conf.py` & `pytest_httpserver-1.0.8/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 author = "Zsolt Cserna"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "1.0.7"
+version = "1.0.8"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `pytest_httpserver-1.0.7/doc/fixtures.rst` & `pytest_httpserver-1.0.8/doc/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/howto.rst` & `pytest_httpserver-1.0.8/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/index.rst` & `pytest_httpserver-1.0.8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/tutorial.rst` & `pytest_httpserver-1.0.8/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/doc/upgrade.rst` & `pytest_httpserver-1.0.8/doc/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/example_pytest.py` & `pytest_httpserver-1.0.8/example_pytest.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/pyproject.toml` & `pytest_httpserver-1.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_httpserver"
-version = "1.0.7"
+version = "1.0.8"
 description = "pytest-httpserver is a httpserver for pytest"
 authors = ["Zsolt Cserna <cserna.zsolt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://pytest-httpserver.readthedocs.io/en/latest/"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pytest_httpserver-1.0.7/pytest_httpserver/__init__.py` & `pytest_httpserver-1.0.8/pytest_httpserver/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/pytest_httpserver/blocking_httpserver.py` & `pytest_httpserver-1.0.8/pytest_httpserver/blocking_httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/pytest_httpserver/httpserver.py` & `pytest_httpserver-1.0.8/pytest_httpserver/httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/pytest_httpserver/pytest_plugin.py` & `pytest_httpserver-1.0.8/pytest_httpserver/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/Makefile` & `pytest_httpserver-1.0.8/tests/assets/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/rootCA.crt` & `pytest_httpserver-1.0.8/tests/assets/rootCA.crt`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/rootCA.key` & `pytest_httpserver-1.0.8/tests/assets/rootCA.key`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/server.crt` & `pytest_httpserver-1.0.8/tests/assets/server.crt`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/server.csr` & `pytest_httpserver-1.0.8/tests/assets/server.csr`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/assets/server.key` & `pytest_httpserver-1.0.8/tests/assets/server.key`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/conftest.py` & `pytest_httpserver-1.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_example_blocking_httpserver.py` & `pytest_httpserver-1.0.8/tests/examples/test_example_blocking_httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_howto_authorization_headers.py` & `pytest_httpserver-1.0.8/tests/examples/test_howto_authorization_headers.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_howto_case_insensitive_matcher.py` & `pytest_httpserver-1.0.8/tests/examples/test_howto_case_insensitive_matcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_howto_check_handler_errors.py` & `pytest_httpserver-1.0.8/tests/examples/test_howto_check_handler_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_howto_header_value_matcher.py` & `pytest_httpserver-1.0.8/tests/examples/test_howto_header_value_matcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/examples/test_howto_wait_success.py` & `pytest_httpserver-1.0.8/tests/examples/test_howto_wait_success.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_blocking_httpserver.py` & `pytest_httpserver-1.0.8/tests/test_blocking_httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_handler_errors.py` & `pytest_httpserver-1.0.8/tests/test_handler_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_headers.py` & `pytest_httpserver-1.0.8/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_ip_protocols.py` & `pytest_httpserver-1.0.8/tests/test_ip_protocols.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_json_matcher.py` & `pytest_httpserver-1.0.8/tests/test_json_matcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_mixed.py` & `pytest_httpserver-1.0.8/tests/test_mixed.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_oneshot.py` & `pytest_httpserver-1.0.8/tests/test_oneshot.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_ordered.py` & `pytest_httpserver-1.0.8/tests/test_ordered.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_parse_qs.py` & `pytest_httpserver-1.0.8/tests/test_parse_qs.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_permanent.py` & `pytest_httpserver-1.0.8/tests/test_permanent.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_port_changing.py` & `pytest_httpserver-1.0.8/tests/test_port_changing.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_querymatcher.py` & `pytest_httpserver-1.0.8/tests/test_querymatcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_querystring.py` & `pytest_httpserver-1.0.8/tests/test_querystring.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_release.py` & `pytest_httpserver-1.0.8/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_ssl.py` & `pytest_httpserver-1.0.8/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_urimatch.py` & `pytest_httpserver-1.0.8/tests/test_urimatch.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/tests/test_wait.py` & `pytest_httpserver-1.0.8/tests/test_wait.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.7/setup.py` & `pytest_httpserver-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Werkzeug>=2.0.0']
 
 entry_points = \
 {'pytest11': ['pytest_httpserver = pytest_httpserver.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'pytest-httpserver',
-    'version': '1.0.7',
+    'version': '1.0.8',
     'description': 'pytest-httpserver is a httpserver for pytest',
     'long_description': '[![Build Status](https://github.com/csernazs/pytest-httpserver/workflows/build/badge.svg?branch=master)](https://github.com/csernazs/pytest-httpserver/actions?query=workflow%3Abuild+branch%3Amaster)\n[![Documentation Status](https://readthedocs.org/projects/pytest-httpserver/badge/?version=latest)](https://pytest-httpserver.readthedocs.io/en/latest/?badge=latest)\n [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=K6PU3AGBZW4QC&item_name=pytest-httpserver&currency_code=EUR&source=url)\n[![codecov](https://codecov.io/gh/csernazs/pytest-httpserver/branch/master/graph/badge.svg?token=MX2JXbHqRH)](https://codecov.io/gh/csernazs/pytest-httpserver)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## pytest_httpserver\n\nHTTP server for pytest\n\n\n### Nutshell\n\nThis library is designed to help to test http clients without contacting the real http server.\nIn other words, it is a fake http server which is accessible via localhost can be started with\nthe pre-defined expected http requests and their responses.\n\n### Example\n\n#### Handling a simple GET request\n```python\ndef test_my_client(\n    httpserver,\n):  # httpserver is a pytest fixture which starts the server\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request("/foobar").respond_with_json({"foo": "bar"})\n    # check that the request is served\n    assert requests.get(httpserver.url_for("/foobar")).json() == {"foo": "bar"}\n```\n\n#### Handing a POST request with an expected json body\n```python\ndef test_json_request(\n    httpserver,\n):  # httpserver is a pytest fixture which starts the server\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request(\n        "/foobar", method="POST", json={"id": 12, "name": "foo"}\n    ).respond_with_json({"foo": "bar"})\n    # check that the request is served\n    assert requests.post(\n        httpserver.url_for("/foobar"), json={"id": 12, "name": "foo"}\n    ).json() == {"foo": "bar"}\n```\n\n\nYou can also use the library without pytest. There\'s a with statement to ensure that the server is stopped.\n\n\n```python\nwith HTTPServer() as httpserver:\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request("/foobar").respond_with_json({"foo": "bar"})\n    # check that the request is served\n    print(requests.get(httpserver.url_for("/foobar")).json())\n```\n\n### Documentation\n\nPlease find the API documentation at https://pytest-httpserver.readthedocs.io/en/latest/.\n\n### Features\n\nYou can set up a dozen of expectations for the requests, and also what response should be sent by the server to the client.\n\n\n#### Requests\n\nThere are three different types:\n\n- **permanent**: this will be always served when there\'s match for this request, you can make as many HTTP requests as you want\n- **oneshot**: this will be served only once when there\'s a match for this request, you can only make 1 HTTP request\n- **ordered**: same as oneshot but the order must be strictly matched to the order of setting up\n\nYou can also fine-tune the expected request. The following can be specified:\n\n- URI (this is a must)\n- HTTP method\n- headers\n- query string\n- data (HTTP body of the request)\n- JSON (HTTP body loaded as JSON)\n\n\n#### Responses\n\nOnce you have the expectations for the request set up, you should also define the response you want to send back.\nThe following is supported currently:\n\n- respond arbitrary data (string or bytearray)\n- respond a json (a python dict converted in-place to json)\n- respond a Response object of werkzeug\n- use your own function\n\nSimilar to requests, you can fine-tune what response you want to send:\n\n- HTTP status\n- headers\n- data\n\n\n#### Behave support\n\nUsing the `BlockingHTTPServer` class, the assertion for a request and the\nresponse can be performed in real order. For more info, see the\n[test](tests/test_blocking_httpserver.py), the\n[howto](https://pytest-httpserver.readthedocs.io/en/latest/howto.html#running-httpserver-in-blocking-mode)\nand the [API\ndocumentation](https://pytest-httpserver.readthedocs.io/en/latest/api.html#blockinghttpserver).\n\n\n### Missing features\n* HTTP/2\n* Keepalive\n* ~~TLS~~\n\n### Donation\n\nIf you want to donate to this project, you can find the donate button at the top\nof the README.\n\nCurrently, this project is based heavily on werkzeug. Werkzeug does all the heavy lifting\nbehind the scenes, parsing HTTP request and defining Request and Response objects, which\nare currently transparent in the API.\n\nIf you wish to donate, please consider donating to them: https://palletsprojects.com/donate\n',
     'author': 'Zsolt Cserna',
     'author_email': 'cserna.zsolt@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csernazs/pytest-httpserver',
```

### Comparing `pytest_httpserver-1.0.7/PKG-INFO` & `pytest_httpserver-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-httpserver
-Version: 1.0.7
+Version: 1.0.8
 Summary: pytest-httpserver is a httpserver for pytest
 Home-page: https://github.com/csernazs/pytest-httpserver
 License: MIT
 Author: Zsolt Cserna
 Author-email: cserna.zsolt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

