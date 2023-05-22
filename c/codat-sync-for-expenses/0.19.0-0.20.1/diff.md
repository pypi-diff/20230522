# Comparing `tmp/codat-sync-for-expenses-0.19.0.tar.gz` & `tmp/codat-sync-for-expenses-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.19.0.tar", last modified: Thu May 18 08:35:01 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.20.1.tar", last modified: Mon May 22 17:58:20 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.19.0.tar` & `codat-sync-for-expenses-0.20.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.503766 codat-sync-for-expenses-0.19.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4616 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/integrationtype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2921 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7137 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4736 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2582 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4739 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2511 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4342 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.19.0/PKG-INFO` & `codat-sync-for-expenses-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.19.0
+Version: 0.20.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.19.0/README.md` & `codat-sync-for-expenses-0.20.1/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/setup.py` & `codat-sync-for-expenses-0.20.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.19.0",
+    version="0.20.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.19.0
+Version: 0.20.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,26 @@
 src/codatsyncexpenses/models/shared/companyconfiguration.py
 src/codatsyncexpenses/models/shared/companysyncstatus.py
 src/codatsyncexpenses/models/shared/createexpenserequest.py
 src/codatsyncexpenses/models/shared/createexpenseresponse.py
 src/codatsyncexpenses/models/shared/customer.py
 src/codatsyncexpenses/models/shared/dataconnection.py
 src/codatsyncexpenses/models/shared/dataconnectionerror.py
-src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
+src/codatsyncexpenses/models/shared/dataconnectionstatus.py
 src/codatsyncexpenses/models/shared/expensetransaction.py
 src/codatsyncexpenses/models/shared/expensetransactionline.py
 src/codatsyncexpenses/models/shared/hallink.py
-src/codatsyncexpenses/models/shared/integrationtype_enum.py
+src/codatsyncexpenses/models/shared/integrationtype.py
 src/codatsyncexpenses/models/shared/mappingoptions.py
 src/codatsyncexpenses/models/shared/postsync.py
 src/codatsyncexpenses/models/shared/recordref.py
 src/codatsyncexpenses/models/shared/security.py
 src/codatsyncexpenses/models/shared/supplier.py
 src/codatsyncexpenses/models/shared/syncinitiated.py
 src/codatsyncexpenses/models/shared/taxratemappinginfo.py
 src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
 src/codatsyncexpenses/models/shared/transactionmetadata.py
 src/codatsyncexpenses/models/shared/transactionmetadatalist.py
-src/codatsyncexpenses/models/shared/transactionstatus_enum.py
+src/codatsyncexpenses/models/shared/transactionstatus.py
 src/codatsyncexpenses/utils/__init__.py
 src/codatsyncexpenses/utils/retries.py
 src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -68,14 +69,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.SaveCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "company_configuration", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         r"""Create Partner Expense connection
         Creates a Partner Expense data connection
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/expenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -71,14 +72,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/mapping_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         r"""Mapping options
         Gets the expense mapping options for a companies accounting software
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncTransactionsRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a sync."""
+    page: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
     
 
 @dataclasses.dataclass
 class ListSyncTransactionsResponse:
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from .companyconfiguration import *
 from .companysyncstatus import *
 from .createexpenserequest import *
 from .createexpenseresponse import *
 from .customer import *
 from .dataconnection import *
 from .dataconnectionerror import *
-from .dataconnectionstatus_enum import *
+from .dataconnectionstatus import *
 from .expensetransaction import *
 from .expensetransactionline import *
 from .hallink import *
-from .integrationtype_enum import *
+from .integrationtype import *
 from .mappingoptions import *
 from .postsync import *
 from .recordref import *
 from .security import *
 from .supplier import *
 from .syncinitiated import *
 from .taxratemappinginfo import *
 from .trackingcategorymappinginfo import *
 from .transactionmetadata import *
 from .transactionmetadatalist import *
-from .transactionstatus_enum import *
+from .transactionstatus import *
 
-__all__ = ["AccountMappingInfo","AccountMappingInfoAccountTypeEnum","AccountMappingInfoValidTransactionTypesEnum","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceTypeEnum","DataConnectionStatusEnum","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionTypeEnum","HalLink","IntegrationTypeEnum","MappingOptions","PostSync","RecordRef","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypesEnum","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatusEnum"]
+__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountMappingInfoValidTransactionTypes","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceType","DataConnectionStatus","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","HalLink","IntegrationType","MappingOptions","PostSync","RecordRef","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatus"]
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 from __future__ import annotations
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class AccountMappingInfoAccountTypeEnum(str, Enum):
+class AccountMappingInfoAccountType(str, Enum):
     r"""Type of the account."""
     ASSET = 'Asset'
     LIABILITY = 'Liability'
     INCOME = 'Income'
     EXPENSE = 'Expense'
     EQUITY = 'Equity'
 
-class AccountMappingInfoValidTransactionTypesEnum(str, Enum):
+class AccountMappingInfoValidTransactionTypes(str, Enum):
     PAYMENT = 'Payment'
     REFUND = 'Refund'
     REWARD = 'Reward'
     CHARGEBACK = 'Chargeback'
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
     ADJUSTMENT_IN = 'AdjustmentIn'
     ADJUSTMENT_OUT = 'AdjustmentOut'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountMappingInfo:
     
-    account_type: Optional[AccountMappingInfoAccountTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
+    account_type: Optional[AccountMappingInfoAccountType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
     r"""Type of the account."""
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
     r"""Currency of the account."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of account."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the account as it appears in the companies accounting software."""
-    valid_transaction_types: Optional[list[AccountMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
+    valid_transaction_types: Optional[list[AccountMappingInfoValidTransactionTypes]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
     r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import dataconnectionerror as shared_dataconnectionerror
-from ..shared import dataconnectionstatus_enum as shared_dataconnectionstatus_enum
+from ..shared import dataconnectionstatus as shared_dataconnectionstatus
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 
-class DataConnectionSourceTypeEnum(str, Enum):
+class DataConnectionSourceType(str, Enum):
     r"""The type of platform of the connection."""
     ACCOUNTING = 'Accounting'
     BANKING = 'Banking'
     COMMERCE = 'Commerce'
     OTHER = 'Other'
     UNKNOWN = 'Unknown'
 
@@ -50,17 +50,17 @@
     r"""A Codat ID representing the integration."""
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
     r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
     link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
     platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
     r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
-    source_type: DataConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    source_type: DataConnectionSourceType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
     r"""The type of platform of the connection."""
-    status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    status: shared_dataconnectionstatus.DataConnectionStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""The current authorization status of the data connection."""
     additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
     connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
     data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 from ..shared import expensetransactionline as shared_expensetransactionline
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class ExpenseTransactionTypeEnum(str, Enum):
+class ExpenseTransactionType(str, Enum):
     r"""The type of transaction."""
     PAYMENT = 'Payment'
     REFUND = 'Refund'
     REWARD = 'Reward'
     CHARGEBACK = 'Chargeback'
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
@@ -45,15 +45,15 @@
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
-    type: ExpenseTransactionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    type: ExpenseTransactionType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of transaction."""
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
     r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
     
     Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
     Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places).
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class TaxRateMappingInfoValidTransactionTypesEnum(str, Enum):
+class TaxRateMappingInfoValidTransactionTypes(str, Enum):
     PAYMENT = 'Payment'
     REFUND = 'Refund'
     REWARD = 'Reward'
     CHARGEBACK = 'Chargeback'
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
     ADJUSTMENT_IN = 'AdjustmentIn'
@@ -28,10 +28,10 @@
     r"""Effective tax rate."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of tax rate."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the tax rate in the accounting platform."""
     total_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxRate'), 'exclude': lambda f: f is None }})
     r"""Total (not compounded) sum of the components of a tax rate."""
-    valid_transaction_types: Optional[list[TaxRateMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
+    valid_transaction_types: Optional[list[TaxRateMappingInfoValidTransactionTypes]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
     r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import integrationtype_enum as shared_integrationtype_enum
-from ..shared import transactionstatus_enum as shared_transactionstatus_enum
+from ..shared import integrationtype as shared_integrationtype
+from ..shared import transactionstatus as shared_transactionstatus
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadata:
     
-    integration_type: Optional[shared_integrationtype_enum.IntegrationTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationType'), 'exclude': lambda f: f is None }})
+    integration_type: Optional[shared_integrationtype.IntegrationType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationType'), 'exclude': lambda f: f is None }})
     r"""Type of transaction that has been processed e.g. Expense or Bank Feed."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
     r"""Metadata such as validation errors or the resulting record created in the accounting software."""
-    status: Optional[shared_transactionstatus_enum.TransactionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_transactionstatus.TransactionStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""Status of the transaction."""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
     r"""Your unique idenfier of the transaction."""
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.19.0"
-    _gen_version: str = "2.30.0"
+    _sdk_version: str = "0.20.1"
+    _gen_version: str = "2.31.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "post_sync", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         r"""Last successful sync
         Gets the status of the last successfull sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -65,14 +66,15 @@
         r"""Latest sync status
         Gets the latest sync status
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -103,14 +105,15 @@
         r"""Get Sync status
         Get the sync status for a specified sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -141,14 +144,15 @@
         r"""List sync statuses
         Gets a list of sync statuses
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/transaction_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         r"""Get Sync Transaction
         Gets the status of a transaction for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         headers = {}
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -66,14 +67,15 @@
         Get's the transactions and status for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
```

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

