# Comparing `tmp/IntuneCD-1.4.5b2.tar.gz` & `tmp/IntuneCD-1.4.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.5b2.tar", last modified: Thu Apr 27 08:51:02 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.6b1.tar", last modified: Mon May 22 06:52:59 2023, max compression
```

## Comparing `IntuneCD-1.4.5b2.tar` & `IntuneCD-1.4.6b1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.989494 IntuneCD-1.4.5b2/
--rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/LICENSE
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-27 08:51:02.989621 IntuneCD-1.4.5b2/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.5b2/README.md
--rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b2/pyproject.toml
--rw-r--r--   0 tobias     (501) staff       (20)      999 2023-04-27 08:51:02.989988 IntuneCD-1.4.5b2/setup.cfg
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.959068 IntuneCD-1.4.5b2/src/
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.983938 IntuneCD-1.4.5b2/src/IntuneCD/
--rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b2/src/IntuneCD/__init__.py
--rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-04-26 08:18:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.5b2/src/IntuneCD/assignment_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-04-24 14:54:23.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-04-24 14:55:45.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_apns.py
--rw-r--r--   0 tobias     (501) staff       (20)     2665 2023-04-24 14:48:58.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-04-24 15:05:44.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-04-24 14:59:21.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_applications.py
--rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-04-24 15:09:16.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-04-24 15:00:03.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-04-24 15:11:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-04-24 15:17:25.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-04-24 15:16:50.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-04-24 15:16:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-04-24 15:01:01.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-04-24 15:08:23.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-04-24 15:07:34.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-04-24 15:04:54.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-04-24 15:09:54.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-04-24 15:10:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-04-24 15:11:43.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-04-24 15:02:06.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-04-24 15:14:33.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-04-24 15:13:25.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-04-26 06:18:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-04-24 15:12:12.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-04-24 15:15:17.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-04-24 14:57:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-04-24 15:06:47.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b2/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-04-03 08:56:31.000000 IntuneCD-1.4.5b2/src/IntuneCD/graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-04-26 06:19:45.000000 IntuneCD-1.4.5b2/src/IntuneCD/graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      987 2023-04-25 09:24:15.000000 IntuneCD-1.4.5b2/src/IntuneCD/remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-04-26 06:16:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_backup.py
--rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_documentation.py
--rw-r--r--   0 tobias     (501) staff       (20)    11471 2023-04-26 11:47:47.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_update.py
--rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.5b2/src/IntuneCD/save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     8178 2023-04-26 11:50:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     7963 2023-04-26 11:50:51.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_assignment.py
--rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 tobias     (501) staff       (20)     9372 2023-04-26 11:51:00.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     7193 2023-04-26 11:51:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     7703 2023-04-26 11:51:17.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     8929 2023-04-26 11:51:24.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)    11648 2023-04-26 11:51:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     8715 2023-04-26 11:51:43.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_frontend.py
--rw-r--r--   0 tobias     (501) staff       (20)    24286 2023-04-26 11:51:50.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     9069 2023-04-26 11:51:58.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     8066 2023-04-26 11:52:05.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     8428 2023-04-26 11:52:12.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)    10612 2023-04-26 11:52:18.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)    16112 2023-04-26 11:52:24.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     8385 2023-04-26 11:52:32.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     7197 2023-04-26 11:52:39.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.985094 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 tobias     (501) staff       (20)        1 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 tobias     (501) staff       (20)      179 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 tobias     (501) staff       (20)      102 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 tobias     (501) staff       (20)        9 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.989311 IntuneCD-1.4.5b2/tests/
--rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-04-26 06:14:42.000000 IntuneCD-1.4.5b2/tests/test_archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b2/tests/test_documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_get_added_removed.py
--rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.5b2/tests/test_graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)    17428 2023-04-27 08:46:23.000000 IntuneCD-1.4.5b2/tests/test_graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.5b2/tests/test_group_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_match.py
--rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_update_frontend.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992976 IntuneCD-1.4.6b1/
+-rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/LICENSE
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.993116 IntuneCD-1.4.6b1/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.6b1/README.md
+-rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/pyproject.toml
+-rw-r--r--   0 tobias     (501) staff       (20)      999 2023-05-22 06:52:59.993592 IntuneCD-1.4.6b1/setup.cfg
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.958227 IntuneCD-1.4.6b1/src/
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.987295 IntuneCD-1.4.6b1/src/IntuneCD/
+-rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3001 2023-05-22 06:37:51.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-05-16 06:42:29.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      987 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11471 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.6b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7900 2023-05-22 06:40:42.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7963 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9372 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7193 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7703 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8929 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11648 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8715 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 tobias     (501) staff       (20)    24286 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9069 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8066 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10612 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    16118 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8385 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7197 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.988462 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        1 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      179 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      102 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        9 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992787 IntuneCD-1.4.6b1/tests/
+-rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_added_removed.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.6b1/tests/test_graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)    17428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.6b1/tests/test_group_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_match.py
+-rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.5b2/LICENSE` & `IntuneCD-1.4.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/PKG-INFO` & `IntuneCD-1.4.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.5b2
+Version: 1.4.6b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.5b2/README.md` & `IntuneCD-1.4.6b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/setup.cfg` & `IntuneCD-1.4.6b1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.5.beta2
+version = 1.4.6.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/archive.py` & `IntuneCD-1.4.6b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 
 """
 This module backs up all App Configuration Polices in Intune.
 """
 
+import base64
+import json
+
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .graph_batch import batch_assignment, get_object_assignment
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = (
-    "https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations"
-)
+ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations"
 APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
 
 
 # Get all App Configuration policies and save them in specified path
 def savebackup(path, output, exclude, token):
     """
     Saves all App Configuration policies in Intune to a JSON or YAML file.
@@ -29,17 +30,15 @@
     """
 
     results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "App Configuration/"
     data = makeapirequest(ENDPOINT, token)
 
     if data["value"]:
-        assignment_responses = batch_assignment(
-            data, "deviceAppManagement/mobileAppConfigurations/", "/assignments", token
-        )
+        assignment_responses = batch_assignment(data, "deviceAppManagement/mobileAppConfigurations/", "/assignments", token)
 
         for profile in data["value"]:
             results["config_count"] += 1
             if "assignments" not in exclude:
                 assignments = get_object_assignment(profile["id"], assignment_responses)
                 if assignments:
                     profile["assignments"] = assignments
@@ -54,20 +53,25 @@
                     app_dict["appName"] = app_data["displayName"]
                     app_dict["type"] = app_data["@odata.type"]
 
             if app_dict:
                 profile.pop("targetedMobileApps")
                 profile["targetedMobileApps"] = app_dict
 
+            if profile.get("payloadJson"):
+                try:
+                    profile["payloadJson"] = base64.b64decode(profile["payloadJson"]).decode("utf-8")
+                    profile["payloadJson"] = json.loads(profile["payloadJson"])
+                except Exception:
+                    print("Unable to decode payloadJson for " + profile["displayName"])
+
             print("Backing up App Configuration: " + profile["displayName"])
 
             # Get filename without illegal characters
-            fname = clean_filename(
-                f"{profile['displayName']}_{str(profile['@odata.type'].split('.')[2])}"
-            )
+            fname = clean_filename(f"{profile['displayName']}_{str(profile['@odata.type'].split('.')[2])}")
             # Save App Configuration as JSON or YAML depending on configured value
             # in "-o"
             save_output(output, configpath, fname, profile)
 
             results["outputs"].append(fname)
 
     return results
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/check_file.py` & `IntuneCD-1.4.6b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/load_file.py` & `IntuneCD-1.4.6b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/run_update.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/save_output.py` & `IntuneCD-1.4.6b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-This module is used to update all App Configuration Assignments in Intune.
+This module is used to update all App Protection Policies in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
 from .graph_request import (
@@ -18,180 +18,175 @@
 from .update_assignment import update_assignment, post_assignment_update
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 from .check_file import check_file
 from .load_file import load_file
 
 # Set MS Graph endpoint
-ENDPOINT = (
-    "https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations"
-)
-APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
+ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/"
 
 
 def update(
     path, token, assignment=False, report=False, create_groups=False, remove=False
 ):
     """
-    This function updates all App Configuration Polices in Intune,
+    This function updates all App Protection Polices in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
 
+    # Set App Protection path
+    configpath = path + "/" + "App Protection/"
     diff_summary = []
-    # Set App Configuration path
-    configpath = path + "/" + "App Configuration/"
     # If App Configuration path exists, continue
     if os.path.exists(configpath):
-        # Get App Configurations
-        mem_data = makeapirequest(ENDPOINT, token)
+        # Get App Protections
+        mem_data = makeapirequest(f"{ENDPOINT}managedAppPolicies", token)
         # Get current assignments
         mem_assignments = batch_assignment(
-            mem_data,
-            "deviceAppManagement/mobileAppConfigurations/",
-            "/assignments",
-            token,
+            mem_data, "deviceAppManagement/", "/assignments", token, app_protection=True
         )
 
         for filename in os.listdir(configpath):
             file = check_file(configpath, filename)
             if file is False:
                 continue
-
             # Check which format the file is saved as then open file, load data
             # and set query parameter
             with open(file) as f:
                 repo_data = load_file(filename, f)
+
+                if repo_data:
+                    if (
+                        repo_data["@odata.type"]
+                        == "#microsoft.graph.mdmWindowsInformationProtectionPolicy"
+                    ):
+                        platform = "mdmWindowsInformationProtectionPolicies"
+                    elif (
+                        repo_data["@odata.type"]
+                        == "#microsoft.graph.windowsInformationProtectionPolicy"
+                    ):
+                        platform = "windowsInformationProtectionPolicies"
+                    else:
+                        platform = f"{str(repo_data['@odata.type']).split('.')[2]}s"
+
                 # Create object to pass in to assignment function
                 assign_obj = {}
                 if "assignments" in repo_data:
                     assign_obj = repo_data["assignments"]
                 repo_data.pop("assignments", None)
 
-                # If App Configuration exists, continue
+                # If App Protection exists, continue
                 data = {"value": ""}
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if (
+                            "targetedAppManagementLevels" in val
+                            and "targetedAppManagementLevels" in repo_data
+                        ):
+                            if (
+                                repo_data["targetedAppManagementLevels"]
+                                == val["targetedAppManagementLevels"]
+                                and repo_data["displayName"] == val["displayName"]
+                            ):
+                                data["value"] = val
+                                mem_data["value"].remove(val)
+                        elif (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
                             mem_data["value"].remove(val)
 
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
-                    data = remove_keys(data)
-                    repo_data.pop("targetedMobileApps", None)
+                    data["value"] = remove_keys(data["value"])
 
                     diff = DeepDiff(data["value"], repo_data, ignore_order=True).get(
                         "values_changed", {}
                     )
 
                     # If any changed values are found, push them to Intune
                     if diff and report is False:
                         request_data = json.dumps(repo_data)
                         q_param = None
                         makeapirequestPatch(
-                            ENDPOINT + "/" + mem_id,
+                            f"{ENDPOINT}{platform}/{mem_id}",
                             token,
                             q_param,
                             request_data,
                             status_code=204,
                         )
 
                     diff_config = DiffSummary(
                         data=diff,
                         name=repo_data["displayName"],
-                        type="App Configuration",
+                        type="App Protection",
                     )
-
                     diff_summary.append(diff_config)
 
                     if assignment:
                         mem_assign_obj = get_object_assignment(mem_id, mem_assignments)
                         update = update_assignment(
                             assign_obj, mem_assign_obj, token, create_groups
                         )
                         if update is not None:
                             request_data = {"assignments": update}
                             post_assignment_update(
                                 request_data,
                                 mem_id,
-                                "deviceAppManagement/mobileAppConfigurations/",
-                                "/microsoft.graph.managedDeviceMobileAppConfiguration/assign",
+                                f"deviceAppManagement/{platform}",
+                                "assign",
                                 token,
+                                status_code=204,
                             )
 
-                # If App Configuration does not exist, create it and assign
+                # If App Protection does not exist, create it and assign
                 else:
                     print("-" * 90)
                     print(
-                        "App Configuration not found, creating: "
+                        "App Protection not found, creating policy: "
                         + repo_data["displayName"]
                     )
-                    app_ids = {}
-                    # If backup contains targeted apps, search for the app
-                    if repo_data["targetedMobileApps"]:
-                        q_param = {
-                            "$filter": "(isof("
-                            + "'"
-                            + str(repo_data["targetedMobileApps"]["type"]).replace(
-                                "#", ""
-                            )
-                            + "'"
-                            + "))",
-                            "$search": repo_data["targetedMobileApps"]["appName"],
-                        }
-                        app_request = makeapirequest(APP_ENDPOINT, token, q_param)
-                        if app_request["value"]:
-                            app_ids = app_request["value"][0]["id"]
-                    # If the app could be found and matches type and name in
-                    # backup, continue to create
-                    if app_ids and report is False:
-                        repo_data.pop("targetedMobileApps")
-                        repo_data["targetedMobileApps"] = [app_ids]
+                    if report is False:
                         request_json = json.dumps(repo_data)
                         post_request = makeapirequestPost(
-                            ENDPOINT,
+                            f"{ENDPOINT}managedAppPolicies",
                             token,
                             q_param=None,
                             jdata=request_json,
                             status_code=201,
                         )
                         mem_assign_obj = []
                         assignment = update_assignment(
                             assign_obj, mem_assign_obj, token, create_groups
                         )
                         if assignment is not None:
                             request_data = {"assignments": assignment}
                             post_assignment_update(
                                 request_data,
                                 post_request["id"],
-                                "deviceAppManagement/mobileAppConfigurations/",
-                                "/microsoft.graph.managedDeviceMobileAppConfiguration/assign",
+                                f"deviceAppManagement/{platform}",
+                                "assign",
                                 token,
+                                status_code=204,
                             )
-                        print(
-                            "App Configuration created with id: " + post_request["id"]
-                        )
-                    else:
-                        print(
-                            "App configured in App Configuration profile could not be found, skipping creation"
-                        )
+                        print("App Protection created with id: " + post_request["id"])
 
-        # If any App Configurations are left in mem_data, remove them from Intune as they are not in the repo
+        # If any App Protections are left in mem_data, remove them from Intune as they are not in the repo
         if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
-                print("Removing App Configuration from Intune: " + val["displayName"])
+                print("Removing App Protection from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
-                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                        f"{ENDPOINT}managedAppPolicies/{val['id']}",
+                        token,
+                        status_code=204,
                     )
 
     return diff_summary
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,192 +1,186 @@
-#!/usr/bin/env python3
-
-"""
-This module is used to update all App Protection Policies in Intune.
-"""
-
-import json
-import os
-
-from deepdiff import DeepDiff
-from .graph_request import (
-    makeapirequest,
-    makeapirequestPatch,
-    makeapirequestPost,
-    makeapirequestDelete,
-)
-from .graph_batch import batch_assignment, get_object_assignment
-from .update_assignment import update_assignment, post_assignment_update
-from .remove_keys import remove_keys
-from .diff_summary import DiffSummary
-from .check_file import check_file
-from .load_file import load_file
-
-# Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/"
-
-
-def update(
-    path, token, assignment=False, report=False, create_groups=False, remove=False
-):
-    """
-    This function updates all App Protection Polices in Intune,
-    if the configuration in Intune differs from the JSON/YAML file.
-
-    :param path: Path to where the backup is saved
-    :param token: Token to use for authenticating the request
-    :param assignment: Boolean to determine if assignments should be updated
-    """
-
-    # Set App Protection path
-    configpath = path + "/" + "App Protection/"
-    diff_summary = []
-    # If App Configuration path exists, continue
-    if os.path.exists(configpath):
-        # Get App Protections
-        mem_data = makeapirequest(f"{ENDPOINT}managedAppPolicies", token)
-        # Get current assignments
-        mem_assignments = batch_assignment(
-            mem_data, "deviceAppManagement/", "/assignments", token, app_protection=True
-        )
-
-        for filename in os.listdir(configpath):
-            file = check_file(configpath, filename)
-            if file is False:
-                continue
-            # Check which format the file is saved as then open file, load data
-            # and set query parameter
-            with open(file) as f:
-                repo_data = load_file(filename, f)
-
-                if repo_data:
-                    if (
-                        repo_data["@odata.type"]
-                        == "#microsoft.graph.mdmWindowsInformationProtectionPolicy"
-                    ):
-                        platform = "mdmWindowsInformationProtectionPolicies"
-                    elif (
-                        repo_data["@odata.type"]
-                        == "#microsoft.graph.windowsInformationProtectionPolicy"
-                    ):
-                        platform = "windowsInformationProtectionPolicies"
-                    else:
-                        platform = f"{str(repo_data['@odata.type']).split('.')[2]}s"
-
-                # Create object to pass in to assignment function
-                assign_obj = {}
-                if "assignments" in repo_data:
-                    assign_obj = repo_data["assignments"]
-                repo_data.pop("assignments", None)
-
-                # If App Protection exists, continue
-                data = {"value": ""}
-                if mem_data["value"]:
-                    for val in mem_data["value"]:
-                        if (
-                            "targetedAppManagementLevels" in val
-                            and "targetedAppManagementLevels" in repo_data
-                        ):
-                            if (
-                                repo_data["targetedAppManagementLevels"]
-                                == val["targetedAppManagementLevels"]
-                                and repo_data["displayName"] == val["displayName"]
-                            ):
-                                data["value"] = val
-                                mem_data["value"].remove(val)
-                        elif (
-                            repo_data["@odata.type"] == val["@odata.type"]
-                            and repo_data["displayName"] == val["displayName"]
-                        ):
-                            data["value"] = val
-                            mem_data["value"].remove(val)
-
-                if data["value"]:
-                    print("-" * 90)
-                    mem_id = data["value"]["id"]
-                    # Remove keys before using DeepDiff
-                    data["value"] = remove_keys(data["value"])
-
-                    diff = DeepDiff(data["value"], repo_data, ignore_order=True).get(
-                        "values_changed", {}
-                    )
-
-                    # If any changed values are found, push them to Intune
-                    if diff and report is False:
-                        request_data = json.dumps(repo_data)
-                        q_param = None
-                        makeapirequestPatch(
-                            f"{ENDPOINT}{platform}/{mem_id}",
-                            token,
-                            q_param,
-                            request_data,
-                            status_code=204,
-                        )
-
-                    diff_config = DiffSummary(
-                        data=diff,
-                        name=repo_data["displayName"],
-                        type="App Protection",
-                    )
-                    diff_summary.append(diff_config)
-
-                    if assignment:
-                        mem_assign_obj = get_object_assignment(mem_id, mem_assignments)
-                        update = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
-                        if update is not None:
-                            request_data = {"assignments": update}
-                            post_assignment_update(
-                                request_data,
-                                mem_id,
-                                f"deviceAppManagement/{platform}",
-                                "assign",
-                                token,
-                                status_code=204,
-                            )
-
-                # If App Protection does not exist, create it and assign
-                else:
-                    print("-" * 90)
-                    print(
-                        "App Protection not found, creating policy: "
-                        + repo_data["displayName"]
-                    )
-                    if report is False:
-                        request_json = json.dumps(repo_data)
-                        post_request = makeapirequestPost(
-                            f"{ENDPOINT}managedAppPolicies",
-                            token,
-                            q_param=None,
-                            jdata=request_json,
-                            status_code=201,
-                        )
-                        mem_assign_obj = []
-                        assignment = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
-                        if assignment is not None:
-                            request_data = {"assignments": assignment}
-                            post_assignment_update(
-                                request_data,
-                                post_request["id"],
-                                f"deviceAppManagement/{platform}",
-                                "assign",
-                                token,
-                                status_code=204,
-                            )
-                        print("App Protection created with id: " + post_request["id"])
-
-        # If any App Protections are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None and remove is True:
-            for val in mem_data["value"]:
-                print("-" * 90)
-                print("Removing App Protection from Intune: " + val["displayName"])
-                if report is False:
-                    makeapirequestDelete(
-                        f"{ENDPOINT}managedAppPolicies/{val['id']}",
-                        token,
-                        status_code=204,
-                    )
-
-    return diff_summary
+#!/usr/bin/env python3
+
+"""
+This module is used to update all Settings Catalog assignments in Intune,
+"""
+
+import json
+import os
+
+from deepdiff import DeepDiff
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPut,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
+from .graph_batch import batch_assignment, get_object_assignment
+from .update_assignment import update_assignment, post_assignment_update
+from .check_file import check_file
+from .load_file import load_file
+from .diff_summary import DiffSummary
+
+# Set MS Graph endpoint
+ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/configurationPolicies"
+
+
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
+    """
+    This function updates all Settings Catalog configurations in Intune,
+    if the configuration in Intune differs from the JSON/YAML file.
+
+    :param path: Path to where the backup is saved
+    :param token: Token to use for authenticating the request
+    :param assignment: Boolean to determine if assignments should be updated
+    """
+
+    diff_summary = []
+    # Set Settings Catalog path
+    configpath = path + "/" + "Settings Catalog/"
+
+    if os.path.exists(configpath):
+        # Get configurations policies
+        mem_data = makeapirequest(ENDPOINT, token)
+        # Get current assignments
+        mem_assignments = batch_assignment(
+            mem_data, "deviceManagement/configurationPolicies/", "/assignments", token
+        )
+
+        for filename in os.listdir(configpath):
+            file = check_file(configpath, filename)
+            if file is False:
+                continue
+            (name, ext) = os.path.splitext(filename)
+            # Check which format the file is saved as then open file, load data
+            # and set query parameter
+            with open(file) as f:
+                repo_data = load_file(filename, f)
+
+                # Create object to pass in to assignment function
+                assign_obj = {}
+                if "assignments" in repo_data:
+                    assign_obj = repo_data["assignments"]
+                repo_data.pop("assignments", None)
+
+                data = {"value": ""}
+                if mem_data["value"]:
+                    for val in mem_data["value"]:
+                        if repo_data["name"] == val["name"]:
+                            data["value"] = val
+                            mem_data["value"].remove(val)
+
+                if (
+                    "templateReference" in repo_data
+                    and repo_data["templateReference"].get("templateDisplayName")
+                    == "Endpoint detection and response"
+                ):
+                    print("-" * 90)
+                    print(
+                        f'Skipping "{repo_data["name"]}", Endpoint detection and response is currently not supported...',
+                    )
+                    continue
+
+                # If Filter exists, continue
+                if data["value"]:
+                    print("-" * 90)
+                    # Get Filter data from Intune
+                    mem_policy_data = makeapirequest(
+                        ENDPOINT + "/" + data["value"]["id"], token
+                    )
+                    # Get Filter settings from Intune
+                    mem_policy_settings = makeapirequest(
+                        ENDPOINT + "/" + data["value"]["id"] + "/settings", token
+                    )
+                    # Add settings to the data dictionary
+                    mem_policy_data["settings"] = mem_policy_settings["value"]
+
+                    diff = DeepDiff(mem_policy_data, repo_data, ignore_order=True).get(
+                        "values_changed", {}
+                    )
+
+                    # If any changed values are found, push them to Intune
+                    if diff and report is False:
+                        request_data = json.dumps(repo_data)
+                        q_param = None
+                        makeapirequestPut(
+                            ENDPOINT + "/" + data["value"]["id"],
+                            token,
+                            q_param,
+                            request_data,
+                            status_code=204,
+                        )
+
+                    diff_policy = DiffSummary(
+                        data=diff,
+                        name=repo_data["name"],
+                        type="Settings Catalog policy",
+                    )
+
+                    diff_summary.append(diff_policy)
+
+                    if assignment:
+                        mem_assign_obj = get_object_assignment(
+                            data["value"]["id"], mem_assignments
+                        )
+                        update = update_assignment(
+                            assign_obj, mem_assign_obj, token, create_groups
+                        )
+                        if update is not None:
+                            request_data = {"assignments": update}
+                            post_assignment_update(
+                                request_data,
+                                data["value"]["id"],
+                                "deviceManagement/configurationPolicies",
+                                "assign",
+                                token,
+                            )
+
+                # If Configuration Policy does not exist, create it and assign
+                else:
+                    print("-" * 90)
+                    print(
+                        "Configuration Policy not found, creating Policy: "
+                        + repo_data["name"]
+                    )
+                    if report is False:
+                        repo_data.pop("settingCount", None)
+                        repo_data.pop("creationSource", None)
+                        request_json = json.dumps(repo_data)
+                        post_request = makeapirequestPost(
+                            ENDPOINT,
+                            token,
+                            q_param=None,
+                            jdata=request_json,
+                            status_code=201,
+                        )
+                        mem_assign_obj = []
+                        assignment = update_assignment(
+                            assign_obj, mem_assign_obj, token, create_groups
+                        )
+                        if assignment is not None:
+                            request_data = {"assignments": assignment}
+                            post_assignment_update(
+                                request_data,
+                                post_request["id"],
+                                "deviceManagement/configurationPolicies",
+                                "assign",
+                                token,
+                            )
+                        print(
+                            "Configuration Policy created with id: "
+                            + post_request["id"]
+                        )
+
+        # If any Configuration Policies are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None and remove is True:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Configuration Policy from Intune: " + val["name"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
+    return diff_summary
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,186 +1,174 @@
-#!/usr/bin/env python3
-
-"""
-This module is used to update all Settings Catalog assignments in Intune,
-"""
-
-import json
-import os
-
-from deepdiff import DeepDiff
-from .graph_request import (
-    makeapirequest,
-    makeapirequestPut,
-    makeapirequestPost,
-    makeapirequestDelete,
-)
-from .graph_batch import batch_assignment, get_object_assignment
-from .update_assignment import update_assignment, post_assignment_update
-from .check_file import check_file
-from .load_file import load_file
-from .diff_summary import DiffSummary
-
-# Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/configurationPolicies"
-
-
-def update(
-    path, token, assignment=False, report=False, create_groups=False, remove=False
-):
-    """
-    This function updates all Settings Catalog configurations in Intune,
-    if the configuration in Intune differs from the JSON/YAML file.
-
-    :param path: Path to where the backup is saved
-    :param token: Token to use for authenticating the request
-    :param assignment: Boolean to determine if assignments should be updated
-    """
-
-    diff_summary = []
-    # Set Settings Catalog path
-    configpath = path + "/" + "Settings Catalog/"
-
-    if os.path.exists(configpath):
-        # Get configurations policies
-        mem_data = makeapirequest(ENDPOINT, token)
-        # Get current assignments
-        mem_assignments = batch_assignment(
-            mem_data, "deviceManagement/configurationPolicies/", "/assignments", token
-        )
-
-        for filename in os.listdir(configpath):
-            file = check_file(configpath, filename)
-            if file is False:
-                continue
-            (name, ext) = os.path.splitext(filename)
-            # Check which format the file is saved as then open file, load data
-            # and set query parameter
-            with open(file) as f:
-                repo_data = load_file(filename, f)
-
-                # Create object to pass in to assignment function
-                assign_obj = {}
-                if "assignments" in repo_data:
-                    assign_obj = repo_data["assignments"]
-                repo_data.pop("assignments", None)
-
-                data = {"value": ""}
-                if mem_data["value"]:
-                    for val in mem_data["value"]:
-                        if repo_data["name"] == val["name"]:
-                            data["value"] = val
-                            mem_data["value"].remove(val)
-
-                if (
-                    "templateReference" in repo_data
-                    and repo_data["templateReference"].get("templateDisplayName")
-                    == "Endpoint detection and response"
-                ):
-                    print("-" * 90)
-                    print(
-                        f'Skipping "{repo_data["name"]}", Endpoint detection and response is currently not supported...',
-                    )
-                    continue
-
-                # If Filter exists, continue
-                if data["value"]:
-                    print("-" * 90)
-                    # Get Filter data from Intune
-                    mem_policy_data = makeapirequest(
-                        ENDPOINT + "/" + data["value"]["id"], token
-                    )
-                    # Get Filter settings from Intune
-                    mem_policy_settings = makeapirequest(
-                        ENDPOINT + "/" + data["value"]["id"] + "/settings", token
-                    )
-                    # Add settings to the data dictionary
-                    mem_policy_data["settings"] = mem_policy_settings["value"]
-
-                    diff = DeepDiff(mem_policy_data, repo_data, ignore_order=True).get(
-                        "values_changed", {}
-                    )
-
-                    # If any changed values are found, push them to Intune
-                    if diff and report is False:
-                        request_data = json.dumps(repo_data)
-                        q_param = None
-                        makeapirequestPut(
-                            ENDPOINT + "/" + data["value"]["id"],
-                            token,
-                            q_param,
-                            request_data,
-                            status_code=204,
-                        )
-
-                    diff_policy = DiffSummary(
-                        data=diff,
-                        name=repo_data["name"],
-                        type="Settings Catalog policy",
-                    )
-
-                    diff_summary.append(diff_policy)
-
-                    if assignment:
-                        mem_assign_obj = get_object_assignment(
-                            data["value"]["id"], mem_assignments
-                        )
-                        update = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
-                        if update is not None:
-                            request_data = {"assignments": update}
-                            post_assignment_update(
-                                request_data,
-                                data["value"]["id"],
-                                "deviceManagement/configurationPolicies",
-                                "assign",
-                                token,
-                            )
-
-                # If Configuration Policy does not exist, create it and assign
-                else:
-                    print("-" * 90)
-                    print(
-                        "Configuration Policy not found, creating Policy: "
-                        + repo_data["name"]
-                    )
-                    if report is False:
-                        repo_data.pop("settingCount", None)
-                        repo_data.pop("creationSource", None)
-                        request_json = json.dumps(repo_data)
-                        post_request = makeapirequestPost(
-                            ENDPOINT,
-                            token,
-                            q_param=None,
-                            jdata=request_json,
-                            status_code=201,
-                        )
-                        mem_assign_obj = []
-                        assignment = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
-                        if assignment is not None:
-                            request_data = {"assignments": assignment}
-                            post_assignment_update(
-                                request_data,
-                                post_request["id"],
-                                "deviceManagement/configurationPolicies",
-                                "assign",
-                                token,
-                            )
-                        print(
-                            "Configuration Policy created with id: "
-                            + post_request["id"]
-                        )
-
-        # If any Configuration Policies are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None and remove is True:
-            for val in mem_data["value"]:
-                print("-" * 90)
-                print("Removing Configuration Policy from Intune: " + val["name"])
-                if report is False:
-                    makeapirequestDelete(
-                        f"{ENDPOINT}/{val['id']}", token, status_code=200
-                    )
-
-    return diff_summary
+#!/usr/bin/env python3
+
+"""
+This module is used to update all Windows Enrollment Profiles in Intune.
+"""
+
+import json
+import os
+
+from deepdiff import DeepDiff
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
+from .graph_batch import batch_assignment, get_object_assignment
+from .update_assignment import update_assignment, post_assignment_update
+from .check_file import check_file
+from .load_file import load_file
+from .remove_keys import remove_keys
+from .diff_summary import DiffSummary
+
+# Set MS Graph endpoint
+ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles"
+
+
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
+    """
+    This function updates all Windows Enrollment Profiles in Intune,
+    if the configuration in Intune differs from the JSON/YAML file.
+
+    :param path: Path to where the backup is saved
+    :param token: Token to use for authenticating the request
+    :param assignment: Boolean to determine if assignments should be updated
+    """
+
+    diff_summary = []
+    # Set Windows Enrollment Profile path
+    configpath = path + "/" + "Enrollment Profiles/Windows"
+    # If Windows Enrollment Profile path exists, continue
+    if os.path.exists(configpath):
+        # Get enrollment profiles
+        mem_data = makeapirequest(ENDPOINT, token)
+        # Get current assignment
+        mem_assignments = batch_assignment(
+            mem_data,
+            "deviceManagement/windowsAutopilotDeploymentProfiles/",
+            "/assignments",
+            token,
+        )
+
+        for filename in os.listdir(configpath):
+            file = check_file(configpath, filename)
+            if file is False:
+                continue
+            # Check which format the file is saved as then open file, load data
+            # and set query parameter
+            with open(file) as f:
+                repo_data = load_file(filename, f)
+
+                # Create object to pass in to assignment function
+                assign_obj = {}
+                if "assignments" in repo_data:
+                    assign_obj = repo_data["assignments"]
+                repo_data.pop("assignments", None)
+
+                data = {"value": ""}
+                if mem_data["value"]:
+                    for val in mem_data["value"]:
+                        if repo_data["displayName"] == val["displayName"]:
+                            data["value"] = val
+                            mem_data["value"].remove(val)
+
+                # If Windows Enrollment Profile exists, continue
+                if data["value"]:
+                    print("-" * 90)
+                    mem_id = data["value"]["id"]
+                    # Remove keys before using DeepDiff
+                    data["value"] = remove_keys(data["value"])
+
+                    diff = DeepDiff(data["value"], repo_data, ignore_order=True).get(
+                        "values_changed", {}
+                    )
+
+                    # If any changed values are found, push them to Intune
+                    if diff and report is False:
+                        if repo_data["managementServiceAppId"]:
+                            pass
+                        else:
+                            repo_data["managementServiceAppId"] = ""
+                        request_data = json.dumps(repo_data)
+                        q_param = None
+                        makeapirequestPatch(
+                            ENDPOINT + "/" + mem_id, token, q_param, request_data
+                        )
+
+                    diff_profile = DiffSummary(
+                        data=diff,
+                        name=repo_data["displayName"],
+                        type="Windows Enrollment Profile",
+                    )
+
+                    diff_summary.append(diff_profile)
+
+                    if assignment:
+                        mem_assign_obj = get_object_assignment(mem_id, mem_assignments)
+                        update = update_assignment(
+                            assign_obj, mem_assign_obj, token, create_groups
+                        )
+                        if update is not None:
+                            for target in update:
+                                request_data = {"target": target["target"]}
+                                post_assignment_update(
+                                    request_data,
+                                    mem_id,
+                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
+                                    "assignments",
+                                    token,
+                                    status_code=201,
+                                )
+
+                # If Autopilot profile does not exist, create it and assign
+                else:
+                    print("-" * 90)
+                    print(
+                        "Autopilot profile not found, creating profile: "
+                        + repo_data["displayName"]
+                    )
+                    if report is False:
+                        request_json = json.dumps(repo_data)
+                        post_request = makeapirequestPost(
+                            ENDPOINT,
+                            token,
+                            q_param=None,
+                            jdata=request_json,
+                            status_code=201,
+                        )
+                        mem_assign_obj = []
+                        assignment = update_assignment(
+                            assign_obj, mem_assign_obj, token, create_groups
+                        )
+                        if assignment is not None:
+                            for target in assignment:
+                                request_data = {"target": target["target"]}
+                                post_assignment_update(
+                                    request_data,
+                                    post_request["id"],
+                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
+                                    "assignments",
+                                    token,
+                                    status_code=201,
+                                )
+                        print(
+                            "Autopilot profile created with id: " + post_request["id"]
+                        )
+
+        # If any Windows Enrollment Profile are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None and remove is True:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Autopilot Profile from Intune: " + val["displayName"])
+                if report is False:
+                    # Remove assignments so we can delete the profile
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}/assignments", token, status_code=200
+                    )
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
+    return diff_summary
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,21 +63,14 @@
                 if "assignments" in repo_data:
                     assign_obj = repo_data["assignments"]
                 repo_data.pop("assignments", None)
 
                 # If Device Configuration exists, continue
                 data = {"value": ""}
                 if mem_data["value"]:
-                    # Updating Windows update rings is currently not supported
-                    if (
-                        repo_data["@odata.type"]
-                        == "#microsoft.graph.windowsUpdateForBusinessConfiguration"
-                    ):
-                        continue
-
                     for val in mem_data["value"]:
                         if (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
                             mem_data["value"].remove(val)
@@ -250,14 +243,21 @@
                                 ENDPOINT + "/" + mem_id,
                                 token,
                                 q_param,
                                 request_data,
                                 status_code=204,
                             )
 
+                    # Updating Windows update rings is currently not supported
+                    elif (
+                        data["value"]["@odata.type"]
+                        == "#microsoft.graph.windowsUpdateForBusinessConfiguration"
+                    ):
+                        continue
+
                     # If Device Configuration is not custom, compare the values
                     else:
                         diff = DeepDiff(
                             data["value"], repo_data, ignore_order=True
                         ).get("values_changed", {})
 
                         # If any changed values are found, push them to Intune
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,174 +1,179 @@
 #!/usr/bin/env python3
 
 """
-This module is used to update all Windows Enrollment Profiles in Intune.
+This module is used to update all App Configuration Assignments in Intune.
 """
 
 import json
 import os
+import base64
 
 from deepdiff import DeepDiff
 from .graph_request import (
     makeapirequest,
     makeapirequestPatch,
     makeapirequestPost,
     makeapirequestDelete,
 )
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
-from .check_file import check_file
-from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
+from .check_file import check_file
+from .load_file import load_file
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles"
+ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations"
+APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
 
 
-def update(
-    path, token, assignment=False, report=False, create_groups=False, remove=False
-):
+def update(path, token, assignment=False, report=False, create_groups=False, remove=False):
     """
-    This function updates all Windows Enrollment Profiles in Intune,
+    This function updates all App Configuration Polices in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
 
     diff_summary = []
-    # Set Windows Enrollment Profile path
-    configpath = path + "/" + "Enrollment Profiles/Windows"
-    # If Windows Enrollment Profile path exists, continue
+    # Set App Configuration path
+    configpath = path + "/" + "App Configuration/"
+    # If App Configuration path exists, continue
     if os.path.exists(configpath):
-        # Get enrollment profiles
+        # Get App Configurations
         mem_data = makeapirequest(ENDPOINT, token)
-        # Get current assignment
+        # Get current assignments
         mem_assignments = batch_assignment(
             mem_data,
-            "deviceManagement/windowsAutopilotDeploymentProfiles/",
+            "deviceAppManagement/mobileAppConfigurations/",
             "/assignments",
             token,
         )
 
         for filename in os.listdir(configpath):
             file = check_file(configpath, filename)
             if file is False:
                 continue
+
             # Check which format the file is saved as then open file, load data
             # and set query parameter
             with open(file) as f:
                 repo_data = load_file(filename, f)
-
                 # Create object to pass in to assignment function
                 assign_obj = {}
                 if "assignments" in repo_data:
                     assign_obj = repo_data["assignments"]
                 repo_data.pop("assignments", None)
 
+                # If App Configuration exists, continue
                 data = {"value": ""}
                 if mem_data["value"]:
                     for val in mem_data["value"]:
-                        if repo_data["displayName"] == val["displayName"]:
+                        if repo_data["@odata.type"] == val["@odata.type"] and repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
                             mem_data["value"].remove(val)
 
-                # If Windows Enrollment Profile exists, continue
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
-                    data["value"] = remove_keys(data["value"])
+                    data = remove_keys(data)
+                    repo_data.pop("targetedMobileApps", None)
 
-                    diff = DeepDiff(data["value"], repo_data, ignore_order=True).get(
-                        "values_changed", {}
-                    )
+                    if repo_data.get("payloadJson"):
+                        repo_data["payloadJson"] = base64.b64encode(
+                            json.dumps(repo_data["payloadJson"]).encode("utf-8")
+                        ).decode("utf-8")
+
+                    diff = DeepDiff(data["value"], repo_data, ignore_order=True).get("values_changed", {})
 
                     # If any changed values are found, push them to Intune
                     if diff and report is False:
-                        if repo_data["managementServiceAppId"]:
-                            pass
-                        else:
-                            repo_data["managementServiceAppId"] = ""
                         request_data = json.dumps(repo_data)
                         q_param = None
                         makeapirequestPatch(
-                            ENDPOINT + "/" + mem_id, token, q_param, request_data
+                            ENDPOINT + "/" + mem_id,
+                            token,
+                            q_param,
+                            request_data,
+                            status_code=204,
                         )
 
-                    diff_profile = DiffSummary(
+                    diff_config = DiffSummary(
                         data=diff,
                         name=repo_data["displayName"],
-                        type="Windows Enrollment Profile",
+                        type="App Configuration",
                     )
 
-                    diff_summary.append(diff_profile)
+                    diff_summary.append(diff_config)
 
                     if assignment:
                         mem_assign_obj = get_object_assignment(mem_id, mem_assignments)
-                        update = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
+                        update = update_assignment(assign_obj, mem_assign_obj, token, create_groups)
                         if update is not None:
-                            for target in update:
-                                request_data = {"target": target["target"]}
-                                post_assignment_update(
-                                    request_data,
-                                    mem_id,
-                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
-                                    "assignments",
-                                    token,
-                                    status_code=201,
-                                )
+                            request_data = {"assignments": update}
+                            post_assignment_update(
+                                request_data,
+                                mem_id,
+                                "deviceAppManagement/mobileAppConfigurations/",
+                                "/microsoft.graph.managedDeviceMobileAppConfiguration/assign",
+                                token,
+                            )
 
-                # If Autopilot profile does not exist, create it and assign
+                # If App Configuration does not exist, create it and assign
                 else:
                     print("-" * 90)
-                    print(
-                        "Autopilot profile not found, creating profile: "
-                        + repo_data["displayName"]
-                    )
-                    if report is False:
+                    print("App Configuration not found, creating: " + repo_data["displayName"])
+                    app_ids = {}
+                    # If backup contains targeted apps, search for the app
+                    if repo_data["targetedMobileApps"]:
+                        q_param = {
+                            "$filter": "(isof("
+                            + "'"
+                            + str(repo_data["targetedMobileApps"]["type"]).replace("#", "")
+                            + "'"
+                            + "))",
+                            "$search": repo_data["targetedMobileApps"]["appName"],
+                        }
+                        app_request = makeapirequest(APP_ENDPOINT, token, q_param)
+                        if app_request["value"]:
+                            app_ids = app_request["value"][0]["id"]
+                    # If the app could be found and matches type and name in
+                    # backup, continue to create
+                    if app_ids and report is False:
+                        repo_data.pop("targetedMobileApps")
+                        repo_data["targetedMobileApps"] = [app_ids]
                         request_json = json.dumps(repo_data)
                         post_request = makeapirequestPost(
                             ENDPOINT,
                             token,
                             q_param=None,
                             jdata=request_json,
                             status_code=201,
                         )
                         mem_assign_obj = []
-                        assignment = update_assignment(
-                            assign_obj, mem_assign_obj, token, create_groups
-                        )
+                        assignment = update_assignment(assign_obj, mem_assign_obj, token, create_groups)
                         if assignment is not None:
-                            for target in assignment:
-                                request_data = {"target": target["target"]}
-                                post_assignment_update(
-                                    request_data,
-                                    post_request["id"],
-                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
-                                    "assignments",
-                                    token,
-                                    status_code=201,
-                                )
-                        print(
-                            "Autopilot profile created with id: " + post_request["id"]
-                        )
+                            request_data = {"assignments": assignment}
+                            post_assignment_update(
+                                request_data,
+                                post_request["id"],
+                                "deviceAppManagement/mobileAppConfigurations/",
+                                "/microsoft.graph.managedDeviceMobileAppConfiguration/assign",
+                                token,
+                            )
+                        print("App Configuration created with id: " + post_request["id"])
+                    else:
+                        print("App configured in App Configuration profile could not be found, skipping creation")
 
-        # If any Windows Enrollment Profile are left in mem_data, remove them from Intune as they are not in the repo
+        # If any App Configurations are left in mem_data, remove them from Intune as they are not in the repo
         if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
-                print("Removing Autopilot Profile from Intune: " + val["displayName"])
+                print("Removing App Configuration from Intune: " + val["displayName"])
                 if report is False:
-                    # Remove assignments so we can delete the profile
-                    makeapirequestDelete(
-                        f"{ENDPOINT}/{val['id']}/assignments", token, status_code=200
-                    )
-                    makeapirequestDelete(
-                        f"{ENDPOINT}/{val['id']}", token, status_code=200
-                    )
+                    makeapirequestDelete(f"{ENDPOINT}/{val['id']}", token, status_code=200)
 
     return diff_summary
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.5b2
+Version: 1.4.6b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.5b2/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_archive.py` & `IntuneCD-1.4.6b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_check_file.py` & `IntuneCD-1.4.6b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_clean_filename.py` & `IntuneCD-1.4.6b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_diff_summary.py` & `IntuneCD-1.4.6b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_documentation_functions.py` & `IntuneCD-1.4.6b1/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_get_added_removed.py` & `IntuneCD-1.4.6b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_get_authparams.py` & `IntuneCD-1.4.6b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_graph_batch.py` & `IntuneCD-1.4.6b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_graph_request.py` & `IntuneCD-1.4.6b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_group_report.py` & `IntuneCD-1.4.6b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_load_file.py` & `IntuneCD-1.4.6b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_match.py` & `IntuneCD-1.4.6b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_remove_keys.py` & `IntuneCD-1.4.6b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_save_output.py` & `IntuneCD-1.4.6b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b2/tests/test_update_frontend.py` & `IntuneCD-1.4.6b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

