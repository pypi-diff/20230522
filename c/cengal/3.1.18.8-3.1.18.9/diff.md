# Comparing `tmp/cengal-3.1.18.8.tar.gz` & `tmp/cengal-3.1.18.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cengal-3.1.18.8.tar", last modified: Sun May 21 23:49:37 2023, max compression
+gzip compressed data, was "cengal-3.1.18.9.tar", last modified: Mon May 22 00:17:14 2023, max compression
```

## Comparing `cengal-3.1.18.8.tar` & `cengal-3.1.18.9.tar`

### file list

```diff
@@ -1,1891 +1,1891 @@
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.689194 cengal-3.1.18.8/
--rw-r--r--   0 mb        (1000) mb        (1000)    11358 2022-04-21 11:25:54.000000 cengal-3.1.18.8/LICENSE.md
--rw-r--r--   0 mb        (1000) mb        (1000)      614 2022-11-01 20:15:42.000000 cengal-3.1.18.8/NOTICE
--rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-21 23:49:37.679194 cengal-3.1.18.8/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    22105 2023-05-21 21:52:36.000000 cengal-3.1.18.8/README.md
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.719189 cengal-3.1.18.8/cengal/
--rw-r--r--   0 mb        (1000) mb        (1000)     8228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/RequestCache.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2761 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ServerClock.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.779189 cengal-3.1.18.8/cengal/base/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.779189 cengal-3.1.18.8/cengal/base/classes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.799189 cengal-3.1.18.8/cengal/base/classes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.809189 cengal-3.1.18.8/cengal/base/classes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1267 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/versions/v_0/classes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.839189 cengal-3.1.18.8/cengal/base/classes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.849189 cengal-3.1.18.8/cengal/base/exceptions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.859189 cengal-3.1.18.8/cengal/base/exceptions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.879189 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1303 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.899189 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.909189 cengal-3.1.18.8/cengal/build_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.909189 cengal-3.1.18.8/cengal/build_tools/current_compiler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.929189 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.939189 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2162 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.959189 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.969189 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.979189 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.989189 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14704 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.009189 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.039189 cengal-3.1.18.8/cengal/bulk_pip_actions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/bulk_pip_actions/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6287 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/bulk_pip_actions/bulk_install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6023 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/bulk_pip_actions/install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/check_is_in_pycharm.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.039189 cengal-3.1.18.8/cengal/code_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.059189 cengal-3.1.18.8/cengal/code_flow_control/args_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.059189 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.089189 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16577 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.119189 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    17267 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.129189 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.129189 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.149189 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.169189 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.189189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.189189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.209189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    36471 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.259189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.289189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35218 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.319189 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.329189 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.349189 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.369189 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    23328 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.449190 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2882 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2624 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1373 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3467 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4392 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.459190 cengal-3.1.18.8/cengal/code_flow_control/none_or/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.459190 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.489189 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1487 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/none_or.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.499189 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.509189 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.529189 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.539189 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    29755 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.559189 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.569190 cengal-3.1.18.8/cengal/code_flow_control/smart_values/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.579190 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.599190 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2828 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.619190 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.639190 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3470 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.649190 cengal-3.1.18.8/cengal/code_inspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.659190 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.669190 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.689190 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6171 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.709190 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.719190 cengal-3.1.18.8/cengal/code_inspection/line_profiling/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.729190 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.759190 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.779190 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.789190 cengal-3.1.18.8/cengal/code_inspection/line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.799190 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.839190 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4305 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.859190 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.859190 cengal-3.1.18.8/cengal/cross_version/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cross_version/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.889190 cengal-3.1.18.8/cengal/cross_version/console_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cross_version/console_print/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cross_version/console_print/python3.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cross_version/console_print/universal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.899190 cengal-3.1.18.8/cengal/ctypes_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.899190 cengal-3.1.18.8/cengal/ctypes_tools/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.919190 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.939190 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.969190 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13438 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.989190 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:05.989190 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.029190 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.059190 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5488 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.069190 cengal-3.1.18.8/cengal/ctypes_tools/functions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.089190 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.159190 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1296 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1317 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.209190 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.219190 cengal-3.1.18.8/cengal/ctypes_tools/libraries/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.259190 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.299190 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.349190 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1482 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.359190 cengal-3.1.18.8/cengal/ctypes_tools/result_api/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.379190 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.439190 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1336 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1222 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1305 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.449190 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2729 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.469190 cengal-3.1.18.8/cengal/ctypes_tools/tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.479190 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.519190 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.539190 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1601 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.549190 cengal-3.1.18.8/cengal/ctypes_tools/types/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.569190 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.579190 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.619190 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7773 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/win_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.639190 cengal-3.1.18.8/cengal/cython_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cython_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1774 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/cython_tools/cythonyser_setup_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.659190 cengal-3.1.18.8/cengal/data_containers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.669190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.679190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.699190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.729190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.759190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.799190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2212 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.839190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.849190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.859190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.879190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.909190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1542 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.959190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:06.989190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.019190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.029190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1598 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.059190 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.079190 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.089190 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.119191 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   755734 2023-05-21 23:48:53.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)    28854 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.149191 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.189190 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   755526 2023-05-21 23:48:53.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)    28797 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.219190 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.229190 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.239190 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.289191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)    39956 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5405 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.309191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.359191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)    41895 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13150 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.379191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.409191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9730 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.449191 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.459191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.479191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.519191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12328 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.539191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.559191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12276 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.589191 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.609191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.619191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.659191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2034 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.689191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.719191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.749191 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.769191 cengal-3.1.18.8/cengal/data_containers/simple_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/simple_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.779191 cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.819191 cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5001 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.819191 cengal-3.1.18.8/cengal/data_containers/stack/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.839191 cengal-3.1.18.8/cengal/data_containers/stack/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.859191 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4660 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.889191 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3696 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.899191 cengal-3.1.18.8/cengal/data_generation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.919191 cengal-3.1.18.8/cengal/data_generation/id_generator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.929191 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.959191 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2218 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.979191 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:07.999191 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3045 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.019191 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.059191 cengal-3.1.18.8/cengal/data_manipulation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.079191 cengal-3.1.18.8/cengal/data_manipulation/conversion/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.089191 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.109191 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.149191 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2012 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.179191 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.199191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.219191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.239191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2476 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.269191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.279191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.299191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.329191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.359191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8111 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.379191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.399191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.419191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.429191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.469191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2549 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.499191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.519191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.529191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.559191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2565 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.579191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.599191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.629191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.679191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.699191 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3539 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.709191 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.729191 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.759191 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3917 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.799191 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.809191 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.839191 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.869191 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1257 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1484 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.909191 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7545 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.919191 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.939191 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.939191 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2981 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.969191 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6512 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.989191 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:08.999191 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.019191 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9311 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.039191 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.059191 cengal-3.1.18.8/cengal/data_manipulation/serialization/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.079191 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.099191 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27321 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.149191 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.169191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.179191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.199191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.279191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2652 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8192 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.319191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.439191 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2615 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2814 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2747 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24128 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5496 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/docten.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.449191 cengal-3.1.18.8/cengal/entities/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.459191 cengal-3.1.18.8/cengal/entities/bindable_to_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.489191 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.549191 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4360 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.589191 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.599191 cengal-3.1.18.8/cengal/entities/copyable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.619191 cengal-3.1.18.8/cengal/entities/copyable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.649191 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4450 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/copyable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.679191 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.729191 cengal-3.1.18.8/cengal/file_settings_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_settings_manager/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7336 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_settings_manager/config_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_settings_manager/dir_templates.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.769191 cengal-3.1.18.8/cengal/file_system/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.789191 cengal-3.1.18.8/cengal/file_system/app_fs_structure/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.809191 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.839191 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.959191 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1548 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4302 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8624 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8513 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7083 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3825 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:09.999191 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8151 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/directory_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2529 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.029191 cengal-3.1.18.8/cengal/file_system/file_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.049191 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.069191 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.099191 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2366 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.109191 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.129191 cengal-3.1.18.8/cengal/file_system/file_patch/generic/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.159191 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.199191 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/generic.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.229191 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.249191 cengal-3.1.18.8/cengal/file_system/file_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.279191 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.309191 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2311 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.359191 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.359191 cengal-3.1.18.8/cengal/file_system/path_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.369191 cengal-3.1.18.8/cengal/file_system/path_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.399191 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2581 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/path_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.419191 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.529191 cengal-3.1.18.8/cengal/file_system/win_fs/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3114 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1851 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/global_install_uninstall.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1997 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/path.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5190 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/shutil.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4437 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/file_system/win_fs/shutil_readable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.529191 cengal-3.1.18.8/cengal/hardware/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.549191 cengal-3.1.18.8/cengal/hardware/info/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.559191 cengal-3.1.18.8/cengal/hardware/info/cpu/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.579191 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.579191 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2282 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.619191 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.639191 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8748 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.659191 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.669191 cengal-3.1.18.8/cengal/hardware/memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.679191 cengal-3.1.18.8/cengal/hardware/memory/barriers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.699191 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.729191 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.759191 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     2022 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1355 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   194870 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.c
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.849191 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.879191 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.909191 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.979191 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:10.999191 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1933 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5299 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c
--rw-r--r--   0 mb        (1000) mb        (1000)   457250 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)     4230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
--rw-r--r--   0 mb        (1000) mb        (1000)   108883 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.039191 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8553 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.059191 cengal-3.1.18.8/cengal/introspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.079191 cengal-3.1.18.8/cengal/introspection/inspect/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.079191 cengal-3.1.18.8/cengal/introspection/inspect/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.109191 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19834 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/inspect.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.149191 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.149191 cengal-3.1.18.8/cengal/introspection/third_party/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.179191 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.179191 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.239191 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5359 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.269191 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.319191 cengal-3.1.18.8/cengal/io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.339191 cengal-3.1.18.8/cengal/io/asock_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.349191 cengal-3.1.18.8/cengal/io/asock_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.429191 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6006 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.479191 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   256320 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)   113359 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/tcp_app_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5057 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.629191 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18746 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)   123889 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/asock_io_core.py
--rw-r--r--   0 mb        (1000) mb        (1000)    15715 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.669191 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3922 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6409 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.699191 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   255677 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4987 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.719191 cengal-3.1.18.8/cengal/io/core/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.739191 cengal-3.1.18.8/cengal/io/core/memory_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.759191 cengal-3.1.18.8/cengal/io/core/memory_management/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.789191 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/memory_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.819191 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.829191 cengal-3.1.18.8/cengal/io/named_connections/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.859191 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.859191 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.899191 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10644 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.929191 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.949191 cengal-3.1.18.8/cengal/io/named_connections/workers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.959191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.969191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:11.999191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6610 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.029191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.039191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.049191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.099191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.149191 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.149191 cengal-3.1.18.8/cengal/io/net_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.149191 cengal-3.1.18.8/cengal/io/net_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.229191 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.249191 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.349191 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11975 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io__linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14773 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3987 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4846 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_method__select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.349191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.379191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.419191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   254835 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.459191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.499191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   254201 2023-05-21 23:48:54.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.539191 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.569191 cengal-3.1.18.8/cengal/io/serve_free_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.579191 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.599191 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5139 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.689191 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.719191 cengal-3.1.18.8/cengal/io/socket/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.779191 cengal-3.1.18.8/cengal/io/socket/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.779191 cengal-3.1.18.8/cengal/io/socket/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.849191 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1282 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.929191 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.949191 cengal-3.1.18.8/cengal/io/socket/errors/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:12.959191 cengal-3.1.18.8/cengal/io/socket/errors/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.029191 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2430 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/errors.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.039191 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.059191 cengal-3.1.18.8/cengal/io/used_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.109191 cengal-3.1.18.8/cengal/io/used_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.159191 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.199191 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3133 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8979 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/used_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.219191 cengal-3.1.18.8/cengal/math/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.229191 cengal-3.1.18.8/cengal/math/algebra/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.239191 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.249191 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.289191 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.349191 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.359191 cengal-3.1.18.8/cengal/math/geometry/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.389191 cengal-3.1.18.8/cengal/math/geometry/ellipse/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.409191 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.429191 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4989 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.479191 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2714 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.499191 cengal-3.1.18.8/cengal/math/geometry/point/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.509191 cengal-3.1.18.8/cengal/math/geometry/point/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.529191 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16020 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/point.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.559191 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.569191 cengal-3.1.18.8/cengal/math/geometry/vector/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.579191 cengal-3.1.18.8/cengal/math/geometry/vector/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.609191 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.659191 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    46033 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/vector.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.669191 cengal-3.1.18.8/cengal/math/numbers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.679191 cengal-3.1.18.8/cengal/math/numbers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.749191 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1347 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/numbers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.759191 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.809191 cengal-3.1.18.8/cengal/modules_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1570 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/alternative_import.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.819191 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.839191 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.869191 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1512 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.909191 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2183 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/modules_management/reload_module.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.959191 cengal-3.1.18.8/cengal/os/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/os/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/os/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.969191 cengal-3.1.18.8/cengal/parallel_execution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.979191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.989191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:13.999191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.029191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1848 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.079191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.119191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.129191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.249191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1361 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12105 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2468 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1990 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
--rw-r--r--   0 mb        (1000) mb        (1000)    51582 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.309191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3773 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6498 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35910 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.329191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.339191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.379191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1393 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.449191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.469191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.479191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.529191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9440 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.569191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.579191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.599191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.639191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3527 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.709191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.709191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.759191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.799191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.859191 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1642 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.899191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/
--rw-r--r--   0 mb        (1000) mb        (1000)     1301 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.929191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.939191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:14.979191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   126514 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.029191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.049191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/
--rw-r--r--   0 mb        (1000) mb        (1000)     1453 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.059191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.069191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.099191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11265 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.109191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.119191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.129191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.149191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    20728 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.189191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.199191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.209191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.239191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6566 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.259191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.269191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.289191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.339191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4174 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.369191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.369191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.379191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.409191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    55878 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.449191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.459191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.489191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.539191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7707 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.579191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.579191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.599191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.609191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7638 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.629191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.649191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.649191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.679191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9089 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.729191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.729191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.759191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.779191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5522 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.809191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.819191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:15.849191 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.669192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7537 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.669192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.669192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.669192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.689192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3908 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.719192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.719192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.729192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.759192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21255 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.789192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.799192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.809192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.839192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13686 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.869192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.919192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.939192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:29.979192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5971 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27436 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.009192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.019192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.039192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.069192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    22657 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.089192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.099192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.139192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.159192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6168 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.189192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.209192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.209192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.239192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    25204 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.299193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.319193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.329192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.439192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4956 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3827 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1399 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5316 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21055 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6044 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5877 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.469192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.479192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.499193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.519193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3465 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.589192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.609192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.619192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.639192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1748 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.649192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.659192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.669192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.699193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2897 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.759193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.769193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.799193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.819193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1652 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.849192 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.869193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.869193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.909193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2901 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.939193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.959193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:30.989193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.029193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1725 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.069193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.099193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.109193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.159193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.169193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6825 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.209193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.209193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.239193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.309193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7154 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.319193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.339193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.379193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.399193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11822 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.419193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.439193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.469193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.509193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11053 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.519193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.529193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.569193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.609193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    28117 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.609193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.639193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.639193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.689193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18947 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.699193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.719193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.739193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.769193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.789193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.799193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.829193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.859193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5687 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.879193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.909193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.919193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.939193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:31.979193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14142 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.039193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.079193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.099193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.119193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5186 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.169193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.219193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.229193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.239193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.289193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3175 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5182 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.329193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.339193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.349193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.409193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5979 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.429193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.439193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.449193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.469193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8391 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.499193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.509193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.529193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.569193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.609193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7876 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.619193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.619193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.639193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.659193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.689193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.699193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.709193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.759193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19201 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.779193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.789193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.819193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.869193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4691 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.899193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.919193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.959193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:32.979193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13310 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.009193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.029193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.039193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.059193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.099193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5547 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.109193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.129193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.149193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.169193 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1530 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.199193 cengal-3.1.18.8/cengal/parallel_execution/green_threads_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/green_threads_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3707 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/green_threads_tools/task_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.259193 cengal-3.1.18.8/cengal/parallel_execution/multiprocess/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multiprocess/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2840 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocess_testing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3086 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24843 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.309193 cengal-3.1.18.8/cengal/parallel_execution/multithreading/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multithreading/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7151 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/parallel_execution/multithreading/thread_workers_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.309193 cengal-3.1.18.8/cengal/performance_test_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.319193 cengal-3.1.18.8/cengal/performance_test_lib/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.349193 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8268 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.369193 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.409193 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9291 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.429193 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.459193 cengal-3.1.18.8/cengal/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.479193 cengal-3.1.18.8/cengal/shared_memory/versions/
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.519193 cengal-3.1.18.8/cengal/shared_memory/versions/1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/shared_memory/versions/1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/shared_memory/versions/1/mmap.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.519193 cengal-3.1.18.8/cengal/statistics/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.529193 cengal-3.1.18.8/cengal/statistics/normal_distribution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.539193 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.569193 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4157 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.589193 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/system.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.629193 cengal-3.1.18.8/cengal/testing_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/testing_lib/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3057 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/testing_lib/tests_list_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.649193 cengal-3.1.18.8/cengal/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.669193 cengal-3.1.18.8/cengal/text_processing/brackets_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.699193 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.759193 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1290 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2345 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6468 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/processing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3780 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.789193 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.799193 cengal-3.1.18.8/cengal/text_processing/encoding_detection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.819193 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.849193 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.869193 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11969 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.879193 cengal-3.1.18.8/cengal/text_processing/optional_formatter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.889193 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.919193 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4275 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.959193 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.969193 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:33.989193 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.009193 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.029193 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.039193 cengal-3.1.18.8/cengal/text_processing/text_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.049193 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.059193 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.119193 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2010 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.149193 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.169193 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.199193 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.219193 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1830 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.269193 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.269193 cengal-3.1.18.8/cengal/text_processing/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.279193 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.309193 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6282 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.329193 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.349193 cengal-3.1.18.8/cengal/text_processing/text_translator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.359193 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.389193 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.459193 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12696 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/text_translator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.469193 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.489193 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.529193 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.559193 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2994 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.579193 cengal-3.1.18.8/cengal/time_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.619193 cengal-3.1.18.8/cengal/time_management/cpu_clock/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.639193 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.679193 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.729193 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1357 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1930 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1640 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.809193 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.829193 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.849193 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.869193 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.909193 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1936 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1412 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c
--rw-r--r--   0 mb        (1000) mb        (1000)   132949 2023-05-21 23:48:55.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.c
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:34.959193 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.009193 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.009193 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.019193 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1369 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   126050 2023-05-21 23:48:55.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.c
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.059193 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.069193 cengal-3.1.18.8/cengal/time_management/load_best_timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/load_best_timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.119193 cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.199193 cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1446 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.209193 cengal-3.1.18.8/cengal/time_management/relative_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1366 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.229193 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.259194 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.319193 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8715 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.329193 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.359193 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.369193 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1490 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.369193 cengal-3.1.18.8/cengal/time_management/relative_time/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.389193 cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.409193 cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1419 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.429193 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.439193 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.479194 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1860 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.519194 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.529193 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.569193 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1633 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.579193 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.609193 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.659193 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1457 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   976597 2023-05-21 23:48:56.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.c
--rw-r--r--   0 mb        (1000) mb        (1000)    13454 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.709194 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16609 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.729194 cengal-3.1.18.8/cengal/time_management/sleep_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.749194 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.799193 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4701 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.869193 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.919193 cengal-3.1.18.8/cengal/time_management/timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.939194 cengal-3.1.18.8/cengal/time_management/timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:35.989194 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.039193 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4568 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.089193 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.119193 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6792 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.129193 cengal-3.1.18.8/cengal/time_management/timer_precision/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.149193 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.209194 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1867 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.239194 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4328 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.259194 cengal-3.1.18.8/cengal/unittest/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.289193 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.319193 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.359193 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.419194 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.429194 cengal-3.1.18.8/cengal/unittest/patcher/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.439194 cengal-3.1.18.8/cengal/unittest/patcher/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.479194 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.509194 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.639194 cengal-3.1.18.8/cengal/universal_parser/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1208 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/help_tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1378 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/idioms.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/parser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8668 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/test.py
--rw-r--r--   0 mb        (1000) mb        (1000)    75710 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/universal_parser/types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.669194 cengal-3.1.18.8/cengal/upk_helping_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/upk_helping_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2300 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/upk_helping_tools/upk_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1822 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/upk_helping_tools/upk_constants.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6519 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/upk_helping_tools/upk_utils_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.689194 cengal-3.1.18.8/cengal/user_interface/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.779193 cengal-3.1.18.8/cengal/user_interface/console/
--rw-r--r--   0 mb        (1000) mb        (1000)     1325 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3505 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/chooser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1550 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/colorama_helpers.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11361 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/encoding_changer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.789193 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.839193 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.869194 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4876 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1275 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.899194 cengal-3.1.18.8/cengal/user_interface/gui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:36.939194 cengal-3.1.18.8/cengal/user_interface/gui/nt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.019194 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.019194 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.109194 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3162 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.139194 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.139194 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.159194 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.239194 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3687 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.259194 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.279193 cengal-3.1.18.8/cengal/user_interface/plot/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.289193 cengal-3.1.18.8/cengal/user_interface/plot/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.319194 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1878 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/plot.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.339194 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.369194 cengal-3.1.18.8/cengal/web_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.369194 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.389194 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.419194 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.429194 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4333 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.469194 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12870 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal/web_tools/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:04.769189 cengal-3.1.18.8/cengal.egg-info/
--rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-21 23:48:50.000000 cengal-3.1.18.8/cengal.egg-info/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    85882 2023-05-21 23:48:56.000000 cengal-3.1.18.8/cengal.egg-info/SOURCES.txt
--rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-21 23:48:50.000000 cengal-3.1.18.8/cengal.egg-info/dependency_links.txt
--rw-r--r--   0 mb        (1000) mb        (1000)      211 2023-05-21 23:48:50.000000 cengal-3.1.18.8/cengal.egg-info/requires.txt
--rw-r--r--   0 mb        (1000) mb        (1000)       28 2023-05-21 23:48:50.000000 cengal-3.1.18.8/cengal.egg-info/top_level.txt
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.539194 cengal-3.1.18.8/cengal_setup_scripts/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/compile_all_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.599194 cengal-3.1.18.8/cengal_setup_scripts/find_and_prepare_cython_modules/
--rw-r--r--   0 mb        (1000) mb        (1000)     1254 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9413 2023-05-21 23:47:50.000000 cengal-3.1.18.8/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 23:49:37.659194 cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10416 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/install_packages.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/set_environment_variables.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/setup__dynamic_list_of_pieces.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/setup__recv_buff_size_computer.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1499 2023-05-21 21:07:08.000000 cengal-3.1.18.8/cengal_setup_scripts/setup__repeat_for_a_time.py
--rw-r--r--   0 mb        (1000) mb        (1000)      156 2022-11-01 20:15:48.000000 cengal-3.1.18.8/pyproject.toml
--rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-21 23:49:37.689194 cengal-3.1.18.8/setup.cfg
--rw-r--r--   0 mb        (1000) mb        (1000)     8722 2023-05-21 23:30:42.000000 cengal-3.1.18.8/setup.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.989192 cengal-3.1.18.9/
+-rw-r--r--   0 mb        (1000) mb        (1000)    11358 2022-04-21 11:25:54.000000 cengal-3.1.18.9/LICENSE.md
+-rw-r--r--   0 mb        (1000) mb        (1000)      614 2022-11-01 20:15:42.000000 cengal-3.1.18.9/NOTICE
+-rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-22 00:17:13.959192 cengal-3.1.18.9/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    22105 2023-05-21 21:52:36.000000 cengal-3.1.18.9/README.md
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.389198 cengal-3.1.18.9/cengal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     8228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/RequestCache.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2761 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ServerClock.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.479199 cengal-3.1.18.9/cengal/base/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.499199 cengal-3.1.18.9/cengal/base/classes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.519199 cengal-3.1.18.9/cengal/base/classes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.559198 cengal-3.1.18.9/cengal/base/classes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1267 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/versions/v_0/classes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.589199 cengal-3.1.18.9/cengal/base/classes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.619199 cengal-3.1.18.9/cengal/base/exceptions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.649199 cengal-3.1.18.9/cengal/base/exceptions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.679199 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1303 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.709199 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.729199 cengal-3.1.18.9/cengal/build_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.759199 cengal-3.1.18.9/cengal/build_tools/current_compiler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.779199 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.819199 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2162 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.859199 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.919199 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.939199 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.989199 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14704 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.039199 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.109199 cengal-3.1.18.9/cengal/bulk_pip_actions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/bulk_pip_actions/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6287 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/bulk_pip_actions/bulk_install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6023 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/bulk_pip_actions/install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/check_is_in_pycharm.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.139199 cengal-3.1.18.9/cengal/code_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.139199 cengal-3.1.18.9/cengal/code_flow_control/args_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.159199 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.199199 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16577 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.259199 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    17267 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.269199 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.279199 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.309199 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.339199 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.349199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.359199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.389199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    36471 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.429199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.469199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35218 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.519199 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.529199 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.559199 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.599199 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    23328 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.729199 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2882 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2624 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1373 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3467 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4392 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.749199 cengal-3.1.18.9/cengal/code_flow_control/none_or/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.789199 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.839199 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1487 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/none_or.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.859199 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.879199 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.899199 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.939199 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    29755 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.959199 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.969199 cengal-3.1.18.9/cengal/code_flow_control/smart_values/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:36.989199 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.029199 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2828 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.049199 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.089199 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3470 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.099199 cengal-3.1.18.9/cengal/code_inspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.119199 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.129199 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.149199 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6171 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.189199 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.209199 cengal-3.1.18.9/cengal/code_inspection/line_profiling/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.229199 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.259199 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.279199 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.299199 cengal-3.1.18.9/cengal/code_inspection/line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.319199 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.359199 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4305 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.389199 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.399199 cengal-3.1.18.9/cengal/cross_version/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cross_version/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.439199 cengal-3.1.18.9/cengal/cross_version/console_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cross_version/console_print/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cross_version/console_print/python3.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cross_version/console_print/universal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.459199 cengal-3.1.18.9/cengal/ctypes_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.469199 cengal-3.1.18.9/cengal/ctypes_tools/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.479199 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.509199 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.549199 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13438 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.569199 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.589199 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.629199 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.669199 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5488 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.669199 cengal-3.1.18.9/cengal/ctypes_tools/functions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.689199 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.729199 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1296 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1317 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.759199 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.779199 cengal-3.1.18.9/cengal/ctypes_tools/libraries/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.789199 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.829199 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.859199 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1482 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.879199 cengal-3.1.18.9/cengal/ctypes_tools/result_api/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.899199 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.959199 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1336 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1222 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1305 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:37.999199 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2729 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.019199 cengal-3.1.18.9/cengal/ctypes_tools/tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.029199 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.089199 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.129199 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1601 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.139199 cengal-3.1.18.9/cengal/ctypes_tools/types/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.159199 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.189199 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.219200 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7773 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/win_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.249199 cengal-3.1.18.9/cengal/cython_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cython_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1774 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/cython_tools/cythonyser_setup_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.259199 cengal-3.1.18.9/cengal/data_containers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.279199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.299199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.319199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.339199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.369199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.399200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2212 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.439200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.449200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.459200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.479200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.509199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1542 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.549199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.559199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.569199 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.619200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1598 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.659200 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.689200 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.709200 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.729200 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   755734 2023-05-22 00:16:06.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)    28854 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.759199 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.789200 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   755526 2023-05-22 00:16:06.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)    28797 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.819200 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.829200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.859200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.939200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)    39956 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5405 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.959200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:38.999200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)    41895 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13150 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.019200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.039200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9730 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.079200 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.119200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.149200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.219200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12328 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.239200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.319200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12276 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.359200 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.389200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.439200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.459200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2034 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.559200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.609200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.669200 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.689200 cengal-3.1.18.9/cengal/data_containers/simple_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/simple_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.699200 cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.799200 cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5001 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.819200 cengal-3.1.18.9/cengal/data_containers/stack/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.869200 cengal-3.1.18.9/cengal/data_containers/stack/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.929200 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4660 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.979200 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3696 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.989200 cengal-3.1.18.9/cengal/data_generation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:39.989200 cengal-3.1.18.9/cengal/data_generation/id_generator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.009200 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.059200 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2218 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.099200 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.119200 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3045 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.149200 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.179200 cengal-3.1.18.9/cengal/data_manipulation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.199200 cengal-3.1.18.9/cengal/data_manipulation/conversion/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.209200 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.229200 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.249200 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2012 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.299200 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.309200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.309200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.339200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2476 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.389200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.449200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.469200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.479200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.539200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8111 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.579200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.599200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.609200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.629200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.659200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2549 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.699200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.709200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.739200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.769200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2565 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.809200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.829200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.839200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.869200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.929200 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3539 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.939200 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.959200 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:40.979200 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3917 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.019200 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.039200 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.049200 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.079200 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1257 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1484 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.109200 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7545 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.119200 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.139200 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.179200 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2981 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.209200 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6512 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.229200 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.239200 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.289200 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9311 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.339200 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.339200 cengal-3.1.18.9/cengal/data_manipulation/serialization/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.339200 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.379200 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27321 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.409200 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.419200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.429200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.469200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.519200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2652 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8192 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.539200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.619200 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2615 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2814 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2747 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24128 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5496 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/docten.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.649201 cengal-3.1.18.9/cengal/entities/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.669201 cengal-3.1.18.9/cengal/entities/bindable_to_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.689200 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.719200 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4360 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.779200 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.789200 cengal-3.1.18.9/cengal/entities/copyable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.809200 cengal-3.1.18.9/cengal/entities/copyable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.839200 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4450 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/copyable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.879201 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.949200 cengal-3.1.18.9/cengal/file_settings_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_settings_manager/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7336 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_settings_manager/config_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_settings_manager/dir_templates.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.999200 cengal-3.1.18.9/cengal/file_system/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:41.999200 cengal-3.1.18.9/cengal/file_system/app_fs_structure/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.019200 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.049201 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.189200 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1548 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4302 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8624 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8513 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7083 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3825 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.229200 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8151 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/directory_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2529 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.239201 cengal-3.1.18.9/cengal/file_system/file_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.259201 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.279201 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.299201 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2366 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.329201 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.349201 cengal-3.1.18.9/cengal/file_system/file_patch/generic/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.369201 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.399201 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/generic.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.459201 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.479201 cengal-3.1.18.9/cengal/file_system/file_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.499201 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.519201 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2311 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.579201 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.589201 cengal-3.1.18.9/cengal/file_system/path_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.609201 cengal-3.1.18.9/cengal/file_system/path_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.639201 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2581 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/path_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.669201 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.759201 cengal-3.1.18.9/cengal/file_system/win_fs/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3114 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1851 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/global_install_uninstall.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1997 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/path.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5190 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/shutil.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4437 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/file_system/win_fs/shutil_readable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.779201 cengal-3.1.18.9/cengal/hardware/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.789201 cengal-3.1.18.9/cengal/hardware/info/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.809201 cengal-3.1.18.9/cengal/hardware/info/cpu/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.819201 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.869201 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2282 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.899201 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.959201 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8748 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:42.969201 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.009201 cengal-3.1.18.9/cengal/hardware/memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.029201 cengal-3.1.18.9/cengal/hardware/memory/barriers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.049201 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.059201 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.089201 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     2022 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1355 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   194870 2023-05-22 00:16:07.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.c
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.129201 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.149201 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.179201 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.219201 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.259201 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1933 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5299 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c
+-rw-r--r--   0 mb        (1000) mb        (1000)   457250 2023-05-22 00:16:07.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     4230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   108883 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.289201 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8553 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.329201 cengal-3.1.18.9/cengal/introspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.349201 cengal-3.1.18.9/cengal/introspection/inspect/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.379201 cengal-3.1.18.9/cengal/introspection/inspect/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.399201 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19834 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/inspect.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.449201 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.459201 cengal-3.1.18.9/cengal/introspection/third_party/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.469201 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.479201 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.529201 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5359 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.569201 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.579201 cengal-3.1.18.9/cengal/io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.619201 cengal-3.1.18.9/cengal/io/asock_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.659201 cengal-3.1.18.9/cengal/io/asock_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.709201 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6006 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.739201 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   256320 2023-05-22 00:16:07.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   113359 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/tcp_app_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5057 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.839201 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18746 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   123889 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/asock_io_core.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    15715 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.869201 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3922 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6409 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.919201 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   255677 2023-05-22 00:16:07.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4987 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.929201 cengal-3.1.18.9/cengal/io/core/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.939201 cengal-3.1.18.9/cengal/io/core/memory_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.959201 cengal-3.1.18.9/cengal/io/core/memory_management/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:43.999201 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/memory_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.039201 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.059201 cengal-3.1.18.9/cengal/io/named_connections/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.069201 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.079201 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.109201 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10644 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.149201 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.149201 cengal-3.1.18.9/cengal/io/named_connections/workers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.149201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.149201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.149201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6610 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.199201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.219201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.239201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.269201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.309201 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.329201 cengal-3.1.18.9/cengal/io/net_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.349201 cengal-3.1.18.9/cengal/io/net_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.419201 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.429201 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.479201 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11975 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io__linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14773 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3987 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4846 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_method__select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.499201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.499201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.519201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   254835 2023-05-22 00:16:07.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.579201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.599201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   254201 2023-05-22 00:16:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.629201 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.649201 cengal-3.1.18.9/cengal/io/serve_free_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.659201 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.699201 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5139 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.709201 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.729201 cengal-3.1.18.9/cengal/io/socket/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.739201 cengal-3.1.18.9/cengal/io/socket/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.759201 cengal-3.1.18.9/cengal/io/socket/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.789201 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1282 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.809201 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.819201 cengal-3.1.18.9/cengal/io/socket/errors/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.839201 cengal-3.1.18.9/cengal/io/socket/errors/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.869201 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2430 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/errors.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.889201 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.919201 cengal-3.1.18.9/cengal/io/used_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.929201 cengal-3.1.18.9/cengal/io/used_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.949201 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.979201 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3133 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8979 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/used_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:44.999201 cengal-3.1.18.9/cengal/math/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.019201 cengal-3.1.18.9/cengal/math/algebra/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.039201 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.049201 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.089201 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.129201 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.149201 cengal-3.1.18.9/cengal/math/geometry/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.169201 cengal-3.1.18.9/cengal/math/geometry/ellipse/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.189201 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.229201 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4989 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.289201 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2714 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.349201 cengal-3.1.18.9/cengal/math/geometry/point/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.369201 cengal-3.1.18.9/cengal/math/geometry/point/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.439201 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16020 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/point.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.469201 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.479201 cengal-3.1.18.9/cengal/math/geometry/vector/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.499201 cengal-3.1.18.9/cengal/math/geometry/vector/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.519201 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.549201 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    46033 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/vector.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.579201 cengal-3.1.18.9/cengal/math/numbers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.579201 cengal-3.1.18.9/cengal/math/numbers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.599202 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1347 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/numbers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.629202 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.649201 cengal-3.1.18.9/cengal/modules_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1570 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/alternative_import.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.659201 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.669201 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.699201 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1512 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.739201 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2183 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/modules_management/reload_module.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.759201 cengal-3.1.18.9/cengal/os/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/os/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/os/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.779201 cengal-3.1.18.9/cengal/parallel_execution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.799202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.819202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.819202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.859202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1848 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.869202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.889201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.899201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:45.969201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1361 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12105 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2468 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1990 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    51582 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.009202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3773 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6498 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35910 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.019202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.029202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.049202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1393 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.069202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.069202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.089202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.109202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9440 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.139201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.149201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.159201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.179201 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3527 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.209202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.219202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.229202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.249202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.279202 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1642 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.289202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1301 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.299202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.319202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.339202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   126514 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.359202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.399202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1453 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.409202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.409202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.449202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11265 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.479202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.489202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.509202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.539202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    20728 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.589202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.619202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.639202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.669202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6566 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.699202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.709202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.729202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.769202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4174 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.819202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.829202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.839202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.869202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    55878 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.909202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.919202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.939202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.959202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7707 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.989202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:46.999202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.019202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.039202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7638 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.069202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.069202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.119202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.139202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9089 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.179202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.219202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.219202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.269202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5522 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.299202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.319202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.319202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.349202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7537 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.389202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.429202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.439202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.489202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3908 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.569202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.569202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.619202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.649202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21255 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.789202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.789202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.819202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.889202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13686 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.909202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.959202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:47.999202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.029202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5971 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27436 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.089202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.099202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.149202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.169202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    22657 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.209202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.219202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.229202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.299202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6168 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.359202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.379202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:48.399202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:04.839203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    25204 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:04.859203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:04.869203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:04.889203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.049203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4956 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3827 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1399 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5316 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21055 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6044 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5877 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.089203 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.119202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.149202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.169202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3465 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.219202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.219202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.229202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.259202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1748 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.279202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.289202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.309202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.359202 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2897 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.409201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.419201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.509201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.589201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1652 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.609201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.629201 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.719200 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.779200 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2901 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.829200 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.869200 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:05.879200 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.099199 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1725 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.189199 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.209199 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.229199 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.309198 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.349198 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6825 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.369198 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.449198 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.519198 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.569197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7154 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.579197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.629197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.639197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.749197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11822 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.749197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.759197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.799197 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.859196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11053 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.859196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.879196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.899196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.919196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    28117 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.939196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.979196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:06.999196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.039196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18947 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.059196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.079196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.099196 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.109195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.159195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.169195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.179195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.189195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5687 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.259195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.289195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.319195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.349195 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.399194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14142 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.439194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.469194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.479194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.529194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5186 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.559194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.569194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.609194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.629194 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.729193 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3175 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5182 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.799193 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.849193 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.859193 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.919192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5979 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:07.969192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.029192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.049192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.069192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8391 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.119192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.119192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.129192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.209191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.249191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7876 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.269191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.289191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.319191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.359191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.399191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.399191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.409191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.449191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19201 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.469191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.489191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.509191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.569191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4691 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.599191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.629191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.649191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.699191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13310 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.759191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.779191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.799191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.879191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.929191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5547 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.959191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:08.969191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.049191 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.109192 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1530 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.179191 cengal-3.1.18.9/cengal/parallel_execution/green_threads_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/green_threads_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3707 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/green_threads_tools/task_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.269191 cengal-3.1.18.9/cengal/parallel_execution/multiprocess/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multiprocess/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2840 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocess_testing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3086 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24843 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.299192 cengal-3.1.18.9/cengal/parallel_execution/multithreading/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multithreading/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7151 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/parallel_execution/multithreading/thread_workers_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.339192 cengal-3.1.18.9/cengal/performance_test_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.359192 cengal-3.1.18.9/cengal/performance_test_lib/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.389191 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8268 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.419191 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.479191 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9291 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.499191 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.499191 cengal-3.1.18.9/cengal/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.529192 cengal-3.1.18.9/cengal/shared_memory/versions/
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.579192 cengal-3.1.18.9/cengal/shared_memory/versions/1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/shared_memory/versions/1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/shared_memory/versions/1/mmap.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.629191 cengal-3.1.18.9/cengal/statistics/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.649191 cengal-3.1.18.9/cengal/statistics/normal_distribution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.669191 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.709191 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4157 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.739192 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/system.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.759192 cengal-3.1.18.9/cengal/testing_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/testing_lib/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3057 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/testing_lib/tests_list_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.809192 cengal-3.1.18.9/cengal/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.819192 cengal-3.1.18.9/cengal/text_processing/brackets_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.829192 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.869192 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1290 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2345 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6468 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/processing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3780 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.959192 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.969192 cengal-3.1.18.9/cengal/text_processing/encoding_detection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:09.989192 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.029192 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.079192 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11969 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.099192 cengal-3.1.18.9/cengal/text_processing/optional_formatter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.119192 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.169192 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4275 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.219192 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.229192 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.239192 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.289192 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.329192 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.339192 cengal-3.1.18.9/cengal/text_processing/text_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.369192 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.379192 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.419192 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2010 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.469192 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.509192 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.519192 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.569192 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1830 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.619192 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.629192 cengal-3.1.18.9/cengal/text_processing/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.649192 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.679192 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6282 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.729192 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.749192 cengal-3.1.18.9/cengal/text_processing/text_translator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.769192 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.829192 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.869192 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12696 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/text_translator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.909192 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.919192 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.969192 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:10.999192 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2994 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.009192 cengal-3.1.18.9/cengal/time_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.039192 cengal-3.1.18.9/cengal/time_management/cpu_clock/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.049192 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.079192 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.109192 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1357 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1930 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1640 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.159192 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.169192 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.189192 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.229192 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.259192 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1936 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1412 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c
+-rw-r--r--   0 mb        (1000) mb        (1000)   132949 2023-05-22 00:16:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.c
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.299192 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.319192 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.329192 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.369192 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1369 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   126050 2023-05-22 00:16:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.c
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.409192 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/load_best_timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/load_best_timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1446 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/relative_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1366 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.419192 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.499192 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8715 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.519192 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.529192 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.579192 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1490 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.599192 cengal-3.1.18.9/cengal/time_management/relative_time/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.619192 cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.669192 cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1419 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.679192 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.689192 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.729192 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1860 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.749192 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.769192 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.799192 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1633 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.849192 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.849192 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.889192 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1457 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   976597 2023-05-22 00:16:09.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.c
+-rw-r--r--   0 mb        (1000) mb        (1000)    13454 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.939192 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16609 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.979192 cengal-3.1.18.9/cengal/time_management/sleep_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:11.999192 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.009192 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4701 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.059192 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.079192 cengal-3.1.18.9/cengal/time_management/timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.109192 cengal-3.1.18.9/cengal/time_management/timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.129192 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.149192 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4568 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.189192 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.209192 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6792 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.219192 cengal-3.1.18.9/cengal/time_management/timer_precision/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.229192 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.269192 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1867 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.299192 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4328 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.309192 cengal-3.1.18.9/cengal/unittest/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.349192 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.359192 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.389192 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.459192 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.469192 cengal-3.1.18.9/cengal/unittest/patcher/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.499192 cengal-3.1.18.9/cengal/unittest/patcher/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.529192 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.579192 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.759192 cengal-3.1.18.9/cengal/universal_parser/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1208 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/help_tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1378 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/idioms.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/parser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8668 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    75710 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/universal_parser/types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.829192 cengal-3.1.18.9/cengal/upk_helping_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/upk_helping_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2300 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/upk_helping_tools/upk_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1822 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/upk_helping_tools/upk_constants.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6519 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/upk_helping_tools/upk_utils_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.839192 cengal-3.1.18.9/cengal/user_interface/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.909192 cengal-3.1.18.9/cengal/user_interface/console/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1325 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3505 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/chooser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1550 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/colorama_helpers.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11361 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/encoding_changer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.929192 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:12.939192 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.009192 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4876 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1275 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.099192 cengal-3.1.18.9/cengal/user_interface/gui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.139192 cengal-3.1.18.9/cengal/user_interface/gui/nt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.139192 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.179192 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.209192 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3162 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.259192 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.279192 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.279192 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.329192 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3687 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.369192 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.429192 cengal-3.1.18.9/cengal/user_interface/plot/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.429192 cengal-3.1.18.9/cengal/user_interface/plot/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.459192 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1878 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/plot.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.519192 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.549192 cengal-3.1.18.9/cengal/web_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.619192 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.629192 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.649192 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.689192 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4333 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.739192 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12870 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal/web_tools/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:16:35.459199 cengal-3.1.18.9/cengal.egg-info/
+-rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-22 00:06:55.000000 cengal-3.1.18.9/cengal.egg-info/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    85882 2023-05-22 00:16:24.000000 cengal-3.1.18.9/cengal.egg-info/SOURCES.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-22 00:06:55.000000 cengal-3.1.18.9/cengal.egg-info/dependency_links.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)      211 2023-05-22 00:06:55.000000 cengal-3.1.18.9/cengal.egg-info/requires.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)       28 2023-05-22 00:06:55.000000 cengal-3.1.18.9/cengal.egg-info/top_level.txt
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.849192 cengal-3.1.18.9/cengal_setup_scripts/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/compile_all_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.879192 cengal-3.1.18.9/cengal_setup_scripts/find_and_prepare_cython_modules/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1254 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9453 2023-05-22 00:15:34.000000 cengal-3.1.18.9/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 00:17:13.939192 cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10416 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/install_packages.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/set_environment_variables.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/setup__dynamic_list_of_pieces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/setup__recv_buff_size_computer.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1499 2023-05-21 21:07:08.000000 cengal-3.1.18.9/cengal_setup_scripts/setup__repeat_for_a_time.py
+-rw-r--r--   0 mb        (1000) mb        (1000)      156 2022-11-01 20:15:48.000000 cengal-3.1.18.9/pyproject.toml
+-rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-22 00:17:13.989192 cengal-3.1.18.9/setup.cfg
+-rw-r--r--   0 mb        (1000) mb        (1000)     8734 2023-05-22 00:15:55.000000 cengal-3.1.18.9/setup.py
```

### Comparing `cengal-3.1.18.8/LICENSE.md` & `cengal-3.1.18.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/NOTICE` & `cengal-3.1.18.9/NOTICE`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/PKG-INFO` & `cengal-3.1.18.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.1.18.8
+Version: 3.1.18.9
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cengal-3.1.18.8/README.md` & `cengal-3.1.18.9/README.md`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/RequestCache.py` & `cengal-3.1.18.9/cengal/RequestCache.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ServerClock.py` & `cengal-3.1.18.9/cengal/ServerClock.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/__init__.py` & `cengal-3.1.18.9/cengal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/__init__.py` & `cengal-3.1.18.9/cengal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/__init__.py` & `cengal-3.1.18.9/cengal/base/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/versions/__init__.py` & `cengal-3.1.18.9/cengal/base/classes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/base/classes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/versions/v_0/classes.py` & `cengal-3.1.18.9/cengal/base/classes/versions/v_0/classes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/base/classes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/__init__.py` & `cengal-3.1.18.9/cengal/base/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/versions/__init__.py` & `cengal-3.1.18.9/cengal/base/exceptions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/exceptions.py` & `cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/bulk_pip_actions/__init__.py` & `cengal-3.1.18.9/cengal/bulk_pip_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/bulk_pip_actions/bulk_install.py` & `cengal-3.1.18.9/cengal/bulk_pip_actions/bulk_install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/bulk_pip_actions/install.py` & `cengal-3.1.18.9/cengal/bulk_pip_actions/install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/check_is_in_pycharm.py` & `cengal-3.1.18.9/cengal/check_is_in_pycharm.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py` & `cengal-3.1.18.9/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py` & `cengal-3.1.18.9/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/none_or.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/none_or.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_0/result_types.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_0/result_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_2/__init__.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py` & `cengal-3.1.18.9/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cross_version/__init__.py` & `cengal-3.1.18.9/cengal/cross_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cross_version/console_print/__init__.py` & `cengal-3.1.18.9/cengal/cross_version/console_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cross_version/console_print/python3.py` & `cengal-3.1.18.9/cengal/cross_version/console_print/python3.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cross_version/console_print/universal.py` & `cengal-3.1.18.9/cengal/cross_version/console_print/universal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/constants/versions/v_0/win_constants.py` & `cengal-3.1.18.9/cengal/ctypes_tools/constants/versions/v_0/win_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py` & `cengal-3.1.18.9/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/functions.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/functions/versions/v_0/win_functions.py` & `cengal-3.1.18.9/cengal/ctypes_tools/functions/versions/v_0/win_functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py` & `cengal-3.1.18.9/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/result_api.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py` & `cengal-3.1.18.9/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/tools.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/tools/versions/v_0/win_tools.py` & `cengal-3.1.18.9/cengal/ctypes_tools/tools/versions/v_0/win_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/versions/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/ctypes_tools/types/versions/v_0/win_types.py` & `cengal-3.1.18.9/cengal/ctypes_tools/types/versions/v_0/win_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cython_tools/__init__.py` & `cengal-3.1.18.9/cengal/cython_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/cython_tools/cythonyser_setup_runner.py` & `cengal-3.1.18.9/cengal/cython_tools/cythonyser_setup_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.c` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.c` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/simple_tree/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/simple_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py` & `cengal-3.1.18.9/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/stack/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/stack.py` & `cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_containers/stack/versions/v_0/tests/test__stack.py` & `cengal-3.1.18.9/cengal/data_containers/stack/versions/v_0/tests/test__stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/id_generator.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/id_generator.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py` & `cengal-3.1.18.9/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/help_tools.py` & `cengal-3.1.18.9/cengal/data_manipulation/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py` & `cengal-3.1.18.9/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/serialization.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py` & `cengal-3.1.18.9/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py` & `cengal-3.1.18.9/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/docten.py` & `cengal-3.1.18.9/cengal/docten.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/__init__.py` & `cengal-3.1.18.9/cengal/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/__init__.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/__init__.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/__init__.py` & `cengal-3.1.18.9/cengal/entities/copyable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/versions/__init__.py` & `cengal-3.1.18.9/cengal/entities/copyable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/copyable.py` & `cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/copyable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_settings_manager/__init__.py` & `cengal-3.1.18.9/cengal/file_settings_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_settings_manager/config_manager.py` & `cengal-3.1.18.9/cengal/file_settings_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_settings_manager/dir_templates.py` & `cengal-3.1.18.9/cengal/file_settings_manager/dir_templates.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/__init__.py` & `cengal-3.1.18.9/cengal/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/__init__.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/__init__.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/directory_manager.py` & `cengal-3.1.18.9/cengal/file_system/directory_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_manager.py` & `cengal-3.1.18.9/cengal/file_system/file_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/generic.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/generic.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/simple.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/__init__.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/versions/__init__.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/path_manager.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/path_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/__init__.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/base.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/global_install_uninstall.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/global_install_uninstall.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/path.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/path.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/shutil.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/shutil.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/file_system/win_fs/shutil_readable.py` & `cengal-3.1.18.9/cengal/file_system/win_fs/shutil_readable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/__init__.py` & `cengal-3.1.18.9/cengal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/cpu.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/cpu.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.c` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.c` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/help_tools.py` & `cengal-3.1.18.9/cengal/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/__init__.py` & `cengal-3.1.18.9/cengal/introspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/__init__.py` & `cengal-3.1.18.9/cengal/introspection/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/versions/__init__.py` & `cengal-3.1.18.9/cengal/introspection/inspect/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/inspect.py` & `cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/inspect.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/__init__.py` & `cengal-3.1.18.9/cengal/introspection/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/__init__.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/__init__.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/__init__.py` & `cengal-3.1.18.9/cengal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/base.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.c` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/tcp_app_server.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/tcp_app_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_0/tcp_link.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_0/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/abstract.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/asock_io_core.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/asock_io_core.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/base.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/io_loops/select.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/io_loops/select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.c` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/asock_io/versions/v_1/tcp_link.py` & `cengal-3.1.18.9/cengal/io/asock_io/versions/v_1/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/__init__.py` & `cengal-3.1.18.9/cengal/io/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/__init__.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/memory_management.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/memory_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/__init__.py` & `cengal-3.1.18.9/cengal/io/net_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/__init__.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io__linux.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io__linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_abstract.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/net_io/versions/v_0/net_io_method__select.py` & `cengal-3.1.18.9/cengal/io/net_io/versions/v_0/net_io_method__select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.c` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.c` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/__init__.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/constants.py` & `cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/errors/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/errors.py` & `cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/errors.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/__init__.py` & `cengal-3.1.18.9/cengal/io/used_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/versions/__init__.py` & `cengal-3.1.18.9/cengal/io/used_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py` & `cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/io/used_ports/versions/v_0/used_ports.py` & `cengal-3.1.18.9/cengal/io/used_ports/versions/v_0/used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/__init__.py` & `cengal-3.1.18.9/cengal/math/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/__init__.py` & `cengal-3.1.18.9/cengal/math/algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/__init__.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/__init__.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/ellipse.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/ellipse.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py` & `cengal-3.1.18.9/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/point/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/versions/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/point/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/point.py` & `cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/point.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/versions/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/geometry/vector/versions/v_0/vector.py` & `cengal-3.1.18.9/cengal/math/geometry/vector/versions/v_0/vector.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/__init__.py` & `cengal-3.1.18.9/cengal/math/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/versions/__init__.py` & `cengal-3.1.18.9/cengal/math/numbers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/math/numbers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/versions/v_0/numbers.py` & `cengal-3.1.18.9/cengal/math/numbers/versions/v_0/numbers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/math/numbers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/__init__.py` & `cengal-3.1.18.9/cengal/modules_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/alternative_import.py` & `cengal-3.1.18.9/cengal/modules_management/alternative_import.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/__init__.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/__init__.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/modules_management/reload_module.py` & `cengal-3.1.18.9/cengal/modules_management/reload_module.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/os/__init__.py` & `cengal-3.1.18.9/cengal/os/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/os/help_tools.py` & `cengal-3.1.18.9/cengal/os/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py` & `cengal-3.1.18.9/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py` & `cengal-3.1.18.9/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/green_threads_tools/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/green_threads_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/green_threads_tools/task_management.py` & `cengal-3.1.18.9/cengal/parallel_execution/green_threads_tools/task_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multiprocess/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocess_testing.py` & `cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocess_testing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py` & `cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py` & `cengal-3.1.18.9/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multithreading/__init__.py` & `cengal-3.1.18.9/cengal/parallel_execution/multithreading/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/parallel_execution/multithreading/thread_workers_pool.py` & `cengal-3.1.18.9/cengal/parallel_execution/multithreading/thread_workers_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/performance_test_lib.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/performance_test_lib.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py` & `cengal-3.1.18.9/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/shared_memory/__init__.py` & `cengal-3.1.18.9/cengal/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/shared_memory/versions/1/__init__.py` & `cengal-3.1.18.9/cengal/shared_memory/versions/1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/shared_memory/versions/1/mmap.py` & `cengal-3.1.18.9/cengal/shared_memory/versions/1/mmap.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/shared_memory/versions/__init__.py` & `cengal-3.1.18.9/cengal/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/__init__.py` & `cengal-3.1.18.9/cengal/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/__init__.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/__init__.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/system.py` & `cengal-3.1.18.9/cengal/system.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/testing_lib/__init__.py` & `cengal-3.1.18.9/cengal/testing_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/testing_lib/tests_list_runner.py` & `cengal-3.1.18.9/cengal/testing_lib/tests_list_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/brackets.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/processing.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/help_tools.py` & `cengal-3.1.18.9/cengal/text_processing/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/simple.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/processing.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/text_translator/versions/v_0/text_translator.py` & `cengal-3.1.18.9/cengal/text_processing/text_translator/versions/v_0/text_translator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py` & `cengal-3.1.18.9/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/__init__.py` & `cengal-3.1.18.9/cengal/time_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.c` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/__init__.py` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.c` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/load_best_timer/__init__.py` & `cengal-3.1.18.9/cengal/time_management/load_best_timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py` & `cengal-3.1.18.9/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/constants/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/constants/versions/v_0/constants.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py` & `cengal-3.1.18.9/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/__init__.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.c` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.c`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py` & `cengal-3.1.18.9/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/__init__.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_0/timer.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_0/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/tests/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer/versions/v_1/timer.py` & `cengal-3.1.18.9/cengal/time_management/timer/versions/v_1/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/versions/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_1/__init__.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/time_management/timer_precision/versions/v_1/timer_precision.py` & `cengal-3.1.18.9/cengal/time_management/timer_precision/versions/v_1/timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/__init__.py` & `cengal-3.1.18.9/cengal/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/__init__.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/__init__.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py` & `cengal-3.1.18.9/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/__init__.py` & `cengal-3.1.18.9/cengal/unittest/patcher/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/versions/__init__.py` & `cengal-3.1.18.9/cengal/unittest/patcher/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/patcher.py` & `cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py` & `cengal-3.1.18.9/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/__init__.py` & `cengal-3.1.18.9/cengal/universal_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/help_tools.py` & `cengal-3.1.18.9/cengal/universal_parser/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/idioms.py` & `cengal-3.1.18.9/cengal/universal_parser/idioms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/parser.py` & `cengal-3.1.18.9/cengal/universal_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/test.py` & `cengal-3.1.18.9/cengal/universal_parser/test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/universal_parser/types.py` & `cengal-3.1.18.9/cengal/universal_parser/types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/upk_helping_tools/__init__.py` & `cengal-3.1.18.9/cengal/upk_helping_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/upk_helping_tools/upk_api.py` & `cengal-3.1.18.9/cengal/upk_helping_tools/upk_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/upk_helping_tools/upk_constants.py` & `cengal-3.1.18.9/cengal/upk_helping_tools/upk_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/upk_helping_tools/upk_utils_api.py` & `cengal-3.1.18.9/cengal/upk_helping_tools/upk_utils_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/chooser.py` & `cengal-3.1.18.9/cengal/user_interface/console/chooser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/colorama_helpers.py` & `cengal-3.1.18.9/cengal/user_interface/console/colorama_helpers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/encoding_changer.py` & `cengal-3.1.18.9/cengal/user_interface/console/encoding_changer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/progress_meter/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/console/progress_meter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py` & `cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py` & `cengal-3.1.18.9/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/versions/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/plot/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/plot.py` & `cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/plot.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.9/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal/web_tools/help_tools.py` & `cengal-3.1.18.9/cengal/web_tools/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal.egg-info/PKG-INFO` & `cengal-3.1.18.9/cengal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.1.18.8
+Version: 3.1.18.9
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cengal-3.1.18.8/cengal.egg-info/SOURCES.txt` & `cengal-3.1.18.9/cengal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/__init__.py` & `cengal-3.1.18.9/cengal_setup_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/compile_all_cython_modules.py` & `cengal-3.1.18.9/cengal_setup_scripts/compile_all_cython_modules.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py` & `cengal-3.1.18.9/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py` & `cengal-3.1.18.9/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from cengal.build_tools.prepare_cflags import prepare_cflags, concat_cflags, prepare_compile_time_env
 from cengal.introspection.inspect import get_exception
 from cengal.system import OS_TYPE, TEMPLATE_MODULE_NAME
 from shutil import rmtree
 from os import remove
 from os.path import splitext, normpath, join as path_join, basename, splitext
 from setuptools import Extension
-from distutils.command.build import build as build_orig
+from distutils.command.build_ext import build_ext as build_ext_orig
 import json
 import importlib
 
 
 BUILD_CONFIG_FILENAME: str = '__build_config.py'
 
 
@@ -203,15 +203,16 @@
             result.append(extension)
         else:
             result.extend(sub_result)
     
     return result
 
 
-class build(build_orig):
+class build_ext(build_ext_orig):
     def finalize_options(self):
         super().finalize_options()
         from Cython.Build import cythonize
         self.distribution.ext_modules = cythonize(self.distribution.ext_modules,
                                                   compiler_directives={'language_level': '3'},
                                                   compile_time_env = prepare_compile_time_env(),
                                                   )
+        k = 12 + 40
```

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/__init__.py` & `cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/install_packages.py` & `cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/install_packages.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/install_required_packages/set_environment_variables.py` & `cengal-3.1.18.9/cengal_setup_scripts/install_required_packages/set_environment_variables.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/setup__dynamic_list_of_pieces.py` & `cengal-3.1.18.9/cengal_setup_scripts/setup__dynamic_list_of_pieces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/setup__recv_buff_size_computer.py` & `cengal-3.1.18.9/cengal_setup_scripts/setup__recv_buff_size_computer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/cengal_setup_scripts/setup__repeat_for_a_time.py` & `cengal-3.1.18.9/cengal_setup_scripts/setup__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.8/setup.py` & `cengal-3.1.18.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "3.1.18.8"
+__version__ = "3.1.18.9"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
 
 from os import environ
@@ -70,15 +70,15 @@
 
 
 setuptools._install_setup_requires({'setup_requires': ['py-cpuinfo', 'Cython']})
 
 
 from cengal_setup_scripts.install_required_packages.install_packages import install_bundled, get_pypi_requirements_list, get_remote_requirements_list
 install_bundled()
-from cengal_setup_scripts.find_and_prepare_cython_modules import find_and_prepare_cython_modules, build
+from cengal_setup_scripts.find_and_prepare_cython_modules import find_and_prepare_cython_modules, build_ext
 from cengal.file_system.path_manager import path_relative_to_src
 from Cython.Build import cythonize
 
 
 with open(path_relative_to_src('README.md'), 'r') as fh:
     long_description = fh.read()
 
@@ -205,9 +205,9 @@
     python_requires='>=3.7',
     ext_modules=find_and_prepare_cython_modules(),
     # ext_modules=cythonize(
     #     find_and_prepare_cython_modules(),
     #     compiler_directives={'language_level': '3'},
     #     compile_time_env = prepare_compile_time_env(),
     # ),
-    cmdclass={"build": build},
+    cmdclass={"build_ext": build_ext},
 )
```

