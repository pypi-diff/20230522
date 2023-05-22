# Comparing `tmp/wiliot-deployment-tools-4.0.0.tar.gz` & `tmp/wiliot-deployment-tools-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.0.tar", last modified: Thu Mar  2 08:11:54 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.3.tar", last modified: Mon May 22 14:49:11 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.0.tar` & `wiliot-deployment-tools-4.0.3.tar`

### file list

```diff
@@ -1,57 +1,67 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2286 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1768 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7436 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/ci.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.574861 wiliot-deployment-tools-4.0.0/wiliot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_core/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_core/local_gateway/
--rw-rw-rw-   0 root         (0) root         (0)    12777 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_core/local_gateway/continuous_listener.py
--rw-rw-rw-   0 root         (0) root         (0)    12777 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_core/local_gateway/custom_energy_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     8151 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_core/update_wiliot_packages.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.574861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/configs/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/configs/.default_surfaces.json
--rw-rw-rw-   0 root         (0) root         (0)     4468 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/get_temperature_sensor_name.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/sample_test_calib_offline.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/utils/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/sample/utils/edit.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/arduino_counter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/arduino_counter/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/arduino_counter/arduino_counter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/configs/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/configs/inlay_data.py
--rw-rw-rw-   0 root         (0) root         (0)    17580 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_testers/yield/yield_tester.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.574861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.578861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/feature_flags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.582861 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/
--rw-rw-rw-   0 root         (0) root         (0)   229471 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/4.0.3_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   424656 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/4.0.3_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   229471 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/4.0.4_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   424656 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)  1176930 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot/wiliot_tools/local_gateway_gui/local_gateway_versions/wifi_4.0.4.hex
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-03-02 08:11:36.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-02 08:11:54.586861 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2286 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-02 08:11:54.000000 wiliot-deployment-tools-4.0.0/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.293935 wiliot-deployment-tools-4.0.3/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.297935 wiliot-deployment-tools-4.0.3/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41546 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/api/gw_ssid.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15155 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26163 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.305935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-22 14:48:54.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 14:49:11.301935 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-22 14:49:11.000000 wiliot-deployment-tools-4.0.3/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.0/LICENSE` & `wiliot-deployment-tools-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.0/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.3/bitbucket-pipelines.yml`

 * *Files 18% similar despite different names*

```diff
@@ -64,78 +64,101 @@
             - apk add tree
             #print current version:
             - python3 wiliot_deployment_tools/utils/get_version.py
             #Update patch version by git tag:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py next_patch`" && echo $version && git tag -a -m "[skip ci] build number $BITBUCKET_BUILD_NUMBER set the library patch version to $version." $version  && git push origin $version
             #print new version
             - python3 wiliot_deployment_tools/utils/get_version.py
-
-    publish-full-version-into-codearfact:
+    
+    publish-full-version-into-old-codeartifact:
       - step:
-          name: Build and publish full version py-wilot into codeartifact
+          name: Build and publish internal version into codeartifact
           <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm
+            - pip3 install setuptools_scm build wheel twine
             - pip3 install gitpython
             # get updated version number:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
-            # update minor version:
-            - python3 setup.py sdist bdist_wheel
-            #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
+            # build python package:
+            - python3 -m build -C internal
+            # update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
             - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
             - twine upload --repository codeartifact dist/*
 
+    publish-full-version-into-new-codeartifact:
+      - step:
+          name: Build and publish internal version into codeartifact
+          image:
+            name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
+            aws:
+              access-key: $CLOUD_AWS_ACCESS_KEY_ID
+              secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
+          script:
+            - pip3 install setuptools_scm build wheel twine
+            - pip3 install gitpython
+            # get updated version number:
+            - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
+            # build python package:
+            - python3 -m build -C internal
+            # update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
+            - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
+            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
+            - twine upload --repository codeartifact dist/*
+
     publish-slim-version-into-pypi:
       - step:
-          name: Build and publish slim version py-wilot into pypi
+          name: Build and publish slim version into pypi
           <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm
+            - pip3 install setuptools_scm build
             - pip3 install gitpython
             - apk add tree
             #Get current version (was already updated by prev steps) before cleaning internal files:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
             #update version.py with new patch version and build number:
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
             # configure testpypi and pypi access
             - echo "[pypi]" > ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $PYPI_KEY" >> ~/.pypirc && echo "[testpypi]" >> ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $TEST_PYPI_KEY" >> ~/.pypirc
             # cleanup all the "internal" folders
             - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
             - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
-            - python3 setup.py sdist bdist_wheel
+            - python3 -m build
             #Logging(?):
-            - ls -al dist/ && ls -al build/
+            - ls -al dist/
             # push into pypi
             - python3 -m twine upload --repository pypi dist/* #python3 -m twine upload --repository testpypi dist/*
 
     publish-slim-version-into-test-pypi:
       - step:
-          name: Build and publish slim version py-wilot into test-pypi
+          name: Build and publish slim version into test-pypi
           <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm
+            - pip3 install setuptools_scm build twine
             - pip3 install gitpython
             - apk add tree
             # configure testpypi and pypi access
             - echo "[testpypi]" >> ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $TEST_PYPI_KEY" >> ~/.pypirc
             # get updated version- before cleaning internal trees:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
             #update version.py with new patch version and build number:
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
             #Print version to log:
             - cat wiliot_deployment_tools/version.py
             # cleanup all the "internal" folders
             - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
             - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
-            - python3 setup.py sdist bdist_wheel
-            - ls -al dist/ && ls -al build/
+            - python3 -m build
+            - ls -al dist/
             # push into test-pypi
             - python3 -m twine upload --repository testpypi dist/*
 
     run-unit-tests:
       - step:
           name: Run unit tests
           <<: *wiliot-ci-image
```

### Comparing `wiliot-deployment-tools-4.0.0/ci.py` & `wiliot-deployment-tools-4.0.3/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.0/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.3/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

