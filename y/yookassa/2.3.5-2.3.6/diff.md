# Comparing `tmp/yookassa-2.3.5.tar.gz` & `tmp/yookassa-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yookassa-2.3.5.tar", last modified: Mon Feb 13 06:48:34 2023, max compression
+gzip compressed data, was "yookassa-2.3.6.tar", last modified: Mon May 22 11:58:41 2023, max compression
```

## Comparing `yookassa-2.3.5.tar` & `yookassa-2.3.6.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.625062 yookassa-2.3.5/
--rw-rw-rw-   0        0        0     1081 2023-02-13 06:48:29.000000 yookassa-2.3.5/LICENSE
--rw-rw-rw-   0        0        0     3243 2023-02-13 06:48:34.626067 yookassa-2.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     6187 2023-02-13 06:48:29.000000 yookassa-2.3.5/README.md
--rw-rw-rw-   0        0        0      107 2023-02-13 06:48:34.631029 yookassa-2.3.5/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-02-13 06:48:29.000000 yookassa-2.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:32.696603 yookassa-2.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:32.796458 yookassa-2.3.5/src/yookassa/
--rw-rw-rw-   0        0        0      466 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/__init__.py
--rw-rw-rw-   0        0        0     3874 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/client.py
--rw-rw-rw-   0        0        0     2545 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/configuration.py
--rw-rw-rw-   0        0        0     1812 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/deal.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:32.849825 yookassa-2.3.5/src/yookassa/domain/
--rw-rw-rw-   0        0        0       88 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.003418 yookassa-2.3.5/src/yookassa/domain/common/
--rw-rw-rw-   0        0        0      858 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/common/__init__.py
--rw-rw-rw-   0        0        0     1490 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/common/base_object.py
--rw-rw-rw-   0        0        0      553 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/common/confirmation_type.py
--rw-rw-rw-   0        0        0      386 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/common/context.py
--rw-rw-rw-   0        0        0      340 2023-02-13 06:48:29.000000 yookassa-2.3.5/src/yookassa/domain/common/data_context.py
--rw-rw-rw-   0        0        0      574 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/http_verb.py
--rw-rw-rw-   0        0        0     1462 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/payment_method_type.py
--rw-rw-rw-   0        0        0      560 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/receipt_type.py
--rw-rw-rw-   0        0        0      381 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/request_object.py
--rw-rw-rw-   0        0        0      290 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/response_object.py
--rw-rw-rw-   0        0        0      696 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/security_helper.py
--rw-rw-rw-   0        0        0     1097 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/type_factory.py
--rw-rw-rw-   0        0        0     3994 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/common/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.112457 yookassa-2.3.5/src/yookassa/domain/exceptions/
--rw-rw-rw-   0        0        0      677 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/__init__.py
--rw-rw-rw-   0        0        0       62 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/api_error.py
--rw-rw-rw-   0        0        0      125 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/authorize_error.py
--rw-rw-rw-   0        0        0      137 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/bad_request_error.py
--rw-rw-rw-   0        0        0      137 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/forbidden_error.py
--rw-rw-rw-   0        0        0      135 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/not_found_error.py
--rw-rw-rw-   0        0        0      145 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/response_processing_error.py
--rw-rw-rw-   0        0        0      142 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/too_many_request_error.py
--rw-rw-rw-   0        0        0      139 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/exceptions/unauthorized_error.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.338894 yookassa-2.3.5/src/yookassa/domain/models/
--rw-rw-rw-   0        0        0     1133 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/airline.py
--rw-rw-rw-   0        0        0      670 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/amount.py
--rw-rw-rw-   0        0        0     1286 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/authorization_details.py
--rw-rw-rw-   0        0        0     1875 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/cancellation_details.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.384438 yookassa-2.3.5/src/yookassa/domain/models/confirmation/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/__init__.py
--rw-rw-rw-   0        0        0      319 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/confirmation.py
--rw-rw-rw-   0        0        0     2515 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/confirmation_class_map.py
--rw-rw-rw-   0        0        0      316 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/confirmation_factory.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.463420 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/__init__.py
--rw-rw-rw-   0        0        0      550 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
--rw-rw-rw-   0        0        0      551 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_external.py
--rw-rw-rw-   0        0        0      922 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
--rw-rw-rw-   0        0        0      521 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
--rw-rw-rw-   0        0        0     1052 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
--rw-rw-rw-   0        0        0      376 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_request.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.539167 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/__init__.py
--rw-rw-rw-   0        0        0      901 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
--rw-rw-rw-   0        0        0      521 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_external.py
--rw-rw-rw-   0        0        0      794 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
--rw-rw-rw-   0        0        0      864 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
--rw-rw-rw-   0        0        0     1248 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
--rw-rw-rw-   0        0        0      215 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/currency.py
--rw-rw-rw-   0        0        0     3800 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/deal.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.602838 yookassa-2.3.5/src/yookassa/domain/models/payment_data/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/__init__.py
--rw-rw-rw-   0        0        0      518 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/card_type.py
--rw-rw-rw-   0        0        0      837 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/payment_data.py
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/payment_data_class_map.py
--rw-rw-rw-   0        0        0      366 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/payment_data_factory.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:33.826176 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/credit_card.py
--rw-rw-rw-   0        0        0      613 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
--rw-rw-rw-   0        0        0      655 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
--rw-rw-rw-   0        0        0     2356 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
--rw-rw-rw-   0        0        0      904 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
--rw-rw-rw-   0        0        0      765 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
--rw-rw-rw-   0        0        0      970 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
--rw-rw-rw-   0        0        0      462 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
--rw-rw-rw-   0        0        0      803 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
--rw-rw-rw-   0        0        0      765 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
--rw-rw-rw-   0        0        0      781 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
--rw-rw-rw-   0        0        0      428 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
--rw-rw-rw-   0        0        0      462 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
--rw-rw-rw-   0        0        0      448 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
--rw-rw-rw-   0        0        0      543 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
--rw-rw-rw-   0        0        0      462 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.071737 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/credit_card.py
--rw-rw-rw-   0        0        0      629 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
--rw-rw-rw-   0        0        0      464 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
--rw-rw-rw-   0        0        0     3397 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
--rw-rw-rw-   0        0        0      921 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
--rw-rw-rw-   0        0        0      781 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
--rw-rw-rw-   0        0        0      471 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
--rw-rw-rw-   0        0        0      478 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
--rw-rw-rw-   0        0        0      819 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
--rw-rw-rw-   0        0        0      444 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
--rw-rw-rw-   0        0        0      781 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
--rw-rw-rw-   0        0        0      816 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
--rw-rw-rw-   0        0        0      444 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
--rw-rw-rw-   0        0        0      478 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
--rw-rw-rw-   0        0        0      464 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
--rw-rw-rw-   0        0        0      559 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
--rw-rw-rw-   0        0        0      478 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
--rw-rw-rw-   0        0        0      206 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.117766 yookassa-2.3.5/src/yookassa/domain/models/payout_data/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/__init__.py
--rw-rw-rw-   0        0        0      328 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/payout_destination.py
--rw-rw-rw-   0        0        0     1403 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
--rw-rw-rw-   0        0        0      395 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/payout_destination_factory.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.168205 yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/__init__.py
--rw-rw-rw-   0        0        0      444 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/credit_card.py
--rw-rw-rw-   0        0        0      940 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
--rw-rw-rw-   0        0        0      711 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.214687 yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/credit_card.py
--rw-rw-rw-   0        0        0      940 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
--rw-rw-rw-   0        0        0      711 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/receipt.py
--rw-rw-rw-   0        0        0     1052 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/receipt_customer.py
--rw-rw-rw-   0        0        0     3518 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/receipt_item.py
--rw-rw-rw-   0        0        0      691 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/receipt_item_supplier.py
--rw-rw-rw-   0        0        0      559 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/recipient.py
--rw-rw-rw-   0        0        0     1257 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/refund_source.py
--rw-rw-rw-   0        0        0     2772 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/requestor.py
--rw-rw-rw-   0        0        0     1121 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/settlement.py
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/models/transfer.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.255414 yookassa-2.3.5/src/yookassa/domain/notification/
--rw-rw-rw-   0        0        0      223 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/notification/__init__.py
--rw-rw-rw-   0        0        0     3976 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/notification/webhook_notification.py
--rw-rw-rw-   0        0        0      468 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/notification/webhook_notification_types.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.451619 yookassa-2.3.5/src/yookassa/domain/request/
--rw-rw-rw-   0        0        0     1121 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/__init__.py
--rw-rw-rw-   0        0        0      745 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/capture_payment_builder.py
--rw-rw-rw-   0        0        0     2631 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/capture_payment_request.py
--rw-rw-rw-   0        0        0     1605 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/deal_request.py
--rw-rw-rw-   0        0        0      609 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/deal_request_builder.py
--rw-rw-rw-   0        0        0     9585 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/payment_request.py
--rw-rw-rw-   0        0        0     1882 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/payment_request_builder.py
--rw-rw-rw-   0        0        0     3646 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/payout_request.py
--rw-rw-rw-   0        0        0      837 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/payout_request_builder.py
--rw-rw-rw-   0        0        0     3377 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/receipt_item_request.py
--rw-rw-rw-   0        0        0     5606 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/receipt_request.py
--rw-rw-rw-   0        0        0     1124 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/receipt_request_builder.py
--rw-rw-rw-   0        0        0     3499 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/refund_request.py
--rw-rw-rw-   0        0        0      814 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/refund_request_builder.py
--rw-rw-rw-   0        0        0      508 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/request/webhook_request.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:34.617031 yookassa-2.3.5/src/yookassa/domain/response/
--rw-rw-rw-   0        0        0      987 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/__init__.py
--rw-rw-rw-   0        0        0      832 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/deal_list_response.py
--rw-rw-rw-   0        0        0     2066 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/deal_response.py
--rw-rw-rw-   0        0        0      844 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/payment_list_response.py
--rw-rw-rw-   0        0        0     5333 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/payment_response.py
--rw-rw-rw-   0        0        0     2341 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/payout_response.py
--rw-rw-rw-   0        0        0     2040 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/receipt_item_response.py
--rw-rw-rw-   0        0        0      844 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/receipt_list_response.py
--rw-rw-rw-   0        0        0     3575 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/receipt_response.py
--rw-rw-rw-   0        0        0      838 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/refund_list_response.py
--rw-rw-rw-   0        0        0     2142 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/refund_response.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/transfer_response.py
--rw-rw-rw-   0        0        0     1062 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/domain/response/webhook_response.py
--rw-rw-rw-   0        0        0     3605 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/payment.py
--rw-rw-rw-   0        0        0     1611 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/payout.py
--rw-rw-rw-   0        0        0     1954 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/receipt.py
--rw-rw-rw-   0        0        0     1914 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/refund.py
--rw-rw-rw-   0        0        0      670 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/settings.py
--rw-rw-rw-   0        0        0     1984 2023-02-13 06:48:30.000000 yookassa-2.3.5/src/yookassa/webhook.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:48:32.829428 yookassa-2.3.5/src/yookassa.egg-info/
--rw-rw-rw-   0        0        0     3243 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8658 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-13 06:48:32.000000 yookassa-2.3.5/src/yookassa.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.526081 yookassa-2.3.6/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1081 2023-05-22 11:58:40.000000 yookassa-2.3.6/LICENSE
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-05-22 11:58:41.526184 yookassa-2.3.6/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6187 2023-05-22 11:58:40.000000 yookassa-2.3.6/README.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2023-05-22 11:58:41.527744 yookassa-2.3.6/setup.cfg
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3784 2023-05-22 11:58:40.000000 yookassa-2.3.6/setup.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.392109 yookassa-2.3.6/src/
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.402552 yookassa-2.3.6/src/yookassa/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      466 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3873 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/client.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2545 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/configuration.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1812 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/deal.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.406282 yookassa-2.3.6/src/yookassa/domain/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       88 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/__init__.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.416508 yookassa-2.3.6/src/yookassa/domain/common/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      858 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1490 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/base_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      553 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/confirmation_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      340 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/data_context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      574 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/http_verb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/payment_method_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      560 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/receipt_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      381 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/request_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      290 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/response_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      696 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/security_helper.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1097 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/type_factory.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3994 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/user_agent.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.424646 yookassa-2.3.6/src/yookassa/domain/exceptions/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      677 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/api_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      125 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/authorize_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/bad_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/forbidden_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      135 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/not_found_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      145 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/response_processing_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/too_many_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      139 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/unauthorized_error.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.439741 yookassa-2.3.6/src/yookassa/domain/models/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1133 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4192 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/airline.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/amount.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1286 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/authorization_details.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1875 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/cancellation_details.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.443251 yookassa-2.3.6/src/yookassa/domain/models/confirmation/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      319 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2515 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      316 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.448811 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      551 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      922 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      376 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.455058 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      901 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      794 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      864 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1248 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      215 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/currency.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3800 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/deal.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.459284 yookassa-2.3.6/src/yookassa/domain/models/payment_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      518 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/card_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6794 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      366 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.474705 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1903 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      613 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      655 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2356 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      904 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      970 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      803 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      428 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      448 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      543 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.489590 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3572 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      629 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3397 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      921 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      471 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      819 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      816 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      206 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.492777 yookassa-2.3.6/src/yookassa/domain/models/payout_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      328 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1403 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      395 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.496748 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.500507 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2190 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2333 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_customer.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3518 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_item.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      691 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_item_supplier.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/recipient.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1257 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/refund_source.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2772 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/requestor.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/settlement.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2088 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/transfer.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.502975 yookassa-2.3.6/src/yookassa/domain/notification/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      223 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3976 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      468 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification_types.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.514466 yookassa-2.3.6/src/yookassa/domain/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      745 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/capture_payment_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2631 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/capture_payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1605 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/deal_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      609 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/deal_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     9585 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1882 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payment_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3646 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payout_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payout_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3377 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_item_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5606 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1124 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3499 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/refund_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      814 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/refund_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/webhook_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.525863 yookassa-2.3.6/src/yookassa/domain/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      987 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      832 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/deal_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/deal_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payment_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5333 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payment_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2341 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payout_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2040 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_item_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3575 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      838 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/refund_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2142 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/refund_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2076 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/transfer_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1062 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/webhook_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3605 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/payment.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1611 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/payout.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1954 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1914 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/refund.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/settings.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1984 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/webhook.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.405750 yookassa-2.3.6/src/yookassa.egg-info/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     8658 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/not-zip-safe
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       43 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/requires.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        9 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/top_level.txt
```

### Comparing `yookassa-2.3.5/LICENSE` & `yookassa-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/PKG-INFO` & `yookassa-2.3.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-Metadata-Version: 2.1
-Name: yookassa
-Version: 2.3.5
-Summary: YooKassa API SDK Python Library
-Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
-Author: YooMoney
-Author-email: cms@yoomoney.ru
-License: MIT
-Keywords: yoomoney,yookassa,payout,sdk,python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# YooKassa API Python Client Library
-
-[![Build Status](https://travis-ci.org/yoomoney/yookassa-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-sdk-python)
-[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa.svg)](https://pypi.org/project/yookassa/)
-[![Total Downloads](https://img.shields.io/pypi/dm/yookassa.svg)](https://pypi.org/project/yookassa/)
-[![License](https://img.shields.io/pypi/l/yookassa.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python)
-
-[Russian](README.md) | English
-
-This product is used for managing payments under [The YooKassa API](https://yookassa.ru/en/developers/api)
-For usage by those who implemented YooKassa using the API method.
-
-## Requirements
-1. Python 2.7 or Python 3.x
-2. pip
-
-## Installation
-### Under console using pip
-
-1. Install pip.
-2. In the console, run the following command:
-```bash
-pip install --upgrade yookassa
-```
-
-### Under console using easy_install
-1. Install easy_install.
-2. In the console, run the following command:
-```bash
-easy_install --upgrade yookassa
-```
-
-### Manually
-
-1. In the console, run the following command:
-```bash
-wget https://pypi.python.org/packages/5a/be/5eafdfb14aa6f32107e9feb6514ca1ad3fe56f8e5ee59d20693b32f7e79f/yookassa-1.0.0.tar.gz#md5=46595279b5578fd82a199bfd4cd51db2
-tar zxf yookassa-1.0.0.tar.gz
-cd yookassa-1.0.0
-python setup.py install
-```
-
-
-## Commencing work
-
-1. Import module
-```python
-import yookassa
-```
-
-2. Configure a Client
-```python
-from yookassa import Configuration
-
-Configuration.configure('<Account Id>', '<Secret Key>')
-```
-
-or
-
-```python
-from yookassa import Configuration
-
-Configuration.account_id = '<Account Id>'
-Configuration.secret_key = '<Secret Key>'
-```
-
-or via oauth
-
-```python
-from yookassa import Configuration
-
-Configuration.configure_auth_token('<Oauth Token>')
-```
-
-If you agree to participate in the development of the SDK, you can submit data about your framework, cms or module:
-
-```python
-from yookassa import Configuration
-from yookassa.domain.common.user_agent import Version
-
-Configuration.configure('<Account Id>', '<Secret Key>')
-Configuration.configure_user_agent(
-    framework=Version('Django', '2.2.3'),
-    cms=Version('Wagtail', '2.6.2'),
-    module=Version('Y.CMS', '0.0.1')
-)
-```
-
-3. Call the required API method. [More details in our documentation for the YooKassa API](https://yookassa.ru/en/developers/api)
+Metadata-Version: 2.1
+Name: yookassa
+Version: 2.3.6
+Summary: YooKassa API SDK Python Library
+Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
+Author: YooMoney
+Author-email: cms@yoomoney.ru
+License: MIT
+Keywords: yoomoney,yookassa,payout,sdk,python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# YooKassa API Python Client Library
+
+[![Build Status](https://travis-ci.org/yoomoney/yookassa-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-sdk-python)
+[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa.svg)](https://pypi.org/project/yookassa/)
+[![Total Downloads](https://img.shields.io/pypi/dm/yookassa.svg)](https://pypi.org/project/yookassa/)
+[![License](https://img.shields.io/pypi/l/yookassa.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python)
+
+[Russian](README.md) | English
+
+This product is used for managing payments under [The YooKassa API](https://yookassa.ru/en/developers/api)
+For usage by those who implemented YooKassa using the API method.
+
+## Requirements
+1. Python 2.7 or Python 3.x
+2. pip
+
+## Installation
+### Under console using pip
+
+1. Install pip.
+2. In the console, run the following command:
+```bash
+pip install --upgrade yookassa
+```
+
+### Under console using easy_install
+1. Install easy_install.
+2. In the console, run the following command:
+```bash
+easy_install --upgrade yookassa
+```
+
+### Manually
+
+1. In the console, run the following command:
+```bash
+wget https://pypi.python.org/packages/5a/be/5eafdfb14aa6f32107e9feb6514ca1ad3fe56f8e5ee59d20693b32f7e79f/yookassa-1.0.0.tar.gz#md5=46595279b5578fd82a199bfd4cd51db2
+tar zxf yookassa-1.0.0.tar.gz
+cd yookassa-1.0.0
+python setup.py install
+```
+
+
+## Commencing work
+
+1. Import module
+```python
+import yookassa
+```
+
+2. Configure a Client
+```python
+from yookassa import Configuration
+
+Configuration.configure('<Account Id>', '<Secret Key>')
+```
+
+or
+
+```python
+from yookassa import Configuration
+
+Configuration.account_id = '<Account Id>'
+Configuration.secret_key = '<Secret Key>'
+```
+
+or via oauth
+
+```python
+from yookassa import Configuration
+
+Configuration.configure_auth_token('<Oauth Token>')
+```
+
+If you agree to participate in the development of the SDK, you can submit data about your framework, cms or module:
+
+```python
+from yookassa import Configuration
+from yookassa.domain.common.user_agent import Version
+
+Configuration.configure('<Account Id>', '<Secret Key>')
+Configuration.configure_user_agent(
+    framework=Version('Django', '2.2.3'),
+    cms=Version('Wagtail', '2.6.2'),
+    module=Version('Y.CMS', '0.0.1')
+)
+```
+
+3. Call the required API method. [More details in our documentation for the YooKassa API](https://yookassa.ru/en/developers/api)
```

### Comparing `yookassa-2.3.5/README.md` & `yookassa-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/setup.py` & `yookassa-2.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,10 +120,12 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9"
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
     ]
 )
```

### Comparing `yookassa-2.3.5/src/yookassa/client.py` & `yookassa-2.3.6/src/yookassa/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                                        json=body)
         return raw_response
 
     def get_session(self):
         session = requests.Session()
         retries = Retry(total=self.max_attempts,
                         backoff_factor=self.timeout / 1000,
-                        method_whitelist=['POST'],
+                        allowed_methods=['POST'],
                         status_forcelist=[202])
         session.mount('https://', HTTPAdapter(max_retries=retries))
         return session
 
     def prepare_request_headers(self, headers):
         request_headers = {'Content-type': 'application/json'}
         if self.auth_token is not None:
```

### Comparing `yookassa-2.3.5/src/yookassa/configuration.py` & `yookassa-2.3.6/src/yookassa/configuration.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/deal.py` & `yookassa-2.3.6/src/yookassa/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/__init__.py` & `yookassa-2.3.6/src/yookassa/domain/common/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/base_object.py` & `yookassa-2.3.6/src/yookassa/domain/common/base_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/confirmation_type.py` & `yookassa-2.3.6/src/yookassa/domain/common/confirmation_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/http_verb.py` & `yookassa-2.3.6/src/yookassa/domain/common/http_verb.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/payment_method_type.py` & `yookassa-2.3.6/src/yookassa/domain/common/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/receipt_type.py` & `yookassa-2.3.6/src/yookassa/domain/common/receipt_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/security_helper.py` & `yookassa-2.3.6/src/yookassa/domain/common/security_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/type_factory.py` & `yookassa-2.3.6/src/yookassa/domain/common/type_factory.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/common/user_agent.py` & `yookassa-2.3.6/src/yookassa/domain/common/user_agent.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/exceptions/__init__.py` & `yookassa-2.3.6/src/yookassa/domain/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/__init__.py` & `yookassa-2.3.6/src/yookassa/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/airline.py` & `yookassa-2.3.6/src/yookassa/domain/models/airline.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/amount.py` & `yookassa-2.3.6/src/yookassa/domain/models/amount.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/authorization_details.py` & `yookassa-2.3.6/src/yookassa/domain/models/authorization_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/cancellation_details.py` & `yookassa-2.3.6/src/yookassa/domain/models/cancellation_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/confirmation_class_map.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_external.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_qr.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_external.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_qr.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py` & `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/deal.py` & `yookassa-2.3.6/src/yookassa/domain/models/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/card_type.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/card_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/payment_data.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/payment_data_class_map.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/credit_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_cash.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/credit_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_cash.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py` & `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/payout_destination_class_map.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/credit_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py` & `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/receipt.py` & `yookassa-2.3.6/src/yookassa/domain/models/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/receipt_customer.py` & `yookassa-2.3.6/src/yookassa/domain/models/receipt_customer.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/receipt_item.py` & `yookassa-2.3.6/src/yookassa/domain/models/receipt_item.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/receipt_item_supplier.py` & `yookassa-2.3.6/src/yookassa/domain/models/receipt_item_supplier.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/recipient.py` & `yookassa-2.3.6/src/yookassa/domain/models/recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/refund_source.py` & `yookassa-2.3.6/src/yookassa/domain/models/refund_source.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/requestor.py` & `yookassa-2.3.6/src/yookassa/domain/models/requestor.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/settlement.py` & `yookassa-2.3.6/src/yookassa/domain/models/settlement.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/models/transfer.py` & `yookassa-2.3.6/src/yookassa/domain/models/transfer.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/notification/webhook_notification.py` & `yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/__init__.py` & `yookassa-2.3.6/src/yookassa/domain/request/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/capture_payment_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/capture_payment_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/capture_payment_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/deal_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/deal_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/deal_request_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/deal_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/payment_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/payment_request_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/payment_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/payout_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/payout_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/payout_request_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/payout_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/receipt_item_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/receipt_item_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/receipt_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/receipt_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/receipt_request_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/receipt_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/refund_request.py` & `yookassa-2.3.6/src/yookassa/domain/request/refund_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/request/refund_request_builder.py` & `yookassa-2.3.6/src/yookassa/domain/request/refund_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/__init__.py` & `yookassa-2.3.6/src/yookassa/domain/response/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/deal_list_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/deal_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/deal_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/deal_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/payment_list_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/payment_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/payment_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/payment_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/payout_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/payout_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/receipt_item_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/receipt_item_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/receipt_list_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/receipt_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/receipt_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/receipt_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/refund_list_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/refund_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/refund_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/refund_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/transfer_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/transfer_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/domain/response/webhook_response.py` & `yookassa-2.3.6/src/yookassa/domain/response/webhook_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/payment.py` & `yookassa-2.3.6/src/yookassa/payment.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/payout.py` & `yookassa-2.3.6/src/yookassa/payout.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/receipt.py` & `yookassa-2.3.6/src/yookassa/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/refund.py` & `yookassa-2.3.6/src/yookassa/refund.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/settings.py` & `yookassa-2.3.6/src/yookassa/settings.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa/webhook.py` & `yookassa-2.3.6/src/yookassa/webhook.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.5/src/yookassa.egg-info/PKG-INFO` & `yookassa-2.3.6/src/yookassa.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-Metadata-Version: 2.1
-Name: yookassa
-Version: 2.3.5
-Summary: YooKassa API SDK Python Library
-Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
-Author: YooMoney
-Author-email: cms@yoomoney.ru
-License: MIT
-Keywords: yoomoney,yookassa,payout,sdk,python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# YooKassa API Python Client Library
-
-[![Build Status](https://travis-ci.org/yoomoney/yookassa-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-sdk-python)
-[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa.svg)](https://pypi.org/project/yookassa/)
-[![Total Downloads](https://img.shields.io/pypi/dm/yookassa.svg)](https://pypi.org/project/yookassa/)
-[![License](https://img.shields.io/pypi/l/yookassa.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python)
-
-[Russian](README.md) | English
-
-This product is used for managing payments under [The YooKassa API](https://yookassa.ru/en/developers/api)
-For usage by those who implemented YooKassa using the API method.
-
-## Requirements
-1. Python 2.7 or Python 3.x
-2. pip
-
-## Installation
-### Under console using pip
-
-1. Install pip.
-2. In the console, run the following command:
-```bash
-pip install --upgrade yookassa
-```
-
-### Under console using easy_install
-1. Install easy_install.
-2. In the console, run the following command:
-```bash
-easy_install --upgrade yookassa
-```
-
-### Manually
-
-1. In the console, run the following command:
-```bash
-wget https://pypi.python.org/packages/5a/be/5eafdfb14aa6f32107e9feb6514ca1ad3fe56f8e5ee59d20693b32f7e79f/yookassa-1.0.0.tar.gz#md5=46595279b5578fd82a199bfd4cd51db2
-tar zxf yookassa-1.0.0.tar.gz
-cd yookassa-1.0.0
-python setup.py install
-```
-
-
-## Commencing work
-
-1. Import module
-```python
-import yookassa
-```
-
-2. Configure a Client
-```python
-from yookassa import Configuration
-
-Configuration.configure('<Account Id>', '<Secret Key>')
-```
-
-or
-
-```python
-from yookassa import Configuration
-
-Configuration.account_id = '<Account Id>'
-Configuration.secret_key = '<Secret Key>'
-```
-
-or via oauth
-
-```python
-from yookassa import Configuration
-
-Configuration.configure_auth_token('<Oauth Token>')
-```
-
-If you agree to participate in the development of the SDK, you can submit data about your framework, cms or module:
-
-```python
-from yookassa import Configuration
-from yookassa.domain.common.user_agent import Version
-
-Configuration.configure('<Account Id>', '<Secret Key>')
-Configuration.configure_user_agent(
-    framework=Version('Django', '2.2.3'),
-    cms=Version('Wagtail', '2.6.2'),
-    module=Version('Y.CMS', '0.0.1')
-)
-```
-
-3. Call the required API method. [More details in our documentation for the YooKassa API](https://yookassa.ru/en/developers/api)
+Metadata-Version: 2.1
+Name: yookassa
+Version: 2.3.6
+Summary: YooKassa API SDK Python Library
+Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
+Author: YooMoney
+Author-email: cms@yoomoney.ru
+License: MIT
+Keywords: yoomoney,yookassa,payout,sdk,python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# YooKassa API Python Client Library
+
+[![Build Status](https://travis-ci.org/yoomoney/yookassa-sdk-python.svg?branch=master)](https://travis-ci.org/yoomoney/yookassa-sdk-python)
+[![Latest Stable Version](https://img.shields.io/pypi/v/yookassa.svg)](https://pypi.org/project/yookassa/)
+[![Total Downloads](https://img.shields.io/pypi/dm/yookassa.svg)](https://pypi.org/project/yookassa/)
+[![License](https://img.shields.io/pypi/l/yookassa.svg)](https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python)
+
+[Russian](README.md) | English
+
+This product is used for managing payments under [The YooKassa API](https://yookassa.ru/en/developers/api)
+For usage by those who implemented YooKassa using the API method.
+
+## Requirements
+1. Python 2.7 or Python 3.x
+2. pip
+
+## Installation
+### Under console using pip
+
+1. Install pip.
+2. In the console, run the following command:
+```bash
+pip install --upgrade yookassa
+```
+
+### Under console using easy_install
+1. Install easy_install.
+2. In the console, run the following command:
+```bash
+easy_install --upgrade yookassa
+```
+
+### Manually
+
+1. In the console, run the following command:
+```bash
+wget https://pypi.python.org/packages/5a/be/5eafdfb14aa6f32107e9feb6514ca1ad3fe56f8e5ee59d20693b32f7e79f/yookassa-1.0.0.tar.gz#md5=46595279b5578fd82a199bfd4cd51db2
+tar zxf yookassa-1.0.0.tar.gz
+cd yookassa-1.0.0
+python setup.py install
+```
+
+
+## Commencing work
+
+1. Import module
+```python
+import yookassa
+```
+
+2. Configure a Client
+```python
+from yookassa import Configuration
+
+Configuration.configure('<Account Id>', '<Secret Key>')
+```
+
+or
+
+```python
+from yookassa import Configuration
+
+Configuration.account_id = '<Account Id>'
+Configuration.secret_key = '<Secret Key>'
+```
+
+or via oauth
+
+```python
+from yookassa import Configuration
+
+Configuration.configure_auth_token('<Oauth Token>')
+```
+
+If you agree to participate in the development of the SDK, you can submit data about your framework, cms or module:
+
+```python
+from yookassa import Configuration
+from yookassa.domain.common.user_agent import Version
+
+Configuration.configure('<Account Id>', '<Secret Key>')
+Configuration.configure_user_agent(
+    framework=Version('Django', '2.2.3'),
+    cms=Version('Wagtail', '2.6.2'),
+    module=Version('Y.CMS', '0.0.1')
+)
+```
+
+3. Call the required API method. [More details in our documentation for the YooKassa API](https://yookassa.ru/en/developers/api)
```

### Comparing `yookassa-2.3.5/src/yookassa.egg-info/SOURCES.txt` & `yookassa-2.3.6/src/yookassa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

