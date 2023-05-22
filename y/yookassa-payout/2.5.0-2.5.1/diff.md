# Comparing `tmp/yookassa-payout-2.5.0.tar.gz` & `tmp/yookassa-payout-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yookassa-payout-2.5.0.tar", last modified: Tue Jan 17 09:50:40 2023, max compression
+gzip compressed data, was "yookassa-payout-2.5.1.tar", last modified: Mon May 22 11:45:44 2023, max compression
```

## Comparing `yookassa-payout-2.5.0.tar` & `yookassa-payout-2.5.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.455535 yookassa-payout-2.5.0/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1102 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/CHANGELOG.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      231 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1079 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/LICENSE
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      150 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/MANIFEST.in
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    12250 2023-01-17 09:50:40.455734 yookassa-payout-2.5.0/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10085 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/README.en.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    13123 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/README.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2023-01-17 09:50:40.456958 yookassa-payout-2.5.0/setup.cfg
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1549 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/setup.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.366803 yookassa-payout-2.5.0/src/
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.403005 yookassa-payout-2.5.0/src/yookassa_payout/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      148 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      106 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/__main__.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.409645 yookassa-payout-2.5.0/src/yookassa_payout/artefacts/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       58 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/artefacts/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6391 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/artefacts/deposit.cer
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1373 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/cli.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2125 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/configuration.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.410235 yookassa-payout-2.5.0/src/yookassa_payout/domain/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/__init__.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.418522 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1490 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/base_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5915 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/cli_client.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7847 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/client.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      129 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/currency.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      361 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/data_context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3315 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/error_converter.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4088 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/generator_csr.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      623 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/http_verb.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      935 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/keychain.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5234 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/openssl_helper.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6346 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/common/xml_helper.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.426951 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/api_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      132 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/authorize_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      144 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/bad_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      144 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/forbidden_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/not_found_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      141 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/open_ssl_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      152 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/response_processing_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      149 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/too_many_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      146 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/exceptions/unauthorized_error.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.428032 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2737 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/organization.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.430923 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7125 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/bank_account_recipient.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6677 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/bank_card_recipient.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      846 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/recipient.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      847 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/recipient_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.433672 yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1416 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3249 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2151 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification_response.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.446474 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1212 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/balance_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3162 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/deposition_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      703 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/deposition_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      463 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/make_deposition_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/request_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/synonym_card_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      463 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/request/test_deposition_request.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.453022 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1295 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/balance_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2116 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/deposition_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      752 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/deposition_response_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/make_deposition_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1078 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/response_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2739 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/synonym_card_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      168 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/domain/response/test_deposition_response.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.455316 yookassa-payout-2.5.0/src/yookassa_payout/logging/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/logging/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      638 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/logging/adapter.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1770 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/logging/classes.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1816 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/logging/config.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3822 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/payout.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      158 2023-01-17 09:50:39.000000 yookassa-payout-2.5.0/src/yookassa_payout/py.typed
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-01-17 09:50:40.408428 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    12250 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3698 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/entry_points.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/not-zip-safe
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       48 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/requires.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       16 2023-01-17 09:50:40.000000 yookassa-payout-2.5.0/src/yookassa_payout.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.529281 yookassa-payout-2.5.1/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1267 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/CHANGELOG.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      231 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/CONTRIBUTING.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1079 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/LICENSE
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      150 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/MANIFEST.in
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10908 2023-05-22 11:45:44.529390 yookassa-payout-2.5.1/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10085 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/README.en.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    13123 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/README.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2023-05-22 11:45:44.530626 yookassa-payout-2.5.1/setup.cfg
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1598 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/setup.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.450636 yookassa-payout-2.5.1/src/
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.463131 yookassa-payout-2.5.1/src/yookassa_payout/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      148 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      106 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/__main__.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.471113 yookassa-payout-2.5.1/src/yookassa_payout/artefacts/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       58 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/artefacts/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6391 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/artefacts/deposit.cer
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1373 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/cli.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2125 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/configuration.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.472501 yookassa-payout-2.5.1/src/yookassa_payout/domain/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/__init__.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.485327 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1490 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/base_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5915 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/cli_client.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7839 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/client.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      129 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/currency.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      361 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/data_context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3315 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/error_converter.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4088 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/generator_csr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      623 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/http_verb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      935 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/keychain.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5234 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/openssl_helper.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6346 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/common/xml_helper.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.494537 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/api_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      132 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/authorize_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      144 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/bad_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      144 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/forbidden_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/not_found_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      141 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/open_ssl_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      152 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/response_processing_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      149 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/too_many_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      146 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/exceptions/unauthorized_error.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.496369 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2737 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/organization.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.501170 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7125 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/bank_account_recipient.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6677 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/bank_card_recipient.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      846 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/recipient.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      847 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/recipient_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.505330 yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1416 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3249 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2151 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification_response.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.516657 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1212 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/balance_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3162 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/deposition_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      703 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/deposition_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      463 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/make_deposition_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/request_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/synonym_card_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      463 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/request/test_deposition_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.524926 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1295 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/balance_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2116 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/deposition_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      752 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/deposition_response_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/make_deposition_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1078 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/response_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2739 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/synonym_card_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      168 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/domain/response/test_deposition_response.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.529063 yookassa-payout-2.5.1/src/yookassa_payout/logging/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/logging/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      638 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/logging/adapter.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1770 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/logging/classes.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1816 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/logging/config.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3822 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/payout.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      158 2023-05-22 11:45:42.000000 yookassa-payout-2.5.1/src/yookassa_payout/py.typed
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:45:44.469675 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10908 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3698 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       61 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/entry_points.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/not-zip-safe
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       48 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/requires.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       16 2023-05-22 11:45:44.000000 yookassa-payout-2.5.1/src/yookassa_payout.egg-info/top_level.txt
```

### Comparing `yookassa-payout-2.5.0/CHANGELOG.md` & `yookassa-payout-2.5.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+### v2.5.1 от 22.05.2023
+* Использование параметра allowed_methods вместо устаревшего method_whitelist в запросах
+
 ### v2.5.0 от 17.01.2023
 * Смена сертификата проверки подписи
 
 ### v2.4.0 от 25.04.2022
 * Обработка необязательных параметров для bank_card_recipient
 * Корректное закрытие ресурса os.pipe()
 * Смена ссылок с github на bitbucket
```

### Comparing `yookassa-payout-2.5.0/LICENSE` & `yookassa-payout-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/PKG-INFO` & `yookassa-payout-2.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,194 +1,195 @@
 Metadata-Version: 2.1
 Name: yookassa-payout
-Version: 2.5.0
+Version: 2.5.1
 Summary: YooKassa Payout API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
-Description: # YooMoney Payout API Python Client Library
-        
-        [![Build Status](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python)
-        [![Latest Stable Version](https://img.shields.io/pypi/v/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
-        [![Total Downloads](https://img.shields.io/pypi/dm/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
-        [![License](https://img.shields.io/pypi/l/yookassa-payout.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python)
-        
-        [Russian](README.md) | English
-        
-        Client to work on the [Protocol for mass payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
-        
-        ## Opportunities
-        You can with this SDK:
-        1. [Generate a certificate](https://yookassa.ru/docs/payment-solution/supplementary/security?lang=en) for interaction with YooMoney.
-        2. [Transfer money](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en) to individuals for wallets in YooMoney, mobile phone numbers, Bank cards and accounts (makeDeposition).
-        3. [To test the possibility of transfer of remittances](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en#test-deposition) to wallets in YooMoney (testDeposition).
-        4. [Keep track of the balance of payouts](https://yookassa.ru/docs/payouts/api/balance?lang=en) (balance).
-        5. [Receive notifications](https://yookassa.ru/docs/payouts/api/error-deposition-notification?lang=en) the unsuccessful status of transfers to a Bank account, card, or mobile phone (errorDepositionNotification).
-        
-        ## Requirements
-        * Python 3.5 (or later version)
-        * pip
-        
-        ## Installation
-        ### Under console using pip
-        
-        1. Install pip.
-        2. In the console, run the following command:
-        ```bash
-        pip install yookassa-payout
-        ```
-        
-        ### Under console using easy_install
-        1. Install easy_install.
-        2. In the console, run the following command:
-        ```bash
-        easy_install --upgrade yookassa-payout
-        ```
-        
-        ### Manually
-        1. In the console, run the following command:
-        ```bash
-        wget https://git.yoomoney.ru/rest/api/latest/projects/SDK/repos/yookassa-payout-sdk-python/archive?format=zip -O yookassa-payout-sdk-python-master.zip
-        unzip yookassa-payout-sdk-python-master.zip -d yookassa-payout-sdk-python-master
-        cd yookassa-payout-sdk-python-master
-        python setup.py install
-        ```
-        
-        ## Getting a certificate for authenticating requests
-        To interact with YooMoney.The cashier must obtain a certificate. For this:
-        1. Create a private key and a certificate request (CSR).
-        2. Fill out the certificate application form.
-        3. Exchange data with YooMoney.
-        
-        ### Step 1. Creating a private key and CSR
-        
-        #### Using the SDK method
-        1. Import classes to create CSR
-        ```python
-        from yookassa_payout.domain.models.organization import Organization
-        from yookassa_payout.payout import Payout
-        ```
-        
-        2. Create an instance of the `Organization` class with data for creating the request. All data must be entered in Latin.
-        ```python
-        org = Organization({
-            "org_name": "YooMoney",              # Organization Name (Latin)
-            "common_name": "/business/yoomoney", # Common Name, for example the name of your organization; must start with «/business/»
-            "email": "cms@yoomoney.ru"           # Email
-        })
-        ```
-        3. Create a CSR and a private key.
-        ```python
-        # Specify the location where the files should be saved and the password for the private key (if necessary)
-        Payout.get_csr(org, './files/output', '12345')
-        ```
-        As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
-        
-        #### Via the console
-        1. In the console, go to your project folder.
-        ```bash
-        cd '<your project folder>'
-        ```
-        
-        2. Execute the command:
-        ```
-        yookassa-payout -getcsr
-        ```
-        
-        3. Enter data for the certificate, following the instructions on the screen. The text must be entered in Latin letters.
-        As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
-        
-        ### Step 2. Filling out the certificate application
-        [Download the application](https://yookassa.ru/docs/ssl_cert_form.doc) to the certificate, fill it out and print it out. Sign and seal the document. Scan.
-        
-        | **Parameter**                                    | **Description**                                                                                                                                                                                                                                                                                                                                                             |
-        |:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | CN                                               | Must match the value of the Common Name parameter (eg, YOUR name). For example, */business/predpriyatie*.                                                                                                                                                                                                                                                                   |
-        | Electronic signature of the certificate request  | The text view obtained in the previous step.                                                                                                                                                                                                                                                                                                                                |
-        | Organization name in Latin letters               | Must match the value of the Organization Name parameter (eg, company) *Internet Widgits Pty Ltd*.                                                                                                                                                                                                                                                                           |
-        | The reason for the request                       | Possible options: <ul><li>*initial* — to get the first certificate;</li><li>*scheduled replacement* — to replace a certificate that has expired;</li><li>*replacement of a compromised* — to replace a previously issued certificate in the event of a security breach;</li><li>*adding a server* — to use the new certificate on additional servers or services.</li></ul> |
-        | Contact person (full name, phone number, e-mail) | Contact a specialist to contact you if you have any questions about the issued certificate.                                                                                                                                                                                                                                                                                 |
-        
-        ### Step 3. Data exchange with YooMoney
-        Send the certificate request file (request.csr) and a scan of the request by email to your YooMoney Manager.Box office.
-        In response to the request, the Manager will send a file with the certificate within 2 business days. The certificate is valid for 1 year.
-        Place the received certificate on your server
-        
-        ## Start of work
-        1. Determine what types of payouts you need and whether you want to check your balance.
-        2. Import required classes
-        ```python
-        from yookassa_payout.domain.common.keychain import KeyChain
-        from yookassa_payout.configuration import Configuration
-        from yookassa_payout.payout import Payout
-        ```
-        
-        3. Import the classes you need to solve your problems.
-        4. Create an instance of the `KeyChain` class by passing the path to the public key, the path to the private key, and, if necessary, the password for the private key.
-        ```python
-        keychain = KeyChain('publicCert.cer', 'privateCert.pem', 'password')
-        ```
-        
-        5. Create an instance of the `Client` class and pass the gateway ID from the [merchant profile](https://yookassa.ru/my) YooMoney and instance of the `KeyChain` class.
-        ```python
-        Configuration.configure('000000', keychain)
-        ```
-        
-        6. Call the appropriate method. [More information about making payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
-        
-        #### Example of payout to a Bank account
-        ```python
-        # Importing classes
-        from yookassa_payout.configuration import Configuration
-        from yookassa_payout.payout import Payout
-        from yookassa_payout.domain.common.keychain import KeyChain
-        from yookassa_payout.domain.models.recipients.bank_account_recipient import BankAccountRecipient
-        from yookassa_payout.domain.request.make_deposition_request import MakeDepositionRequest
-        
-        # Creating a housekeeper and saving settings
-        keychain = KeyChain('./files/250000.cer', './files/privateKey.pem', '12345')
-        Configuration.configure(250000, keychain)
-        
-        # Getting the current balance
-        balance = Payout.get_balance()
-        
-        # The compilation of data on the beneficiary
-        recipient = BankAccountRecipient()
-        recipient.pof_offer_accepted = True
-        recipient.bank_name = 'Barclays'
-        recipient.bank_city = 'London'
-        recipient.bank_cor_account = '30101810400000000225'
-        recipient.customer_account = '40817810255030943620'
-        recipient.bank_bik = '042809679'
-        recipient.payment_purpose = 'Refund under the agreement 25-001, without VAT'
-        recipient.pdr_first_name = 'John'
-        recipient.pdr_last_name = 'Watson'
-        recipient.pdr_doc_number = '4002109067'
-        recipient.pdr_doc_issue_date = '1999-07-30'
-        recipient.pdr_address = 'Baker street, 221'
-        recipient.pdr_birth_date = '1987-05-24'
-        recipient.sms_phone_number = '79653457676'
-        
-        # Preparing a request to create a payout
-        request = MakeDepositionRequest()
-        request.agent_id = 250000
-        request.client_order_id = '215d8da0-000f-50be-b000-0003308c89be'
-        request.request_dt = '2020-03-04T15:39:45.456+03:00'
-        request.payment_params = recipient
-        
-        # The carrying out of the payout
-        result = Payout.create_deposition(request)
-        ```
-        
 Keywords: yoomoney,yookassa,payout,sdk,python
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# YooMoney Payout API Python Client Library
+
+[![Build Status](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python)
+[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
+[![Total Downloads](https://img.shields.io/pypi/dm/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
+[![License](https://img.shields.io/pypi/l/yookassa-payout.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python)
+
+[Russian](README.md) | English
+
+Client to work on the [Protocol for mass payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
+
+## Opportunities
+You can with this SDK:
+1. [Generate a certificate](https://yookassa.ru/docs/payment-solution/supplementary/security?lang=en) for interaction with YooMoney.
+2. [Transfer money](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en) to individuals for wallets in YooMoney, mobile phone numbers, Bank cards and accounts (makeDeposition).
+3. [To test the possibility of transfer of remittances](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en#test-deposition) to wallets in YooMoney (testDeposition).
+4. [Keep track of the balance of payouts](https://yookassa.ru/docs/payouts/api/balance?lang=en) (balance).
+5. [Receive notifications](https://yookassa.ru/docs/payouts/api/error-deposition-notification?lang=en) the unsuccessful status of transfers to a Bank account, card, or mobile phone (errorDepositionNotification).
+
+## Requirements
+* Python 3.5 (or later version)
+* pip
+
+## Installation
+### Under console using pip
+
+1. Install pip.
+2. In the console, run the following command:
+```bash
+pip install yookassa-payout
+```
+
+### Under console using easy_install
+1. Install easy_install.
+2. In the console, run the following command:
+```bash
+easy_install --upgrade yookassa-payout
+```
+
+### Manually
+1. In the console, run the following command:
+```bash
+wget https://git.yoomoney.ru/rest/api/latest/projects/SDK/repos/yookassa-payout-sdk-python/archive?format=zip -O yookassa-payout-sdk-python-master.zip
+unzip yookassa-payout-sdk-python-master.zip -d yookassa-payout-sdk-python-master
+cd yookassa-payout-sdk-python-master
+python setup.py install
+```
+
+## Getting a certificate for authenticating requests
+To interact with YooMoney.The cashier must obtain a certificate. For this:
+1. Create a private key and a certificate request (CSR).
+2. Fill out the certificate application form.
+3. Exchange data with YooMoney.
+
+### Step 1. Creating a private key and CSR
+
+#### Using the SDK method
+1. Import classes to create CSR
+```python
+from yookassa_payout.domain.models.organization import Organization
+from yookassa_payout.payout import Payout
+```
+
+2. Create an instance of the `Organization` class with data for creating the request. All data must be entered in Latin.
+```python
+org = Organization({
+    "org_name": "YooMoney",              # Organization Name (Latin)
+    "common_name": "/business/yoomoney", # Common Name, for example the name of your organization; must start with «/business/»
+    "email": "cms@yoomoney.ru"           # Email
+})
+```
+3. Create a CSR and a private key.
+```python
+# Specify the location where the files should be saved and the password for the private key (if necessary)
+Payout.get_csr(org, './files/output', '12345')
+```
+As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
+
+#### Via the console
+1. In the console, go to your project folder.
+```bash
+cd '<your project folder>'
+```
+
+2. Execute the command:
+```
+yookassa-payout -getcsr
+```
+
+3. Enter data for the certificate, following the instructions on the screen. The text must be entered in Latin letters.
+As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
+
+### Step 2. Filling out the certificate application
+[Download the application](https://yookassa.ru/docs/ssl_cert_form.doc) to the certificate, fill it out and print it out. Sign and seal the document. Scan.
+
+| **Parameter**                                    | **Description**                                                                                                                                                                                                                                                                                                                                                             |
+|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CN                                               | Must match the value of the Common Name parameter (eg, YOUR name). For example, */business/predpriyatie*.                                                                                                                                                                                                                                                                   |
+| Electronic signature of the certificate request  | The text view obtained in the previous step.                                                                                                                                                                                                                                                                                                                                |
+| Organization name in Latin letters               | Must match the value of the Organization Name parameter (eg, company) *Internet Widgits Pty Ltd*.                                                                                                                                                                                                                                                                           |
+| The reason for the request                       | Possible options: <ul><li>*initial* — to get the first certificate;</li><li>*scheduled replacement* — to replace a certificate that has expired;</li><li>*replacement of a compromised* — to replace a previously issued certificate in the event of a security breach;</li><li>*adding a server* — to use the new certificate on additional servers or services.</li></ul> |
+| Contact person (full name, phone number, e-mail) | Contact a specialist to contact you if you have any questions about the issued certificate.                                                                                                                                                                                                                                                                                 |
+
+### Step 3. Data exchange with YooMoney
+Send the certificate request file (request.csr) and a scan of the request by email to your YooMoney Manager.Box office.
+In response to the request, the Manager will send a file with the certificate within 2 business days. The certificate is valid for 1 year.
+Place the received certificate on your server
+
+## Start of work
+1. Determine what types of payouts you need and whether you want to check your balance.
+2. Import required classes
+```python
+from yookassa_payout.domain.common.keychain import KeyChain
+from yookassa_payout.configuration import Configuration
+from yookassa_payout.payout import Payout
+```
+
+3. Import the classes you need to solve your problems.
+4. Create an instance of the `KeyChain` class by passing the path to the public key, the path to the private key, and, if necessary, the password for the private key.
+```python
+keychain = KeyChain('publicCert.cer', 'privateCert.pem', 'password')
+```
+
+5. Create an instance of the `Client` class and pass the gateway ID from the [merchant profile](https://yookassa.ru/my) YooMoney and instance of the `KeyChain` class.
+```python
+Configuration.configure('000000', keychain)
+```
+
+6. Call the appropriate method. [More information about making payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
+
+#### Example of payout to a Bank account
+```python
+# Importing classes
+from yookassa_payout.configuration import Configuration
+from yookassa_payout.payout import Payout
+from yookassa_payout.domain.common.keychain import KeyChain
+from yookassa_payout.domain.models.recipients.bank_account_recipient import BankAccountRecipient
+from yookassa_payout.domain.request.make_deposition_request import MakeDepositionRequest
+
+# Creating a housekeeper and saving settings
+keychain = KeyChain('./files/250000.cer', './files/privateKey.pem', '12345')
+Configuration.configure(250000, keychain)
+
+# Getting the current balance
+balance = Payout.get_balance()
+
+# The compilation of data on the beneficiary
+recipient = BankAccountRecipient()
+recipient.pof_offer_accepted = True
+recipient.bank_name = 'Barclays'
+recipient.bank_city = 'London'
+recipient.bank_cor_account = '30101810400000000225'
+recipient.customer_account = '40817810255030943620'
+recipient.bank_bik = '042809679'
+recipient.payment_purpose = 'Refund under the agreement 25-001, without VAT'
+recipient.pdr_first_name = 'John'
+recipient.pdr_last_name = 'Watson'
+recipient.pdr_doc_number = '4002109067'
+recipient.pdr_doc_issue_date = '1999-07-30'
+recipient.pdr_address = 'Baker street, 221'
+recipient.pdr_birth_date = '1987-05-24'
+recipient.sms_phone_number = '79653457676'
+
+# Preparing a request to create a payout
+request = MakeDepositionRequest()
+request.agent_id = 250000
+request.client_order_id = '215d8da0-000f-50be-b000-0003308c89be'
+request.request_dt = '2020-03-04T15:39:45.456+03:00'
+request.payment_params = recipient
+
+# The carrying out of the payout
+result = Payout.create_deposition(request)
+```
```

### Comparing `yookassa-payout-2.5.0/README.en.md` & `yookassa-payout-2.5.1/README.en.md`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/README.md` & `yookassa-payout-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/setup.py` & `yookassa-payout-2.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,9 +35,10 @@
         "Natural Language :: Russian",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
     ],
 )
```

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/artefacts/deposit.cer` & `yookassa-payout-2.5.1/src/yookassa_payout/artefacts/deposit.cer`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/cli.py` & `yookassa-payout-2.5.1/src/yookassa_payout/cli.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/configuration.py` & `yookassa-payout-2.5.1/src/yookassa_payout/configuration.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/base_object.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/base_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/cli_client.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/cli_client.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/client.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         return raw_response
 
     def get_session(self, is_ssl=True):
         session = requests.Session()
         retries = Retry(total=self.max_attempts,
                         backoff_factor=self.timeout / 1000,
-                        method_whitelist=['POST'],
+                        allowed_methods=['POST'],
                         status_forcelist=[202])
         if is_ssl:
             session.mount('https://', SSLAdapter(keychain=self.keychain, max_retries=retries))
         else:
             session.mount('https://', HTTPAdapter(max_retries=retries))
         return session
 
@@ -177,15 +177,15 @@
             message = 'Response with code [{}] received.'.format(info['status_code'])
             Configuration.logger.info(message, context=context)
 
 
 class SSLAdapter(HTTPAdapter):
     def __init__(self, keychain, *args, **kwargs):
         self._keychain = keychain
-        return super(SSLAdapter, self).__init__(*args, **kwargs)
+        super(SSLAdapter, self).__init__(*args, **kwargs)
 
     def init_poolmanager(self, *args, **kwargs):
         self._add_ssl_context(kwargs)
         return super(SSLAdapter, self).init_poolmanager(*args, **kwargs)
 
     def proxy_manager_for(self, *args, **kwargs):
         self._add_ssl_context(kwargs)
```

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/error_converter.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/error_converter.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/generator_csr.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/generator_csr.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/http_verb.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/http_verb.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/keychain.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/keychain.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/openssl_helper.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/openssl_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/common/xml_helper.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/common/xml_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/models/organization.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/models/organization.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/bank_account_recipient.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/bank_account_recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/bank_card_recipient.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/bank_card_recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/recipient.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/models/recipients/recipient_factory.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/models/recipients/recipient_factory.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification_request.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/notification/error_deposition_notification_response.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/notification/error_deposition_notification_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/request/balance_request.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/request/balance_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/request/deposition_request.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/request/deposition_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/request/deposition_request_builder.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/request/deposition_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/request/request_object.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/request/request_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/request/synonym_card_request.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/request/synonym_card_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/response/balance_response.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/response/balance_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/response/deposition_response.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/response/deposition_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/response/deposition_response_builder.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/response/deposition_response_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/response/response_object.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/response/response_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/domain/response/synonym_card_response.py` & `yookassa-payout-2.5.1/src/yookassa_payout/domain/response/synonym_card_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/logging/adapter.py` & `yookassa-payout-2.5.1/src/yookassa_payout/logging/adapter.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/logging/classes.py` & `yookassa-payout-2.5.1/src/yookassa_payout/logging/classes.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/logging/config.py` & `yookassa-payout-2.5.1/src/yookassa_payout/logging/config.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout/payout.py` & `yookassa-payout-2.5.1/src/yookassa_payout/payout.py`

 * *Files identical despite different names*

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout.egg-info/PKG-INFO` & `yookassa-payout-2.5.1/src/yookassa_payout.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,194 +1,195 @@
 Metadata-Version: 2.1
 Name: yookassa-payout
-Version: 2.5.0
+Version: 2.5.1
 Summary: YooKassa Payout API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
-Description: # YooMoney Payout API Python Client Library
-        
-        [![Build Status](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python)
-        [![Latest Stable Version](https://img.shields.io/pypi/v/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
-        [![Total Downloads](https://img.shields.io/pypi/dm/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
-        [![License](https://img.shields.io/pypi/l/yookassa-payout.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python)
-        
-        [Russian](README.md) | English
-        
-        Client to work on the [Protocol for mass payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
-        
-        ## Opportunities
-        You can with this SDK:
-        1. [Generate a certificate](https://yookassa.ru/docs/payment-solution/supplementary/security?lang=en) for interaction with YooMoney.
-        2. [Transfer money](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en) to individuals for wallets in YooMoney, mobile phone numbers, Bank cards and accounts (makeDeposition).
-        3. [To test the possibility of transfer of remittances](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en#test-deposition) to wallets in YooMoney (testDeposition).
-        4. [Keep track of the balance of payouts](https://yookassa.ru/docs/payouts/api/balance?lang=en) (balance).
-        5. [Receive notifications](https://yookassa.ru/docs/payouts/api/error-deposition-notification?lang=en) the unsuccessful status of transfers to a Bank account, card, or mobile phone (errorDepositionNotification).
-        
-        ## Requirements
-        * Python 3.5 (or later version)
-        * pip
-        
-        ## Installation
-        ### Under console using pip
-        
-        1. Install pip.
-        2. In the console, run the following command:
-        ```bash
-        pip install yookassa-payout
-        ```
-        
-        ### Under console using easy_install
-        1. Install easy_install.
-        2. In the console, run the following command:
-        ```bash
-        easy_install --upgrade yookassa-payout
-        ```
-        
-        ### Manually
-        1. In the console, run the following command:
-        ```bash
-        wget https://git.yoomoney.ru/rest/api/latest/projects/SDK/repos/yookassa-payout-sdk-python/archive?format=zip -O yookassa-payout-sdk-python-master.zip
-        unzip yookassa-payout-sdk-python-master.zip -d yookassa-payout-sdk-python-master
-        cd yookassa-payout-sdk-python-master
-        python setup.py install
-        ```
-        
-        ## Getting a certificate for authenticating requests
-        To interact with YooMoney.The cashier must obtain a certificate. For this:
-        1. Create a private key and a certificate request (CSR).
-        2. Fill out the certificate application form.
-        3. Exchange data with YooMoney.
-        
-        ### Step 1. Creating a private key and CSR
-        
-        #### Using the SDK method
-        1. Import classes to create CSR
-        ```python
-        from yookassa_payout.domain.models.organization import Organization
-        from yookassa_payout.payout import Payout
-        ```
-        
-        2. Create an instance of the `Organization` class with data for creating the request. All data must be entered in Latin.
-        ```python
-        org = Organization({
-            "org_name": "YooMoney",              # Organization Name (Latin)
-            "common_name": "/business/yoomoney", # Common Name, for example the name of your organization; must start with «/business/»
-            "email": "cms@yoomoney.ru"           # Email
-        })
-        ```
-        3. Create a CSR and a private key.
-        ```python
-        # Specify the location where the files should be saved and the password for the private key (if necessary)
-        Payout.get_csr(org, './files/output', '12345')
-        ```
-        As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
-        
-        #### Via the console
-        1. In the console, go to your project folder.
-        ```bash
-        cd '<your project folder>'
-        ```
-        
-        2. Execute the command:
-        ```
-        yookassa-payout -getcsr
-        ```
-        
-        3. Enter data for the certificate, following the instructions on the screen. The text must be entered in Latin letters.
-        As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
-        
-        ### Step 2. Filling out the certificate application
-        [Download the application](https://yookassa.ru/docs/ssl_cert_form.doc) to the certificate, fill it out and print it out. Sign and seal the document. Scan.
-        
-        | **Parameter**                                    | **Description**                                                                                                                                                                                                                                                                                                                                                             |
-        |:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | CN                                               | Must match the value of the Common Name parameter (eg, YOUR name). For example, */business/predpriyatie*.                                                                                                                                                                                                                                                                   |
-        | Electronic signature of the certificate request  | The text view obtained in the previous step.                                                                                                                                                                                                                                                                                                                                |
-        | Organization name in Latin letters               | Must match the value of the Organization Name parameter (eg, company) *Internet Widgits Pty Ltd*.                                                                                                                                                                                                                                                                           |
-        | The reason for the request                       | Possible options: <ul><li>*initial* — to get the first certificate;</li><li>*scheduled replacement* — to replace a certificate that has expired;</li><li>*replacement of a compromised* — to replace a previously issued certificate in the event of a security breach;</li><li>*adding a server* — to use the new certificate on additional servers or services.</li></ul> |
-        | Contact person (full name, phone number, e-mail) | Contact a specialist to contact you if you have any questions about the issued certificate.                                                                                                                                                                                                                                                                                 |
-        
-        ### Step 3. Data exchange with YooMoney
-        Send the certificate request file (request.csr) and a scan of the request by email to your YooMoney Manager.Box office.
-        In response to the request, the Manager will send a file with the certificate within 2 business days. The certificate is valid for 1 year.
-        Place the received certificate on your server
-        
-        ## Start of work
-        1. Determine what types of payouts you need and whether you want to check your balance.
-        2. Import required classes
-        ```python
-        from yookassa_payout.domain.common.keychain import KeyChain
-        from yookassa_payout.configuration import Configuration
-        from yookassa_payout.payout import Payout
-        ```
-        
-        3. Import the classes you need to solve your problems.
-        4. Create an instance of the `KeyChain` class by passing the path to the public key, the path to the private key, and, if necessary, the password for the private key.
-        ```python
-        keychain = KeyChain('publicCert.cer', 'privateCert.pem', 'password')
-        ```
-        
-        5. Create an instance of the `Client` class and pass the gateway ID from the [merchant profile](https://yookassa.ru/my) YooMoney and instance of the `KeyChain` class.
-        ```python
-        Configuration.configure('000000', keychain)
-        ```
-        
-        6. Call the appropriate method. [More information about making payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
-        
-        #### Example of payout to a Bank account
-        ```python
-        # Importing classes
-        from yookassa_payout.configuration import Configuration
-        from yookassa_payout.payout import Payout
-        from yookassa_payout.domain.common.keychain import KeyChain
-        from yookassa_payout.domain.models.recipients.bank_account_recipient import BankAccountRecipient
-        from yookassa_payout.domain.request.make_deposition_request import MakeDepositionRequest
-        
-        # Creating a housekeeper and saving settings
-        keychain = KeyChain('./files/250000.cer', './files/privateKey.pem', '12345')
-        Configuration.configure(250000, keychain)
-        
-        # Getting the current balance
-        balance = Payout.get_balance()
-        
-        # The compilation of data on the beneficiary
-        recipient = BankAccountRecipient()
-        recipient.pof_offer_accepted = True
-        recipient.bank_name = 'Barclays'
-        recipient.bank_city = 'London'
-        recipient.bank_cor_account = '30101810400000000225'
-        recipient.customer_account = '40817810255030943620'
-        recipient.bank_bik = '042809679'
-        recipient.payment_purpose = 'Refund under the agreement 25-001, without VAT'
-        recipient.pdr_first_name = 'John'
-        recipient.pdr_last_name = 'Watson'
-        recipient.pdr_doc_number = '4002109067'
-        recipient.pdr_doc_issue_date = '1999-07-30'
-        recipient.pdr_address = 'Baker street, 221'
-        recipient.pdr_birth_date = '1987-05-24'
-        recipient.sms_phone_number = '79653457676'
-        
-        # Preparing a request to create a payout
-        request = MakeDepositionRequest()
-        request.agent_id = 250000
-        request.client_order_id = '215d8da0-000f-50be-b000-0003308c89be'
-        request.request_dt = '2020-03-04T15:39:45.456+03:00'
-        request.payment_params = recipient
-        
-        # The carrying out of the payout
-        result = Payout.create_deposition(request)
-        ```
-        
 Keywords: yoomoney,yookassa,payout,sdk,python
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# YooMoney Payout API Python Client Library
+
+[![Build Status](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-payout-sdk-python)
+[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
+[![Total Downloads](https://img.shields.io/pypi/dm/yookassa-payout.svg)](https://pypi.org/project/yookassa-payout/)
+[![License](https://img.shields.io/pypi/l/yookassa-payout.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-payout-sdk-python)
+
+[Russian](README.md) | English
+
+Client to work on the [Protocol for mass payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
+
+## Opportunities
+You can with this SDK:
+1. [Generate a certificate](https://yookassa.ru/docs/payment-solution/supplementary/security?lang=en) for interaction with YooMoney.
+2. [Transfer money](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en) to individuals for wallets in YooMoney, mobile phone numbers, Bank cards and accounts (makeDeposition).
+3. [To test the possibility of transfer of remittances](https://yookassa.ru/docs/payouts/api/make-deposition/basics?lang=en#test-deposition) to wallets in YooMoney (testDeposition).
+4. [Keep track of the balance of payouts](https://yookassa.ru/docs/payouts/api/balance?lang=en) (balance).
+5. [Receive notifications](https://yookassa.ru/docs/payouts/api/error-deposition-notification?lang=en) the unsuccessful status of transfers to a Bank account, card, or mobile phone (errorDepositionNotification).
+
+## Requirements
+* Python 3.5 (or later version)
+* pip
+
+## Installation
+### Under console using pip
+
+1. Install pip.
+2. In the console, run the following command:
+```bash
+pip install yookassa-payout
+```
+
+### Under console using easy_install
+1. Install easy_install.
+2. In the console, run the following command:
+```bash
+easy_install --upgrade yookassa-payout
+```
+
+### Manually
+1. In the console, run the following command:
+```bash
+wget https://git.yoomoney.ru/rest/api/latest/projects/SDK/repos/yookassa-payout-sdk-python/archive?format=zip -O yookassa-payout-sdk-python-master.zip
+unzip yookassa-payout-sdk-python-master.zip -d yookassa-payout-sdk-python-master
+cd yookassa-payout-sdk-python-master
+python setup.py install
+```
+
+## Getting a certificate for authenticating requests
+To interact with YooMoney.The cashier must obtain a certificate. For this:
+1. Create a private key and a certificate request (CSR).
+2. Fill out the certificate application form.
+3. Exchange data with YooMoney.
+
+### Step 1. Creating a private key and CSR
+
+#### Using the SDK method
+1. Import classes to create CSR
+```python
+from yookassa_payout.domain.models.organization import Organization
+from yookassa_payout.payout import Payout
+```
+
+2. Create an instance of the `Organization` class with data for creating the request. All data must be entered in Latin.
+```python
+org = Organization({
+    "org_name": "YooMoney",              # Organization Name (Latin)
+    "common_name": "/business/yoomoney", # Common Name, for example the name of your organization; must start with «/business/»
+    "email": "cms@yoomoney.ru"           # Email
+})
+```
+3. Create a CSR and a private key.
+```python
+# Specify the location where the files should be saved and the password for the private key (if necessary)
+Payout.get_csr(org, './files/output', '12345')
+```
+As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
+
+#### Via the console
+1. In the console, go to your project folder.
+```bash
+cd '<your project folder>'
+```
+
+2. Execute the command:
+```
+yookassa-payout -getcsr
+```
+
+3. Enter data for the certificate, following the instructions on the screen. The text must be entered in Latin letters.
+As a result, the SDK will generate a private key, CSR, and a text file with an electronic signature (necessary for further steps).
+
+### Step 2. Filling out the certificate application
+[Download the application](https://yookassa.ru/docs/ssl_cert_form.doc) to the certificate, fill it out and print it out. Sign and seal the document. Scan.
+
+| **Parameter**                                    | **Description**                                                                                                                                                                                                                                                                                                                                                             |
+|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CN                                               | Must match the value of the Common Name parameter (eg, YOUR name). For example, */business/predpriyatie*.                                                                                                                                                                                                                                                                   |
+| Electronic signature of the certificate request  | The text view obtained in the previous step.                                                                                                                                                                                                                                                                                                                                |
+| Organization name in Latin letters               | Must match the value of the Organization Name parameter (eg, company) *Internet Widgits Pty Ltd*.                                                                                                                                                                                                                                                                           |
+| The reason for the request                       | Possible options: <ul><li>*initial* — to get the first certificate;</li><li>*scheduled replacement* — to replace a certificate that has expired;</li><li>*replacement of a compromised* — to replace a previously issued certificate in the event of a security breach;</li><li>*adding a server* — to use the new certificate on additional servers or services.</li></ul> |
+| Contact person (full name, phone number, e-mail) | Contact a specialist to contact you if you have any questions about the issued certificate.                                                                                                                                                                                                                                                                                 |
+
+### Step 3. Data exchange with YooMoney
+Send the certificate request file (request.csr) and a scan of the request by email to your YooMoney Manager.Box office.
+In response to the request, the Manager will send a file with the certificate within 2 business days. The certificate is valid for 1 year.
+Place the received certificate on your server
+
+## Start of work
+1. Determine what types of payouts you need and whether you want to check your balance.
+2. Import required classes
+```python
+from yookassa_payout.domain.common.keychain import KeyChain
+from yookassa_payout.configuration import Configuration
+from yookassa_payout.payout import Payout
+```
+
+3. Import the classes you need to solve your problems.
+4. Create an instance of the `KeyChain` class by passing the path to the public key, the path to the private key, and, if necessary, the password for the private key.
+```python
+keychain = KeyChain('publicCert.cer', 'privateCert.pem', 'password')
+```
+
+5. Create an instance of the `Client` class and pass the gateway ID from the [merchant profile](https://yookassa.ru/my) YooMoney and instance of the `KeyChain` class.
+```python
+Configuration.configure('000000', keychain)
+```
+
+6. Call the appropriate method. [More information about making payouts](https://yookassa.ru/docs/payouts/api/using-api/basics?lang=en)
+
+#### Example of payout to a Bank account
+```python
+# Importing classes
+from yookassa_payout.configuration import Configuration
+from yookassa_payout.payout import Payout
+from yookassa_payout.domain.common.keychain import KeyChain
+from yookassa_payout.domain.models.recipients.bank_account_recipient import BankAccountRecipient
+from yookassa_payout.domain.request.make_deposition_request import MakeDepositionRequest
+
+# Creating a housekeeper and saving settings
+keychain = KeyChain('./files/250000.cer', './files/privateKey.pem', '12345')
+Configuration.configure(250000, keychain)
+
+# Getting the current balance
+balance = Payout.get_balance()
+
+# The compilation of data on the beneficiary
+recipient = BankAccountRecipient()
+recipient.pof_offer_accepted = True
+recipient.bank_name = 'Barclays'
+recipient.bank_city = 'London'
+recipient.bank_cor_account = '30101810400000000225'
+recipient.customer_account = '40817810255030943620'
+recipient.bank_bik = '042809679'
+recipient.payment_purpose = 'Refund under the agreement 25-001, without VAT'
+recipient.pdr_first_name = 'John'
+recipient.pdr_last_name = 'Watson'
+recipient.pdr_doc_number = '4002109067'
+recipient.pdr_doc_issue_date = '1999-07-30'
+recipient.pdr_address = 'Baker street, 221'
+recipient.pdr_birth_date = '1987-05-24'
+recipient.sms_phone_number = '79653457676'
+
+# Preparing a request to create a payout
+request = MakeDepositionRequest()
+request.agent_id = 250000
+request.client_order_id = '215d8da0-000f-50be-b000-0003308c89be'
+request.request_dt = '2020-03-04T15:39:45.456+03:00'
+request.payment_params = recipient
+
+# The carrying out of the payout
+result = Payout.create_deposition(request)
+```
```

### Comparing `yookassa-payout-2.5.0/src/yookassa_payout.egg-info/SOURCES.txt` & `yookassa-payout-2.5.1/src/yookassa_payout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

