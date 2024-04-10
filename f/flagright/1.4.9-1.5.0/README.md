# Comparing `tmp/flagright-1.4.9.tar.gz` & `tmp/flagright-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagright-1.4.9.tar", max compression
+gzip compressed data, was "flagright-1.5.0.tar", max compression
```

## Comparing `flagright-1.4.9.tar` & `flagright-1.5.0.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0      829 2024-03-07 13:19:29.549217 flagright-1.4.9/README.md
--rw-r--r--   0        0        0      404 2024-03-07 13:19:29.549217 flagright-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     9601 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/__init__.py
--rw-r--r--   0        0        0     3441 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/client.py
--rw-r--r--   0        0        0      519 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/api_error.py
--rw-r--r--   0        0        0     1078 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      168 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/environment.py
--rw-r--r--   0        0        0      358 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/errors/forbidden_error.py
--rw-r--r--   0        0        0      253 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      250 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/py.typed
--rw-r--r--   0        0        0      647 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_user_events/__init__.py
--rw-r--r--   0        0        0    64479 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_user_events/client.py
--rw-r--r--   0        0        0      155 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_users/__init__.py
--rw-r--r--   0        0        0    38422 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_users/client.py
--rw-r--r--   0        0        0      180 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/business_users/types/business_users_create_response.py
--rw-r--r--   0        0        0       65 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_user_events/__init__.py
--rw-r--r--   0        0        0    21529 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_user_events/client.py
--rw-r--r--   0        0        0      155 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_users/__init__.py
--rw-r--r--   0        0        0    20856 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_users/client.py
--rw-r--r--   0        0        0      180 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
--rw-r--r--   0        0        0       65 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transaction_events/__init__.py
--rw-r--r--   0        0        0    16375 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transaction_events/client.py
--rw-r--r--   0        0        0      153 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transactions/__init__.py
--rw-r--r--   0        0        0    19718 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transactions/client.py
--rw-r--r--   0        0        0      176 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transactions/types/__init__.py
--rw-r--r--   0        0        0      927 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/resources/transactions/types/transactions_verify_response.py
--rw-r--r--   0        0        0    12150 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/__init__.py
--rw-r--r--   0        0        0     1947 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/ach_details.py
--rw-r--r--   0        0        0      143 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/ach_payment_method.py
--rw-r--r--   0        0        0     1167 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/acquisition_channel.py
--rw-r--r--   0        0        0     1637 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/address.py
--rw-r--r--   0        0        0     1667 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/alert_closed_details.py
--rw-r--r--   0        0        0     1160 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/amount.py
--rw-r--r--   0        0        0      448 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/boolean_string.py
--rw-r--r--   0        0        0     3230 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business.py
--rw-r--r--   0        0        0     1296 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_base.py
--rw-r--r--   0        0        0     1080 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_entity_link.py
--rw-r--r--   0        0        0     3090 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_optional.py
--rw-r--r--   0        0        0     3143 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_optional_saved_payment_details_item.py
--rw-r--r--   0        0        0     1137 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_response.py
--rw-r--r--   0        0        0     1282 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_user_segment.py
--rw-r--r--   0        0        0     1546 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_users_response.py
--rw-r--r--   0        0        0     1307 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/business_with_rules_result.py
--rw-r--r--   0        0        0     1247 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_brand.py
--rw-r--r--   0        0        0     3079 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_details.py
--rw-r--r--   0        0        0      920 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_expiry.py
--rw-r--r--   0        0        0      661 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_funding.py
--rw-r--r--   0        0        0     1200 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_merchant_details.py
--rw-r--r--   0        0        0      145 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_payment_method.py
--rw-r--r--   0        0        0      497 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/card_type.py
--rw-r--r--   0        0        0     1357 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/case_closed_details.py
--rw-r--r--   0        0        0     2130 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/case_management_event.py
--rw-r--r--   0        0        0      558 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/case_management_event_case_status.py
--rw-r--r--   0        0        0     1174 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/case_management_event_case_status_reason.py
--rw-r--r--   0        0        0     1169 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/case_opened_details.py
--rw-r--r--   0        0        0     1133 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/check_delivery_status.py
--rw-r--r--   0        0        0     1608 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/check_details.py
--rw-r--r--   0        0        0      147 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/check_payment_method.py
--rw-r--r--   0        0        0     1420 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/company_financial_details.py
--rw-r--r--   0        0        0     2026 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/company_general_details.py
--rw-r--r--   0        0        0     1878 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/company_registration_details.py
--rw-r--r--   0        0        0     1272 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/consumer_name.py
--rw-r--r--   0        0        0      511 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/consumer_user_segment.py
--rw-r--r--   0        0        0     1546 2024-03-07 13:19:29.549217 flagright-1.4.9/src/flagright/types/consumer_users_response.py
--rw-r--r--   0        0        0     1731 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/contact_details.py
--rw-r--r--   0        0        0    29271 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/country_code.py
--rw-r--r--   0        0        0    56920 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/currency_code.py
--rw-r--r--   0        0        0     1066 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/date.py
--rw-r--r--   0        0        0     2967 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/device_data.py
--rw-r--r--   0        0        0       79 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/email_id.py
--rw-r--r--   0        0        0     1685 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/employment_status.py
--rw-r--r--   0        0        0     1771 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/executed_rules_result.py
--rw-r--r--   0        0        0     1426 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/failed_rules_result.py
--rw-r--r--   0        0        0     1049 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/false_positive_details.py
--rw-r--r--   0        0        0      584 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/gender.py
--rw-r--r--   0        0        0      175 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/general_bank_account_payment_method.py
--rw-r--r--   0        0        0     2260 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/generic_bank_account_details.py
--rw-r--r--   0        0        0     1709 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/hit_rules_details.py
--rw-r--r--   0        0        0     2249 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/iban_details.py
--rw-r--r--   0        0        0      145 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/iban_payment_method.py
--rw-r--r--   0        0        0     1396 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/kyc_status.py
--rw-r--r--   0        0        0     1078 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/kyc_status_details.py
--rw-r--r--   0        0        0     2153 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/legal_document.py
--rw-r--r--   0        0        0     1939 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/legal_entity.py
--rw-r--r--   0        0        0     1115 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_data.py
--rw-r--r--   0        0        0     1162 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_existed.py
--rw-r--r--   0        0        0     1275 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_header.py
--rw-r--r--   0        0        0      958 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_item.py
--rw-r--r--   0        0        0      127 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_key_metadata.py
--rw-r--r--   0        0        0     1084 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_metadata.py
--rw-r--r--   0        0        0     2152 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_subtype.py
--rw-r--r--   0        0        0      697 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/list_type.py
--rw-r--r--   0        0        0     1006 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/mcc_details.py
--rw-r--r--   0        0        0     1573 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/mpesa_details.py
--rw-r--r--   0        0        0      147 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/mpesa_payment_method.py
--rw-r--r--   0        0        0     1312 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/mpesa_transaction_type.py
--rw-r--r--   0        0        0     1465 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/payment_method.py
--rw-r--r--   0        0        0     1029 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/pep_status.py
--rw-r--r--   0        0        0     1781 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/person.py
--rw-r--r--   0        0        0      884 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/risk_level.py
--rw-r--r--   0        0        0      921 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_action.py
--rw-r--r--   0        0        0     1121 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_failure_exception.py
--rw-r--r--   0        0        0      497 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_hit_direction.py
--rw-r--r--   0        0        0     1462 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_hit_meta.py
--rw-r--r--   0        0        0     2235 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_labels.py
--rw-r--r--   0        0        0      735 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rule_nature.py
--rw-r--r--   0        0        0     1293 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/rules_results.py
--rw-r--r--   0        0        0     1172 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/sanctions_details.py
--rw-r--r--   0        0        0     1694 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/sanctions_details_entity_type.py
--rw-r--r--   0        0        0     2433 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/source_of_funds.py
--rw-r--r--   0        0        0     2071 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/swift_details.py
--rw-r--r--   0        0        0      147 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/swift_payment_method.py
--rw-r--r--   0        0        0     1156 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/tag.py
--rw-r--r--   0        0        0      907 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction.py
--rw-r--r--   0        0        0     1291 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_amount_details.py
--rw-r--r--   0        0        0     1028 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_amount_limit.py
--rw-r--r--   0        0        0     1616 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_base.py
--rw-r--r--   0        0        0      996 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_count_limit.py
--rw-r--r--   0        0        0     1923 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_event.py
--rw-r--r--   0        0        0     1073 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_event_monitoring_result.py
--rw-r--r--   0        0        0     1408 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_limit.py
--rw-r--r--   0        0        0     1947 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_limits.py
--rw-r--r--   0        0        0     1686 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_limits_payment_method_limits.py
--rw-r--r--   0        0        0     1332 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_monitoring_result.py
--rw-r--r--   0        0        0     1122 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_risk_scoring_result.py
--rw-r--r--   0        0        0     1669 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_state.py
--rw-r--r--   0        0        0     1066 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_status_details.py
--rw-r--r--   0        0        0     1140 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_type.py
--rw-r--r--   0        0        0     3339 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_updatable.py
--rw-r--r--   0        0        0     3257 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_updatable_destination_payment_details.py
--rw-r--r--   0        0        0     3162 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_updatable_origin_payment_details.py
--rw-r--r--   0        0        0     1534 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/transaction_with_rules_result.py
--rw-r--r--   0        0        0     1635 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/upi_details.py
--rw-r--r--   0        0        0      143 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/upi_payment_method.py
--rw-r--r--   0        0        0      899 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user.py
--rw-r--r--   0        0        0     1141 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_base.py
--rw-r--r--   0        0        0     1476 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_details.py
--rw-r--r--   0        0        0     3056 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_optional.py
--rw-r--r--   0        0        0      540 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_registration_status.py
--rw-r--r--   0        0        0     1121 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_response.py
--rw-r--r--   0        0        0     1279 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_risk_score_details.py
--rw-r--r--   0        0        0     1232 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_state.py
--rw-r--r--   0        0        0     1060 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_state_details.py
--rw-r--r--   0        0        0     1296 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/user_with_rules_result.py
--rw-r--r--   0        0        0     2124 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/wallet_details.py
--rw-r--r--   0        0        0      149 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/wallet_payment_method.py
--rw-r--r--   0        0        0      987 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/webhook_event.py
--rw-r--r--   0        0        0     1387 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/webhook_event_base.py
--rw-r--r--   0        0        0      562 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/webhook_event_base_triggered_by.py
--rw-r--r--   0        0        0      578 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/webhook_event_data.py
--rw-r--r--   0        0        0     1201 2024-03-07 13:19:29.553217 flagright-1.4.9/src/flagright/types/webhook_event_type.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0      829 2024-04-10 14:12:44.593927 flagright-1.5.0/README.md
+-rw-r--r--   0        0        0      404 2024-04-10 14:12:44.593927 flagright-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9613 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/client.py
+-rw-r--r--   0        0        0      519 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/api_error.py
+-rw-r--r--   0        0        0     1078 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      168 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/environment.py
+-rw-r--r--   0        0        0      358 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/errors/forbidden_error.py
+-rw-r--r--   0        0        0      253 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      250 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/py.typed
+-rw-r--r--   0        0        0      647 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_user_events/__init__.py
+-rw-r--r--   0        0        0    70170 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_users/__init__.py
+-rw-r--r--   0        0        0    38466 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/business_users/types/business_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-10 14:12:44.593927 flagright-1.5.0/src/flagright/resources/consumer_user_events/__init__.py
+-rw-r--r--   0        0        0    23686 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/consumer_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/consumer_users/__init__.py
+-rw-r--r--   0        0        0    20900 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/consumer_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/consumer_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transaction_events/__init__.py
+-rw-r--r--   0        0        0    16377 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transaction_events/client.py
+-rw-r--r--   0        0        0      153 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    19718 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transactions/client.py
+-rw-r--r--   0        0        0      176 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transactions/types/__init__.py
+-rw-r--r--   0        0        0      927 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/resources/transactions/types/transactions_verify_response.py
+-rw-r--r--   0        0        0    12170 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/ach_details.py
+-rw-r--r--   0        0        0      143 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/ach_payment_method.py
+-rw-r--r--   0        0        0     1167 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/acquisition_channel.py
+-rw-r--r--   0        0        0     1637 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/address.py
+-rw-r--r--   0        0        0     1667 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/alert_closed_details.py
+-rw-r--r--   0        0        0     1160 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/amount.py
+-rw-r--r--   0        0        0      448 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/boolean_string.py
+-rw-r--r--   0        0        0     3230 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business.py
+-rw-r--r--   0        0        0     1296 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_base.py
+-rw-r--r--   0        0        0     1080 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_entity_link.py
+-rw-r--r--   0        0        0     3090 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_optional.py
+-rw-r--r--   0        0        0     3143 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_optional_saved_payment_details_item.py
+-rw-r--r--   0        0        0     1658 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_user_event.py
+-rw-r--r--   0        0        0     1282 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_users_response.py
+-rw-r--r--   0        0        0     1470 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/business_with_rules_result.py
+-rw-r--r--   0        0        0     1247 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_brand.py
+-rw-r--r--   0        0        0     3079 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_details.py
+-rw-r--r--   0        0        0      920 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_expiry.py
+-rw-r--r--   0        0        0      661 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_funding.py
+-rw-r--r--   0        0        0     1200 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_merchant_details.py
+-rw-r--r--   0        0        0      145 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_payment_method.py
+-rw-r--r--   0        0        0      497 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/card_type.py
+-rw-r--r--   0        0        0     1357 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/case_closed_details.py
+-rw-r--r--   0        0        0     2130 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/case_management_event.py
+-rw-r--r--   0        0        0      558 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/case_management_event_case_status.py
+-rw-r--r--   0        0        0     1174 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/case_management_event_case_status_reason.py
+-rw-r--r--   0        0        0     1169 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/case_opened_details.py
+-rw-r--r--   0        0        0     1133 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/check_delivery_status.py
+-rw-r--r--   0        0        0     1608 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/check_details.py
+-rw-r--r--   0        0        0      147 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/check_payment_method.py
+-rw-r--r--   0        0        0     1420 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/company_financial_details.py
+-rw-r--r--   0        0        0     2026 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/company_general_details.py
+-rw-r--r--   0        0        0     1878 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/company_registration_details.py
+-rw-r--r--   0        0        0     1272 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/consumer_name.py
+-rw-r--r--   0        0        0     1646 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/consumer_user_event.py
+-rw-r--r--   0        0        0      511 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/consumer_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/consumer_users_response.py
+-rw-r--r--   0        0        0     1731 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/contact_details.py
+-rw-r--r--   0        0        0    29271 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/country_code.py
+-rw-r--r--   0        0        0    56920 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/currency_code.py
+-rw-r--r--   0        0        0     1066 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/date.py
+-rw-r--r--   0        0        0     2967 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/device_data.py
+-rw-r--r--   0        0        0       79 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/email_id.py
+-rw-r--r--   0        0        0     1685 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/employment_status.py
+-rw-r--r--   0        0        0     1771 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/executed_rules_result.py
+-rw-r--r--   0        0        0     1426 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/failed_rules_result.py
+-rw-r--r--   0        0        0     1049 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/false_positive_details.py
+-rw-r--r--   0        0        0      584 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/gender.py
+-rw-r--r--   0        0        0      175 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/general_bank_account_payment_method.py
+-rw-r--r--   0        0        0     2340 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/generic_bank_account_details.py
+-rw-r--r--   0        0        0     1709 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/hit_rules_details.py
+-rw-r--r--   0        0        0     2249 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/iban_details.py
+-rw-r--r--   0        0        0      145 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/iban_payment_method.py
+-rw-r--r--   0        0        0     1575 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/kyc_status.py
+-rw-r--r--   0        0        0     1078 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/kyc_status_details.py
+-rw-r--r--   0        0        0     2153 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/legal_document.py
+-rw-r--r--   0        0        0     1939 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/legal_entity.py
+-rw-r--r--   0        0        0     1115 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_data.py
+-rw-r--r--   0        0        0     1162 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_existed.py
+-rw-r--r--   0        0        0     1275 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_header.py
+-rw-r--r--   0        0        0      958 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_item.py
+-rw-r--r--   0        0        0      127 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_key_metadata.py
+-rw-r--r--   0        0        0     1084 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_metadata.py
+-rw-r--r--   0        0        0     2152 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_subtype.py
+-rw-r--r--   0        0        0      697 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/list_type.py
+-rw-r--r--   0        0        0     1006 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/mcc_details.py
+-rw-r--r--   0        0        0     1573 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/mpesa_details.py
+-rw-r--r--   0        0        0      147 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/mpesa_payment_method.py
+-rw-r--r--   0        0        0     1312 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/mpesa_transaction_type.py
+-rw-r--r--   0        0        0     1465 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/payment_method.py
+-rw-r--r--   0        0        0     1029 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/pep_status.py
+-rw-r--r--   0        0        0     1781 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/person.py
+-rw-r--r--   0        0        0      884 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/risk_level.py
+-rw-r--r--   0        0        0      921 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_action.py
+-rw-r--r--   0        0        0     1121 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_failure_exception.py
+-rw-r--r--   0        0        0      497 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_hit_direction.py
+-rw-r--r--   0        0        0     1562 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_hit_meta.py
+-rw-r--r--   0        0        0     2235 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_labels.py
+-rw-r--r--   0        0        0      735 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rule_nature.py
+-rw-r--r--   0        0        0     1293 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/rules_results.py
+-rw-r--r--   0        0        0     1172 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/sanctions_details.py
+-rw-r--r--   0        0        0     1694 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/sanctions_details_entity_type.py
+-rw-r--r--   0        0        0     2433 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/source_of_funds.py
+-rw-r--r--   0        0        0     2071 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/swift_details.py
+-rw-r--r--   0        0        0      147 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/swift_payment_method.py
+-rw-r--r--   0        0        0     1156 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/tag.py
+-rw-r--r--   0        0        0      907 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction.py
+-rw-r--r--   0        0        0     1291 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_amount_details.py
+-rw-r--r--   0        0        0     1028 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_amount_limit.py
+-rw-r--r--   0        0        0     1616 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_base.py
+-rw-r--r--   0        0        0      996 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_count_limit.py
+-rw-r--r--   0        0        0     1923 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_event.py
+-rw-r--r--   0        0        0     1260 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_event_monitoring_result.py
+-rw-r--r--   0        0        0     1408 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_limit.py
+-rw-r--r--   0        0        0     1947 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_limits.py
+-rw-r--r--   0        0        0     1686 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_limits_payment_method_limits.py
+-rw-r--r--   0        0        0     1332 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_monitoring_result.py
+-rw-r--r--   0        0        0     1122 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_risk_scoring_result.py
+-rw-r--r--   0        0        0     1669 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_state.py
+-rw-r--r--   0        0        0     1100 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_status_details.py
+-rw-r--r--   0        0        0     1140 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_type.py
+-rw-r--r--   0        0        0     3339 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_updatable.py
+-rw-r--r--   0        0        0     3257 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_updatable_destination_payment_details.py
+-rw-r--r--   0        0        0     3162 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_updatable_origin_payment_details.py
+-rw-r--r--   0        0        0     1534 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/transaction_with_rules_result.py
+-rw-r--r--   0        0        0     1635 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/upi_details.py
+-rw-r--r--   0        0        0      143 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/upi_payment_method.py
+-rw-r--r--   0        0        0      899 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user.py
+-rw-r--r--   0        0        0     1141 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_base.py
+-rw-r--r--   0        0        0     1476 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_details.py
+-rw-r--r--   0        0        0     3056 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_optional.py
+-rw-r--r--   0        0        0      540 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_registration_status.py
+-rw-r--r--   0        0        0     1279 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_risk_score_details.py
+-rw-r--r--   0        0        0     1232 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_state.py
+-rw-r--r--   0        0        0     1060 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_state_details.py
+-rw-r--r--   0        0        0     1459 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/user_with_rules_result.py
+-rw-r--r--   0        0        0     2124 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/wallet_details.py
+-rw-r--r--   0        0        0      149 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/wallet_payment_method.py
+-rw-r--r--   0        0        0      987 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/webhook_event.py
+-rw-r--r--   0        0        0     1387 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/webhook_event_base.py
+-rw-r--r--   0        0        0      562 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/webhook_event_base_triggered_by.py
+-rw-r--r--   0        0        0      578 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/webhook_event_data.py
+-rw-r--r--   0        0        0     1201 2024-04-10 14:12:44.597927 flagright-1.5.0/src/flagright/types/webhook_event_type.py
+-rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.5.0/PKG-INFO
```

### Comparing `flagright-1.4.9/README.md` & `flagright-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/__init__.py` & `flagright-1.5.0/src/flagright/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     BusinessOptionalSavedPaymentDetailsItem_Check,
     BusinessOptionalSavedPaymentDetailsItem_GenericBankAccount,
     BusinessOptionalSavedPaymentDetailsItem_Iban,
     BusinessOptionalSavedPaymentDetailsItem_Mpesa,
     BusinessOptionalSavedPaymentDetailsItem_Swift,
     BusinessOptionalSavedPaymentDetailsItem_Upi,
     BusinessOptionalSavedPaymentDetailsItem_Wallet,
-    BusinessResponse,
+    BusinessUserEvent,
     BusinessUserSegment,
     BusinessUsersResponse,
     BusinessWithRulesResult,
     CardBrand,
     CardDetails,
     CardExpiry,
     CardFunding,
@@ -41,14 +41,15 @@
     CheckDeliveryStatus,
     CheckDetails,
     CheckPaymentMethod,
     CompanyFinancialDetails,
     CompanyGeneralDetails,
     CompanyRegistrationDetails,
     ConsumerName,
+    ConsumerUserEvent,
     ConsumerUserSegment,
     ConsumerUsersResponse,
     ContactDetails,
     CountryCode,
     CurrencyCode,
     Date,
     DeviceData,
@@ -136,15 +137,14 @@
     UpiDetails,
     UpiPaymentMethod,
     User,
     UserBase,
     UserDetails,
     UserOptional,
     UserRegistrationStatus,
-    UserResponse,
     UserRiskScoreDetails,
     UserState,
     UserStateDetails,
     UserWithRulesResult,
     WalletDetails,
     WalletPaymentMethod,
     WebhookEvent,
@@ -186,15 +186,15 @@
     "BusinessOptionalSavedPaymentDetailsItem_Check",
     "BusinessOptionalSavedPaymentDetailsItem_GenericBankAccount",
     "BusinessOptionalSavedPaymentDetailsItem_Iban",
     "BusinessOptionalSavedPaymentDetailsItem_Mpesa",
     "BusinessOptionalSavedPaymentDetailsItem_Swift",
     "BusinessOptionalSavedPaymentDetailsItem_Upi",
     "BusinessOptionalSavedPaymentDetailsItem_Wallet",
-    "BusinessResponse",
+    "BusinessUserEvent",
     "BusinessUserSegment",
     "BusinessUsersCreateResponse",
     "BusinessUsersResponse",
     "BusinessWithRulesResult",
     "CardBrand",
     "CardDetails",
     "CardExpiry",
@@ -210,14 +210,15 @@
     "CheckDeliveryStatus",
     "CheckDetails",
     "CheckPaymentMethod",
     "CompanyFinancialDetails",
     "CompanyGeneralDetails",
     "CompanyRegistrationDetails",
     "ConsumerName",
+    "ConsumerUserEvent",
     "ConsumerUserSegment",
     "ConsumerUsersCreateResponse",
     "ConsumerUsersResponse",
     "ContactDetails",
     "CountryCode",
     "CurrencyCode",
     "Date",
@@ -311,15 +312,14 @@
     "UpiDetails",
     "UpiPaymentMethod",
     "User",
     "UserBase",
     "UserDetails",
     "UserOptional",
     "UserRegistrationStatus",
-    "UserResponse",
     "UserRiskScoreDetails",
     "UserState",
     "UserStateDetails",
     "UserWithRulesResult",
     "WalletDetails",
     "WalletPaymentMethod",
     "WebhookEvent",
```

### Comparing `flagright-1.4.9/src/flagright/client.py` & `flagright-1.5.0/src/flagright/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/core/__init__.py` & `flagright-1.5.0/src/flagright/core/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/core/client_wrapper.py` & `flagright-1.5.0/src/flagright/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "flagright",
-            "X-Fern-SDK-Version": "1.4.9",
+            "X-Fern-SDK-Version": "1.5.0",
         }
         headers["x-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `flagright-1.4.9/src/flagright/core/datetime_utils.py` & `flagright-1.5.0/src/flagright/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/core/jsonable_encoder.py` & `flagright-1.5.0/src/flagright/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/resources/__init__.py` & `flagright-1.5.0/src/flagright/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/resources/business_user_events/client.py` & `flagright-1.5.0/src/flagright/resources/business_user_events/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...errors.bad_request_error import BadRequestError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.boolean_string import BooleanString
-from ...types.business_optional import BusinessOptional
+from ...types.business_user_event import BusinessUserEvent
 from ...types.business_with_rules_result import BusinessWithRulesResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -25,23 +25,15 @@
 
 
 class BusinessUserEventsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
-        self,
-        *,
-        allow_user_type_conversion: typing.Optional[BooleanString] = None,
-        timestamp: float,
-        user_id: str,
-        event_id: typing.Optional[str] = OMIT,
-        reason: typing.Optional[str] = OMIT,
-        event_description: typing.Optional[str] = OMIT,
-        updated_business_user_attributes: typing.Optional[BusinessOptional] = OMIT,
+        self, *, allow_user_type_conversion: typing.Optional[BooleanString] = None, request: BusinessUserEvent
     ) -> BusinessWithRulesResult:
         """
         ## POST Business User Events
 
         `/events/business/user` endpoint allows you to operate on the Business User Events entity.
 
         User events are created after the initial `POST /business/users` call (which creates a user) and are used to:
@@ -59,30 +51,21 @@
         - `userId` - The ID of the transaction for which this event is generated.
 
         In order to make individual events retrievable, you also need to pass in a unique `eventId` to the request body.
 
         Parameters:
             - allow_user_type_conversion: typing.Optional[BooleanString]. Boolean string whether Flagright should allow a Business user event to be applied to a Consumer user with the same user ID. This will converts a Consumer user to a Business user.
 
-            - timestamp: float. Timestamp of the event
-
-            - user_id: str. Transaction ID the event pertains to
-
-            - event_id: typing.Optional[str]. Unique event ID
-
-            - reason: typing.Optional[str]. Reason for the event or a state change
-
-            - event_description: typing.Optional[str]. Event description
-
-            - updated_business_user_attributes: typing.Optional[BusinessOptional].
+            - request: BusinessUserEvent.
         ---
         from flagright import (
             Address,
             Amount,
             BusinessOptional,
+            BusinessUserEvent,
             CompanyFinancialDetails,
             CompanyGeneralDetails,
             CompanyRegistrationDetails,
             ConsumerName,
             ContactDetails,
             CountryCode,
             CurrencyCode,
@@ -95,160 +78,64 @@
         )
         from flagright.client import Flagright
 
         client = Flagright(
             api_key="YOUR_API_KEY",
         )
         client.business_user_events.create(
-            timestamp=1.1,
-            user_id="userId",
-            updated_business_user_attributes=BusinessOptional(
-                legal_entity=LegalEntity(
-                    company_general_details=CompanyGeneralDetails(
-                        legal_name="Ozkan Hazelnut Export JSC",
-                        business_industry=["Farming", "businessIndustry"],
-                        main_products_services_sold=[
-                            "Hazelnut",
-                            "mainProductsServicesSold",
-                        ],
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    company_financial_details=CompanyFinancialDetails(
-                        expected_transaction_amount_per_month=Amount(
-                            amount_value=800.0,
-                            amount_currency=CurrencyCode.GBP,
+            request=BusinessUserEvent(
+                timestamp=1.1,
+                user_id="userId",
+                updated_business_user_attributes=BusinessOptional(
+                    legal_entity=LegalEntity(
+                        company_general_details=CompanyGeneralDetails(
+                            legal_name="Ozkan Hazelnut Export JSC",
+                            business_industry=["Farming", "businessIndustry"],
+                            main_products_services_sold=[
+                                "Hazelnut",
+                                "mainProductsServicesSold",
+                            ],
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
                         ),
-                        expected_turnover_per_month=Amount(
-                            amount_value=8000.0,
-                            amount_currency=CurrencyCode.USD,
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    company_registration_details=CompanyRegistrationDetails(
-                        registration_identifier="PSJ554342",
-                        registration_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    reason_for_account_opening=["string", "reasonForAccountOpening"],
-                    contact_details=ContactDetails(
-                        addresses=[
-                            Address(
-                                address_lines=["Klara-Franke Str 20"],
-                                postcode="10557",
-                                city="Berlin",
-                                state="Berlin",
-                                country="Germany",
-                                tags=[
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                            ),
-                            Address(
-                                address_lines=["Klara-Franke Str 20"],
-                                postcode="10557",
-                                city="Berlin",
-                                state="Berlin",
-                                country="Germany",
-                                tags=[
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                            ),
-                        ],
-                    ),
-                ),
-                share_holders=[
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
-                            ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
-                            ),
+                        company_financial_details=CompanyFinancialDetails(
+                            expected_transaction_amount_per_month=Amount(
+                                amount_value=800.0,
+                                amount_currency=CurrencyCode.GBP,
+                            ),
+                            expected_turnover_per_month=Amount(
+                                amount_value=8000.0,
+                                amount_currency=CurrencyCode.USD,
+                            ),
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
+                        ),
+                        company_registration_details=CompanyRegistrationDetails(
+                            registration_identifier="PSJ554342",
+                            registration_country=CountryCode.DE,
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
+                        ),
+                        reason_for_account_opening=[
+                            "string",
+                            "reasonForAccountOpening",
                         ],
                         contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
                             addresses=[
                                 Address(
                                     address_lines=["Klara-Franke Str 20"],
                                     postcode="10557",
                                     city="Berlin",
                                     state="Berlin",
                                     country="Germany",
@@ -278,408 +165,500 @@
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
                                 ),
                             ],
                         ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
                     ),
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                    share_holders=[
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
+                                    tags=[
+                                        Tag(
+                                            key="customerType",
+                                            value="wallet",
+                                        ),
+                                        Tag(
+                                            key="customKey",
+                                            value="customValue",
+                                        ),
+                                    ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
+                                ),
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
+                                    tags=[
+                                        Tag(
+                                            key="customerType",
+                                            value="wallet",
+                                        ),
+                                        Tag(
+                                            key="customKey",
+                                            value="customValue",
+                                        ),
+                                    ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
+                                ),
+                            ],
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
+                            ),
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                    ),
-                ],
-                directors=[
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
                             ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                    ],
+                    directors=[
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                    ),
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
                             ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                ],
                             ),
-                        ],
-                    ),
-                ],
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                    ],
+                    transaction_limits=TransactionLimits(
+                        maximum_daily_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_weekly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_monthly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_quarterly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_yearly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
                     ),
+                    tags=[
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                    ],
                 ),
-                tags=[
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                ],
             ),
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"timestamp": timestamp, "userId": user_id}
-        if event_id is not OMIT:
-            _request["eventId"] = event_id
-        if reason is not OMIT:
-            _request["reason"] = reason
-        if event_description is not OMIT:
-            _request["eventDescription"] = event_description
-        if updated_business_user_attributes is not OMIT:
-            _request["updatedBusinessUserAttributes"] = updated_business_user_attributes
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "events/business/user"),
             params=remove_none_from_dict({"allowUserTypeConversion": allow_user_type_conversion}),
-            json=jsonable_encoder(_request),
+            json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BusinessWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -689,29 +668,57 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get(self, event_id: str) -> BusinessUserEvent:
+        """
+        ### GET a Business User Event
+
+        You can retrieve any business user event you created using the [POST Business User Events](/api-reference/api-reference/business-user-events/create) call.
+
+        Parameters:
+            - event_id: str. Unique Business User Event Identifier
+        ---
+        from flagright.client import Flagright
+
+        client = Flagright(
+            api_key="YOUR_API_KEY",
+        )
+        client.business_user_events.get(
+            event_id="eventId",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"events/business/user/{event_id}"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(BusinessUserEvent, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncBusinessUserEventsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
-        self,
-        *,
-        allow_user_type_conversion: typing.Optional[BooleanString] = None,
-        timestamp: float,
-        user_id: str,
-        event_id: typing.Optional[str] = OMIT,
-        reason: typing.Optional[str] = OMIT,
-        event_description: typing.Optional[str] = OMIT,
-        updated_business_user_attributes: typing.Optional[BusinessOptional] = OMIT,
+        self, *, allow_user_type_conversion: typing.Optional[BooleanString] = None, request: BusinessUserEvent
     ) -> BusinessWithRulesResult:
         """
         ## POST Business User Events
 
         `/events/business/user` endpoint allows you to operate on the Business User Events entity.
 
         User events are created after the initial `POST /business/users` call (which creates a user) and are used to:
@@ -729,30 +736,21 @@
         - `userId` - The ID of the transaction for which this event is generated.
 
         In order to make individual events retrievable, you also need to pass in a unique `eventId` to the request body.
 
         Parameters:
             - allow_user_type_conversion: typing.Optional[BooleanString]. Boolean string whether Flagright should allow a Business user event to be applied to a Consumer user with the same user ID. This will converts a Consumer user to a Business user.
 
-            - timestamp: float. Timestamp of the event
-
-            - user_id: str. Transaction ID the event pertains to
-
-            - event_id: typing.Optional[str]. Unique event ID
-
-            - reason: typing.Optional[str]. Reason for the event or a state change
-
-            - event_description: typing.Optional[str]. Event description
-
-            - updated_business_user_attributes: typing.Optional[BusinessOptional].
+            - request: BusinessUserEvent.
         ---
         from flagright import (
             Address,
             Amount,
             BusinessOptional,
+            BusinessUserEvent,
             CompanyFinancialDetails,
             CompanyGeneralDetails,
             CompanyRegistrationDetails,
             ConsumerName,
             ContactDetails,
             CountryCode,
             CurrencyCode,
@@ -765,160 +763,64 @@
         )
         from flagright.client import AsyncFlagright
 
         client = AsyncFlagright(
             api_key="YOUR_API_KEY",
         )
         await client.business_user_events.create(
-            timestamp=1.1,
-            user_id="userId",
-            updated_business_user_attributes=BusinessOptional(
-                legal_entity=LegalEntity(
-                    company_general_details=CompanyGeneralDetails(
-                        legal_name="Ozkan Hazelnut Export JSC",
-                        business_industry=["Farming", "businessIndustry"],
-                        main_products_services_sold=[
-                            "Hazelnut",
-                            "mainProductsServicesSold",
-                        ],
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    company_financial_details=CompanyFinancialDetails(
-                        expected_transaction_amount_per_month=Amount(
-                            amount_value=800.0,
-                            amount_currency=CurrencyCode.GBP,
+            request=BusinessUserEvent(
+                timestamp=1.1,
+                user_id="userId",
+                updated_business_user_attributes=BusinessOptional(
+                    legal_entity=LegalEntity(
+                        company_general_details=CompanyGeneralDetails(
+                            legal_name="Ozkan Hazelnut Export JSC",
+                            business_industry=["Farming", "businessIndustry"],
+                            main_products_services_sold=[
+                                "Hazelnut",
+                                "mainProductsServicesSold",
+                            ],
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
                         ),
-                        expected_turnover_per_month=Amount(
-                            amount_value=8000.0,
-                            amount_currency=CurrencyCode.USD,
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    company_registration_details=CompanyRegistrationDetails(
-                        registration_identifier="PSJ554342",
-                        registration_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            )
-                        ],
-                    ),
-                    reason_for_account_opening=["string", "reasonForAccountOpening"],
-                    contact_details=ContactDetails(
-                        addresses=[
-                            Address(
-                                address_lines=["Klara-Franke Str 20"],
-                                postcode="10557",
-                                city="Berlin",
-                                state="Berlin",
-                                country="Germany",
-                                tags=[
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                            ),
-                            Address(
-                                address_lines=["Klara-Franke Str 20"],
-                                postcode="10557",
-                                city="Berlin",
-                                state="Berlin",
-                                country="Germany",
-                                tags=[
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                            ),
-                        ],
-                    ),
-                ),
-                share_holders=[
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
-                            ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
-                            ),
+                        company_financial_details=CompanyFinancialDetails(
+                            expected_transaction_amount_per_month=Amount(
+                                amount_value=800.0,
+                                amount_currency=CurrencyCode.GBP,
+                            ),
+                            expected_turnover_per_month=Amount(
+                                amount_value=8000.0,
+                                amount_currency=CurrencyCode.USD,
+                            ),
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
+                        ),
+                        company_registration_details=CompanyRegistrationDetails(
+                            registration_identifier="PSJ554342",
+                            registration_country=CountryCode.DE,
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                )
+                            ],
+                        ),
+                        reason_for_account_opening=[
+                            "string",
+                            "reasonForAccountOpening",
                         ],
                         contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
                             addresses=[
                                 Address(
                                     address_lines=["Klara-Franke Str 20"],
                                     postcode="10557",
                                     city="Berlin",
                                     state="Berlin",
                                     country="Germany",
@@ -948,417 +850,545 @@
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
                                 ),
                             ],
                         ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
                     ),
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                    share_holders=[
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
+                                    tags=[
+                                        Tag(
+                                            key="customerType",
+                                            value="wallet",
+                                        ),
+                                        Tag(
+                                            key="customKey",
+                                            value="customValue",
+                                        ),
+                                    ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
+                                ),
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
+                                    tags=[
+                                        Tag(
+                                            key="customerType",
+                                            value="wallet",
+                                        ),
+                                        Tag(
+                                            key="customKey",
+                                            value="customValue",
+                                        ),
+                                    ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
+                                ),
+                            ],
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
+                            ),
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                    ),
-                ],
-                directors=[
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
                             ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                    ],
+                    directors=[
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                    ),
-                    Person(
-                        general_details=UserDetails(
-                            name=ConsumerName(
-                                first_name="Baran",
-                                middle_name="Realblood",
-                                last_name="Ozkan",
-                            ),
-                            date_of_birth="1991-01-01",
-                            country_of_residence=CountryCode.US,
-                            country_of_nationality=CountryCode.DE,
-                        ),
-                        legal_documents=[
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
                                     ),
                                 ],
-                                name_on_document=ConsumerName(
-                                    first_name="Baran",
-                                    middle_name="Realblood",
-                                    last_name="Ozkan",
-                                ),
                             ),
-                            LegalDocument(
-                                document_type="passport",
-                                document_number="Z9431P",
-                                document_issued_date=1639939034000.0,
-                                document_expiration_date=1839939034000.0,
-                                document_issued_country=CountryCode.DE,
-                                tags=[
-                                    Tag(
-                                        key="customerType",
-                                        value="wallet",
-                                    ),
-                                    Tag(
-                                        key="customKey",
-                                        value="customValue",
-                                    ),
-                                ],
-                                name_on_document=ConsumerName(
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                        Person(
+                            general_details=UserDetails(
+                                name=ConsumerName(
                                     first_name="Baran",
                                     middle_name="Realblood",
                                     last_name="Ozkan",
                                 ),
-                            ),
-                        ],
-                        contact_details=ContactDetails(
-                            email_ids=["baran@flagright.com", "emailIds"],
-                            contact_numbers=["+371 123132", "contactNumbers"],
-                            websites=["flagright.com", "websites"],
-                            addresses=[
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                date_of_birth="1991-01-01",
+                                country_of_residence=CountryCode.US,
+                                country_of_nationality=CountryCode.DE,
+                            ),
+                            legal_documents=[
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
-                                Address(
-                                    address_lines=["Klara-Franke Str 20"],
-                                    postcode="10557",
-                                    city="Berlin",
-                                    state="Berlin",
-                                    country="Germany",
+                                LegalDocument(
+                                    document_type="passport",
+                                    document_number="Z9431P",
+                                    document_issued_date=1639939034000.0,
+                                    document_expiration_date=1839939034000.0,
+                                    document_issued_country=CountryCode.DE,
                                     tags=[
                                         Tag(
-                                            key="customKey",
-                                            value="customValue",
+                                            key="customerType",
+                                            value="wallet",
                                         ),
                                         Tag(
                                             key="customKey",
                                             value="customValue",
                                         ),
                                     ],
+                                    name_on_document=ConsumerName(
+                                        first_name="Baran",
+                                        middle_name="Realblood",
+                                        last_name="Ozkan",
+                                    ),
                                 ),
                             ],
-                        ),
-                        tags=[
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
+                            contact_details=ContactDetails(
+                                email_ids=["baran@flagright.com", "emailIds"],
+                                contact_numbers=["+371 123132", "contactNumbers"],
+                                websites=["flagright.com", "websites"],
+                                addresses=[
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                    Address(
+                                        address_lines=["Klara-Franke Str 20"],
+                                        postcode="10557",
+                                        city="Berlin",
+                                        state="Berlin",
+                                        country="Germany",
+                                        tags=[
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                            Tag(
+                                                key="customKey",
+                                                value="customValue",
+                                            ),
+                                        ],
+                                    ),
+                                ],
                             ),
-                        ],
-                    ),
-                ],
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                            tags=[
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                                Tag(
+                                    key="customKey",
+                                    value="customValue",
+                                ),
+                            ],
+                        ),
+                    ],
+                    transaction_limits=TransactionLimits(
+                        maximum_daily_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_weekly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_monthly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_quarterly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_yearly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
                     ),
+                    tags=[
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                    ],
                 ),
-                tags=[
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                ],
             ),
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"timestamp": timestamp, "userId": user_id}
-        if event_id is not OMIT:
-            _request["eventId"] = event_id
-        if reason is not OMIT:
-            _request["reason"] = reason
-        if event_description is not OMIT:
-            _request["eventDescription"] = event_description
-        if updated_business_user_attributes is not OMIT:
-            _request["updatedBusinessUserAttributes"] = updated_business_user_attributes
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "events/business/user"),
             params=remove_none_from_dict({"allowUserTypeConversion": allow_user_type_conversion}),
-            json=jsonable_encoder(_request),
+            json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BusinessWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get(self, event_id: str) -> BusinessUserEvent:
+        """
+        ### GET a Business User Event
+
+        You can retrieve any business user event you created using the [POST Business User Events](/api-reference/api-reference/business-user-events/create) call.
+
+        Parameters:
+            - event_id: str. Unique Business User Event Identifier
+        ---
+        from flagright.client import AsyncFlagright
+
+        client = AsyncFlagright(
+            api_key="YOUR_API_KEY",
+        )
+        await client.business_user_events.get(
+            event_id="eventId",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"events/business/user/{event_id}"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(BusinessUserEvent, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flagright-1.4.9/src/flagright/resources/business_users/client.py` & `flagright-1.5.0/src/flagright/resources/business_users/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...errors.bad_request_error import BadRequestError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.business import Business
-from ...types.business_response import BusinessResponse
+from ...types.business_with_rules_result import BusinessWithRulesResult
 from .types.business_users_create_response import BusinessUsersCreateResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -389,15 +389,15 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, user_id: str) -> BusinessResponse:
+    def get(self, user_id: str) -> BusinessWithRulesResult:
         """
         ### GET Business User
 
         `/business/user` endpoint allows you to operate on the Business User entity.
 
         Calling `GET /business/user/{userId}` will return the entire User payload and rule execution results for the User with the corresponding `userId`
 
@@ -416,15 +416,15 @@
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"business/users/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BusinessResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BusinessWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -798,15 +798,15 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, user_id: str) -> BusinessResponse:
+    async def get(self, user_id: str) -> BusinessWithRulesResult:
         """
         ### GET Business User
 
         `/business/user` endpoint allows you to operate on the Business User entity.
 
         Calling `GET /business/user/{userId}` will return the entire User payload and rule execution results for the User with the corresponding `userId`
 
@@ -825,15 +825,15 @@
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"business/users/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BusinessResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BusinessWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `flagright-1.4.9/src/flagright/resources/business_users/types/business_users_create_response.py` & `flagright-1.5.0/src/flagright/resources/business_users/types/business_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/resources/consumer_user_events/client.py` & `flagright-1.5.0/src/flagright/resources/consumer_user_events/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...errors.bad_request_error import BadRequestError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.boolean_string import BooleanString
-from ...types.user_optional import UserOptional
+from ...types.consumer_user_event import ConsumerUserEvent
 from ...types.user_with_rules_result import UserWithRulesResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -25,23 +25,15 @@
 
 
 class ConsumerUserEventsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
-        self,
-        *,
-        allow_user_type_conversion: typing.Optional[BooleanString] = None,
-        timestamp: float,
-        user_id: str,
-        event_id: typing.Optional[str] = OMIT,
-        reason: typing.Optional[str] = OMIT,
-        event_description: typing.Optional[str] = OMIT,
-        updated_consumer_user_attributes: typing.Optional[UserOptional] = OMIT,
+        self, *, allow_user_type_conversion: typing.Optional[BooleanString] = None, request: ConsumerUserEvent
     ) -> UserWithRulesResult:
         """
         ## POST Consumer User Events
 
         `/events/consumer/user` endpoint allows you to operate on the Consumer User Events entity.
 
         User events are created after the initial `POST /consumer/users` call (which creates a user) and are used to:
@@ -59,30 +51,21 @@
         - `userId` - The ID of the transaction for which this event is generated.
 
         In order to make individual events retrievable, you also need to pass in a unique `eventId` to the request body.
 
         Parameters:
             - allow_user_type_conversion: typing.Optional[BooleanString]. Boolean string whether Flagright should allow a Consumer user event to be applied to a Business user with the same user ID. This will converts a Business user to a Consumer user.
 
-            - timestamp: float. Timestamp of the event
-
-            - user_id: str. Transaction ID the event pertains to
-
-            - event_id: typing.Optional[str]. Unique event ID
-
-            - reason: typing.Optional[str]. Reason for the event or a state change
-
-            - event_description: typing.Optional[str]. Event description
-
-            - updated_consumer_user_attributes: typing.Optional[UserOptional].
+            - request: ConsumerUserEvent.
         ---
         from flagright import (
             Address,
             Amount,
             ConsumerName,
+            ConsumerUserEvent,
             ContactDetails,
             CountryCode,
             CurrencyCode,
             LegalDocument,
             Tag,
             TransactionLimits,
             UserDetails,
@@ -90,167 +73,160 @@
         )
         from flagright.client import Flagright
 
         client = Flagright(
             api_key="YOUR_API_KEY",
         )
         client.consumer_user_events.create(
-            timestamp=1.1,
-            user_id="userId",
-            updated_consumer_user_attributes=UserOptional(
-                user_details=UserDetails(
-                    name=ConsumerName(
-                        first_name="Baran",
-                        middle_name="Realblood",
-                        last_name="Ozkan",
-                    ),
-                    date_of_birth="1991-01-01",
-                    country_of_residence=CountryCode.US,
-                    country_of_nationality=CountryCode.DE,
-                ),
-                legal_documents=[
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
+            request=ConsumerUserEvent(
+                timestamp=1.1,
+                user_id="userId",
+                updated_consumer_user_attributes=UserOptional(
+                    user_details=UserDetails(
+                        name=ConsumerName(
                             first_name="Baran",
                             middle_name="Realblood",
                             last_name="Ozkan",
                         ),
-                    ),
-                ],
-                contact_details=ContactDetails(
-                    email_ids=["baran@flagright.com", "emailIds"],
-                    contact_numbers=["+37112345432", "contactNumbers"],
-                    websites=["flagright.com", "websites"],
-                    addresses=[
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
+                        date_of_birth="1991-01-01",
+                        country_of_residence=CountryCode.US,
+                        country_of_nationality=CountryCode.DE,
+                    ),
+                    legal_documents=[
+                        LegalDocument(
+                            document_type="passport",
+                            document_number="Z9431P",
+                            document_issued_date=1639939034000.0,
+                            document_expiration_date=1839939034000.0,
+                            document_issued_country=CountryCode.DE,
                             tags=[
                                 Tag(
-                                    key="customKey",
-                                    value="customValue",
+                                    key="customerType",
+                                    value="wallet",
                                 ),
                                 Tag(
                                     key="customKey",
                                     value="customValue",
                                 ),
                             ],
+                            name_on_document=ConsumerName(
+                                first_name="Baran",
+                                middle_name="Realblood",
+                                last_name="Ozkan",
+                            ),
                         ),
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
+                        LegalDocument(
+                            document_type="passport",
+                            document_number="Z9431P",
+                            document_issued_date=1639939034000.0,
+                            document_expiration_date=1839939034000.0,
+                            document_issued_country=CountryCode.DE,
                             tags=[
                                 Tag(
-                                    key="customKey",
-                                    value="customValue",
+                                    key="customerType",
+                                    value="wallet",
                                 ),
                                 Tag(
                                     key="customKey",
                                     value="customValue",
                                 ),
                             ],
+                            name_on_document=ConsumerName(
+                                first_name="Baran",
+                                middle_name="Realblood",
+                                last_name="Ozkan",
+                            ),
                         ),
                     ],
-                ),
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                    contact_details=ContactDetails(
+                        email_ids=["baran@flagright.com", "emailIds"],
+                        contact_numbers=["+37112345432", "contactNumbers"],
+                        websites=["flagright.com", "websites"],
+                        addresses=[
+                            Address(
+                                address_lines=["Klara-Franke Str 20"],
+                                postcode="10557",
+                                city="Berlin",
+                                state="Berlin",
+                                country="Germany",
+                                tags=[
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                ],
+                            ),
+                            Address(
+                                address_lines=["Klara-Franke Str 20"],
+                                postcode="10557",
+                                city="Berlin",
+                                state="Berlin",
+                                country="Germany",
+                                tags=[
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                ],
+                            ),
+                        ],
                     ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                    transaction_limits=TransactionLimits(
+                        maximum_daily_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_weekly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_monthly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_quarterly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_yearly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
                     ),
+                    tags=[
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                    ],
                 ),
-                tags=[
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                ],
             ),
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"timestamp": timestamp, "userId": user_id}
-        if event_id is not OMIT:
-            _request["eventId"] = event_id
-        if reason is not OMIT:
-            _request["reason"] = reason
-        if event_description is not OMIT:
-            _request["eventDescription"] = event_description
-        if updated_consumer_user_attributes is not OMIT:
-            _request["updatedConsumerUserAttributes"] = updated_consumer_user_attributes
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "events/consumer/user"),
             params=remove_none_from_dict({"allowUserTypeConversion": allow_user_type_conversion}),
-            json=jsonable_encoder(_request),
+            json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -260,29 +236,57 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get(self, event_id: str) -> ConsumerUserEvent:
+        """
+        ### GET a Consumer User Event
+
+        You can retrieve any consumer user event you created using the [POST Consumer User Events](/api-reference/api-reference/consumer-user-events/create) call.
+
+        Parameters:
+            - event_id: str. Unique Consumer User Event Identifier
+        ---
+        from flagright.client import Flagright
+
+        client = Flagright(
+            api_key="YOUR_API_KEY",
+        )
+        client.consumer_user_events.get(
+            event_id="eventId",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"events/consumer/user/{event_id}"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ConsumerUserEvent, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncConsumerUserEventsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
-        self,
-        *,
-        allow_user_type_conversion: typing.Optional[BooleanString] = None,
-        timestamp: float,
-        user_id: str,
-        event_id: typing.Optional[str] = OMIT,
-        reason: typing.Optional[str] = OMIT,
-        event_description: typing.Optional[str] = OMIT,
-        updated_consumer_user_attributes: typing.Optional[UserOptional] = OMIT,
+        self, *, allow_user_type_conversion: typing.Optional[BooleanString] = None, request: ConsumerUserEvent
     ) -> UserWithRulesResult:
         """
         ## POST Consumer User Events
 
         `/events/consumer/user` endpoint allows you to operate on the Consumer User Events entity.
 
         User events are created after the initial `POST /consumer/users` call (which creates a user) and are used to:
@@ -300,30 +304,21 @@
         - `userId` - The ID of the transaction for which this event is generated.
 
         In order to make individual events retrievable, you also need to pass in a unique `eventId` to the request body.
 
         Parameters:
             - allow_user_type_conversion: typing.Optional[BooleanString]. Boolean string whether Flagright should allow a Consumer user event to be applied to a Business user with the same user ID. This will converts a Business user to a Consumer user.
 
-            - timestamp: float. Timestamp of the event
-
-            - user_id: str. Transaction ID the event pertains to
-
-            - event_id: typing.Optional[str]. Unique event ID
-
-            - reason: typing.Optional[str]. Reason for the event or a state change
-
-            - event_description: typing.Optional[str]. Event description
-
-            - updated_consumer_user_attributes: typing.Optional[UserOptional].
+            - request: ConsumerUserEvent.
         ---
         from flagright import (
             Address,
             Amount,
             ConsumerName,
+            ConsumerUserEvent,
             ContactDetails,
             CountryCode,
             CurrencyCode,
             LegalDocument,
             Tag,
             TransactionLimits,
             UserDetails,
@@ -331,176 +326,205 @@
         )
         from flagright.client import AsyncFlagright
 
         client = AsyncFlagright(
             api_key="YOUR_API_KEY",
         )
         await client.consumer_user_events.create(
-            timestamp=1.1,
-            user_id="userId",
-            updated_consumer_user_attributes=UserOptional(
-                user_details=UserDetails(
-                    name=ConsumerName(
-                        first_name="Baran",
-                        middle_name="Realblood",
-                        last_name="Ozkan",
-                    ),
-                    date_of_birth="1991-01-01",
-                    country_of_residence=CountryCode.US,
-                    country_of_nationality=CountryCode.DE,
-                ),
-                legal_documents=[
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
-                            first_name="Baran",
-                            middle_name="Realblood",
-                            last_name="Ozkan",
-                        ),
-                    ),
-                    LegalDocument(
-                        document_type="passport",
-                        document_number="Z9431P",
-                        document_issued_date=1639939034000.0,
-                        document_expiration_date=1839939034000.0,
-                        document_issued_country=CountryCode.DE,
-                        tags=[
-                            Tag(
-                                key="customerType",
-                                value="wallet",
-                            ),
-                            Tag(
-                                key="customKey",
-                                value="customValue",
-                            ),
-                        ],
-                        name_on_document=ConsumerName(
+            request=ConsumerUserEvent(
+                timestamp=1.1,
+                user_id="userId",
+                updated_consumer_user_attributes=UserOptional(
+                    user_details=UserDetails(
+                        name=ConsumerName(
                             first_name="Baran",
                             middle_name="Realblood",
                             last_name="Ozkan",
                         ),
-                    ),
-                ],
-                contact_details=ContactDetails(
-                    email_ids=["baran@flagright.com", "emailIds"],
-                    contact_numbers=["+37112345432", "contactNumbers"],
-                    websites=["flagright.com", "websites"],
-                    addresses=[
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
+                        date_of_birth="1991-01-01",
+                        country_of_residence=CountryCode.US,
+                        country_of_nationality=CountryCode.DE,
+                    ),
+                    legal_documents=[
+                        LegalDocument(
+                            document_type="passport",
+                            document_number="Z9431P",
+                            document_issued_date=1639939034000.0,
+                            document_expiration_date=1839939034000.0,
+                            document_issued_country=CountryCode.DE,
                             tags=[
                                 Tag(
-                                    key="customKey",
-                                    value="customValue",
+                                    key="customerType",
+                                    value="wallet",
                                 ),
                                 Tag(
                                     key="customKey",
                                     value="customValue",
                                 ),
                             ],
+                            name_on_document=ConsumerName(
+                                first_name="Baran",
+                                middle_name="Realblood",
+                                last_name="Ozkan",
+                            ),
                         ),
-                        Address(
-                            address_lines=["Klara-Franke Str 20"],
-                            postcode="10557",
-                            city="Berlin",
-                            state="Berlin",
-                            country="Germany",
+                        LegalDocument(
+                            document_type="passport",
+                            document_number="Z9431P",
+                            document_issued_date=1639939034000.0,
+                            document_expiration_date=1839939034000.0,
+                            document_issued_country=CountryCode.DE,
                             tags=[
                                 Tag(
-                                    key="customKey",
-                                    value="customValue",
+                                    key="customerType",
+                                    value="wallet",
                                 ),
                                 Tag(
                                     key="customKey",
                                     value="customValue",
                                 ),
                             ],
+                            name_on_document=ConsumerName(
+                                first_name="Baran",
+                                middle_name="Realblood",
+                                last_name="Ozkan",
+                            ),
                         ),
                     ],
-                ),
-                transaction_limits=TransactionLimits(
-                    maximum_daily_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_weekly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_monthly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_quarterly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
-                    ),
-                    maximum_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                    contact_details=ContactDetails(
+                        email_ids=["baran@flagright.com", "emailIds"],
+                        contact_numbers=["+37112345432", "contactNumbers"],
+                        websites=["flagright.com", "websites"],
+                        addresses=[
+                            Address(
+                                address_lines=["Klara-Franke Str 20"],
+                                postcode="10557",
+                                city="Berlin",
+                                state="Berlin",
+                                country="Germany",
+                                tags=[
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                ],
+                            ),
+                            Address(
+                                address_lines=["Klara-Franke Str 20"],
+                                postcode="10557",
+                                city="Berlin",
+                                state="Berlin",
+                                country="Germany",
+                                tags=[
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                    Tag(
+                                        key="customKey",
+                                        value="customValue",
+                                    ),
+                                ],
+                            ),
+                        ],
                     ),
-                    maximum_yearly_transaction_limit=Amount(
-                        amount_value=800.0,
-                        amount_currency=CurrencyCode.GBP,
+                    transaction_limits=TransactionLimits(
+                        maximum_daily_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_weekly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_monthly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_quarterly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
+                        maximum_yearly_transaction_limit=Amount(
+                            amount_value=800.0,
+                            amount_currency=CurrencyCode.GBP,
+                        ),
                     ),
+                    tags=[
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                        Tag(
+                            key="customKey",
+                            value="customValue",
+                        ),
+                    ],
                 ),
-                tags=[
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                    Tag(
-                        key="customKey",
-                        value="customValue",
-                    ),
-                ],
             ),
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"timestamp": timestamp, "userId": user_id}
-        if event_id is not OMIT:
-            _request["eventId"] = event_id
-        if reason is not OMIT:
-            _request["reason"] = reason
-        if event_description is not OMIT:
-            _request["eventDescription"] = event_description
-        if updated_consumer_user_attributes is not OMIT:
-            _request["updatedConsumerUserAttributes"] = updated_consumer_user_attributes
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "events/consumer/user"),
             params=remove_none_from_dict({"allowUserTypeConversion": allow_user_type_conversion}),
-            json=jsonable_encoder(_request),
+            json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get(self, event_id: str) -> ConsumerUserEvent:
+        """
+        ### GET a Consumer User Event
+
+        You can retrieve any consumer user event you created using the [POST Consumer User Events](/api-reference/api-reference/consumer-user-events/create) call.
+
+        Parameters:
+            - event_id: str. Unique Consumer User Event Identifier
+        ---
+        from flagright.client import AsyncFlagright
+
+        client = AsyncFlagright(
+            api_key="YOUR_API_KEY",
+        )
+        await client.consumer_user_events.get(
+            event_id="eventId",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"events/consumer/user/{event_id}"),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ConsumerUserEvent, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 429:
+            raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flagright-1.4.9/src/flagright/resources/consumer_users/client.py` & `flagright-1.5.0/src/flagright/resources/consumer_users/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...errors.bad_request_error import BadRequestError
 from ...errors.too_many_requests_error import TooManyRequestsError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.user import User
-from ...types.user_response import UserResponse
+from ...types.user_with_rules_result import UserWithRulesResult
 from .types.consumer_users_create_response import ConsumerUsersCreateResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -220,15 +220,15 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, user_id: str) -> UserResponse:
+    def get(self, user_id: str) -> UserWithRulesResult:
         """
         ### GET Consumer User
 
         `/consumer/user` endpoint allows you to operate on the Consumer User entity.
 
         Calling `GET /consumer/user/{userId}` will return the entire user payload and rule execution results for the user with the corresponding `userId`
 
@@ -247,15 +247,15 @@
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"consumer/users/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -460,15 +460,15 @@
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, user_id: str) -> UserResponse:
+    async def get(self, user_id: str) -> UserWithRulesResult:
         """
         ### GET Consumer User
 
         `/consumer/user` endpoint allows you to operate on the Consumer User entity.
 
         Calling `GET /consumer/user/{userId}` will return the entire user payload and rule execution results for the user with the corresponding `userId`
 
@@ -487,15 +487,15 @@
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"consumer/users/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserWithRulesResult, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 429:
             raise TooManyRequestsError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `flagright-1.4.9/src/flagright/resources/consumer_users/types/consumer_users_create_response.py` & `flagright-1.5.0/src/flagright/resources/consumer_users/types/consumer_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/resources/transaction_events/client.py` & `flagright-1.5.0/src/flagright/resources/transaction_events/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     def get(self, event_id: str) -> TransactionEvent:
         """
         ### GET Transaction Events
 
         `/events/transaction` endpoint allows you to operate on the [Transaction Events entity.](/guides/overview/entities#transaction-event).
 
-        You can retrieve any transaction event you create using the [POST Transaction Events](/api-reference/api-reference/transaction-events/create) call.
+        You can retrieve any transaction event you created using the [POST Transaction Events](/api-reference/api-reference/transaction-events/create) call.
 
         Parameters:
             - event_id: str. Unique Transaction Identifier
         ---
         from flagright.client import Flagright
 
         client = Flagright(
@@ -329,15 +329,15 @@
 
     async def get(self, event_id: str) -> TransactionEvent:
         """
         ### GET Transaction Events
 
         `/events/transaction` endpoint allows you to operate on the [Transaction Events entity.](/guides/overview/entities#transaction-event).
 
-        You can retrieve any transaction event you create using the [POST Transaction Events](/api-reference/api-reference/transaction-events/create) call.
+        You can retrieve any transaction event you created using the [POST Transaction Events](/api-reference/api-reference/transaction-events/create) call.
 
         Parameters:
             - event_id: str. Unique Transaction Identifier
         ---
         from flagright.client import AsyncFlagright
 
         client = AsyncFlagright(
```

### Comparing `flagright-1.4.9/src/flagright/resources/transactions/client.py` & `flagright-1.5.0/src/flagright/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/resources/transactions/types/transactions_verify_response.py` & `flagright-1.5.0/src/flagright/resources/transactions/types/transactions_verify_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/__init__.py` & `flagright-1.5.0/src/flagright/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     BusinessOptionalSavedPaymentDetailsItem_GenericBankAccount,
     BusinessOptionalSavedPaymentDetailsItem_Iban,
     BusinessOptionalSavedPaymentDetailsItem_Mpesa,
     BusinessOptionalSavedPaymentDetailsItem_Swift,
     BusinessOptionalSavedPaymentDetailsItem_Upi,
     BusinessOptionalSavedPaymentDetailsItem_Wallet,
 )
-from .business_response import BusinessResponse
+from .business_user_event import BusinessUserEvent
 from .business_user_segment import BusinessUserSegment
 from .business_users_response import BusinessUsersResponse
 from .business_with_rules_result import BusinessWithRulesResult
 from .card_brand import CardBrand
 from .card_details import CardDetails
 from .card_expiry import CardExpiry
 from .card_funding import CardFunding
@@ -42,14 +42,15 @@
 from .check_delivery_status import CheckDeliveryStatus
 from .check_details import CheckDetails
 from .check_payment_method import CheckPaymentMethod
 from .company_financial_details import CompanyFinancialDetails
 from .company_general_details import CompanyGeneralDetails
 from .company_registration_details import CompanyRegistrationDetails
 from .consumer_name import ConsumerName
+from .consumer_user_event import ConsumerUserEvent
 from .consumer_user_segment import ConsumerUserSegment
 from .consumer_users_response import ConsumerUsersResponse
 from .contact_details import ContactDetails
 from .country_code import CountryCode
 from .currency_code import CurrencyCode
 from .date import Date
 from .device_data import DeviceData
@@ -141,15 +142,14 @@
 from .upi_details import UpiDetails
 from .upi_payment_method import UpiPaymentMethod
 from .user import User
 from .user_base import UserBase
 from .user_details import UserDetails
 from .user_optional import UserOptional
 from .user_registration_status import UserRegistrationStatus
-from .user_response import UserResponse
 from .user_risk_score_details import UserRiskScoreDetails
 from .user_state import UserState
 from .user_state_details import UserStateDetails
 from .user_with_rules_result import UserWithRulesResult
 from .wallet_details import WalletDetails
 from .wallet_payment_method import WalletPaymentMethod
 from .webhook_event import WebhookEvent
@@ -176,15 +176,15 @@
     "BusinessOptionalSavedPaymentDetailsItem_Check",
     "BusinessOptionalSavedPaymentDetailsItem_GenericBankAccount",
     "BusinessOptionalSavedPaymentDetailsItem_Iban",
     "BusinessOptionalSavedPaymentDetailsItem_Mpesa",
     "BusinessOptionalSavedPaymentDetailsItem_Swift",
     "BusinessOptionalSavedPaymentDetailsItem_Upi",
     "BusinessOptionalSavedPaymentDetailsItem_Wallet",
-    "BusinessResponse",
+    "BusinessUserEvent",
     "BusinessUserSegment",
     "BusinessUsersResponse",
     "BusinessWithRulesResult",
     "CardBrand",
     "CardDetails",
     "CardExpiry",
     "CardFunding",
@@ -199,14 +199,15 @@
     "CheckDeliveryStatus",
     "CheckDetails",
     "CheckPaymentMethod",
     "CompanyFinancialDetails",
     "CompanyGeneralDetails",
     "CompanyRegistrationDetails",
     "ConsumerName",
+    "ConsumerUserEvent",
     "ConsumerUserSegment",
     "ConsumerUsersResponse",
     "ContactDetails",
     "CountryCode",
     "CurrencyCode",
     "Date",
     "DeviceData",
@@ -294,15 +295,14 @@
     "UpiDetails",
     "UpiPaymentMethod",
     "User",
     "UserBase",
     "UserDetails",
     "UserOptional",
     "UserRegistrationStatus",
-    "UserResponse",
     "UserRiskScoreDetails",
     "UserState",
     "UserStateDetails",
     "UserWithRulesResult",
     "WalletDetails",
     "WalletPaymentMethod",
     "WebhookEvent",
```

### Comparing `flagright-1.4.9/src/flagright/types/ach_details.py` & `flagright-1.5.0/src/flagright/types/ach_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/acquisition_channel.py` & `flagright-1.5.0/src/flagright/types/acquisition_channel.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/address.py` & `flagright-1.5.0/src/flagright/types/address.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/alert_closed_details.py` & `flagright-1.5.0/src/flagright/types/alert_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/amount.py` & `flagright-1.5.0/src/flagright/types/amount.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business.py` & `flagright-1.5.0/src/flagright/types/business.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_base.py` & `flagright-1.5.0/src/flagright/types/business_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_entity_link.py` & `flagright-1.5.0/src/flagright/types/business_entity_link.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_optional.py` & `flagright-1.5.0/src/flagright/types/business_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_optional_saved_payment_details_item.py` & `flagright-1.5.0/src/flagright/types/business_optional_saved_payment_details_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_response.py` & `flagright-1.5.0/src/flagright/types/user_with_rules_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .business_with_rules_result import BusinessWithRulesResult
+from .executed_rules_result import ExecutedRulesResult
+from .hit_rules_details import HitRulesDetails
+from .user import User
 from .user_risk_score_details import UserRiskScoreDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class BusinessResponse(BusinessWithRulesResult):
+class UserWithRulesResult(User):
+    """
+    Model for consumer user payload with rules result
+    """
+
+    executed_rules: typing.Optional[typing.List[ExecutedRulesResult]] = pydantic.Field(alias="executedRules")
+    hit_rules: typing.Optional[typing.List[HitRulesDetails]] = pydantic.Field(alias="hitRules")
     risk_score_details: typing.Optional[UserRiskScoreDetails] = pydantic.Field(alias="riskScoreDetails")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flagright-1.4.9/src/flagright/types/business_user_segment.py` & `flagright-1.5.0/src/flagright/types/business_user_segment.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_users_response.py` & `flagright-1.5.0/src/flagright/types/business_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/business_with_rules_result.py` & `flagright-1.5.0/src/flagright/types/transaction_monitoring_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .business import Business
-from .executed_rules_result import ExecutedRulesResult
-from .hit_rules_details import HitRulesDetails
+from .rule_action import RuleAction
+from .rules_results import RulesResults
+from .transaction_risk_scoring_result import TransactionRiskScoringResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class BusinessWithRulesResult(Business):
-    """
-    Model for business payload with rules result
-    """
-
-    executed_rules: typing.Optional[typing.List[ExecutedRulesResult]] = pydantic.Field(alias="executedRules")
-    hit_rules: typing.Optional[typing.List[HitRulesDetails]] = pydantic.Field(alias="hitRules")
+class TransactionMonitoringResult(RulesResults):
+    transaction_id: str = pydantic.Field(
+        alias="transactionId", description="Transaction ID that the results pertain to"
+    )
+    status: RuleAction
+    risk_score_details: typing.Optional[TransactionRiskScoringResult] = pydantic.Field(alias="riskScoreDetails")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/card_brand.py` & `flagright-1.5.0/src/flagright/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/card_details.py` & `flagright-1.5.0/src/flagright/types/card_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/card_expiry.py` & `flagright-1.5.0/src/flagright/types/card_expiry.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/card_funding.py` & `flagright-1.5.0/src/flagright/types/card_funding.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/card_merchant_details.py` & `flagright-1.5.0/src/flagright/types/card_merchant_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/case_closed_details.py` & `flagright-1.5.0/src/flagright/types/case_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/case_management_event.py` & `flagright-1.5.0/src/flagright/types/case_management_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/case_management_event_case_status.py` & `flagright-1.5.0/src/flagright/types/case_management_event_case_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/case_management_event_case_status_reason.py` & `flagright-1.5.0/src/flagright/types/case_management_event_case_status_reason.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/case_opened_details.py` & `flagright-1.5.0/src/flagright/types/case_opened_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/check_delivery_status.py` & `flagright-1.5.0/src/flagright/types/check_delivery_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/check_details.py` & `flagright-1.5.0/src/flagright/types/check_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/company_financial_details.py` & `flagright-1.5.0/src/flagright/types/company_financial_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/company_general_details.py` & `flagright-1.5.0/src/flagright/types/company_general_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/company_registration_details.py` & `flagright-1.5.0/src/flagright/types/company_registration_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/consumer_name.py` & `flagright-1.5.0/src/flagright/types/consumer_name.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/consumer_users_response.py` & `flagright-1.5.0/src/flagright/types/consumer_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/contact_details.py` & `flagright-1.5.0/src/flagright/types/contact_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/country_code.py` & `flagright-1.5.0/src/flagright/types/country_code.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/currency_code.py` & `flagright-1.5.0/src/flagright/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/date.py` & `flagright-1.5.0/src/flagright/types/date.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/device_data.py` & `flagright-1.5.0/src/flagright/types/device_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/employment_status.py` & `flagright-1.5.0/src/flagright/types/employment_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/executed_rules_result.py` & `flagright-1.5.0/src/flagright/types/executed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/failed_rules_result.py` & `flagright-1.5.0/src/flagright/types/failed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/false_positive_details.py` & `flagright-1.5.0/src/flagright/types/false_positive_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/gender.py` & `flagright-1.5.0/src/flagright/types/gender.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/generic_bank_account_details.py` & `flagright-1.5.0/src/flagright/types/generic_bank_account_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .address import Address
+from .country_code import CountryCode
 from .email_id import EmailId
 from .tag import Tag
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
@@ -24,14 +25,15 @@
         alias="accountType", description="Bank account type. E.g. Checking, Savings etc."
     )
     bank_name: typing.Optional[str] = pydantic.Field(alias="bankName", description="Name of the bank")
     bank_code: typing.Optional[str] = pydantic.Field(
         alias="bankCode",
         description="Unique identifier of the bank. In some countries, this can be the same as the bank's SWIFT code",
     )
+    country: typing.Optional[CountryCode]
     name: typing.Optional[str] = pydantic.Field(description="Name of the account holder")
     bank_address: typing.Optional[Address] = pydantic.Field(alias="bankAddress")
     email_id: typing.Optional[EmailId] = pydantic.Field(alias="emailId")
     special_instructions: typing.Optional[str] = pydantic.Field(
         alias="specialInstructions", description="Special instructions to be specified if any"
     )
     payment_channel: typing.Optional[str] = pydantic.Field(alias="paymentChannel")
```

### Comparing `flagright-1.4.9/src/flagright/types/hit_rules_details.py` & `flagright-1.5.0/src/flagright/types/hit_rules_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/iban_details.py` & `flagright-1.5.0/src/flagright/types/iban_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/kyc_status.py` & `flagright-1.5.0/src/flagright/types/transaction_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,44 +2,52 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class KycStatus(str, enum.Enum):
-    SUCCESSFUL = "SUCCESSFUL"
-    FAILED = "FAILED"
-    NOT_STARTED = "NOT_STARTED"
-    IN_PROGRESS = "IN_PROGRESS"
+class TransactionState(str, enum.Enum):
+    """
+    Model for transaction states. E.g. Processing, Refunded, Successful etc.
+    """
+
+    CREATED = "CREATED"
+    PROCESSING = "PROCESSING"
+    SENT = "SENT"
     EXPIRED = "EXPIRED"
-    NEW = "NEW"
-    CANCELLED = "CANCELLED"
-    MANUAL_REVIEW = "MANUAL_REVIEW"
+    DECLINED = "DECLINED"
+    SUSPENDED = "SUSPENDED"
+    REFUNDED = "REFUNDED"
+    SUCCESSFUL = "SUCCESSFUL"
+    REVERSED = "REVERSED"
 
     def visit(
         self,
-        successful: typing.Callable[[], T_Result],
-        failed: typing.Callable[[], T_Result],
-        not_started: typing.Callable[[], T_Result],
-        in_progress: typing.Callable[[], T_Result],
+        created: typing.Callable[[], T_Result],
+        processing: typing.Callable[[], T_Result],
+        sent: typing.Callable[[], T_Result],
         expired: typing.Callable[[], T_Result],
-        new: typing.Callable[[], T_Result],
-        cancelled: typing.Callable[[], T_Result],
-        manual_review: typing.Callable[[], T_Result],
+        declined: typing.Callable[[], T_Result],
+        suspended: typing.Callable[[], T_Result],
+        refunded: typing.Callable[[], T_Result],
+        successful: typing.Callable[[], T_Result],
+        reversed: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is KycStatus.SUCCESSFUL:
-            return successful()
-        if self is KycStatus.FAILED:
-            return failed()
-        if self is KycStatus.NOT_STARTED:
-            return not_started()
-        if self is KycStatus.IN_PROGRESS:
-            return in_progress()
-        if self is KycStatus.EXPIRED:
+        if self is TransactionState.CREATED:
+            return created()
+        if self is TransactionState.PROCESSING:
+            return processing()
+        if self is TransactionState.SENT:
+            return sent()
+        if self is TransactionState.EXPIRED:
             return expired()
-        if self is KycStatus.NEW:
-            return new()
-        if self is KycStatus.CANCELLED:
-            return cancelled()
-        if self is KycStatus.MANUAL_REVIEW:
-            return manual_review()
+        if self is TransactionState.DECLINED:
+            return declined()
+        if self is TransactionState.SUSPENDED:
+            return suspended()
+        if self is TransactionState.REFUNDED:
+            return refunded()
+        if self is TransactionState.SUCCESSFUL:
+            return successful()
+        if self is TransactionState.REVERSED:
+            return reversed()
```

### Comparing `flagright-1.4.9/src/flagright/types/kyc_status_details.py` & `flagright-1.5.0/src/flagright/types/kyc_status_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/legal_document.py` & `flagright-1.5.0/src/flagright/types/legal_document.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/legal_entity.py` & `flagright-1.5.0/src/flagright/types/legal_entity.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_data.py` & `flagright-1.5.0/src/flagright/types/list_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_existed.py` & `flagright-1.5.0/src/flagright/types/list_existed.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_header.py` & `flagright-1.5.0/src/flagright/types/list_header.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_item.py` & `flagright-1.5.0/src/flagright/types/list_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_metadata.py` & `flagright-1.5.0/src/flagright/types/list_metadata.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_subtype.py` & `flagright-1.5.0/src/flagright/types/list_subtype.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/list_type.py` & `flagright-1.5.0/src/flagright/types/list_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/mcc_details.py` & `flagright-1.5.0/src/flagright/types/mcc_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/mpesa_details.py` & `flagright-1.5.0/src/flagright/types/mpesa_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/mpesa_transaction_type.py` & `flagright-1.5.0/src/flagright/types/mpesa_transaction_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/payment_method.py` & `flagright-1.5.0/src/flagright/types/payment_method.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/pep_status.py` & `flagright-1.5.0/src/flagright/types/pep_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/person.py` & `flagright-1.5.0/src/flagright/types/person.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/risk_level.py` & `flagright-1.5.0/src/flagright/types/risk_level.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/rule_action.py` & `flagright-1.5.0/src/flagright/types/rule_action.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/rule_failure_exception.py` & `flagright-1.5.0/src/flagright/types/rule_failure_exception.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/rule_hit_meta.py` & `flagright-1.5.0/src/flagright/types/rule_hit_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """
     Details of rule execution, for internal purposes only
     """
 
     hit_directions: typing.Optional[typing.List[RuleHitDirection]] = pydantic.Field(alias="hitDirections")
     false_positive_details: typing.Optional[FalsePositiveDetails] = pydantic.Field(alias="falsePositiveDetails")
     sanctions_details: typing.Optional[typing.List[SanctionsDetails]] = pydantic.Field(alias="sanctionsDetails")
+    is_ongoing_screening_hit: typing.Optional[bool] = pydantic.Field(alias="isOngoingScreeningHit")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/rule_labels.py` & `flagright-1.5.0/src/flagright/types/rule_labels.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/rule_nature.py` & `flagright-1.5.0/src/flagright/types/rule_nature.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/rules_results.py` & `flagright-1.5.0/src/flagright/types/rules_results.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/sanctions_details.py` & `flagright-1.5.0/src/flagright/types/sanctions_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/sanctions_details_entity_type.py` & `flagright-1.5.0/src/flagright/types/sanctions_details_entity_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/source_of_funds.py` & `flagright-1.5.0/src/flagright/types/source_of_funds.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/swift_details.py` & `flagright-1.5.0/src/flagright/types/swift_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/tag.py` & `flagright-1.5.0/src/flagright/types/tag.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction.py` & `flagright-1.5.0/src/flagright/types/transaction.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_amount_details.py` & `flagright-1.5.0/src/flagright/types/transaction_amount_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_amount_limit.py` & `flagright-1.5.0/src/flagright/types/transaction_amount_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_base.py` & `flagright-1.5.0/src/flagright/types/transaction_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_count_limit.py` & `flagright-1.5.0/src/flagright/types/transaction_count_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_event.py` & `flagright-1.5.0/src/flagright/types/transaction_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_event_monitoring_result.py` & `flagright-1.5.0/src/flagright/types/transaction_event_monitoring_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .rules_results import RulesResults
 from .transaction import Transaction
+from .transaction_risk_scoring_result import TransactionRiskScoringResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class TransactionEventMonitoringResult(RulesResults):
     event_id: str = pydantic.Field(alias="eventId")
     transaction: Transaction
+    risk_score_details: typing.Optional[TransactionRiskScoringResult] = pydantic.Field(alias="riskScoreDetails")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/transaction_limit.py` & `flagright-1.5.0/src/flagright/types/transaction_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_limits.py` & `flagright-1.5.0/src/flagright/types/transaction_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_limits_payment_method_limits.py` & `flagright-1.5.0/src/flagright/types/transaction_limits_payment_method_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_monitoring_result.py` & `flagright-1.5.0/src/flagright/types/user_state_details.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .rule_action import RuleAction
-from .rules_results import RulesResults
-from .transaction_risk_scoring_result import TransactionRiskScoringResult
+from .user_state import UserState
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TransactionMonitoringResult(RulesResults):
-    transaction_id: str = pydantic.Field(
-        alias="transactionId", description="Transaction ID that the results pertain to"
-    )
-    status: RuleAction
-    risk_score_details: typing.Optional[TransactionRiskScoringResult] = pydantic.Field(alias="riskScoreDetails")
+class UserStateDetails(pydantic.BaseModel):
+    user_id: typing.Optional[str] = pydantic.Field(alias="userId")
+    reason: typing.Optional[str]
+    state: UserState
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/transaction_risk_scoring_result.py` & `flagright-1.5.0/src/flagright/types/transaction_risk_scoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_state.py` & `flagright-1.5.0/src/flagright/types/transaction_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,52 +2,36 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class TransactionState(str, enum.Enum):
-    """
-    Model for transaction states. E.g. Processing, Refunded, Successful etc.
-    """
-
-    CREATED = "CREATED"
-    PROCESSING = "PROCESSING"
-    SENT = "SENT"
-    EXPIRED = "EXPIRED"
-    DECLINED = "DECLINED"
-    SUSPENDED = "SUSPENDED"
-    REFUNDED = "REFUNDED"
-    SUCCESSFUL = "SUCCESSFUL"
-    REVERSED = "REVERSED"
+class TransactionType(str, enum.Enum):
+    DEPOSIT = "DEPOSIT"
+    TRANSFER = "TRANSFER"
+    EXTERNAL_PAYMENT = "EXTERNAL_PAYMENT"
+    WITHDRAWAL = "WITHDRAWAL"
+    REFUND = "REFUND"
+    OTHER = "OTHER"
 
     def visit(
         self,
-        created: typing.Callable[[], T_Result],
-        processing: typing.Callable[[], T_Result],
-        sent: typing.Callable[[], T_Result],
-        expired: typing.Callable[[], T_Result],
-        declined: typing.Callable[[], T_Result],
-        suspended: typing.Callable[[], T_Result],
-        refunded: typing.Callable[[], T_Result],
-        successful: typing.Callable[[], T_Result],
-        reversed: typing.Callable[[], T_Result],
+        deposit: typing.Callable[[], T_Result],
+        transfer: typing.Callable[[], T_Result],
+        external_payment: typing.Callable[[], T_Result],
+        withdrawal: typing.Callable[[], T_Result],
+        refund: typing.Callable[[], T_Result],
+        other: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is TransactionState.CREATED:
-            return created()
-        if self is TransactionState.PROCESSING:
-            return processing()
-        if self is TransactionState.SENT:
-            return sent()
-        if self is TransactionState.EXPIRED:
-            return expired()
-        if self is TransactionState.DECLINED:
-            return declined()
-        if self is TransactionState.SUSPENDED:
-            return suspended()
-        if self is TransactionState.REFUNDED:
-            return refunded()
-        if self is TransactionState.SUCCESSFUL:
-            return successful()
-        if self is TransactionState.REVERSED:
-            return reversed()
+        if self is TransactionType.DEPOSIT:
+            return deposit()
+        if self is TransactionType.TRANSFER:
+            return transfer()
+        if self is TransactionType.EXTERNAL_PAYMENT:
+            return external_payment()
+        if self is TransactionType.WITHDRAWAL:
+            return withdrawal()
+        if self is TransactionType.REFUND:
+            return refund()
+        if self is TransactionType.OTHER:
+            return other()
```

### Comparing `flagright-1.4.9/src/flagright/types/transaction_status_details.py` & `flagright-1.5.0/src/flagright/types/transaction_status_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     import pydantic  # type: ignore
 
 
 class TransactionStatusDetails(pydantic.BaseModel):
     transaction_id: str = pydantic.Field(alias="transactionId")
     reasons: typing.List[str]
     status: RuleAction
+    comment: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/transaction_type.py` & `flagright-1.5.0/src/flagright/types/user_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class TransactionType(str, enum.Enum):
-    DEPOSIT = "DEPOSIT"
-    TRANSFER = "TRANSFER"
-    EXTERNAL_PAYMENT = "EXTERNAL_PAYMENT"
-    WITHDRAWAL = "WITHDRAWAL"
-    REFUND = "REFUND"
-    OTHER = "OTHER"
+class UserState(str, enum.Enum):
+    UNACCEPTABLE = "UNACCEPTABLE"
+    TERMINATED = "TERMINATED"
+    ACTIVE = "ACTIVE"
+    DORMANT = "DORMANT"
+    CREATED = "CREATED"
+    SUSPENDED = "SUSPENDED"
+    BLOCKED = "BLOCKED"
 
     def visit(
         self,
-        deposit: typing.Callable[[], T_Result],
-        transfer: typing.Callable[[], T_Result],
-        external_payment: typing.Callable[[], T_Result],
-        withdrawal: typing.Callable[[], T_Result],
-        refund: typing.Callable[[], T_Result],
-        other: typing.Callable[[], T_Result],
+        unacceptable: typing.Callable[[], T_Result],
+        terminated: typing.Callable[[], T_Result],
+        active: typing.Callable[[], T_Result],
+        dormant: typing.Callable[[], T_Result],
+        created: typing.Callable[[], T_Result],
+        suspended: typing.Callable[[], T_Result],
+        blocked: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is TransactionType.DEPOSIT:
-            return deposit()
-        if self is TransactionType.TRANSFER:
-            return transfer()
-        if self is TransactionType.EXTERNAL_PAYMENT:
-            return external_payment()
-        if self is TransactionType.WITHDRAWAL:
-            return withdrawal()
-        if self is TransactionType.REFUND:
-            return refund()
-        if self is TransactionType.OTHER:
-            return other()
+        if self is UserState.UNACCEPTABLE:
+            return unacceptable()
+        if self is UserState.TERMINATED:
+            return terminated()
+        if self is UserState.ACTIVE:
+            return active()
+        if self is UserState.DORMANT:
+            return dormant()
+        if self is UserState.CREATED:
+            return created()
+        if self is UserState.SUSPENDED:
+            return suspended()
+        if self is UserState.BLOCKED:
+            return blocked()
```

### Comparing `flagright-1.4.9/src/flagright/types/transaction_updatable.py` & `flagright-1.5.0/src/flagright/types/transaction_updatable.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_updatable_destination_payment_details.py` & `flagright-1.5.0/src/flagright/types/transaction_updatable_destination_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_updatable_origin_payment_details.py` & `flagright-1.5.0/src/flagright/types/transaction_updatable_origin_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/transaction_with_rules_result.py` & `flagright-1.5.0/src/flagright/types/transaction_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/upi_details.py` & `flagright-1.5.0/src/flagright/types/upi_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user.py` & `flagright-1.5.0/src/flagright/types/user.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_base.py` & `flagright-1.5.0/src/flagright/types/user_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_details.py` & `flagright-1.5.0/src/flagright/types/user_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_optional.py` & `flagright-1.5.0/src/flagright/types/user_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_registration_status.py` & `flagright-1.5.0/src/flagright/types/user_registration_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_response.py` & `flagright-1.5.0/src/flagright/types/business_with_rules_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .business import Business
+from .executed_rules_result import ExecutedRulesResult
+from .hit_rules_details import HitRulesDetails
 from .user_risk_score_details import UserRiskScoreDetails
-from .user_with_rules_result import UserWithRulesResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserResponse(UserWithRulesResult):
+class BusinessWithRulesResult(Business):
+    """
+    Model for business payload with rules result
+    """
+
+    executed_rules: typing.Optional[typing.List[ExecutedRulesResult]] = pydantic.Field(alias="executedRules")
+    hit_rules: typing.Optional[typing.List[HitRulesDetails]] = pydantic.Field(alias="hitRules")
     risk_score_details: typing.Optional[UserRiskScoreDetails] = pydantic.Field(alias="riskScoreDetails")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flagright-1.4.9/src/flagright/types/user_risk_score_details.py` & `flagright-1.5.0/src/flagright/types/user_risk_score_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/user_state_details.py` & `flagright-1.5.0/src/flagright/types/webhook_event_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .user_state import UserState
+from .webhook_event_base_triggered_by import WebhookEventBaseTriggeredBy
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserStateDetails(pydantic.BaseModel):
-    user_id: typing.Optional[str] = pydantic.Field(alias="userId")
-    reason: typing.Optional[str]
-    state: UserState
+class WebhookEventBase(pydantic.BaseModel):
+    id: str = pydantic.Field(description="Unique identifier for the event")
+    triggered_by: WebhookEventBaseTriggeredBy = pydantic.Field(
+        alias="triggeredBy", description="Event triggered by a user or system"
+    )
+    created_timestamp: float = pydantic.Field(
+        alias="createdTimestamp",
+        description="Time at which the event was created. Measured in ms since the Unix epoch.",
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.4.9/src/flagright/types/wallet_details.py` & `flagright-1.5.0/src/flagright/types/wallet_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/webhook_event.py` & `flagright-1.5.0/src/flagright/types/webhook_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/webhook_event_base.py` & `flagright-1.5.0/src/flagright/types/business_user_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .webhook_event_base_triggered_by import WebhookEventBaseTriggeredBy
+from .business_optional import BusinessOptional
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WebhookEventBase(pydantic.BaseModel):
-    id: str = pydantic.Field(description="Unique identifier for the event")
-    triggered_by: WebhookEventBaseTriggeredBy = pydantic.Field(
-        alias="triggeredBy", description="Event triggered by a user or system"
-    )
-    created_timestamp: float = pydantic.Field(
-        alias="createdTimestamp",
-        description="Time at which the event was created. Measured in ms since the Unix epoch.",
+class BusinessUserEvent(pydantic.BaseModel):
+    """
+    Model for business user-related events
+    """
+
+    timestamp: float = pydantic.Field(description="Timestamp of the event")
+    user_id: str = pydantic.Field(alias="userId", description="Transaction ID the event pertains to")
+    event_id: typing.Optional[str] = pydantic.Field(alias="eventId", description="Unique event ID")
+    reason: typing.Optional[str] = pydantic.Field(description="Reason for the event or a state change")
+    event_description: typing.Optional[str] = pydantic.Field(alias="eventDescription", description="Event description")
+    updated_business_user_attributes: typing.Optional[BusinessOptional] = pydantic.Field(
+        alias="updatedBusinessUserAttributes"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flagright-1.4.9/src/flagright/types/webhook_event_base_triggered_by.py` & `flagright-1.5.0/src/flagright/types/webhook_event_base_triggered_by.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/webhook_event_data.py` & `flagright-1.5.0/src/flagright/types/webhook_event_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/src/flagright/types/webhook_event_type.py` & `flagright-1.5.0/src/flagright/types/webhook_event_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.4.9/PKG-INFO` & `flagright-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagright
-Version: 1.4.9
+Version: 1.5.0
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

