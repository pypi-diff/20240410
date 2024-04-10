# Comparing `tmp/yookassa-3.0.1.tar.gz` & `tmp/yookassa-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yookassa-3.0.1.tar", last modified: Wed Jan 31 14:47:46 2024, max compression
+gzip compressed data, was "yookassa-3.1.0.tar", last modified: Wed Apr 10 14:16:46 2024, max compression
```

## Comparing `yookassa-3.0.1.tar` & `yookassa-3.1.0.tar`

### file list

```diff
@@ -1,240 +1,236 @@
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.138280 yookassa-3.0.1/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1082 2024-01-31 14:47:44.000000 yookassa-3.0.1/LICENSE
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4334 2024-01-31 14:47:46.138143 yookassa-3.0.1/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10636 2024-01-31 14:47:44.000000 yookassa-3.0.1/README.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2024-01-31 14:47:46.139353 yookassa-3.0.1/setup.cfg
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5279 2024-01-31 14:47:44.000000 yookassa-3.0.1/setup.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.788322 yookassa-3.0.1/src/
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.807779 yookassa-3.0.1/src/yookassa/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      602 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5708 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/client.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3339 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/configuration.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1868 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/deal.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.814358 yookassa-3.0.1/src/yookassa/domain/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       88 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/__init__.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.833265 yookassa-3.0.1/src/yookassa/domain/common/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      858 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1562 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/base_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      553 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/confirmation_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      340 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/data_context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      574 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/http_verb.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1625 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/payment_method_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      560 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/receipt_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      381 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/request_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      290 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/response_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      696 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/security_helper.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1097 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/type_factory.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3916 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/common/user_agent.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.850412 yookassa-3.0.1/src/yookassa/domain/exceptions/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      677 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/api_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      125 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/authorize_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/bad_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/forbidden_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      135 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/not_found_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      145 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/response_processing_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/too_many_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      139 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/exceptions/unauthorized_error.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.871685 yookassa-3.0.1/src/yookassa/domain/models/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1486 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/amount.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    15470 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/cancellation_details.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.876324 yookassa-3.0.1/src/yookassa/domain/models/confirmation/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      319 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/confirmation.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2515 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/confirmation_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      316 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/confirmation_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.885262 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      551 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_external.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      922 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1064 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      376 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_request.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.891258 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      822 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_external.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      794 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      864 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1248 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      215 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/currency.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3800 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/deal.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4803 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/me.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.905479 yookassa-3.0.1/src/yookassa/domain/models/payment_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      518 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/card_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/payment_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6809 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/payment_data_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      366 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/payment_data_factory.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/recipient.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.928450 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4518 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/airline.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1903 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1327 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/fraud_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      916 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/merchant_customer_bank_account.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      715 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      655 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2356 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      904 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      970 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      803 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      450 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_sber_loan.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      428 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      543 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.954396 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1280 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/authorization_details.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3572 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      629 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3397 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      921 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      471 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      819 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1329 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      816 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      671 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      460 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_unknown.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      456 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      206 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.956122 yookassa-3.0.1/src/yookassa/domain/models/payout_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      328 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/payout_destination.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2029 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      395 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/payout_destination_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:45.972175 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1403 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/income_receipt.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1370 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.035975 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2190 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1361 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/income_receipt.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1169 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      474 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_unknown.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2419 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/personal_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3930 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.047341 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1453 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/additional_user_props.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2086 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/industry_details.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5824 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/mark_code_info.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2022 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/mark_quantity.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1753 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/operational_details.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1051 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_customer.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6822 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_item.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      691 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_item_supplier.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.059940 yookassa-3.0.1/src/yookassa/domain/models/refund_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      323 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      719 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_data_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      360 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_data_factory.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1257 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_source.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.063379 yookassa-3.0.1/src/yookassa/domain/models/refund_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      665 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/response/refund_data_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      454 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/refund_data/response/refund_data_unknown.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      698 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/sbp_participant_bank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1952 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.065172 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      647 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/confirmation.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      949 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/confirmation_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      370 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/confirmation_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.067160 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      491 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/request/confirmation_redirect.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.069777 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      790 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/response/confirmation_redirect.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.074471 yookassa-3.0.1/src/yookassa/domain/models/settings/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      170 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/settings/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1338 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/settings/fiscalization_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      841 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/settings/fiscalization_provider.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/settlement.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2009 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/models/transfer.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.077094 yookassa-3.0.1/src/yookassa/domain/notification/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      223 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/notification/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3976 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/notification/webhook_notification.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      468 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/notification/webhook_notification_types.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.109596 yookassa-3.0.1/src/yookassa/domain/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1463 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      737 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/capture_payment_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3208 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/capture_payment_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1533 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/deal_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      609 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/deal_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     9967 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/payment_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1982 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/payment_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6279 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/payout_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/payout_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3620 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/personal_data_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      731 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/personal_data_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6534 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/receipt_item_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7930 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/receipt_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1688 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/receipt_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3511 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/refund_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      814 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/refund_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2144 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/self_employed_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      725 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/self_employed_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/request/webhook_request.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.133128 yookassa-3.0.1/src/yookassa/domain/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1229 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      832 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/deal_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/deal_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/payment_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5609 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/payment_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3202 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/payout_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1560 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/personal_data_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4620 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/receipt_item_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/receipt_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4575 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/receipt_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      838 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/refund_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3123 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/refund_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      795 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/sbp_bank_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1912 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/self_employed_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2534 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/transfer_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1062 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/domain/response/webhook_response.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.135081 yookassa-3.0.1/src/yookassa/logging/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/logging/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      594 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/logging/adapter.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1800 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/logging/classes.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1876 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/logging/config.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3661 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/payment.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1611 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/payout.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/personal_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1954 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/receipt.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1914 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/refund.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      479 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/sbp_banks.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/self_employed.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      710 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/settings.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1984 2024-01-31 14:47:44.000000 yookassa-3.0.1/src/yookassa/webhook.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-01-31 14:47:46.136800 yookassa-3.0.1/src/yookassa.egg-info/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4334 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    11732 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/not-zip-safe
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       43 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/requires.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        9 2024-01-31 14:47:45.000000 yookassa-3.0.1/src/yookassa.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.478902 yookassa-3.1.0/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1082 2024-04-10 14:16:45.000000 yookassa-3.1.0/LICENSE
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4334 2024-04-10 14:16:46.478736 yookassa-3.1.0/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    10636 2024-04-10 14:16:45.000000 yookassa-3.1.0/README.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2024-04-10 14:16:46.480610 yookassa-3.1.0/setup.cfg
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5279 2024-04-10 14:16:45.000000 yookassa-3.1.0/setup.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.235246 yookassa-3.1.0/src/
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.247046 yookassa-3.1.0/src/yookassa/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      602 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5708 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/client.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3339 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/configuration.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1868 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/deal.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.249439 yookassa-3.1.0/src/yookassa/domain/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       88 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/__init__.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.254650 yookassa-3.1.0/src/yookassa/domain/common/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      858 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1562 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/base_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      553 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/confirmation_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      340 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/data_context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      574 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/http_verb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1625 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/payment_method_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      560 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/receipt_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      381 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/request_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      290 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/response_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      696 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/security_helper.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1097 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/type_factory.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3916 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/common/user_agent.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.258507 yookassa-3.1.0/src/yookassa/domain/exceptions/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      677 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/api_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      125 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/authorize_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/bad_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/forbidden_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      135 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/not_found_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      145 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/response_processing_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/too_many_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      139 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/exceptions/unauthorized_error.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.265472 yookassa-3.1.0/src/yookassa/domain/models/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1486 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/amount.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    15470 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/cancellation_details.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.269003 yookassa-3.1.0/src/yookassa/domain/models/confirmation/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      319 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/confirmation.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2515 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/confirmation_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      316 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/confirmation_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.276417 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      551 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      922 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1064 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      376 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.296567 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      822 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      794 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      864 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1248 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      215 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/currency.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3800 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/deal.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4803 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/me.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.304100 yookassa-3.1.0/src/yookassa/domain/models/payment_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      518 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/card_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/payment_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6627 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/payment_data_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      366 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/payment_data_factory.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/recipient.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.327314 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4518 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/airline.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1903 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1327 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/fraud_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      916 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/merchant_customer_bank_account.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      655 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2356 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      904 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      970 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      803 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      450 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_sber_loan.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      428 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.388795 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1280 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/authorization_details.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3572 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      629 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3397 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      921 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      471 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      819 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1329 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      816 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      671 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      460 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_unknown.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      456 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      206 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.395005 yookassa-3.1.0/src/yookassa/domain/models/payout_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      328 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/payout_destination.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2029 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      395 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/payout_destination_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.405079 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1403 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/income_receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1370 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.411123 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2190 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1361 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/income_receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1169 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      474 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_unknown.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2419 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/personal_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3930 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.421805 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1453 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/additional_user_props.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2086 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/industry_details.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5824 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/mark_code_info.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2022 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/mark_quantity.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1753 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/operational_details.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1051 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_customer.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6822 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_item.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      691 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_item_supplier.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.427036 yookassa-3.1.0/src/yookassa/domain/models/refund_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      323 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      719 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_data_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      360 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_data_factory.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1257 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_source.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.432289 yookassa-3.1.0/src/yookassa/domain/models/refund_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      665 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/response/refund_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      454 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/refund_data/response/refund_data_unknown.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      698 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/sbp_participant_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1952 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.439587 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      647 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/confirmation.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      949 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/confirmation_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      370 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/confirmation_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.440588 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      491 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/request/confirmation_redirect.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.443123 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      790 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/response/confirmation_redirect.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.445981 yookassa-3.1.0/src/yookassa/domain/models/settings/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      170 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/settings/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1338 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/settings/fiscalization_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      841 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/settings/fiscalization_provider.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/settlement.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2009 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/models/transfer.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.447574 yookassa-3.1.0/src/yookassa/domain/notification/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      223 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/notification/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3976 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/notification/webhook_notification.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      468 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/notification/webhook_notification_types.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.463955 yookassa-3.1.0/src/yookassa/domain/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1463 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      737 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/capture_payment_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3208 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/capture_payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1533 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/deal_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      609 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/deal_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     9967 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1982 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/payment_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6279 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/payout_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/payout_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3620 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/personal_data_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      731 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/personal_data_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6534 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/receipt_item_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     7930 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/receipt_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1688 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/receipt_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3511 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/refund_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      814 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/refund_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2144 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/self_employed_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      725 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/self_employed_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/request/webhook_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.473388 yookassa-3.1.0/src/yookassa/domain/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1229 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      832 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/deal_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/deal_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/payment_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5609 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/payment_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3202 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/payout_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1560 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/personal_data_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4620 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/receipt_item_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/receipt_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4575 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/receipt_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      838 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/refund_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3123 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/refund_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      795 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/sbp_bank_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1912 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/self_employed_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2534 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/transfer_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1062 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/domain/response/webhook_response.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.477145 yookassa-3.1.0/src/yookassa/logging/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/logging/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      594 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/logging/adapter.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1800 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/logging/classes.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1876 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/logging/config.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3661 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/payment.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1611 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/payout.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/personal_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1954 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1914 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/refund.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      479 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/sbp_banks.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1720 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/self_employed.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      710 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/settings.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1984 2024-04-10 14:16:45.000000 yookassa-3.1.0/src/yookassa/webhook.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2024-04-10 14:16:46.477822 yookassa-3.1.0/src/yookassa.egg-info/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4334 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)    11446 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/not-zip-safe
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       43 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/requires.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        9 2024-04-10 14:16:46.000000 yookassa-3.1.0/src/yookassa.egg-info/top_level.txt
```

### Comparing `yookassa-3.0.1/LICENSE` & `yookassa-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/PKG-INFO` & `yookassa-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yookassa
-Version: 3.0.1
+Version: 3.1.0
 Summary: YooKassa API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
 Keywords: yoomoney,yookassa,payout,sdk,python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yookassa-3.0.1/README.md` & `yookassa-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/setup.py` & `yookassa-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/__init__.py` & `yookassa-3.1.0/src/yookassa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from yookassa.sbp_banks import SbpBanks
 from yookassa.self_employed import SelfEmployed
 from yookassa.settings import Settings
 from yookassa.webhook import Webhook
 
 __author__ = "YooMoney"
 __email__ = 'cms@yoomoney.ru'
-__version__ = '3.0.1'
+__version__ = '3.1.0'
```

### Comparing `yookassa-3.0.1/src/yookassa/client.py` & `yookassa-3.1.0/src/yookassa/client.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/configuration.py` & `yookassa-3.1.0/src/yookassa/configuration.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/deal.py` & `yookassa-3.1.0/src/yookassa/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/__init__.py` & `yookassa-3.1.0/src/yookassa/domain/common/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/base_object.py` & `yookassa-3.1.0/src/yookassa/domain/common/base_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/confirmation_type.py` & `yookassa-3.1.0/src/yookassa/domain/common/confirmation_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/http_verb.py` & `yookassa-3.1.0/src/yookassa/domain/common/http_verb.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/payment_method_type.py` & `yookassa-3.1.0/src/yookassa/domain/common/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/receipt_type.py` & `yookassa-3.1.0/src/yookassa/domain/common/receipt_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/security_helper.py` & `yookassa-3.1.0/src/yookassa/domain/common/security_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/type_factory.py` & `yookassa-3.1.0/src/yookassa/domain/common/type_factory.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/common/user_agent.py` & `yookassa-3.1.0/src/yookassa/domain/common/user_agent.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/exceptions/__init__.py` & `yookassa-3.1.0/src/yookassa/domain/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/__init__.py` & `yookassa-3.1.0/src/yookassa/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/amount.py` & `yookassa-3.1.0/src/yookassa/domain/models/amount.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/cancellation_details.py` & `yookassa-3.1.0/src/yookassa/domain/models/cancellation_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/confirmation_class_map.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/confirmation_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_external.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_qr.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_external.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_qr.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py` & `yookassa-3.1.0/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/deal.py` & `yookassa-3.1.0/src/yookassa/domain/models/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/me.py` & `yookassa-3.1.0/src/yookassa/domain/models/me.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/card_type.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/card_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/payment_data.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/payment_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/payment_data_class_map.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/payment_data_class_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     PaymentDataCash as RequestPaymentDataCash
 from yookassa.domain.models.payment_data.request.payment_data_google_pay import \
     PaymentDataGooglePay as RequestPaymentDataGooglePay
 from yookassa.domain.models.payment_data.request.payment_data_installments import \
     PaymentDataInstallments as RequestPaymentDataInstallments
 from yookassa.domain.models.payment_data.request.payment_data_mobile_balance import \
     PaymentDataMobileBalance as RequestPaymentDataMobileBalance
-from yookassa.domain.models.payment_data.request.payment_data_qiwi import \
-    PaymentDataQiwi as RequestPaymentDataQiwi
 from yookassa.domain.models.payment_data.request.payment_data_sberbank import \
     PaymentDataSberbank as RequestPaymentDataSberbank
 from yookassa.domain.models.payment_data.request.payment_data_tinkoff_bank import \
     PaymentDataTinkoffBank as RequestPaymentDataTinkoffBank
 from yookassa.domain.models.payment_data.request.payment_data_yoomoney_wallet import \
     PaymentDataYooMoneyWallet as RequestPaymentDataYooMoneyWallet
 from yookassa.domain.models.payment_data.request.payment_data_sbp import \
@@ -73,15 +71,14 @@
     def request(self):
         return {
             PaymentMethodType.BANK_CARD: RequestPaymentDataBankCard,
             PaymentMethodType.CASH: RequestPaymentDataCash,
             PaymentMethodType.MOBILE_BALANCE: RequestPaymentDataMobileBalance,
             PaymentMethodType.SBERBANK: RequestPaymentDataSberbank,
             PaymentMethodType.YOO_MONEY: RequestPaymentDataYooMoneyWallet,
-            PaymentMethodType.QIWI: RequestPaymentDataQiwi,
             PaymentMethodType.APPLEPAY: RequestPaymentDataApplepay,
             PaymentMethodType.GOOGLE_PAY: RequestPaymentDataGooglePay,
             PaymentMethodType.INSTALMENTS: RequestPaymentDataInstallments,
             PaymentMethodType.B2B_SBERBANK: RequestPaymentDataB2bSberbank,
             PaymentMethodType.TINKOFF_BANK: RequestPaymentDataTinkoffBank,
             PaymentMethodType.SBP: RequestPaymentDataSbp,
             PaymentMethodType.SBER_LOAN: RequestPaymentDataSberLoan,
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/recipient.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/airline.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/airline.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/credit_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/fraud_data.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/fraud_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/merchant_customer_bank_account.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/merchant_customer_bank_account.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
-from deprecated import deprecated
 from yookassa.domain.common.payment_method_type import PaymentMethodType
-from yookassa.domain.models.payment_data.payment_data import PaymentData
+from yookassa.domain.models.payment_data.payment_data import ResponsePaymentData
 
 
-@deprecated("This class will be removed in one of future versions")
-class PaymentDataAlfabank(PaymentData):
+class PaymentDataAlfabank(ResponsePaymentData):
     __login = None
 
     def __init__(self, *args, **kwargs):
         super(PaymentDataAlfabank, self).__init__(*args, **kwargs)
         if self.type is None or self.type is not PaymentMethodType.ALFABANK:
             self.type = PaymentMethodType.ALFABANK
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_cash.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import re
 
 from yookassa.domain.common.payment_method_type import PaymentMethodType
-from yookassa.domain.models.payment_data.payment_data import PaymentData
+from yookassa.domain.models.payment_data.payment_data import ResponsePaymentData
 
 
-class PaymentDataQiwi(PaymentData):
+class PaymentDataQiwi(ResponsePaymentData):
     __phone = None
 
     def __init__(self, *args, **kwargs):
         super(PaymentDataQiwi, self).__init__(*args, **kwargs)
         if self.type is None or self.type is not PaymentMethodType.QIWI:
             self.type = PaymentMethodType.QIWI
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py` & `yookassa-3.1.0/src/yookassa/domain/models/refund_data/response/refund_data_sbp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # -*- coding: utf-8 -*-
-from deprecated import deprecated
-
 from yookassa.domain.common.payment_method_type import PaymentMethodType
-from yookassa.domain.models.payment_data.payment_data import PaymentData
+from yookassa.domain.models.refund_data.refund_data import ResponseRefundData
+
+
+class RefundDataSbp(ResponseRefundData):
 
+    __sbp_operation_id = None
 
-@deprecated("This class will be removed in one of future versions")
-class PaymentDataWechat(PaymentData):
     def __init__(self, *args, **kwargs):
-        super(PaymentDataWechat, self).__init__(*args, **kwargs)
-        if self.type is None or self.type is not PaymentMethodType.WECHAT:
-            self.type = PaymentMethodType.WECHAT
+        super(RefundDataSbp, self).__init__(*args, **kwargs)
+        if self.type is None or self.type is not PaymentMethodType.SBP:
+            self.type = PaymentMethodType.SBP
+
+    @property
+    def sbp_operation_id(self):
+        return self.__sbp_operation_id
+
+    @sbp_operation_id.setter
+    def sbp_operation_id(self, value):
+        self.__sbp_operation_id = value
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/authorization_details.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/authorization_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/credit_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # -*- coding: utf-8 -*-
+import re
+
 from yookassa.domain.common.payment_method_type import PaymentMethodType
 from yookassa.domain.models.payment_data.payment_data import ResponsePaymentData
 
 
-class PaymentDataAlfabank(ResponsePaymentData):
-    __login = None
+class PaymentDataMobileBalance(ResponsePaymentData):
+    __phone = None
 
     def __init__(self, *args, **kwargs):
-        super(PaymentDataAlfabank, self).__init__(*args, **kwargs)
-        if self.type is None or self.type is not PaymentMethodType.ALFABANK:
-            self.type = PaymentMethodType.ALFABANK
+        super(PaymentDataMobileBalance, self).__init__(*args, **kwargs)
+        if self.type is None or self.type is not PaymentMethodType.MOBILE_BALANCE:
+            self.type = PaymentMethodType.MOBILE_BALANCE
 
     @property
-    def login(self):
-        return self.__login
+    def phone(self):
+        return self.__phone
 
-    @login.setter
-    def login(self, value):
-        self.__login = str(value)
+    @phone.setter
+    def phone(self, value):
+        cast_value = str(value)
+        if re.match('^[0-9]{4,15}$', cast_value):
+            self.__phone = cast_value
+        else:
+            raise ValueError('Invalid phone value type')
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_cash.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import re
 
 from yookassa.domain.common.payment_method_type import PaymentMethodType
-from yookassa.domain.models.payment_data.payment_data import ResponsePaymentData
+from yookassa.domain.models.payment_data.response.payment_data_bank_card import PaymentDataBankCard
 
 
-class PaymentDataMobileBalance(ResponsePaymentData):
+class PaymentDataSberbank(PaymentDataBankCard):
     __phone = None
 
     def __init__(self, *args, **kwargs):
-        super(PaymentDataMobileBalance, self).__init__(*args, **kwargs)
-        if self.type is None or self.type is not PaymentMethodType.MOBILE_BALANCE:
-            self.type = PaymentMethodType.MOBILE_BALANCE
+        super(PaymentDataSberbank, self).__init__(*args, **kwargs)
+        if self.type is None or self.type is not PaymentMethodType.SBERBANK:
+            self.type = PaymentMethodType.SBERBANK
 
     @property
     def phone(self):
         return self.__phone
 
     @phone.setter
     def phone(self, value):
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # -*- coding: utf-8 -*-
-import re
-
 from yookassa.domain.common.payment_method_type import PaymentMethodType
 from yookassa.domain.models.payment_data.payment_data import ResponsePaymentData
 
 
-class PaymentDataQiwi(ResponsePaymentData):
-    __phone = None
+class PaymentDataSbp(ResponsePaymentData):
+
+    __sbp_operation_id = None
 
     def __init__(self, *args, **kwargs):
-        super(PaymentDataQiwi, self).__init__(*args, **kwargs)
-        if self.type is None or self.type is not PaymentMethodType.QIWI:
-            self.type = PaymentMethodType.QIWI
+        super(PaymentDataSbp, self).__init__(*args, **kwargs)
+        if self.type is None or self.type is not PaymentMethodType.SBP:
+            self.type = PaymentMethodType.SBP
 
     @property
-    def phone(self):
-        return self.__phone
+    def sbp_operation_id(self):
+        return self.__sbp_operation_id
 
-    @phone.setter
-    def phone(self, value):
-        cast_value = str(value)
-        if re.match('^[0-9]{4,15}$', cast_value):
-            self.__phone = cast_value
-        else:
-            raise ValueError('Invalid phone value type')
+    @sbp_operation_id.setter
+    def sbp_operation_id(self, value):
+        self.__sbp_operation_id = value
```

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py` & `yookassa-3.1.0/src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/payout_destination_class_map.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/payout_destination_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/income_receipt.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/income_receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_sbp.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_sbp.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/credit_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/income_receipt.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/income_receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_sbp.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_sbp.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py` & `yookassa-3.1.0/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/personal_data.py` & `yookassa-3.1.0/src/yookassa/domain/models/personal_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/additional_user_props.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/additional_user_props.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/industry_details.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/industry_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/mark_code_info.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/mark_code_info.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/mark_quantity.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/mark_quantity.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/operational_details.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/operational_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_customer.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_customer.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_item.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_item.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/receipt_data/receipt_item_supplier.py` & `yookassa-3.1.0/src/yookassa/domain/models/receipt_data/receipt_item_supplier.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_data_class_map.py` & `yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_data_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/refund_data/refund_source.py` & `yookassa-3.1.0/src/yookassa/domain/models/refund_data/refund_source.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/sbp_participant_bank.py` & `yookassa-3.1.0/src/yookassa/domain/models/sbp_participant_bank.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/self_employed.py` & `yookassa-3.1.0/src/yookassa/domain/models/self_employed.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/confirmation.py` & `yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/confirmation.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/confirmation_class_map.py` & `yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/confirmation_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/self_employed_data/response/confirmation_redirect.py` & `yookassa-3.1.0/src/yookassa/domain/models/self_employed_data/response/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/settings/fiscalization_data.py` & `yookassa-3.1.0/src/yookassa/domain/models/settings/fiscalization_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/settings/fiscalization_provider.py` & `yookassa-3.1.0/src/yookassa/domain/models/settings/fiscalization_provider.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/settlement.py` & `yookassa-3.1.0/src/yookassa/domain/models/settlement.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/models/transfer.py` & `yookassa-3.1.0/src/yookassa/domain/models/transfer.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/notification/webhook_notification.py` & `yookassa-3.1.0/src/yookassa/domain/notification/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/__init__.py` & `yookassa-3.1.0/src/yookassa/domain/request/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/capture_payment_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/capture_payment_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/capture_payment_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/deal_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/deal_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/deal_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/deal_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/payment_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/payment_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/payment_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/payout_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/payout_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/payout_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/payout_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/personal_data_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/personal_data_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/personal_data_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/personal_data_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/receipt_item_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/receipt_item_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/receipt_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/receipt_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/receipt_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/receipt_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/refund_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/refund_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/refund_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/refund_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/self_employed_request.py` & `yookassa-3.1.0/src/yookassa/domain/request/self_employed_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/request/self_employed_request_builder.py` & `yookassa-3.1.0/src/yookassa/domain/request/self_employed_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/__init__.py` & `yookassa-3.1.0/src/yookassa/domain/response/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/deal_list_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/deal_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/deal_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/deal_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/payment_list_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/payment_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/payment_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/payment_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/payout_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/payout_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/personal_data_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/personal_data_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/receipt_item_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/receipt_item_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/receipt_list_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/receipt_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/receipt_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/receipt_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/refund_list_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/refund_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/refund_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/refund_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/sbp_bank_list_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/sbp_bank_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/self_employed_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/self_employed_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/transfer_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/transfer_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/domain/response/webhook_response.py` & `yookassa-3.1.0/src/yookassa/domain/response/webhook_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/logging/adapter.py` & `yookassa-3.1.0/src/yookassa/logging/adapter.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/logging/classes.py` & `yookassa-3.1.0/src/yookassa/logging/classes.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/logging/config.py` & `yookassa-3.1.0/src/yookassa/logging/config.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/payment.py` & `yookassa-3.1.0/src/yookassa/payment.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/payout.py` & `yookassa-3.1.0/src/yookassa/payout.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/personal_data.py` & `yookassa-3.1.0/src/yookassa/personal_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/receipt.py` & `yookassa-3.1.0/src/yookassa/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/refund.py` & `yookassa-3.1.0/src/yookassa/refund.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/self_employed.py` & `yookassa-3.1.0/src/yookassa/self_employed.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/settings.py` & `yookassa-3.1.0/src/yookassa/settings.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa/webhook.py` & `yookassa-3.1.0/src/yookassa/webhook.py`

 * *Files identical despite different names*

### Comparing `yookassa-3.0.1/src/yookassa.egg-info/PKG-INFO` & `yookassa-3.1.0/src/yookassa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yookassa
-Version: 3.0.1
+Version: 3.1.0
 Summary: YooKassa API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
 Keywords: yoomoney,yookassa,payout,sdk,python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yookassa-3.0.1/src/yookassa.egg-info/SOURCES.txt` & `yookassa-3.1.0/src/yookassa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,25 @@
 src/yookassa/domain/models/payment_data/payment_data_factory.py
 src/yookassa/domain/models/payment_data/recipient.py
 src/yookassa/domain/models/payment_data/request/__init__.py
 src/yookassa/domain/models/payment_data/request/airline.py
 src/yookassa/domain/models/payment_data/request/credit_card.py
 src/yookassa/domain/models/payment_data/request/fraud_data.py
 src/yookassa/domain/models/payment_data/request/merchant_customer_bank_account.py
-src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
 src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
 src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
 src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
 src/yookassa/domain/models/payment_data/request/payment_data_cash.py
 src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
 src/yookassa/domain/models/payment_data/request/payment_data_installments.py
 src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
-src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
 src/yookassa/domain/models/payment_data/request/payment_data_sber_loan.py
 src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
 src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
 src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
-src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
-src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
 src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
 src/yookassa/domain/models/payment_data/response/__init__.py
 src/yookassa/domain/models/payment_data/response/authorization_details.py
 src/yookassa/domain/models/payment_data/response/credit_card.py
 src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
 src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
 src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
```

