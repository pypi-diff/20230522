# Comparing `tmp/paideia_contracts-1.1.2.tar.gz` & `tmp/paideia_contracts-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paideia_contracts-1.1.2.tar", last modified: Tue Feb 21 11:44:01 2023, max compression
+gzip compressed data, was "paideia_contracts-1.1.3.tar", last modified: Mon May 22 07:39:26 2023, max compression
```

## Comparing `paideia_contracts-1.1.2.tar` & `paideia_contracts-1.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1065 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/LICENSE
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3698 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/PKG-INFO
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3251 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/README.md
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/__init__.py
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/__init__.py
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    12716 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/__init__.py
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/ergoscript/
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/ergoscript/latest/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     7558 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/ergoscript/latest/plasmaStaking.es
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    70539 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/__init__.py
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/addStakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10547 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/emission.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     3250 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stake.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9522 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakePool.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-02-21 11:23:31.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27267 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakeState.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3855 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakingIncentive.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/unstakeProxy.es
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/addStakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10709 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/emission.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    11379 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stake.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9673 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakePool.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-02-21 11:23:25.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27423 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakeState.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    13752 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakingIncentive.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/unstakeProxy.es
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/__init__.py
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/addStakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10709 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/emission.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    11379 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stake.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9673 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakePool.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-02-21 11:22:08.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakeProxy.es
--rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27423 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakeState.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    13752 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakingIncentive.es
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2023-02-21 10:51:24.000000 paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/unstakeProxy.es
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.910939 paideia_contracts-1.1.2/paideia_contracts.egg-info/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3698 2023-02-21 11:44:01.000000 paideia_contracts-1.1.2/paideia_contracts.egg-info/PKG-INFO
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2161 2023-02-21 11:44:01.000000 paideia_contracts-1.1.2/paideia_contracts.egg-info/SOURCES.txt
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        1 2023-02-21 11:44:01.000000 paideia_contracts-1.1.2/paideia_contracts.egg-info/dependency_links.txt
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       43 2023-02-21 11:44:01.000000 paideia_contracts-1.1.2/paideia_contracts.egg-info/requires.txt
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       18 2023-02-21 11:44:01.000000 paideia_contracts-1.1.2/paideia_contracts.egg-info/top_level.txt
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       38 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/setup.cfg
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1152 2023-02-21 11:24:07.000000 paideia_contracts-1.1.2/setup.py
-drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-02-21 11:44:01.914939 paideia_contracts-1.1.2/test/
--rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    27193 2023-02-21 11:19:59.000000 paideia_contracts-1.1.2/test/test_staking.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.707963 paideia_contracts-1.1.3/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1065 2022-05-18 10:32:40.000000 paideia_contracts-1.1.3/LICENSE
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3698 2023-05-22 07:39:26.707963 paideia_contracts-1.1.3/PKG-INFO
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3251 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/README.md
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.659963 paideia_contracts-1.1.3/paideia_contracts/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2022-05-18 10:32:40.000000 paideia_contracts-1.1.3/paideia_contracts/__init__.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.663963 paideia_contracts-1.1.3/paideia_contracts/contracts/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2022-05-18 10:32:40.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/__init__.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.663963 paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    12716 2022-08-10 15:22:32.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/__init__.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.659963 paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/ergoscript/
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.663963 paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/ergoscript/latest/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     7558 2022-08-10 12:46:38.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/ergoscript/latest/plasmaStaking.es
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.671963 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    72261 2023-05-22 07:37:33.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/__init__.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.659963 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.687963 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/addStakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10547 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/emission.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     3250 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stake.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9522 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakePool.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-05-22 07:28:45.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27267 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakeState.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3855 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakingIncentive.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/unstakeProxy.es
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.695963 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/addStakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10709 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/emission.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    11379 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stake.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9673 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakePool.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-05-22 07:28:45.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27423 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakeState.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    13752 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakingIncentive.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2022-07-01 11:49:01.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/unstakeProxy.es
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.707963 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        0 2022-06-17 07:20:50.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/__init__.py
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2059 2022-06-17 07:20:50.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/addStakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    10709 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/emission.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    11379 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stake.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)     9673 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakePool.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2129 2023-05-22 07:28:45.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakeProxy.es
+-rwxrwxr-x   0 luivatra  (1000) luivatra  (1000)    27423 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakeState.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    13752 2022-06-17 07:27:07.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakingIncentive.es
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1970 2022-06-17 07:20:51.000000 paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/unstakeProxy.es
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.659963 paideia_contracts-1.1.3/paideia_contracts.egg-info/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     3698 2023-05-22 07:39:26.000000 paideia_contracts-1.1.3/paideia_contracts.egg-info/PKG-INFO
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     2161 2023-05-22 07:39:26.000000 paideia_contracts-1.1.3/paideia_contracts.egg-info/SOURCES.txt
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)        1 2023-05-22 07:39:26.000000 paideia_contracts-1.1.3/paideia_contracts.egg-info/dependency_links.txt
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       43 2023-05-22 07:39:26.000000 paideia_contracts-1.1.3/paideia_contracts.egg-info/requires.txt
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       18 2023-05-22 07:39:26.000000 paideia_contracts-1.1.3/paideia_contracts.egg-info/top_level.txt
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)       38 2023-05-22 07:39:26.707963 paideia_contracts-1.1.3/setup.cfg
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)     1152 2023-05-22 07:28:56.000000 paideia_contracts-1.1.3/setup.py
+drwxrwxr-x   0 luivatra  (1000) luivatra  (1000)        0 2023-05-22 07:39:26.707963 paideia_contracts-1.1.3/test/
+-rw-rw-r--   0 luivatra  (1000) luivatra  (1000)    27193 2023-05-22 07:28:45.000000 paideia_contracts-1.1.3/test/test_staking.py
```

### Comparing `paideia_contracts-1.1.2/LICENSE` & `paideia_contracts-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/PKG-INFO` & `paideia_contracts-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paideia_contracts
-Version: 1.1.2
+Version: 1.1.3
 Summary: ErgoScript and Python wrappers for Paideia
 Home-page: https://github.com/ergo-pad/paideia-contracts
 Author: Robert Pieter van Leeuwen
 Author-email: luivatra@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `paideia_contracts-1.1.2/README.md` & `paideia_contracts-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/__init__.py` & `paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/__init__.py`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/plasma_staking/ergoscript/latest/plasmaStaking.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/plasma_staking/ergoscript/latest/plasmaStaking.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/__init__.py` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1359,14 +1359,48 @@
     result.emissionContract = EmissionContract(result)
     result.stakingIncentiveContract = StakingIncentiveContract(result)
     result.stakeProxyContract = StakeProxyContract(result)
     result.addStakeProxyContract = AddStakeProxyContract(result)
     result.unstakeProxyContract = UnstakeProxyContract(result)
     return result
 
+def AHTConfig(appKit: ErgoAppKit) -> StakingConfig:
+    result = StakingConfig(
+        version = "1.1",
+        appKit = appKit,
+        stakeStateNFT = "4517aed531db665693495fd3544faf75717816509cb0987513d24939977abbb6",
+        stakePoolNFT = "9d90e7567d066263104d1afd13bc23a1a259d733507bf1f33cd02155e7ff0df1",
+        emissionNFT = "dff51ec85263da408181394c72fa6ef3b9c82048e6783c7fea1642cc0472f414",
+        stakeTokenId = "6c6e6ec794585aeeac8d9a211a270caec3d0fce9c352f8df2cc54b2c32217648",
+        stakedTokenId = "18c938e1924fc3eadc266e75ec02d81fe73b56e4e9f4e268dffffcb30387c42d",
+        stakePoolKey = "8511259d53540169a3ee54b062fcca600c3e67ba2f28e8981ba544adde9bbea2",
+        stakedTokenName = "AHT",
+        stakedTokenDecimals = 4,
+        proxyToStakingIncentive = int(1e8),
+        proxyAddToStakingIncentive = int(1e7),
+        proxyExecutorReward = int(2e6),
+        proxyMinerFee = int(2e6),
+        dustCollectionReward = int(5e5),
+        dustCollectionMinerFee = int(1e6),
+        emitReward = int(3e6),
+        emitMinerFee = int(1e6),
+        baseCompoundReward = int(5e5),
+        baseCompoundMinerFee = int(1e6),
+        variableCompoundReward = int(15e4),
+        variableCompoundMinerFee = int(1e5))
+    result.stakeContract = StakeContract(result)
+    result.stakeStateContract = StakeStateContract(result)
+    result.stakePoolContract = StakePoolContract(result)
+    result.emissionContract = EmissionContract(result)
+    result.stakingIncentiveContract = StakingIncentiveContract(result)
+    result.stakeProxyContract = StakeProxyContract(result)
+    result.addStakeProxyContract = AddStakeProxyContract(result)
+    result.unstakeProxyContract = UnstakeProxyContract(result)
+    return result
+
 def BootstrapStaking(appKit: ErgoAppKit, nodeAddress: str, tokenId: str, stakingStart: int, stakingCycleDuration: int, dailyEmission: int, stakePoolSize: int, version: str = "latest") -> StakingConfig:
     res = requests.get(f"{appKit._explorerUrl}/api/v1/tokens/{tokenId}")
     stakedTokenName = res.json()["name"]
     stakedTokenDecimals = res.json()["decimals"]
     print(stakedTokenName)
     nodeContract = appKit.contractFromAddress(nodeAddress)
     nodeInputs = appKit.boxesToSpend(nodeAddress,int(14e6),{tokenId: int(stakePoolSize*10**stakedTokenDecimals)})
```

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/addStakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/addStakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/emission.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/emission.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stake.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stake.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakePool.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakePool.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakeState.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakeState.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/stakingIncentive.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/stakingIncentive.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.0/unstakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.0/unstakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/addStakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/addStakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/emission.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/emission.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stake.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stake.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakePool.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakePool.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakeState.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakeState.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/stakingIncentive.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/stakingIncentive.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/1.1/unstakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/1.1/unstakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/addStakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/addStakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/emission.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/emission.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stake.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stake.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakePool.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakePool.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakeState.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakeState.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/stakingIncentive.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/stakingIncentive.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts/contracts/staking/ergoscript/latest/unstakeProxy.es` & `paideia_contracts-1.1.3/paideia_contracts/contracts/staking/ergoscript/latest/unstakeProxy.es`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/paideia_contracts.egg-info/PKG-INFO` & `paideia_contracts-1.1.3/paideia_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paideia-contracts
-Version: 1.1.2
+Version: 1.1.3
 Summary: ErgoScript and Python wrappers for Paideia
 Home-page: https://github.com/ergo-pad/paideia-contracts
 Author: Robert Pieter van Leeuwen
 Author-email: luivatra@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `paideia_contracts-1.1.2/paideia_contracts.egg-info/SOURCES.txt` & `paideia_contracts-1.1.3/paideia_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paideia_contracts-1.1.2/setup.py` & `paideia_contracts-1.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # this assumes setup.py lives in the folder that contains the package
     package_path = Path(f'./{package_name}').resolve()
     return [str(path.relative_to(package_path)) 
             for path in package_path.glob(glob)]
 
 setuptools.setup(
     name='paideia_contracts',  
-    version='1.1.2',
+    version='1.1.3',
     my_packages=['paideia_contracts'],
     author="Robert Pieter van Leeuwen",
     author_email="luivatra@gmail.com",
     description="ErgoScript and Python wrappers for Paideia",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ergo-pad/paideia-contracts",
@@ -24,11 +24,11 @@
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'ergo_python_appkit>=0.2.0',
+        'ergo_python_appkit>=0.2.1',
         'requests>=2.27.1'
     ]
  )
```

### Comparing `paideia_contracts-1.1.2/test/test_staking.py` & `paideia_contracts-1.1.3/test/test_staking.py`

 * *Files identical despite different names*

