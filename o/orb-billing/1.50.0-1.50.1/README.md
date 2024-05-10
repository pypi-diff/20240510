# Comparing `tmp/orb_billing-1.50.0.tar.gz` & `tmp/orb_billing-1.50.1.tar.gz`

## Comparing `orb_billing-1.50.0.tar` & `orb_billing-1.50.1.tar`

### file list

```diff
@@ -1,187 +1,184 @@
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/__init__.py
--rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_base_client.py
--rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_constants.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_files.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_legacy_response.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_qs.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_resource.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_response.py
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_streaming.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_version.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/lib/.keep
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/__init__.py
--rw-r--r--   0        0        0    48439 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/alerts.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/credit_notes.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/invoice_line_items.py
--rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/invoices.py
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/items.py
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/metrics.py
--rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/subscriptions.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/top_level.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/webhooks.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/coupons/__init__.py
--rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/coupons/coupons.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/coupons/subscriptions.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/__init__.py
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/balance_transactions.py
--rw-r--r--   0        0        0    44927 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/costs.py
--rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/customers.py
--rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/usage.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/credits/__init__.py
--rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/credits/credits.py
--rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/credits/ledger.py
--rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/customers/credits/top_ups.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/events/__init__.py
--rw-r--r--   0        0        0    27956 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/events/backfills.py
--rw-r--r--   0        0        0    52976 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/events/events.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/plans/__init__.py
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/plans/external_plan_id.py
--rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/plans/plans.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/prices/__init__.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/prices/external_price_id.py
--rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/resources/prices/prices.py
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_create_for_customer_params.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_create_for_external_customer_params.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_create_for_plan_params.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_create_for_subscription_params.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_disable_params.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_enable_params.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/alert_list_params.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/coupon.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/coupon_create_params.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/coupon_list_params.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/credit_note.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/credit_note_list_params.py
--rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customer.py
--rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customer_create_params.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customer_list_params.py
--rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customer_update_by_external_id_params.py
--rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customer_update_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/evaluate_price_group.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_deprecate_response.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_ingest_params.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_ingest_response.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_search_params.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_search_response.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_update_params.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/event_update_response.py
--rw-r--r--   0        0        0    38015 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_create_params.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_fetch_upcoming_params.py
--rw-r--r--   0        0        0    38056 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_fetch_upcoming_response.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_line_item_create_params.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_line_item_create_response.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_list_params.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/invoice_mark_paid_params.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/item.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/item_create_params.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/item_list_params.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/metric_create_params.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/metric_create_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/metric_fetch_response.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/metric_list_params.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/metric_list_response.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plan.py
--rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plan_create_params.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plan_list_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plan_update_params.py
--rw-r--r--   0        0        0    36435 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/price.py
--rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/price_create_params.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/price_evaluate_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/price_evaluate_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/price_list_params.py
--rw-r--r--   0        0        0    16883 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_cancel_params.py
--rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_create_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_fetch_costs_params.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_fetch_costs_response.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_fetch_schedule_params.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_fetch_schedule_response.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_fetch_usage_params.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_list_params.py
--rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_price_intervals_params.py
--rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_schedule_plan_change_params.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_trigger_phase_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_update_params.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscription_usage.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/subscriptions.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/top_level_ping_response.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/beta/evaluate_price_group.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/beta/price_evaluate_params.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/beta/price_evaluate_response.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/coupons/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/coupons/subscription_list_params.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/balance_transaction_create_params.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/balance_transaction_create_response.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/balance_transaction_list_params.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/balance_transaction_list_response.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/cost_list_by_external_id_params.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/cost_list_by_external_id_response.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/cost_list_params.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/cost_list_response.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credit_list_by_external_id_params.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credit_list_by_external_id_response.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credit_list_params.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credit_list_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/usage_update_by_external_id_params.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/usage_update_by_external_id_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/usage_update_params.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/usage_update_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/__init__.py
--rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_params.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_response.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_params.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_response.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_params.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_params.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_response.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_close_response.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_create_params.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_create_response.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_fetch_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_list_params.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_list_response.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/events/backfill_revert_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plans/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/plans/external_plan_id_update_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/prices/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared/billing_cycle_relative_date.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared/discount.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared/pagination_metadata.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared_params/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.50.0/src/orb/types/shared_params/billing_cycle_relative_date.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.50.0/.gitignore
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.50.0/LICENSE
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.50.0/pyproject.toml
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.50.0/PKG-INFO
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/__init__.py
+-rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_base_client.py
+-rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_constants.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_files.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_legacy_response.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_qs.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_resource.py
+-rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_response.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_streaming.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_version.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/lib/.keep
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/__init__.py
+-rw-r--r--   0        0        0    38318 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/alerts.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/credit_notes.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/invoice_line_items.py
+-rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/invoices.py
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/items.py
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/metrics.py
+-rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/subscriptions.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/top_level.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/webhooks.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/__init__.py
+-rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/coupons.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/coupons/subscriptions.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/__init__.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/balance_transactions.py
+-rw-r--r--   0        0        0    44995 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/costs.py
+-rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/customers.py
+-rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/usage.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/__init__.py
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/credits.py
+-rw-r--r--   0        0        0   203726 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/ledger.py
+-rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/customers/credits/top_ups.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/__init__.py
+-rw-r--r--   0        0        0    28366 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/backfills.py
+-rw-r--r--   0        0        0    53314 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/events/events.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/__init__.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/external_plan_id.py
+-rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/plans/plans.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/__init__.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/external_price_id.py
+-rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/resources/prices/prices.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_customer_params.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_external_customer_params.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_create_for_subscription_params.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/alert_list_params.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon_create_params.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupon_list_params.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/credit_note.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/credit_note_list_params.py
+-rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer.py
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_create_params.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_list_params.py
+-rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_update_by_external_id_params.py
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customer_update_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/evaluate_price_group.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_deprecate_response.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_ingest_params.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_ingest_response.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_search_params.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_search_response.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_update_params.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/event_update_response.py
+-rw-r--r--   0        0        0    38126 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_create_params.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_params.py
+-rw-r--r--   0        0        0    38167 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_response.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_line_item_create_params.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_line_item_create_response.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_list_params.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/invoice_mark_paid_params.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item_create_params.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/item_list_params.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_create_params.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_create_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_fetch_response.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_list_params.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/metric_list_response.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan.py
+-rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_create_params.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_list_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plan_update_params.py
+-rw-r--r--   0        0        0    36618 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price.py
+-rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_create_params.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_evaluate_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_evaluate_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/price_list_params.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_cancel_params.py
+-rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_create_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_params.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_response.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_params.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_response.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_fetch_usage_params.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_list_params.py
+-rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_price_intervals_params.py
+-rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_schedule_plan_change_params.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_trigger_phase_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_update_params.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscription_usage.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/subscriptions.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/top_level_ping_response.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/evaluate_price_group.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/price_evaluate_params.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/beta/price_evaluate_response.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupons/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/coupons/subscription_list_params.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_params.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_response.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_params.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_response.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_params.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_response.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_params.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/cost_list_response.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_params.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_response.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_params.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credit_list_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_params.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_params.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/usage_update_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/__init__.py
+-rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_params.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_response.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_params.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_response.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_params.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_response.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_params.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_response.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_close_response.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_create_params.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_create_response.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_fetch_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_list_params.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_list_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/events/backfill_revert_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plans/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/plans/external_plan_id_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/prices/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/discount.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared/pagination_metadata.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.50.1/src/orb/types/shared_params/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.50.1/.gitignore
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.50.1/LICENSE
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.50.1/pyproject.toml
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.50.1/PKG-INFO
```

### Comparing `orb_billing-1.50.0/src/orb/__init__.py` & `orb_billing-1.50.1/src/orb/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_base_client.py` & `orb_billing-1.50.1/src/orb/_base_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_client.py` & `orb_billing-1.50.1/src/orb/_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_compat.py` & `orb_billing-1.50.1/src/orb/_compat.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_exceptions.py` & `orb_billing-1.50.1/src/orb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_files.py` & `orb_billing-1.50.1/src/orb/_files.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_legacy_response.py` & `orb_billing-1.50.1/src/orb/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_models.py` & `orb_billing-1.50.1/src/orb/_models.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_qs.py` & `orb_billing-1.50.1/src/orb/_qs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_resource.py` & `orb_billing-1.50.1/src/orb/_resource.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_response.py` & `orb_billing-1.50.1/src/orb/_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_streaming.py` & `orb_billing-1.50.1/src/orb/_streaming.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_types.py` & `orb_billing-1.50.1/src/orb/_types.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/pagination.py` & `orb_billing-1.50.1/src/orb/pagination.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/__init__.py` & `orb_billing-1.50.1/src/orb/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_logs.py` & `orb_billing-1.50.1/src/orb/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_proxy.py` & `orb_billing-1.50.1/src/orb/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_sync.py` & `orb_billing-1.50.1/src/orb/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_transform.py` & `orb_billing-1.50.1/src/orb/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_typing.py` & `orb_billing-1.50.1/src/orb/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/_utils/_utils.py` & `orb_billing-1.50.1/src/orb/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/__init__.py` & `orb_billing-1.50.1/src/orb/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/alerts.py` & `orb_billing-1.50.1/src/orb/resources/alerts.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from datetime import datetime
 
 import httpx
 
 from .. import _legacy_response
 from ..types import (
     alert_list_params,
-    alert_enable_params,
-    alert_disable_params,
-    alert_create_for_plan_params,
     alert_create_for_customer_params,
     alert_create_for_subscription_params,
     alert_create_for_external_customer_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
@@ -84,52 +81,45 @@
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         customer_id: Optional[str] | NotGiven = NOT_GIVEN,
         external_customer_id: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        plan_id: Optional[str] | NotGiven = NOT_GIVEN,
-        plan_version: Optional[int] | NotGiven = NOT_GIVEN,
         subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Alert]:
         """
-        This endpoint returns a list of all
-        [`alerts`](https://docs.withorb.com/guides/product-catalog/configuring-alerts).
+        This endpoint returns a list of alerts within Orb.
 
-        The list of alerts is ordered starting from the most recently created alert.
-        This endpoint follows Orb's
-        [standardized pagination format](../reference/pagination).
-
-        The request must specify one of customer_id, external_customer_id,
-        subscription_id, or plan_id
+        The request must specify one of `customer_id`, `external_customer_id`, or
+        `subscription_id`.
 
         If querying by subscripion_id, the endpoint will return the subscription level
         alerts as well as the plan level alerts associated with the subscription.
 
+        The list of alerts is ordered starting from the most recently created alert.
+        This endpoint follows Orb's
+        [standardized pagination format](../reference/pagination).
+
         Args:
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           customer_id: Fetch alerts scoped to this customer_id
 
           external_customer_id: Fetch alerts scoped to this external_customer_id
 
           limit: The number of items to fetch. Defaults to 20.
 
-          plan_id: Fetch alerts scoped to this plan_id
-
-          plan_version: If provided alongside plan_id, only the alerts that are scoped to the specified plan_version will be returned.
-
           subscription_id: Fetch alerts scoped to this subscription_id
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -150,16 +140,14 @@
                         "created_at_gte": created_at_gte,
                         "created_at_lt": created_at_lt,
                         "created_at_lte": created_at_lte,
                         "cursor": cursor,
                         "customer_id": customer_id,
                         "external_customer_id": external_customer_id,
                         "limit": limit,
-                        "plan_id": plan_id,
-                        "plan_version": plan_version,
                         "subscription_id": subscription_id,
                     },
                     alert_list_params.AlertListParams,
                 ),
             ),
             model=Alert,
         )
@@ -294,87 +282,14 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Alert,
         )
 
-    def create_for_plan(
-        self,
-        plan_id: str,
-        *,
-        thresholds: Iterable[alert_create_for_plan_params.Threshold],
-        type: str,
-        metric_id: Optional[str] | NotGiven = NOT_GIVEN,
-        plan_version: Optional[int] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-        idempotency_key: str | None = None,
-    ) -> Alert:
-        """This endpoint is used to create alerts at the plan level.
-
-        Plan level alerts are
-        automatically propagated to all subscriptions associated with the plan. These
-        alerts are scoped to a specific plan version; if no version is specified, the
-        active plan version is used.
-
-        Plan level alerts can be of two types: `usage_exceeded` or `cost_exceeded`. A
-        `usage_exceeded` alert is scoped to a particular metric and is triggered when
-        the usage of that metric exceeds a predefined thresholds during the current
-        invoice cycle. A `cost_exceeded` alert is triggered when the total cost of the
-        subscription on the plan surpasses predefined thresholds in the current invoice
-        cycle.Each plan can have one `cost_exceeded` alert and one `usage_exceeded`
-        alert per metric that is apart of the plan.
-
-        Args:
-          thresholds: The thresholds for the alert.
-
-          type: The thresholds that define the values at which the alert will be triggered.
-
-          metric_id: The metric to track usage for.
-
-          plan_version: The plan version to create alerts for. If not specified, the default will be the plan's active plan version.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        if not plan_id:
-            raise ValueError(f"Expected a non-empty value for `plan_id` but received {plan_id!r}")
-        return self._post(
-            f"/alerts/plan_id/{plan_id}",
-            body=maybe_transform(
-                {
-                    "thresholds": thresholds,
-                    "type": type,
-                    "metric_id": metric_id,
-                    "plan_version": plan_version,
-                },
-                alert_create_for_plan_params.AlertCreateForPlanParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=Alert,
-        )
-
     def create_for_subscription(
         self,
         subscription_id: str,
         *,
         thresholds: Iterable[alert_create_for_subscription_params.Threshold],
         type: str,
         metric_id: Optional[str] | NotGiven = NOT_GIVEN,
@@ -387,21 +302,21 @@
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint is used to create alerts at the subscription level.
 
         Subscription level alerts can be one of two types: `usage_exceeded` or
         `cost_exceeded`. A `usage_exceeded` alert is scoped to a particular metric and
-        is triggered when the usage of that metric exceeds a predefined thresholds
-        during the current invoice cycle. A `cost_exceeded` alert is triggered when the
-        total cost of the subscription surpasses predefined thresholds in the current
-        invoice cycle. Each subscription can have one `cost_exceeded` alert and one
-        `usage_exceeded` alert per metric that is apart of the subscription. Alerts are
-        triggered based on usage or cost conditions met during the current invoice
-        cycle.
+        is triggered when the usage of that metric exceeds predefined thresholds during
+        the current billing cycle. A `cost_exceeded` alert is triggered when the total
+        amount due during the current billing cycle surpasses predefined thresholds.
+        `cost_exceeded` alerts do not include burndown of pre-purchase credits. Each
+        subscription can have one `cost_exceeded` alert and one `usage_exceeded` alert
+        per metric that is a part of the subscription. Alerts are triggered based on
+        usage or cost conditions met during the current billing cycle.
 
         Args:
           thresholds: The thresholds for the alert.
 
           type: The thresholds that define the values at which the alert will be triggered.
 
           metric_id: The metric to track usage for.
@@ -438,34 +353,26 @@
             cast_to=Alert,
         )
 
     def disable(
         self,
         alert_configuration_id: str,
         *,
-        subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint can be used to disable an alert.
 
-        By default, disabling a plan level alert will apply to all subscriptions on that
-        plan. In order to toggle a plan level alert for a specific subscription, the
-        client must provide the plan level alert id as well as the subscription_id
-        parameter.
-
         Args:
-          subscription_id: Used to update the status of a plan alert scoped to this subscription_id
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -480,43 +387,34 @@
             f"/alerts/{alert_configuration_id}/disable",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
-                query=maybe_transform({"subscription_id": subscription_id}, alert_disable_params.AlertDisableParams),
             ),
             cast_to=Alert,
         )
 
     def enable(
         self,
         alert_configuration_id: str,
         *,
-        subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint can be used to enable an alert.
 
-        By default, enabling a plan level alert will apply to all subscriptions on that
-        plan. In order to toggle a plan level alert for a specific subscription, the
-        client must provide the plan level alert id as well as the subscription_id
-        parameter.
-
         Args:
-          subscription_id: Used to update the status of a plan alert scoped to this subscription_id
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -531,15 +429,14 @@
             f"/alerts/{alert_configuration_id}/enable",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
-                query=maybe_transform({"subscription_id": subscription_id}, alert_enable_params.AlertEnableParams),
             ),
             cast_to=Alert,
         )
 
 
 class AsyncAlerts(AsyncAPIResource):
     @cached_property
@@ -590,52 +487,45 @@
         created_at_gte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lt: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         created_at_lte: Union[str, datetime, None] | NotGiven = NOT_GIVEN,
         cursor: Optional[str] | NotGiven = NOT_GIVEN,
         customer_id: Optional[str] | NotGiven = NOT_GIVEN,
         external_customer_id: Optional[str] | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        plan_id: Optional[str] | NotGiven = NOT_GIVEN,
-        plan_version: Optional[int] | NotGiven = NOT_GIVEN,
         subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Alert, AsyncPage[Alert]]:
         """
-        This endpoint returns a list of all
-        [`alerts`](https://docs.withorb.com/guides/product-catalog/configuring-alerts).
-
-        The list of alerts is ordered starting from the most recently created alert.
-        This endpoint follows Orb's
-        [standardized pagination format](../reference/pagination).
+        This endpoint returns a list of alerts within Orb.
 
-        The request must specify one of customer_id, external_customer_id,
-        subscription_id, or plan_id
+        The request must specify one of `customer_id`, `external_customer_id`, or
+        `subscription_id`.
 
         If querying by subscripion_id, the endpoint will return the subscription level
         alerts as well as the plan level alerts associated with the subscription.
 
+        The list of alerts is ordered starting from the most recently created alert.
+        This endpoint follows Orb's
+        [standardized pagination format](../reference/pagination).
+
         Args:
           cursor: Cursor for pagination. This can be populated by the `next_cursor` value returned
               from the initial request.
 
           customer_id: Fetch alerts scoped to this customer_id
 
           external_customer_id: Fetch alerts scoped to this external_customer_id
 
           limit: The number of items to fetch. Defaults to 20.
 
-          plan_id: Fetch alerts scoped to this plan_id
-
-          plan_version: If provided alongside plan_id, only the alerts that are scoped to the specified plan_version will be returned.
-
           subscription_id: Fetch alerts scoped to this subscription_id
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -656,16 +546,14 @@
                         "created_at_gte": created_at_gte,
                         "created_at_lt": created_at_lt,
                         "created_at_lte": created_at_lte,
                         "cursor": cursor,
                         "customer_id": customer_id,
                         "external_customer_id": external_customer_id,
                         "limit": limit,
-                        "plan_id": plan_id,
-                        "plan_version": plan_version,
                         "subscription_id": subscription_id,
                     },
                     alert_list_params.AlertListParams,
                 ),
             ),
             model=Alert,
         )
@@ -800,87 +688,14 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Alert,
         )
 
-    async def create_for_plan(
-        self,
-        plan_id: str,
-        *,
-        thresholds: Iterable[alert_create_for_plan_params.Threshold],
-        type: str,
-        metric_id: Optional[str] | NotGiven = NOT_GIVEN,
-        plan_version: Optional[int] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-        idempotency_key: str | None = None,
-    ) -> Alert:
-        """This endpoint is used to create alerts at the plan level.
-
-        Plan level alerts are
-        automatically propagated to all subscriptions associated with the plan. These
-        alerts are scoped to a specific plan version; if no version is specified, the
-        active plan version is used.
-
-        Plan level alerts can be of two types: `usage_exceeded` or `cost_exceeded`. A
-        `usage_exceeded` alert is scoped to a particular metric and is triggered when
-        the usage of that metric exceeds a predefined thresholds during the current
-        invoice cycle. A `cost_exceeded` alert is triggered when the total cost of the
-        subscription on the plan surpasses predefined thresholds in the current invoice
-        cycle.Each plan can have one `cost_exceeded` alert and one `usage_exceeded`
-        alert per metric that is apart of the plan.
-
-        Args:
-          thresholds: The thresholds for the alert.
-
-          type: The thresholds that define the values at which the alert will be triggered.
-
-          metric_id: The metric to track usage for.
-
-          plan_version: The plan version to create alerts for. If not specified, the default will be the plan's active plan version.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        if not plan_id:
-            raise ValueError(f"Expected a non-empty value for `plan_id` but received {plan_id!r}")
-        return await self._post(
-            f"/alerts/plan_id/{plan_id}",
-            body=await async_maybe_transform(
-                {
-                    "thresholds": thresholds,
-                    "type": type,
-                    "metric_id": metric_id,
-                    "plan_version": plan_version,
-                },
-                alert_create_for_plan_params.AlertCreateForPlanParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=Alert,
-        )
-
     async def create_for_subscription(
         self,
         subscription_id: str,
         *,
         thresholds: Iterable[alert_create_for_subscription_params.Threshold],
         type: str,
         metric_id: Optional[str] | NotGiven = NOT_GIVEN,
@@ -893,21 +708,21 @@
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint is used to create alerts at the subscription level.
 
         Subscription level alerts can be one of two types: `usage_exceeded` or
         `cost_exceeded`. A `usage_exceeded` alert is scoped to a particular metric and
-        is triggered when the usage of that metric exceeds a predefined thresholds
-        during the current invoice cycle. A `cost_exceeded` alert is triggered when the
-        total cost of the subscription surpasses predefined thresholds in the current
-        invoice cycle. Each subscription can have one `cost_exceeded` alert and one
-        `usage_exceeded` alert per metric that is apart of the subscription. Alerts are
-        triggered based on usage or cost conditions met during the current invoice
-        cycle.
+        is triggered when the usage of that metric exceeds predefined thresholds during
+        the current billing cycle. A `cost_exceeded` alert is triggered when the total
+        amount due during the current billing cycle surpasses predefined thresholds.
+        `cost_exceeded` alerts do not include burndown of pre-purchase credits. Each
+        subscription can have one `cost_exceeded` alert and one `usage_exceeded` alert
+        per metric that is a part of the subscription. Alerts are triggered based on
+        usage or cost conditions met during the current billing cycle.
 
         Args:
           thresholds: The thresholds for the alert.
 
           type: The thresholds that define the values at which the alert will be triggered.
 
           metric_id: The metric to track usage for.
@@ -944,34 +759,26 @@
             cast_to=Alert,
         )
 
     async def disable(
         self,
         alert_configuration_id: str,
         *,
-        subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint can be used to disable an alert.
 
-        By default, disabling a plan level alert will apply to all subscriptions on that
-        plan. In order to toggle a plan level alert for a specific subscription, the
-        client must provide the plan level alert id as well as the subscription_id
-        parameter.
-
         Args:
-          subscription_id: Used to update the status of a plan alert scoped to this subscription_id
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -986,45 +793,34 @@
             f"/alerts/{alert_configuration_id}/disable",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
-                query=await async_maybe_transform(
-                    {"subscription_id": subscription_id}, alert_disable_params.AlertDisableParams
-                ),
             ),
             cast_to=Alert,
         )
 
     async def enable(
         self,
         alert_configuration_id: str,
         *,
-        subscription_id: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Alert:
         """
         This endpoint can be used to enable an alert.
 
-        By default, enabling a plan level alert will apply to all subscriptions on that
-        plan. In order to toggle a plan level alert for a specific subscription, the
-        client must provide the plan level alert id as well as the subscription_id
-        parameter.
-
         Args:
-          subscription_id: Used to update the status of a plan alert scoped to this subscription_id
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
@@ -1039,17 +835,14 @@
             f"/alerts/{alert_configuration_id}/enable",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
-                query=await async_maybe_transform(
-                    {"subscription_id": subscription_id}, alert_enable_params.AlertEnableParams
-                ),
             ),
             cast_to=Alert,
         )
 
 
 class AlertsWithRawResponse:
     def __init__(self, alerts: Alerts) -> None:
@@ -1063,17 +856,14 @@
         )
         self.create_for_customer = _legacy_response.to_raw_response_wrapper(
             alerts.create_for_customer,
         )
         self.create_for_external_customer = _legacy_response.to_raw_response_wrapper(
             alerts.create_for_external_customer,
         )
-        self.create_for_plan = _legacy_response.to_raw_response_wrapper(
-            alerts.create_for_plan,
-        )
         self.create_for_subscription = _legacy_response.to_raw_response_wrapper(
             alerts.create_for_subscription,
         )
         self.disable = _legacy_response.to_raw_response_wrapper(
             alerts.disable,
         )
         self.enable = _legacy_response.to_raw_response_wrapper(
@@ -1093,17 +883,14 @@
         )
         self.create_for_customer = _legacy_response.async_to_raw_response_wrapper(
             alerts.create_for_customer,
         )
         self.create_for_external_customer = _legacy_response.async_to_raw_response_wrapper(
             alerts.create_for_external_customer,
         )
-        self.create_for_plan = _legacy_response.async_to_raw_response_wrapper(
-            alerts.create_for_plan,
-        )
         self.create_for_subscription = _legacy_response.async_to_raw_response_wrapper(
             alerts.create_for_subscription,
         )
         self.disable = _legacy_response.async_to_raw_response_wrapper(
             alerts.disable,
         )
         self.enable = _legacy_response.async_to_raw_response_wrapper(
@@ -1123,17 +910,14 @@
         )
         self.create_for_customer = to_streamed_response_wrapper(
             alerts.create_for_customer,
         )
         self.create_for_external_customer = to_streamed_response_wrapper(
             alerts.create_for_external_customer,
         )
-        self.create_for_plan = to_streamed_response_wrapper(
-            alerts.create_for_plan,
-        )
         self.create_for_subscription = to_streamed_response_wrapper(
             alerts.create_for_subscription,
         )
         self.disable = to_streamed_response_wrapper(
             alerts.disable,
         )
         self.enable = to_streamed_response_wrapper(
@@ -1153,17 +937,14 @@
         )
         self.create_for_customer = async_to_streamed_response_wrapper(
             alerts.create_for_customer,
         )
         self.create_for_external_customer = async_to_streamed_response_wrapper(
             alerts.create_for_external_customer,
         )
-        self.create_for_plan = async_to_streamed_response_wrapper(
-            alerts.create_for_plan,
-        )
         self.create_for_subscription = async_to_streamed_response_wrapper(
             alerts.create_for_subscription,
         )
         self.disable = async_to_streamed_response_wrapper(
             alerts.disable,
         )
         self.enable = async_to_streamed_response_wrapper(
```

### Comparing `orb_billing-1.50.0/src/orb/resources/credit_notes.py` & `orb_billing-1.50.1/src/orb/resources/credit_notes.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/invoice_line_items.py` & `orb_billing-1.50.1/src/orb/resources/invoice_line_items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/invoices.py` & `orb_billing-1.50.1/src/orb/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/items.py` & `orb_billing-1.50.1/src/orb/resources/items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/metrics.py` & `orb_billing-1.50.1/src/orb/resources/metrics.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/subscriptions.py` & `orb_billing-1.50.1/src/orb/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/top_level.py` & `orb_billing-1.50.1/src/orb/resources/top_level.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/webhooks.py` & `orb_billing-1.50.1/src/orb/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/coupons/__init__.py` & `orb_billing-1.50.1/src/orb/resources/coupons/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/coupons/coupons.py` & `orb_billing-1.50.1/src/orb/resources/coupons/coupons.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/coupons/subscriptions.py` & `orb_billing-1.50.1/src/orb/resources/coupons/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/__init__.py` & `orb_billing-1.50.1/src/orb/resources/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/balance_transactions.py` & `orb_billing-1.50.1/src/orb/resources/customers/balance_transactions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/costs.py` & `orb_billing-1.50.1/src/orb/resources/customers/costs.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,19 +125,19 @@
         calculated by taking the difference of each timeframe with the last. Note that
         in the above example, the `Total` value would be 0 for the second two data
         points, since the minimum commitment has not yet been hit and each day is not
         contributing anything to the total cost.
 
         ## Timeframe bounds
 
-        If no timeframe bounds are specified, the response will default to the current
-        billing period for the customer's subscription. For subscriptions that have
-        ended, this will be the billing period when they were last active. If the
-        subscription starts or ends within the timeframe, the response will only include
-        windows where the subscription is active.
+        For an active subscription, both timeframes should be specified in the request.
+        If a subscription starts or ends within the timeframe, the response will only
+        include windows where the subscription is active. If a subscription has ended,
+        no timeframe bounds need to be specified and the response will default to the
+        billing period when the subscription was last active.
 
         As noted above, `timeframe_start` for a given cumulative datapoint is always the
         beginning of the billing period, and `timeframe_end` is incremented one day at a
         time to construct the response. When a timeframe is passed in that is not
         aligned to the current subscription's billing period, the response will contain
         cumulative totals from multiple billing periods.
 
@@ -314,19 +314,19 @@
         calculated by taking the difference of each timeframe with the last. Note that
         in the above example, the `Total` value would be 0 for the second two data
         points, since the minimum commitment has not yet been hit and each day is not
         contributing anything to the total cost.
 
         ## Timeframe bounds
 
-        If no timeframe bounds are specified, the response will default to the current
-        billing period for the customer's subscription. For subscriptions that have
-        ended, this will be the billing period when they were last active. If the
-        subscription starts or ends within the timeframe, the response will only include
-        windows where the subscription is active.
+        For an active subscription, both timeframes should be specified in the request.
+        If a subscription starts or ends within the timeframe, the response will only
+        include windows where the subscription is active. If a subscription has ended,
+        no timeframe bounds need to be specified and the response will default to the
+        billing period when the subscription was last active.
 
         As noted above, `timeframe_start` for a given cumulative datapoint is always the
         beginning of the billing period, and `timeframe_end` is incremented one day at a
         time to construct the response. When a timeframe is passed in that is not
         aligned to the current subscription's billing period, the response will contain
         cumulative totals from multiple billing periods.
 
@@ -515,19 +515,19 @@
         calculated by taking the difference of each timeframe with the last. Note that
         in the above example, the `Total` value would be 0 for the second two data
         points, since the minimum commitment has not yet been hit and each day is not
         contributing anything to the total cost.
 
         ## Timeframe bounds
 
-        If no timeframe bounds are specified, the response will default to the current
-        billing period for the customer's subscription. For subscriptions that have
-        ended, this will be the billing period when they were last active. If the
-        subscription starts or ends within the timeframe, the response will only include
-        windows where the subscription is active.
+        For an active subscription, both timeframes should be specified in the request.
+        If a subscription starts or ends within the timeframe, the response will only
+        include windows where the subscription is active. If a subscription has ended,
+        no timeframe bounds need to be specified and the response will default to the
+        billing period when the subscription was last active.
 
         As noted above, `timeframe_start` for a given cumulative datapoint is always the
         beginning of the billing period, and `timeframe_end` is incremented one day at a
         time to construct the response. When a timeframe is passed in that is not
         aligned to the current subscription's billing period, the response will contain
         cumulative totals from multiple billing periods.
 
@@ -704,19 +704,19 @@
         calculated by taking the difference of each timeframe with the last. Note that
         in the above example, the `Total` value would be 0 for the second two data
         points, since the minimum commitment has not yet been hit and each day is not
         contributing anything to the total cost.
 
         ## Timeframe bounds
 
-        If no timeframe bounds are specified, the response will default to the current
-        billing period for the customer's subscription. For subscriptions that have
-        ended, this will be the billing period when they were last active. If the
-        subscription starts or ends within the timeframe, the response will only include
-        windows where the subscription is active.
+        For an active subscription, both timeframes should be specified in the request.
+        If a subscription starts or ends within the timeframe, the response will only
+        include windows where the subscription is active. If a subscription has ended,
+        no timeframe bounds need to be specified and the response will default to the
+        billing period when the subscription was last active.
 
         As noted above, `timeframe_start` for a given cumulative datapoint is always the
         beginning of the billing period, and `timeframe_end` is incremented one day at a
         time to construct the response. When a timeframe is passed in that is not
         aligned to the current subscription's billing period, the response will contain
         cumulative totals from multiple billing periods.
```

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/customers.py` & `orb_billing-1.50.1/src/orb/resources/customers/customers.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/usage.py` & `orb_billing-1.50.1/src/orb/resources/customers/usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/credits/__init__.py` & `orb_billing-1.50.1/src/orb/resources/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/credits/credits.py` & `orb_billing-1.50.1/src/orb/resources/customers/credits/credits.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/credits/ledger.py` & `orb_billing-1.50.1/src/orb/resources/customers/credits/ledger.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/customers/credits/top_ups.py` & `orb_billing-1.50.1/src/orb/resources/customers/credits/top_ups.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/events/__init__.py` & `orb_billing-1.50.1/src/orb/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/events/backfills.py` & `orb_billing-1.50.1/src/orb/resources/events/backfills.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
         closed.
 
         If the `replace_existing_events` is `true`, existing events in the backfill's
         timeframe will be replaced with the newly ingested events associated with the
         backfill. If `false`, newly ingested events will be added to the existing
         events.
 
+        If a `customer_id` or `external_customer_id` is specified, the backfill will
+        only affect events for that customer. If neither is specified, the backfill will
+        affect all customers.
+
         Args:
           timeframe_end: The (exclusive) end of the usage timeframe affected by this backfill.
 
           timeframe_start: The (inclusive) start of the usage timeframe affected by this backfill.
 
           close_time: The time at which no more events will be accepted for this backfill. The
               backfill will automatically begin reflecting throughout Orb at the close time.
@@ -361,14 +365,18 @@
         closed.
 
         If the `replace_existing_events` is `true`, existing events in the backfill's
         timeframe will be replaced with the newly ingested events associated with the
         backfill. If `false`, newly ingested events will be added to the existing
         events.
 
+        If a `customer_id` or `external_customer_id` is specified, the backfill will
+        only affect events for that customer. If neither is specified, the backfill will
+        affect all customers.
+
         Args:
           timeframe_end: The (exclusive) end of the usage timeframe affected by this backfill.
 
           timeframe_start: The (inclusive) start of the usage timeframe affected by this backfill.
 
           close_time: The time at which no more events will be accepted for this backfill. The
               backfill will automatically begin reflecting throughout Orb at the close time.
```

### Comparing `orb_billing-1.50.0/src/orb/resources/events/events.py` & `orb_billing-1.50.1/src/orb/resources/events/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,17 @@
           offset).
 
         ## Idempotency and retry semantics
 
         Orb's idempotency guarantees allow you to implement safe retry logic in the
         event of network or machine failures, ensuring data fidelity. Each event in the
         request payload is associated with an idempotency key, and Orb guarantees that a
-        single idempotency key will be successfully ingested at most once.
+        single idempotency key will be successfully ingested at most once. Note that
+        when Orb encounters events with duplicate idempotency keys and differing event
+        bodies in a batch of events, the entire batch will be rejected.
 
         - Successful responses return a 200 HTTP status code. The response contains
           information about previously processed events.
         - Requests that return a `4xx` HTTP status code indicate a payload error and
           contain at least one event with a validation failure. An event with a
           validation failure can be re-sent to the ingestion endpoint (after the payload
           is fixed) with the original idempotency key since that key is not marked as
@@ -909,15 +911,17 @@
           offset).
 
         ## Idempotency and retry semantics
 
         Orb's idempotency guarantees allow you to implement safe retry logic in the
         event of network or machine failures, ensuring data fidelity. Each event in the
         request payload is associated with an idempotency key, and Orb guarantees that a
-        single idempotency key will be successfully ingested at most once.
+        single idempotency key will be successfully ingested at most once. Note that
+        when Orb encounters events with duplicate idempotency keys and differing event
+        bodies in a batch of events, the entire batch will be rejected.
 
         - Successful responses return a 200 HTTP status code. The response contains
           information about previously processed events.
         - Requests that return a `4xx` HTTP status code indicate a payload error and
           contain at least one event with a validation failure. An event with a
           validation failure can be re-sent to the ingestion endpoint (after the payload
           is fixed) with the original idempotency key since that key is not marked as
```

### Comparing `orb_billing-1.50.0/src/orb/resources/plans/__init__.py` & `orb_billing-1.50.1/src/orb/resources/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/plans/external_plan_id.py` & `orb_billing-1.50.1/src/orb/resources/plans/external_plan_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/plans/plans.py` & `orb_billing-1.50.1/src/orb/resources/plans/plans.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/prices/__init__.py` & `orb_billing-1.50.1/src/orb/resources/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/prices/external_price_id.py` & `orb_billing-1.50.1/src/orb/resources/prices/external_price_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/resources/prices/prices.py` & `orb_billing-1.50.1/src/orb/resources/prices/prices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/__init__.py` & `orb_billing-1.50.1/src/orb/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,19 @@
 from .price_list_params import PriceListParams as PriceListParams
 from .coupon_list_params import CouponListParams as CouponListParams
 from .item_create_params import ItemCreateParams as ItemCreateParams
 from .metric_list_params import MetricListParams as MetricListParams
 from .plan_create_params import PlanCreateParams as PlanCreateParams
 from .plan_update_params import PlanUpdateParams as PlanUpdateParams
 from .subscription_usage import SubscriptionUsage as SubscriptionUsage
-from .alert_enable_params import AlertEnableParams as AlertEnableParams
 from .event_ingest_params import EventIngestParams as EventIngestParams
 from .event_search_params import EventSearchParams as EventSearchParams
 from .event_update_params import EventUpdateParams as EventUpdateParams
 from .invoice_list_params import InvoiceListParams as InvoiceListParams
 from .price_create_params import PriceCreateParams as PriceCreateParams
-from .alert_disable_params import AlertDisableParams as AlertDisableParams
 from .coupon_create_params import CouponCreateParams as CouponCreateParams
 from .customer_list_params import CustomerListParams as CustomerListParams
 from .evaluate_price_group import EvaluatePriceGroup as EvaluatePriceGroup
 from .metric_create_params import MetricCreateParams as MetricCreateParams
 from .metric_list_response import MetricListResponse as MetricListResponse
 from .event_ingest_response import EventIngestResponse as EventIngestResponse
 from .event_search_response import EventSearchResponse as EventSearchResponse
@@ -53,15 +51,14 @@
 from .top_level_ping_response import TopLevelPingResponse as TopLevelPingResponse
 from .event_deprecate_response import EventDeprecateResponse as EventDeprecateResponse
 from .invoice_mark_paid_params import InvoiceMarkPaidParams as InvoiceMarkPaidParams
 from .subscription_list_params import SubscriptionListParams as SubscriptionListParams
 from .subscription_cancel_params import SubscriptionCancelParams as SubscriptionCancelParams
 from .subscription_create_params import SubscriptionCreateParams as SubscriptionCreateParams
 from .subscription_update_params import SubscriptionUpdateParams as SubscriptionUpdateParams
-from .alert_create_for_plan_params import AlertCreateForPlanParams as AlertCreateForPlanParams
 from .invoice_fetch_upcoming_params import InvoiceFetchUpcomingParams as InvoiceFetchUpcomingParams
 from .invoice_fetch_upcoming_response import InvoiceFetchUpcomingResponse as InvoiceFetchUpcomingResponse
 from .invoice_line_item_create_params import InvoiceLineItemCreateParams as InvoiceLineItemCreateParams
 from .subscription_fetch_costs_params import SubscriptionFetchCostsParams as SubscriptionFetchCostsParams
 from .subscription_fetch_usage_params import SubscriptionFetchUsageParams as SubscriptionFetchUsageParams
 from .alert_create_for_customer_params import AlertCreateForCustomerParams as AlertCreateForCustomerParams
 from .invoice_line_item_create_response import InvoiceLineItemCreateResponse as InvoiceLineItemCreateResponse
```

### Comparing `orb_billing-1.50.0/src/orb/types/alert.py` & `orb_billing-1.50.1/src/orb/types/alert.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     id: str
     """Also referred to as alert_id in this documentation."""
 
     created_at: datetime
     """The creation time of the resource in Orb."""
 
     currency: Optional[str] = None
-    """The name of the currency the credit balance for this alert is denominated in."""
+    """The name of the currency the credit balance or invoice cost is denominated in."""
 
     customer: Optional[Dict[str, Optional[str]]] = None
     """The customer the alert applies to."""
 
     enabled: bool
     """Whether the alert is enabled or disabled."""
```

### Comparing `orb_billing-1.50.0/src/orb/types/alert_create_for_customer_params.py` & `orb_billing-1.50.1/src/orb/types/alert_create_for_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/alert_create_for_external_customer_params.py` & `orb_billing-1.50.1/src/orb/types/alert_create_for_external_customer_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/alert_create_for_plan_params.py` & `orb_billing-1.50.1/src/orb/types/alert_create_for_subscription_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Iterable, Optional
 from typing_extensions import Required, TypedDict
 
-__all__ = ["AlertCreateForPlanParams", "Threshold"]
+__all__ = ["AlertCreateForSubscriptionParams", "Threshold"]
 
 
-class AlertCreateForPlanParams(TypedDict, total=False):
+class AlertCreateForSubscriptionParams(TypedDict, total=False):
     thresholds: Required[Iterable[Threshold]]
     """The thresholds for the alert."""
 
     type: Required[str]
     """The thresholds that define the values at which the alert will be triggered."""
 
     metric_id: Optional[str]
     """The metric to track usage for."""
 
-    plan_version: Optional[int]
-    """The plan version to create alerts for.
-
-    If not specified, the default will be the plan's active plan version.
-    """
-
 
 class Threshold(TypedDict, total=False):
     value: Required[float]
     """The value at which an alert will fire.
 
     For credit balance alerts, the alert will fire at or below this value. For usage
     and cost alerts, the alert will fire at or above this value.
```

### Comparing `orb_billing-1.50.0/src/orb/types/alert_list_params.py` & `orb_billing-1.50.1/src/orb/types/alert_list_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,18 +32,9 @@
 
     external_customer_id: Optional[str]
     """Fetch alerts scoped to this external_customer_id"""
 
     limit: int
     """The number of items to fetch. Defaults to 20."""
 
-    plan_id: Optional[str]
-    """Fetch alerts scoped to this plan_id"""
-
-    plan_version: Optional[int]
-    """
-    If provided alongside plan_id, only the alerts that are scoped to the specified
-    plan_version will be returned.
-    """
-
     subscription_id: Optional[str]
     """Fetch alerts scoped to this subscription_id"""
```

### Comparing `orb_billing-1.50.0/src/orb/types/coupon.py` & `orb_billing-1.50.1/src/orb/types/coupon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from .._utils import PropertyInfo
 from .._models import BaseModel
 
 __all__ = ["Coupon", "Discount", "DiscountPercentageDiscount", "DiscountAmountDiscount"]
 
 
 class DiscountPercentageDiscount(BaseModel):
     applies_to_price_ids: List[str]
@@ -38,15 +39,17 @@
     """
 
     discount_type: Literal["amount"]
 
     reason: Optional[str] = None
 
 
-Discount = Union[DiscountPercentageDiscount, DiscountAmountDiscount]
+Discount = Annotated[
+    Union[DiscountPercentageDiscount, DiscountAmountDiscount], PropertyInfo(discriminator="discount_type")
+]
 
 
 class Coupon(BaseModel):
     id: str
     """Also referred to as coupon_id in this documentation."""
 
     archived_at: Optional[datetime] = None
```

### Comparing `orb_billing-1.50.0/src/orb/types/coupon_create_params.py` & `orb_billing-1.50.1/src/orb/types/coupon_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/coupon_list_params.py` & `orb_billing-1.50.1/src/orb/types/coupon_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/credit_note.py` & `orb_billing-1.50.1/src/orb/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customer.py` & `orb_billing-1.50.1/src/orb/types/customer.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customer_create_params.py` & `orb_billing-1.50.1/src/orb/types/customer_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customer_list_params.py` & `orb_billing-1.50.1/src/orb/types/customer_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customer_update_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customer_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customer_update_params.py` & `orb_billing-1.50.1/src/orb/types/customer_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/event_ingest_params.py` & `orb_billing-1.50.1/src/orb/types/event_ingest_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/event_ingest_response.py` & `orb_billing-1.50.1/src/orb/types/event_ingest_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/event_search_params.py` & `orb_billing-1.50.1/src/orb/types/event_search_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/event_search_response.py` & `orb_billing-1.50.1/src/orb/types/event_search_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/event_update_params.py` & `orb_billing-1.50.1/src/orb/types/event_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/invoice.py` & `orb_billing-1.50.1/src/orb/types/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
 from .price import Price
+from .._utils import PropertyInfo
 from .._models import BaseModel
 from .shared.discount import Discount
 
 __all__ = [
     "Invoice",
     "AutoCollection",
     "BillingAddress",
@@ -408,16 +409,19 @@
     name: str
 
     quantity: float
 
     type: Literal["'null'"]
 
 
-LineItemSubLineItem = Union[
-    LineItemSubLineItemMatrixSubLineItem, LineItemSubLineItemTierSubLineItem, LineItemSubLineItemOtherSubLineItem
+LineItemSubLineItem = Annotated[
+    Union[
+        LineItemSubLineItemMatrixSubLineItem, LineItemSubLineItemTierSubLineItem, LineItemSubLineItemOtherSubLineItem
+    ],
+    PropertyInfo(discriminator="type"),
 ]
 
 
 class LineItemTaxAmount(BaseModel):
     amount: str
     """The amount of additional tax incurred by this tax rate."""
```

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_create_params.py` & `orb_billing-1.50.1/src/orb/types/invoice_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_fetch_upcoming_response.py` & `orb_billing-1.50.1/src/orb/types/invoice_fetch_upcoming_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
 from .price import Price
+from .._utils import PropertyInfo
 from .._models import BaseModel
 from .shared.discount import Discount
 
 __all__ = [
     "InvoiceFetchUpcomingResponse",
     "AutoCollection",
     "BillingAddress",
@@ -408,16 +409,19 @@
     name: str
 
     quantity: float
 
     type: Literal["'null'"]
 
 
-LineItemSubLineItem = Union[
-    LineItemSubLineItemMatrixSubLineItem, LineItemSubLineItemTierSubLineItem, LineItemSubLineItemOtherSubLineItem
+LineItemSubLineItem = Annotated[
+    Union[
+        LineItemSubLineItemMatrixSubLineItem, LineItemSubLineItemTierSubLineItem, LineItemSubLineItemOtherSubLineItem
+    ],
+    PropertyInfo(discriminator="type"),
 ]
 
 
 class LineItemTaxAmount(BaseModel):
     amount: str
     """The amount of additional tax incurred by this tax rate."""
```

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_line_item_create_params.py` & `orb_billing-1.50.1/src/orb/types/invoice_line_item_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_line_item_create_response.py` & `orb_billing-1.50.1/src/orb/types/invoice_line_item_create_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
 from .price import Price
+from .._utils import PropertyInfo
 from .._models import BaseModel
 from .shared.discount import Discount
 
 __all__ = [
     "InvoiceLineItemCreateResponse",
     "Maximum",
     "Minimum",
@@ -120,15 +121,18 @@
     name: str
 
     quantity: float
 
     type: Literal["'null'"]
 
 
-SubLineItem = Union[SubLineItemMatrixSubLineItem, SubLineItemTierSubLineItem, SubLineItemOtherSubLineItem]
+SubLineItem = Annotated[
+    Union[SubLineItemMatrixSubLineItem, SubLineItemTierSubLineItem, SubLineItemOtherSubLineItem],
+    PropertyInfo(discriminator="type"),
+]
 
 
 class TaxAmount(BaseModel):
     amount: str
     """The amount of additional tax incurred by this tax rate."""
 
     tax_rate_description: str
```

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_list_params.py` & `orb_billing-1.50.1/src/orb/types/invoice_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/invoice_mark_paid_params.py` & `orb_billing-1.50.1/src/orb/types/invoice_mark_paid_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/item.py` & `orb_billing-1.50.1/src/orb/types/item.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/metric_create_params.py` & `orb_billing-1.50.1/src/orb/types/metric_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/metric_create_response.py` & `orb_billing-1.50.1/src/orb/types/metric_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/metric_fetch_response.py` & `orb_billing-1.50.1/src/orb/types/metric_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/metric_list_params.py` & `orb_billing-1.50.1/src/orb/types/metric_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/metric_list_response.py` & `orb_billing-1.50.1/src/orb/types/metric_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/plan.py` & `orb_billing-1.50.1/src/orb/types/plan.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/plan_create_params.py` & `orb_billing-1.50.1/src/orb/types/plan_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/plan_list_params.py` & `orb_billing-1.50.1/src/orb/types/plan_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/plan_update_params.py` & `orb_billing-1.50.1/src/orb/types/plan_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/price.py` & `orb_billing-1.50.1/src/orb/types/price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
 from pydantic import Field as FieldInfo
 
+from .._utils import PropertyInfo
 from .._models import BaseModel
 from .shared.discount import Discount
 
 __all__ = [
     "Price",
     "UnitPrice",
     "UnitPriceBillableMetric",
@@ -1545,25 +1546,28 @@
     name: str
 
     plan_phase_order: Optional[int] = None
 
     price_type: Literal["usage_price", "fixed_price"]
 
 
-Price = Union[
-    UnitPrice,
-    PackagePrice,
-    MatrixPrice,
-    TieredPrice,
-    TieredBpsPrice,
-    BpsPrice,
-    BulkBpsPrice,
-    BulkPrice,
-    ThresholdTotalAmountPrice,
-    TieredPackagePrice,
-    GroupedTieredPrice,
-    TieredWithMinimumPrice,
-    TieredPackageWithMinimumPrice,
-    PackageWithAllocationPrice,
-    UnitWithPercentPrice,
-    MatrixWithAllocationPrice,
+Price = Annotated[
+    Union[
+        UnitPrice,
+        PackagePrice,
+        MatrixPrice,
+        TieredPrice,
+        TieredBpsPrice,
+        BpsPrice,
+        BulkBpsPrice,
+        BulkPrice,
+        ThresholdTotalAmountPrice,
+        TieredPackagePrice,
+        GroupedTieredPrice,
+        TieredWithMinimumPrice,
+        TieredPackageWithMinimumPrice,
+        PackageWithAllocationPrice,
+        UnitWithPercentPrice,
+        MatrixWithAllocationPrice,
+    ],
+    PropertyInfo(discriminator="price_model_type"),
 ]
```

### Comparing `orb_billing-1.50.0/src/orb/types/price_create_params.py` & `orb_billing-1.50.1/src/orb/types/price_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/price_evaluate_params.py` & `orb_billing-1.50.1/src/orb/types/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription.py` & `orb_billing-1.50.1/src/orb/types/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, List, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
 from .plan import Plan
 from .price import Price
+from .._utils import PropertyInfo
 from .._models import BaseModel
 from .customer import Customer
 
 __all__ = [
     "Subscription",
     "DiscountInterval",
     "DiscountIntervalAmountDiscountInterval",
@@ -84,18 +85,21 @@
     usage_discount: float
     """Only available if discount_type is `usage`.
 
     Number of usage units that this discount is for
     """
 
 
-DiscountInterval = Union[
-    DiscountIntervalAmountDiscountInterval,
-    DiscountIntervalPercentageDiscountInterval,
-    DiscountIntervalUsageDiscountInterval,
+DiscountInterval = Annotated[
+    Union[
+        DiscountIntervalAmountDiscountInterval,
+        DiscountIntervalPercentageDiscountInterval,
+        DiscountIntervalUsageDiscountInterval,
+    ],
+    PropertyInfo(discriminator="discount_type"),
 ]
 
 
 class FixedFeeQuantitySchedule(BaseModel):
     end_date: Optional[datetime] = None
 
     price_id: str
```

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_cancel_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_cancel_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_create_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_fetch_costs_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_fetch_costs_response.py` & `orb_billing-1.50.1/src/orb/types/subscription_fetch_costs_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_fetch_schedule_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_fetch_schedule_response.py` & `orb_billing-1.50.1/src/orb/types/subscription_fetch_schedule_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_fetch_usage_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_fetch_usage_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_list_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_price_intervals_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_price_intervals_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_schedule_plan_change_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_schedule_plan_change_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_trigger_phase_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_trigger_phase_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_update_fixed_fee_quantity_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_update_params.py` & `orb_billing-1.50.1/src/orb/types/subscription_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/subscription_usage.py` & `orb_billing-1.50.1/src/orb/types/subscription_usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/beta/price_evaluate_params.py` & `orb_billing-1.50.1/src/orb/types/beta/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/coupons/subscription_list_params.py` & `orb_billing-1.50.1/src/orb/types/coupons/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/__init__.py` & `orb_billing-1.50.1/src/orb/types/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/balance_transaction_create_response.py` & `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/balance_transaction_list_params.py` & `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/balance_transaction_list_response.py` & `orb_billing-1.50.1/src/orb/types/customers/balance_transaction_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/cost_list_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/cost_list_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/cost_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/cost_list_params.py` & `orb_billing-1.50.1/src/orb/types/customers/cost_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/cost_list_response.py` & `orb_billing-1.50.1/src/orb/types/customers/cost_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credit_list_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credit_list_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credit_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credit_list_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credit_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/usage_update_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/usage_update_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/usage_update_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/usage_update_params.py` & `orb_billing-1.50.1/src/orb/types/customers/usage_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/__init__.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from ...._utils import PropertyInfo
 from ...._models import BaseModel
 
 __all__ = [
     "LedgerCreateEntryByExternalIDResponse",
     "IncrementLedgerEntry",
     "IncrementLedgerEntryCreditBlock",
     "IncrementLedgerEntryCustomer",
@@ -382,16 +383,19 @@
     removed by setting the value to `null`, and the entire metadata mapping can be
     cleared by setting `metadata` to `null`.
     """
 
     starting_balance: float
 
 
-LedgerCreateEntryByExternalIDResponse = Union[
-    IncrementLedgerEntry,
-    DecrementLedgerEntry,
-    ExpirationChangeLedgerEntry,
-    CreditBlockExpiryLedgerEntry,
-    VoidLedgerEntry,
-    VoidInitiatedLedgerEntry,
-    AmendmentLedgerEntry,
+LedgerCreateEntryByExternalIDResponse = Annotated[
+    Union[
+        IncrementLedgerEntry,
+        DecrementLedgerEntry,
+        ExpirationChangeLedgerEntry,
+        CreditBlockExpiryLedgerEntry,
+        VoidLedgerEntry,
+        VoidInitiatedLedgerEntry,
+        AmendmentLedgerEntry,
+    ],
+    PropertyInfo(discriminator="entry_type"),
 ]
```

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_create_entry_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_create_entry_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from ...._utils import PropertyInfo
 from ...._models import BaseModel
 
 __all__ = [
     "LedgerCreateEntryResponse",
     "IncrementLedgerEntry",
     "IncrementLedgerEntryCreditBlock",
     "IncrementLedgerEntryCustomer",
@@ -382,16 +383,19 @@
     removed by setting the value to `null`, and the entire metadata mapping can be
     cleared by setting `metadata` to `null`.
     """
 
     starting_balance: float
 
 
-LedgerCreateEntryResponse = Union[
-    IncrementLedgerEntry,
-    DecrementLedgerEntry,
-    ExpirationChangeLedgerEntry,
-    CreditBlockExpiryLedgerEntry,
-    VoidLedgerEntry,
-    VoidInitiatedLedgerEntry,
-    AmendmentLedgerEntry,
+LedgerCreateEntryResponse = Annotated[
+    Union[
+        IncrementLedgerEntry,
+        DecrementLedgerEntry,
+        ExpirationChangeLedgerEntry,
+        CreditBlockExpiryLedgerEntry,
+        VoidLedgerEntry,
+        VoidInitiatedLedgerEntry,
+        AmendmentLedgerEntry,
+    ],
+    PropertyInfo(discriminator="entry_type"),
 ]
```

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_by_external_id_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from ...._utils import PropertyInfo
 from ...._models import BaseModel
 
 __all__ = [
     "LedgerListByExternalIDResponse",
     "IncrementLedgerEntry",
     "IncrementLedgerEntryCreditBlock",
     "IncrementLedgerEntryCustomer",
@@ -382,16 +383,19 @@
     removed by setting the value to `null`, and the entire metadata mapping can be
     cleared by setting `metadata` to `null`.
     """
 
     starting_balance: float
 
 
-LedgerListByExternalIDResponse = Union[
-    IncrementLedgerEntry,
-    DecrementLedgerEntry,
-    ExpirationChangeLedgerEntry,
-    CreditBlockExpiryLedgerEntry,
-    VoidLedgerEntry,
-    VoidInitiatedLedgerEntry,
-    AmendmentLedgerEntry,
+LedgerListByExternalIDResponse = Annotated[
+    Union[
+        IncrementLedgerEntry,
+        DecrementLedgerEntry,
+        ExpirationChangeLedgerEntry,
+        CreditBlockExpiryLedgerEntry,
+        VoidLedgerEntry,
+        VoidInitiatedLedgerEntry,
+        AmendmentLedgerEntry,
+    ],
+    PropertyInfo(discriminator="entry_type"),
 ]
```

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/ledger_list_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/ledger_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, Union, Optional
 from datetime import datetime
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from ...._utils import PropertyInfo
 from ...._models import BaseModel
 
 __all__ = [
     "LedgerListResponse",
     "IncrementLedgerEntry",
     "IncrementLedgerEntryCreditBlock",
     "IncrementLedgerEntryCustomer",
@@ -382,16 +383,19 @@
     removed by setting the value to `null`, and the entire metadata mapping can be
     cleared by setting `metadata` to `null`.
     """
 
     starting_balance: float
 
 
-LedgerListResponse = Union[
-    IncrementLedgerEntry,
-    DecrementLedgerEntry,
-    ExpirationChangeLedgerEntry,
-    CreditBlockExpiryLedgerEntry,
-    VoidLedgerEntry,
-    VoidInitiatedLedgerEntry,
-    AmendmentLedgerEntry,
+LedgerListResponse = Annotated[
+    Union[
+        IncrementLedgerEntry,
+        DecrementLedgerEntry,
+        ExpirationChangeLedgerEntry,
+        CreditBlockExpiryLedgerEntry,
+        VoidLedgerEntry,
+        VoidInitiatedLedgerEntry,
+        AmendmentLedgerEntry,
+    ],
+    PropertyInfo(discriminator="entry_type"),
 ]
```

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_create_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/customers/credits/top_up_list_response.py` & `orb_billing-1.50.1/src/orb/types/customers/credits/top_up_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/__init__.py` & `orb_billing-1.50.1/src/orb/types/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_close_response.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_close_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_create_params.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_create_response.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_fetch_response.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_list_response.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/events/backfill_revert_response.py` & `orb_billing-1.50.1/src/orb/types/events/backfill_revert_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/plans/external_plan_id_update_params.py` & `orb_billing-1.50.1/src/orb/types/plans/external_plan_id_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/src/orb/types/shared/discount.py` & `orb_billing-1.50.1/src/orb/types/shared/discount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
-from typing_extensions import Literal
+from typing_extensions import Literal, Annotated
 
+from ..._utils import PropertyInfo
 from ..._models import BaseModel
 
 __all__ = ["Discount", "PercentageDiscount", "TrialDiscount", "UsageDiscount", "AmountDiscount"]
 
 
 class PercentageDiscount(BaseModel):
     applies_to_price_ids: List[str]
@@ -73,8 +74,10 @@
     """
 
     discount_type: Literal["amount"]
 
     reason: Optional[str] = None
 
 
-Discount = Union[PercentageDiscount, TrialDiscount, UsageDiscount, AmountDiscount]
+Discount = Annotated[
+    Union[PercentageDiscount, TrialDiscount, UsageDiscount, AmountDiscount], PropertyInfo(discriminator="discount_type")
+]
```

### Comparing `orb_billing-1.50.0/LICENSE` & `orb_billing-1.50.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orb_billing-1.50.0/pyproject.toml` & `orb_billing-1.50.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "orb-billing"
-version = "1.50.0"
+version = "1.50.1"
 description = "The official Python library for the orb API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Orb", email = "team@withorb.com" },
 ]
 dependencies = [
```

### Comparing `orb_billing-1.50.0/PKG-INFO` & `orb_billing-1.50.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: orb-billing
-Version: 1.50.0
+Version: 1.50.1
 Summary: The official Python library for the orb API
 Project-URL: Homepage, https://github.com/orbcorp/orb-python
 Project-URL: Repository, https://github.com/orbcorp/orb-python
 Author-email: Orb <team@withorb.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

