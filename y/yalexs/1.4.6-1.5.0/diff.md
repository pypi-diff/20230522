# Comparing `tmp/yalexs-1.4.6.tar.gz` & `tmp/yalexs-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.4.6.tar", last modified: Wed May 17 21:49:22 2023, max compression
+gzip compressed data, was "yalexs-1.5.0.tar", last modified: Mon May 22 13:34:16 2023, max compression
```

## Comparing `yalexs-1.4.6.tar` & `yalexs-1.5.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451650 yalexs-1.4.6/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.438040 yalexs-1.4.6/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.440323 yalexs-1.4.6/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.6/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.6/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.6/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.6/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 21:49:22.451727 yalexs-1.4.6/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.6/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.6/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.6/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.6/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.6/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-05-17 21:24:49.000000 yalexs-1.4.6/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 21:49:22.452006 yalexs-1.4.6/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 21:45:28.000000 yalexs-1.4.6/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.441727 yalexs-1.4.6/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.447492 yalexs-1.4.6/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    42924 2023-05-17 21:45:20.000000 yalexs-1.4.6/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    16539 2023-05-17 21:25:12.000000 yalexs-1.4.6/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.6/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.6/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.450786 yalexs-1.4.6/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 21:45:28.000000 yalexs-1.4.6/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.6/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.4.6/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15146 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11642 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.4.6/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.6/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451541 yalexs-1.4.6/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1100 2023-05-17 20:48:17.000000 yalexs-1.4.6/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      776 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.6/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4555 2023-05-17 21:25:12.000000 yalexs-1.4.6/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4502 2023-05-17 20:48:17.000000 yalexs-1.4.6/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.6/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451373 yalexs-1.4.6/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.154382 yalexs-1.5.0/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.136196 yalexs-1.5.0/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.138849 yalexs-1.5.0/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.5.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.5.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.5.0/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-22 13:34:16.154469 yalexs-1.5.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.5.0/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.5.0/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.5.0/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.5.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.5.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      141 2023-05-22 13:33:40.000000 yalexs-1.5.0/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-22 13:34:16.154767 yalexs-1.5.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1054 2023-05-22 13:33:47.000000 yalexs-1.5.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.140959 yalexs-1.5.0/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.149072 yalexs-1.5.0/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.5.0/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.5.0/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    42924 2023-05-17 21:45:20.000000 yalexs-1.5.0/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.5.0/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.5.0/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    17841 2023-05-18 17:20:56.000000 yalexs-1.5.0/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15595 2023-05-22 13:33:40.000000 yalexs-1.5.0/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.5.0/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.153373 yalexs-1.5.0/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-22 13:33:47.000000 yalexs-1.5.0/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14170 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.5.0/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15146 2023-05-17 21:45:20.000000 yalexs-1.5.0/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11644 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.5.0/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.5.0/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5282 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.154238 yalexs-1.5.0/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.5.0/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.5.0/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1846 2023-05-18 17:02:22.000000 yalexs-1.5.0/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1283 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.5.0/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4251 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      776 2023-05-17 21:45:20.000000 yalexs-1.5.0/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1044 2023-05-18 17:02:22.000000 yalexs-1.5.0/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7922 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2403 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4555 2023-05-17 21:25:12.000000 yalexs-1.5.0/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4484 2023-05-22 13:11:27.000000 yalexs-1.5.0/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      298 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/time.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.5.0/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3913 2023-05-22 13:33:40.000000 yalexs-1.5.0/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:34:16.153874 yalexs-1.5.0/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-22 13:34:16.000000 yalexs-1.5.0/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2884 2023-05-22 13:34:16.000000 yalexs-1.5.0/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-22 13:34:16.000000 yalexs-1.5.0/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      107 2023-05-22 13:34:16.000000 yalexs-1.5.0/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-22 13:34:16.000000 yalexs-1.5.0/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.4.6/.github/workflows/ci.yaml` & `yalexs-1.5.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/.gitignore` & `yalexs-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/LICENSE` & `yalexs-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/PKG-INFO` & `yalexs-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.6
+Version: 1.5.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.6/README.md` & `yalexs-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/known_activities.md` & `yalexs-1.5.0/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/pylintrc` & `yalexs-1.5.0/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/setup.cfg` & `yalexs-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.6
+current_version = 1.5.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.4.6/setup.py` & `yalexs-1.5.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.4.6",
+    version="1.5.0",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
@@ -17,14 +17,15 @@
     url="https://github.com/bdraco/yalexs",
     license="MIT",
     author="bdraco",
     author_email="nick@koston.org",
     description="Python API for Yale Access (formerly August) Smart Lock and Doorbell",
     packages=find_packages(include=["yalexs", "yalexs.backports", "yalexs.*"]),
     install_requires=[
+        "ciso8601>=2.1.3",
         "pyjwt",
         "requests",
         "vol",
         "python-dateutil",
         "aiohttp",
         "aiofiles",
         "pubnub>=7.1.0",
```

### Comparing `yalexs-1.4.6/tests/fixtures/auto_relock_activity.json` & `yalexs-1.5.0/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.5.0/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.5.0/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/door_closed_activity.json` & `yalexs-1.5.0/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.5.0/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.5.0/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/door_open_activity.json` & `yalexs-1.5.0/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.5.0/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.5.0/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.5.0/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_doorbells.json` & `yalexs-1.5.0/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_house_activities.json` & `yalexs-1.5.0/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.5.0/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.5.0/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.offline.json` & `yalexs-1.5.0/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.online.json` & `yalexs-1.5.0/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.5.0/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.5.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.5.0/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/get_pins.json` & `yalexs-1.5.0/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.5.0/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/lock.json` & `yalexs-1.5.0/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/lock_activity.json` & `yalexs-1.5.0/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.5.0/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/remote_lock_activity.json` & `yalexs-1.5.0/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.5.0/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/unlock.json` & `yalexs-1.5.0/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/unlock_activity.json` & `yalexs-1.5.0/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.5.0/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_activity.py` & `yalexs-1.5.0/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_api.py` & `yalexs-1.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_api_async.py` & `yalexs-1.5.0/tests/test_api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_authenticator.py` & `yalexs-1.5.0/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_authenticator_async.py` & `yalexs-1.5.0/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/tests/test_pubnub_activity.py` & `yalexs-1.5.0/tests/test_pubnub_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 import os
 import unittest
 
 import dateutil.parser
 from dateutil.tz import tzlocal
 
@@ -283,14 +284,48 @@
             },
         )
         assert isinstance(activities[0], LockOperationActivity)
         assert "LockOperationActivity" in str(activities[0])
         assert activities[0].action == "unlock"
         assert activities[0].operated_by == "bob smith"
 
+        activities = activities_from_pubnub_message(
+            lock,
+            datetime.datetime.fromtimestamp(16844292526891571 / 1000000),
+            {
+                "status": "unlocked",
+                "callingUserID": "manualunlock",
+                "doorState": "open",
+            },
+        )
+        assert isinstance(activities[0], LockOperationActivity)
+        assert "LockOperationActivity" in str(activities[0])
+        assert activities[0].action == "unlock"
+        assert (
+            activities[0].activity_type is ActivityType.LOCK_OPERATION_WITHOUT_OPERATOR
+        )
+        assert activities[0].operated_by is None
+
+        activities = activities_from_pubnub_message(
+            lock,
+            datetime.datetime.fromtimestamp(16844299539729015 / 1000000),
+            {
+                "status": "locked",
+                "callingUserID": "manuallock",
+                "doorState": "open",
+            },
+        )
+        assert isinstance(activities[0], LockOperationActivity)
+        assert "LockOperationActivity" in str(activities[0])
+        assert activities[0].action == "lock"
+        assert (
+            activities[0].activity_type is ActivityType.LOCK_OPERATION_WITHOUT_OPERATOR
+        )
+        assert activities[0].operated_by is None
+
 
 class TestDetail(unittest.TestCase):
     def test_update_doorbell_details_from_pubnub_message(self):
         doorbell = DoorbellDetail(json.loads(load_fixture("get_doorbell.json")))
         self.assertEqual("K98GiDT45GUL", doorbell.device_id)
         self.assertEqual(
             dateutil.parser.parse("2017-12-10T08:01:35Z"),
```

### Comparing `yalexs-1.4.6/tests/test_util.py` & `yalexs-1.5.0/tests/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     SOURCE_PUBNUB,
     BridgeOperationActivity,
     DoorbellMotionActivity,
     DoorOperationActivity,
     LockOperationActivity,
 )
 from yalexs.api import _convert_lock_result_to_activities
+from yalexs.const import Brand
 from yalexs.doorbell import DoorbellDetail
 from yalexs.lock import LockDetail, LockDoorStatus, LockStatus
 from yalexs.pubnub_activity import activities_from_pubnub_message
 from yalexs.util import (
     as_utc_from_local,
+    get_configuration_url,
     get_latest_activity,
     update_doorbell_image_from_activity,
     update_lock_detail_from_activity,
 )
 
 
 def load_fixture(filename):
@@ -382,7 +384,17 @@
             update_doorbell_image_from_activity(doorbell, doorbell_motion_activity)
         )
         self.assertEqual(
             dateutil.parser.parse("2020-02-20T17:44:45Z"),
             doorbell.image_created_at_datetime,
         )
         self.assertEqual("https://my.updated.image/image.jpg", doorbell.image_url)
+
+
+def test_get_configuration_url():
+    """Test that we get the correct configuration url for the brand."""
+    assert get_configuration_url("august") == "https://account.august.com"
+    assert get_configuration_url("yale_access") == "https://account.august.com"
+    assert get_configuration_url("yale_home") == "https://account.aaecosystem.com"
+    assert get_configuration_url(Brand.AUGUST) == "https://account.august.com"
+    assert get_configuration_url(Brand.YALE_ACCESS) == "https://account.august.com"
+    assert get_configuration_url(Brand.YALE_HOME) == "https://account.aaecosystem.com"
```

### Comparing `yalexs-1.4.6/tox.ini` & `yalexs-1.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/activity.py` & `yalexs-1.5.0/yalexs/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 
-import dateutil.parser
-
 from .lock import LockDoorStatus, LockStatus
+from .time import parse_datetime
 from .users import get_user_info
 
 ACTION_LOCK_ONETOUCHLOCK = "onetouchlock"
 ACTION_LOCK_ONETOUCHLOCK_2 = "one_touch_lock"
 ACTION_LOCK_LOCK = "lock"
 ACTION_RF_LOCK = "rf_lock"
 ACTION_RF_SECURE = "rf_secure"
@@ -230,15 +229,15 @@
         self._image_url = (
             None if image is None else image.get("secure_url")
         ) or data.get("attachment")
         self._image_created_at_datetime = None
         if image is None:
             return
         if "created_at" in image:
-            self._image_created_at_datetime = dateutil.parser.parse(image["created_at"])
+            self._image_created_at_datetime = parse_datetime(image["created_at"])
         else:
             self._image_created_at_datetime = self._activity_time
 
     def __repr__(self):
         return (
             f"<{self.__class__.__name__} action={self.action} activity_type={self.activity_type} "
             f"activity_start_time={self.activity_start_time} "
```

### Comparing `yalexs-1.4.6/yalexs/api.py` & `yalexs-1.5.0/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/api_async.py` & `yalexs-1.5.0/yalexs/api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/api_common.py` & `yalexs-1.5.0/yalexs/api_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Api functions common between sync and async."""
 import datetime
 import logging
 from typing import Any, Dict, List, Optional, Union
 
-import dateutil.parser
-
 from .activity import (
     ACTIVITY_ACTIONS_BRIDGE_OPERATION,
     ACTIVITY_ACTIONS_DOOR_OPERATION,
     ACTIVITY_ACTIONS_DOORBELL_DING,
     ACTIVITY_ACTIONS_DOORBELL_IMAGE_CAPTURE,
     ACTIVITY_ACTIONS_DOORBELL_MOTION,
     ACTIVITY_ACTIONS_DOORBELL_VIEW,
@@ -22,14 +20,15 @@
     DoorbellViewActivity,
     DoorOperationActivity,
     LockOperationActivity,
 )
 from .const import BASE_URLS, BRANDING, Brand
 from .doorbell import Doorbell
 from .lock import Lock, LockDoorStatus, determine_door_state, door_state_to_string
+from .time import parse_datetime
 
 API_EXCEPTION_RETRY_TIME = 0.1
 API_RETRY_TIME = 2.5
 API_RETRY_ATTEMPTS = 10
 
 HEADER_ACCEPT_VERSION = "Accept-Version"
 HEADER_AUGUST_ACCESS_TOKEN = "x-august-access-token"  # nosec
@@ -167,15 +166,15 @@
         "deviceType": "lock",
         "action": action_text,
     }
     return _activity_from_dict(SOURCE_LOCK_OPERATE, mapped_dict)
 
 
 def _datetime_string_to_epoch(datetime_string: str) -> datetime.datetime:
-    return dateutil.parser.parse(datetime_string).timestamp() * 1000
+    return parse_datetime(datetime_string).timestamp() * 1000
 
 
 def _process_activity_json(json_dict: Dict[str, Any]) -> List[ActivityType]:
     if "events" in json_dict:
         json_dict = json_dict["events"]
     activities = []
     for activity_json in json_dict:
```

### Comparing `yalexs-1.4.6/yalexs/authenticator.py` & `yalexs-1.5.0/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/authenticator_async.py` & `yalexs-1.5.0/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/authenticator_common.py` & `yalexs-1.5.0/yalexs/authenticator_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from datetime import datetime, timedelta, timezone
 from enum import Enum
 import json
 import logging
 from typing import Any, Optional
 import uuid
 
-import dateutil.parser
 import jwt
 
 from .api import HEADER_AUGUST_ACCESS_TOKEN, ApiCommon
+from .time import parse_datetime
 
 # The default time before expiration to refresh a token
 DEFAULT_RENEWAL_THRESHOLD = timedelta(days=7)
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -47,15 +47,15 @@
     ):
         self._state = state
         self._install_id = str(uuid.uuid4()) if install_id is None else install_id
         self._access_token = access_token
         self._access_token_expires = access_token_expires
         self._parsed_expiration_time = None
         if access_token_expires:
-            self._parsed_expiration_time = dateutil.parser.parse(access_token_expires)
+            self._parsed_expiration_time = parse_datetime(access_token_expires)
 
     @property
     def install_id(self):
         return self._install_id
 
     @property
     def access_token(self):
```

### Comparing `yalexs-1.4.6/yalexs/backports/enum.py` & `yalexs-1.5.0/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/bridge.py` & `yalexs-1.5.0/yalexs/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 
-from yalexs.device import DeviceDetail
+from .device import DeviceDetail
 
 
 class BridgeStatus(Enum):
     OFFLINE = "offline"
     ONLINE = "online"
     UNKNOWN = "unknown"
```

### Comparing `yalexs-1.4.6/yalexs/const.py` & `yalexs-1.5.0/yalexs/const.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,7 +39,13 @@
         "publish": "pub-c-567d7f2d-270a-438a-a785-f0af12ad8312f",
     },
     Brand.YALE_HOME: {
         "subscribe": "sub-c-c9c38d4d-5796-46c9-9262-af20cf6a1d42",
         "publish": "pub-c-353e8881-cf58-4b26-9baf-96f296de0677",
     },
 }
+
+CONFIGURATION_URLS = {
+    Brand.AUGUST: "https://account.august.com",
+    Brand.YALE_ACCESS: "https://account.august.com",
+    Brand.YALE_HOME: "https://account.aaecosystem.com",
+}
```

### Comparing `yalexs-1.4.6/yalexs/device.py` & `yalexs-1.5.0/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/doorbell.py` & `yalexs-1.5.0/yalexs/doorbell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
-import dateutil.parser
 import requests
 
 from .device import Device, DeviceDetail
+from .time import parse_datetime
 
 DOORBELL_STATUS_KEY = "status"
 
 
 class Doorbell(Device):
     def __init__(self, device_id, data):
         super().__init__(device_id, data["name"], data["HouseID"])
@@ -66,17 +66,15 @@
         self._image_created_at_datetime = None
         self._model = None
 
         if "type" in data:
             self._model = data["type"]
 
         if "created_at" in recent_image:
-            self._image_created_at_datetime = dateutil.parser.parse(
-                recent_image["created_at"]
-            )
+            self._image_created_at_datetime = parse_datetime(recent_image["created_at"])
 
         self._battery_level = None
         if "telemetry" in data:
             telemetry = data["telemetry"]
             if "battery_soc" in telemetry:
                 self._battery_level = telemetry.get("battery_soc", None)
             elif telemetry.get("doorbell_low_battery"):
```

### Comparing `yalexs-1.4.6/yalexs/exceptions.py` & `yalexs-1.5.0/yalexs/exceptions.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/keypad.py` & `yalexs-1.5.0/yalexs/keypad.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yalexs.device import DeviceDetail
+from .device import DeviceDetail
 
 BATTERY_LEVEL_FULL = "Full"
 BATTERY_LEVEL_MEDIUM = "Medium"
 BATTERY_LEVEL_LOW = "Low"
 
 
 class KeypadDetail(DeviceDetail):
```

### Comparing `yalexs-1.4.6/yalexs/lock.py` & `yalexs-1.5.0/yalexs/lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import datetime
 from enum import Enum
 from typing import List, Optional
 
-import dateutil.parser
-
-from yalexs.bridge import BridgeDetail, BridgeStatus
-from yalexs.device import Device, DeviceDetail
-from yalexs.keypad import KeypadDetail
-
+from .bridge import BridgeDetail, BridgeStatus
+from .device import Device, DeviceDetail
+from .keypad import KeypadDetail
+from .time import parse_datetime
 from .users import cache_user_info
 
 LOCKED_STATUS = ("locked", "kAugLockState_Locked", "kAugLockState_SecureMode")
 LOCKING_STATUS = ("kAugLockState_Locking",)
 UNLOCKED_STATUS = ("unlocked", "kAugLockState_Unlocked")
 UNLOCKING_STATUS = ("kAugLockState_Unlocking",)
 JAMMED_STATUS = (
@@ -73,17 +71,15 @@
         if "LockStatus" in data:
             lock_status = data["LockStatus"]
 
             self._lock_status = determine_lock_status(lock_status.get(LOCK_STATUS_KEY))
             self._door_state = determine_door_state(lock_status.get(DOOR_STATE_KEY))
 
             if "dateTime" in lock_status:
-                self._lock_status_datetime = dateutil.parser.parse(
-                    lock_status["dateTime"]
-                )
+                self._lock_status_datetime = parse_datetime(lock_status["dateTime"])
                 self._door_state_datetime = self._lock_status_datetime
 
             if (
                 DOOR_STATE_KEY in lock_status
                 and self._door_state != LockDoorStatus.DISABLED
             ):
                 self._doorsense = True
```

### Comparing `yalexs-1.4.6/yalexs/pin.py` & `yalexs-1.5.0/yalexs/pin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import dateutil.parser
+from .time import parse_datetime
 
 
 class Pin:
     def __init__(self, data):
         self._pin_id = data["_id"]
         self._lock_id = data["lockID"]
         self._user_id = data["userID"]
@@ -60,39 +60,39 @@
 
     @property
     def unverified(self):
         return self._unverified
 
     @property
     def created_at(self):
-        return dateutil.parser.parse(self._created_at)
+        return parse_datetime(self._created_at)
 
     @property
     def updated_at(self):
-        return dateutil.parser.parse(self._updated_at)
+        return parse_datetime(self._updated_at)
 
     @property
     def loaded_date(self):
-        return dateutil.parser.parse(self._loaded_date)
+        return parse_datetime(self._loaded_date)
 
     @property
     def access_start_time(self):
         if not self._access_start_time:
             return None
-        return dateutil.parser.parse(self._access_start_time)
+        return parse_datetime(self._access_start_time)
 
     @property
     def access_end_time(self):
         if not self._access_end_time:
             return None
-        return dateutil.parser.parse(self._access_end_time)
+        return parse_datetime(self._access_end_time)
 
     @property
     def access_times(self):
         if not self._access_times:
             return None
-        return dateutil.parser.parse(self._access_times)
+        return parse_datetime(self._access_times)
 
     def __repr__(self):
         return "Pin(id={} firstName={}, lastName={})".format(
             self.pin_id, self.first_name, self.last_name
         )
```

### Comparing `yalexs-1.4.6/yalexs/pubnub_activity.py` & `yalexs-1.5.0/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/pubnub_async.py` & `yalexs-1.5.0/yalexs/pubnub_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Connect to pubnub."""
 
 import datetime
 import logging
-from typing import Any, Callable, List
+from typing import Any, Callable
 
 from pubnub.callbacks import SubscribeCallback
 from pubnub.enums import PNReconnectionPolicy, PNStatusCategory
 from pubnub.models.consumer.common import PNStatus
 from pubnub.models.consumer.pubsub import PNMessageResult
 from pubnub.pnconfiguration import PNConfiguration
 from pubnub.pubnub_asyncio import AsyncioSubscriptionManager, PubNubAsyncio
@@ -106,15 +106,15 @@
     @property
     def channels(self):
         """Return a list of registered channels."""
         return self._device_channels.keys()
 
 
 def async_create_pubnub(
-    user_uuid: str, subscriptions: List[UpdateCallbackType], brand: Brand = Brand.AUGUST
+    user_uuid: str, subscriptions: AugustPubNub, brand: Brand = Brand.AUGUST
 ) -> Callable[[], None]:
     """Create a pubnub subscription."""
     tokens = PUBNUB_TOKENS[brand]
     pnconfig = PNConfiguration()
     pnconfig.subscribe_key = tokens["subscribe"]
     pnconfig.publish_key = tokens["publish"]
     pnconfig.uuid = f"pn-{str(user_uuid).upper()}"
```

### Comparing `yalexs-1.4.6/yalexs/users.py` & `yalexs-1.5.0/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.6/yalexs/util.py` & `yalexs-1.5.0/yalexs/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import datetime
 from typing import Optional, Union
 
-from yalexs.activity import (
+from .activity import (
     ACTION_BRIDGE_OFFLINE,
     ACTION_BRIDGE_ONLINE,
     ACTIVITY_ACTION_STATES,
     MOVING_STATES,
     BridgeOperationActivity,
     DoorbellImageCaptureActivity,
     DoorbellMotionActivity,
     DoorOperationActivity,
     LockOperationActivity,
 )
-from yalexs.lock import LockDetail
+from .const import CONFIGURATION_URLS, Brand
+from .lock import LockDetail
 
 
 def get_latest_activity(
     activity1: Optional[
         Union[LockOperationActivity, DoorOperationActivity, BridgeOperationActivity]
     ],
     activity2: Optional[
@@ -103,7 +104,12 @@
 
     return True
 
 
 def as_utc_from_local(dtime: datetime.datetime) -> datetime.datetime:
     """Converts the datetime returned from an activity to UTC."""
     return dtime.astimezone(tz=datetime.timezone.utc)
+
+
+def get_configuration_url(brand: Brand) -> str:
+    """Return the configuration URL for the brand."""
+    return CONFIGURATION_URLS[brand]
```

### Comparing `yalexs-1.4.6/yalexs.egg-info/PKG-INFO` & `yalexs-1.5.0/yalexs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.6
+Version: 1.5.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.6/yalexs.egg-info/SOURCES.txt` & `yalexs-1.5.0/yalexs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 yalexs/doorbell.py
 yalexs/exceptions.py
 yalexs/keypad.py
 yalexs/lock.py
 yalexs/pin.py
 yalexs/pubnub_activity.py
 yalexs/pubnub_async.py
+yalexs/time.py
 yalexs/users.py
 yalexs/util.py
 yalexs.egg-info/PKG-INFO
 yalexs.egg-info/SOURCES.txt
 yalexs.egg-info/dependency_links.txt
 yalexs.egg-info/requires.txt
 yalexs.egg-info/top_level.txt
```

