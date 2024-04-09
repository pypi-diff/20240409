# Comparing `tmp/ozon_api_client-0.0.4.tar.gz` & `tmp/ozon_api_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozon_api_client-0.0.4.tar", max compression
+gzip compressed data, was "ozon_api_client-0.0.5.tar", max compression
```

## Comparing `ozon_api_client-0.0.4.tar` & `ozon_api_client-0.0.5.tar`

### file list

```diff
@@ -1,687 +1,687 @@
--rw-r--r--   0        0        0    92068 2024-03-20 13:08:55.010924 ozon_api_client-0.0.4/README.md
--rw-r--r--   0        0        0    70903 2024-03-20 13:08:55.232514 ozon_api_client-0.0.4/ozon_api_client/__init__.py
--rw-r--r--   0        0        0     1540 2024-03-20 13:08:55.313909 ozon_api_client-0.0.4/ozon_api_client/api/__init__.py
--rw-r--r--   0        0        0    12841 2024-03-20 13:08:55.732365 ozon_api_client-0.0.4/ozon_api_client/api/analytics_api_api.py
--rw-r--r--   0        0        0    11016 2024-03-20 13:08:55.796024 ozon_api_client-0.0.4/ozon_api_client/api/barcode_api_api.py
--rw-r--r--   0        0        0     7370 2024-03-20 13:08:55.138752 ozon_api_client-0.0.4/ozon_api_client/api/brand_api_api.py
--rw-r--r--   0        0        0    24123 2024-03-20 13:08:54.933560 ozon_api_client-0.0.4/ozon_api_client/api/cancellation_api_api.py
--rw-r--r--   0        0        0    19449 2024-03-20 13:08:55.736657 ozon_api_client-0.0.4/ozon_api_client/api/category_api_api.py
--rw-r--r--   0        0        0    63927 2024-03-20 13:08:54.880946 ozon_api_client-0.0.4/ozon_api_client/api/certification_api_api.py
--rw-r--r--   0        0        0    32367 2024-03-20 13:08:54.953498 ozon_api_client-0.0.4/ozon_api_client/api/chat_api_api.py
--rw-r--r--   0        0        0    34465 2024-03-20 13:08:55.155750 ozon_api_client-0.0.4/ozon_api_client/api/fbo_api.py
--rw-r--r--   0        0        0   218207 2024-03-20 13:08:54.852669 ozon_api_client-0.0.4/ozon_api_client/api/fbs_api.py
--rw-r--r--   0        0        0    51898 2024-03-20 13:08:54.817343 ozon_api_client-0.0.4/ozon_api_client/api/fbsr_fbs_marks_api.py
--rw-r--r--   0        0        0    19230 2024-03-20 13:08:55.590615 ozon_api_client-0.0.4/ozon_api_client/api/finance_api_api.py
--rw-r--r--   0        0        0    11762 2024-03-20 13:08:55.131653 ozon_api_client-0.0.4/ozon_api_client/api/polygon_api_api.py
--rw-r--r--   0        0        0    49168 2024-03-20 13:08:55.001110 ozon_api_client-0.0.4/ozon_api_client/api/prices_stocks_api_api.py
--rw-r--r--   0        0        0    46970 2024-03-20 13:08:55.227205 ozon_api_client-0.0.4/ozon_api_client/api/pricing_strategy_api_api.py
--rw-r--r--   0        0        0   140217 2024-03-20 13:08:55.302869 ozon_api_client-0.0.4/ozon_api_client/api/product_api_api.py
--rw-r--r--   0        0        0    48513 2024-03-20 13:08:55.346639 ozon_api_client-0.0.4/ozon_api_client/api/promos_api.py
--rw-r--r--   0        0        0    57166 2024-03-20 13:08:55.623046 ozon_api_client-0.0.4/ozon_api_client/api/report_api_api.py
--rw-r--r--   0        0        0    37321 2024-03-20 13:08:55.218520 ozon_api_client-0.0.4/ozon_api_client/api/return_api_api.py
--rw-r--r--   0        0        0     9794 2024-03-20 13:08:55.658984 ozon_api_client-0.0.4/ozon_api_client/api/returns_api_api.py
--rw-r--r--   0        0        0    39878 2024-03-20 13:08:54.827228 ozon_api_client-0.0.4/ozon_api_client/api/rfbs_returns_api_api.py
--rw-r--r--   0        0        0     8920 2024-03-20 13:08:55.733840 ozon_api_client-0.0.4/ozon_api_client/api/seller_rating_api.py
--rw-r--r--   0        0        0    12746 2024-03-20 13:08:55.091479 ozon_api_client-0.0.4/ozon_api_client/api/supplier_api_api.py
--rw-r--r--   0        0        0    10914 2024-03-20 13:08:55.158738 ozon_api_client-0.0.4/ozon_api_client/api/warehouse_api_api.py
--rw-r--r--   0        0        0    25375 2024-03-20 13:08:55.340695 ozon_api_client-0.0.4/ozon_api_client/api_client.py
--rw-r--r--   0        0        0     8388 2024-03-20 13:08:55.390475 ozon_api_client-0.0.4/ozon_api_client/configuration.py
--rw-r--r--   0        0        0    69296 2024-03-20 13:08:54.869242 ozon_api_client-0.0.4/ozon_api_client/models/__init__.py
--rw-r--r--   0        0        0     5190 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/add_strategy_items_response_error.py
--rw-r--r--   0        0        0    15912 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_analytics_get_data_request.py
--rw-r--r--   0        0        0     4496 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_analytics_get_data_response.py
--rw-r--r--   0        0        0     4517 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_data_row.py
--rw-r--r--   0        0        0     4187 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_data_row_dimension.py
--rw-r--r--   0        0        0     5033 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_filter.py
--rw-r--r--   0        0        0     4506 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_get_data_response_result.py
--rw-r--r--   0        0        0     3048 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_get_stock_on_warehouses_request_warehouse_type.py
--rw-r--r--   0        0        0     2755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_metric.py
--rw-r--r--   0        0        0     4228 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_sorting.py
--rw-r--r--   0        0        0     5918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_request.py
--rw-r--r--   0        0        0     3634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_response.py
--rw-r--r--   0        0        0     3812 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_response_result.py
--rw-r--r--   0        0        0    10216 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_result_rows.py
--rw-r--r--   0        0        0     4771 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/approve_decline_discount_tasks_response_fail_detail.py
--rw-r--r--   0        0        0     4703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/brand_brand_company_certification_list_request.py
--rw-r--r--   0        0        0     3772 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/brand_brand_company_certification_list_response.py
--rw-r--r--   0        0        0     5246 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/brand_company_certification_list_response_brand_certification.py
--rw-r--r--   0        0        0     5303 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/brand_company_certification_list_response_brand_certification_result.py
--rw-r--r--   0        0        0    11334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/certificate_create_body.py
--rw-r--r--   0        0        0     5308 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_file_request.py
--rw-r--r--   0        0        0     3606 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_file_response.py
--rw-r--r--   0        0        0     4405 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_message_request.py
--rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_message_response.py
--rw-r--r--   0        0        0     3728 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_start_request.py
--rw-r--r--   0        0        0     3490 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_start_response.py
--rw-r--r--   0        0        0     7093 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_history.py
--rw-r--r--   0        0        0     9357 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_info.py
--rw-r--r--   0        0        0     5404 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_list.py
--rw-r--r--   0        0        0     4958 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_list_request_filter.py
--rw-r--r--   0        0        0     4563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_read.py
--rw-r--r--   0        0        0     3584 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/chat_start_response_result.py
--rw-r--r--   0        0        0     3533 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/common_create_report_response.py
--rw-r--r--   0        0        0     7329 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/common_price_indexes.py
--rw-r--r--   0        0        0    15020 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/common_returns_company_item_fbo.py
--rw-r--r--   0        0        0    30723 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/common_returns_company_item_fbs.py
--rw-r--r--   0        0        0     4985 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/common_time_range_last_day.py
--rw-r--r--   0        0        0     4495 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/conditional_cancellation_cancellation_reason.py
--rw-r--r--   0        0        0     5620 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/conditional_cancellation_state.py
--rw-r--r--   0        0        0     3582 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/create_report_response_code.py
--rw-r--r--   0        0        0     4120 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/created_at.py
--rw-r--r--   0        0        0     3760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/delete_products_request_product.py
--rw-r--r--   0        0        0     5779 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/delete_products_response_delete_status.py
--rw-r--r--   0        0        0     5834 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/delivery_method_list_request_filter.py
--rw-r--r--   0        0        0    12629 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/delivery_method_list_response_delivery_method.py
--rw-r--r--   0        0        0     5334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_delivery_details.py
--rw-r--r--   0        0        0     4181 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_others.py
--rw-r--r--   0        0        0     4335 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_payment.py
--rw-r--r--   0        0        0     5263 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_return_details.py
--rw-r--r--   0        0        0     4193 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_returns.py
--rw-r--r--   0        0        0     9333 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_rfbs_details.py
--rw-r--r--   0        0        0     4175 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_service.py
--rw-r--r--   0        0        0     4211 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/details_services.py
--rw-r--r--   0        0        0    10453 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbo_posting_fbo_posting_analytics_data.py
--rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_barcodes.py
--rw-r--r--   0        0        0     5955 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_detail_courier.py
--rw-r--r--   0        0        0     6995 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_detail_prr_option.py
--rw-r--r--   0        0        0     8525 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_fbs_posting_analytics_data.py
--rw-r--r--   0        0        0     5605 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_move_status_response_move_status.py
--rw-r--r--   0        0        0     4314 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result.py
--rw-r--r--   0        0        0     7844 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product.py
--rw-r--r--   0        0        0    10226 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product_exemplar.py
--rw-r--r--   0        0        0     3816 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_package.py
--rw-r--r--   0        0        0     4655 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_package_product.py
--rw-r--r--   0        0        0     3917 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_with.py
--rw-r--r--   0        0        0     4938 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_response_ship_additional_data.py
--rw-r--r--   0        0        0     5025 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_tracking_number_set_request_tracking_number.py
--rw-r--r--   0        0        0     5680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_request.py
--rw-r--r--   0        0        0     4874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_response.py
--rw-r--r--   0        0        0     3824 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_request.py
--rw-r--r--   0        0        0     6179 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response.py
--rw-r--r--   0        0        0     4934 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product.py
--rw-r--r--   0        0        0    21322 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product_exemplar.py
--rw-r--r--   0        0        0    10112 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_posting_product_detail_without_dimensions.py
--rw-r--r--   0        0        0     4727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request.py
--rw-r--r--   0        0        0     4899 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request_product.py
--rw-r--r--   0        0        0     9179 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request_product_exemplar.py
--rw-r--r--   0        0        0     3795 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_response.py
--rw-r--r--   0        0        0     2727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/filter_op.py
--rw-r--r--   0        0        0     4456 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/filter_period.py
--rw-r--r--   0        0        0    10569 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_cash_flow.py
--rw-r--r--   0        0        0     5735 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_delivery_service.py
--rw-r--r--   0        0        0    12749 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_details.py
--rw-r--r--   0        0        0     5897 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_details_others.py
--rw-r--r--   0        0        0     5557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_return_service.py
--rw-r--r--   0        0        0     7535 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_service.py
--rw-r--r--   0        0        0     3675 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_get_realization_report_request.py
--rw-r--r--   0        0        0     3755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_get_realization_report_response.py
--rw-r--r--   0        0        0    15984 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_header.py
--rw-r--r--   0        0        0     4573 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_result.py
--rw-r--r--   0        0        0    24348 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_rows.py
--rw-r--r--   0        0        0    15083 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_list_v3_request_filter.py
--rw-r--r--   0        0        0    17234 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_list_v3_response_operation.py
--rw-r--r--   0        0        0     4756 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_totals_v3_request_date.py
--rw-r--r--   0        0        0     5522 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_request.py
--rw-r--r--   0        0        0     3722 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_response.py
--rw-r--r--   0        0        0     5876 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_response_result.py
--rw-r--r--   0        0        0     6301 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_request.py
--rw-r--r--   0        0        0     3744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_response.py
--rw-r--r--   0        0        0    14909 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_response_result.py
--rw-r--r--   0        0        0     4473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/financev3_period.py
--rw-r--r--   0        0        0    21918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_carriage_available_list_response_result.py
--rw-r--r--   0        0        0     4407 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_competitors_response_competitor_info.py
--rw-r--r--   0        0        0     8136 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_request_filters.py
--rw-r--r--   0        0        0     3931 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_request_with.py
--rw-r--r--   0        0        0     5822 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_response_counters.py
--rw-r--r--   0        0        0     4168 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_request_date.py
--rw-r--r--   0        0        0     4383 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_response_result.py
--rw-r--r--   0        0        0     5211 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_response_result_etgb.py
--rw-r--r--   0        0        0     6938 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_geo_restrictions_by_filter_response_geo_restriction.py
--rw-r--r--   0        0        0     9879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_hot_sales_list_response_hot_sale.py
--rw-r--r--   0        0        0     7387 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_import_products_info_response_result_item.py
--rw-r--r--   0        0        0     5301 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_image.py
--rw-r--r--   0        0        0     4303 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_image360.py
--rw-r--r--   0        0        0     5340 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_pdf.py
--rw-r--r--   0        0        0     6640 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_v3_response_attribute.py
--rw-r--r--   0        0        0     4967 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_v3_response_dictionary_value.py
--rw-r--r--   0        0        0     4475 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_list_response_reason.py
--rw-r--r--   0        0        0     3783 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_list_response_reasons.py
--rw-r--r--   0        0        0     5282 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_stocks_v3_response_stock.py
--rw-r--r--   0        0        0     5739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_product_rating.py
--rw-r--r--   0        0        0     6618 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_condition.py
--rw-r--r--   0        0        0    10309 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_group.py
--rw-r--r--   0        0        0     4571 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_improve_attribute.py
--rw-r--r--   0        0        0    19464 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_seller_actions_v1_response_action.py
--rw-r--r--   0        0        0     4873 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_strategy_ids_by_item_ids_response_product_info.py
--rw-r--r--   0        0        0    10790 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_strategy_list_response_strategy.py
--rw-r--r--   0        0        0     6986 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_supply_order_items_response_item.py
--rw-r--r--   0        0        0    19218 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_supply_orders_list_response_supply_order.py
--rw-r--r--   0        0        0     5653 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_daily_create.py
--rw-r--r--   0        0        0     5665 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_daily_update.py
--rw-r--r--   0        0        0     4511 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_total.py
--rw-r--r--   0        0        0     6338 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/giveout_info_response_article_details.py
--rw-r--r--   0        0        0    10894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/giveout_list_response_giveout_details.py
--rw-r--r--   0        0        0     5056 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/googlerpc_status.py
--rw-r--r--   0        0        0     5242 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/import_products_request_pdf_list.py
--rw-r--r--   0        0        0     3624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/invoice_get_response_result.py
--rw-r--r--   0        0        0    25953 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/item_commissions.py
--rw-r--r--   0        0        0     7518 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/item_marketing_actions.py
--rw-r--r--   0        0        0    15056 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/item_price.py
--rw-r--r--   0        0        0     2890 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/language_language.py
--rw-r--r--   0        0        0     6473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/marketing_actions_marketing_action.py
--rw-r--r--   0        0        0     4165 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/operation_item.py
--rw-r--r--   0        0        0     6859 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/operation_posting.py
--rw-r--r--   0        0        0    11115 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/operation_service.py
--rw-r--r--   0        0        0     4565 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygon_bind_requestpolygon.py
--rw-r--r--   0        0        0     4463 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygon_bind_requestwh_location.py
--rw-r--r--   0        0        0     2751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_empty.py
--rw-r--r--   0        0        0     5781 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_bind_request.py
--rw-r--r--   0        0        0     3822 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_create_request.py
--rw-r--r--   0        0        0     3716 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_create_response.py
--rw-r--r--   0        0        0     3737 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_boolean_response.py
--rw-r--r--   0        0        0     6226 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_fbs_posting_request.py
--rw-r--r--   0        0        0     7656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason.py
--rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_list_response.py
--rw-r--r--   0        0        0     3946 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_request.py
--rw-r--r--   0        0        0     3679 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_response.py
--rw-r--r--   0        0        0     4981 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbo_posting_with_params.py
--rw-r--r--   0        0        0    14274 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_act_check_status_response_status.py
--rw-r--r--   0        0        0     3666 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_act_create_response_act.py
--rw-r--r--   0        0        0     3850 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_delivered_request.py
--rw-r--r--   0        0        0     3858 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_delivering_request.py
--rw-r--r--   0        0        0     3842 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_last_mile_request.py
--rw-r--r--   0        0        0     3801 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_move_status_response.py
--rw-r--r--   0        0        0     3908 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_request.py
--rw-r--r--   0        0        0     3826 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_response.py
--rw-r--r--   0        0        0     5417 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_response_item.py
--rw-r--r--   0        0        0     4195 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_tracking_number_set_request.py
--rw-r--r--   0        0        0    17884 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_financial_data_product.py
--rw-r--r--   0        0        0    19874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_financial_data_services.py
--rw-r--r--   0        0        0     8557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_list_request.py
--rw-r--r--   0        0        0     5836 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_list_request_filter.py
--rw-r--r--   0        0        0     5492 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_request.py
--rw-r--r--   0        0        0     3696 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbs_posting_by_barcode_request.py
--rw-r--r--   0        0        0     3786 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_move_posting_request.py
--rw-r--r--   0        0        0     3994 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_check_status_request.py
--rw-r--r--   0        0        0     3679 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_check_status_response.py
--rw-r--r--   0        0        0     6891 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_create_request.py
--rw-r--r--   0        0        0     3615 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_create_response.py
--rw-r--r--   0        0        0     4050 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_request.py
--rw-r--r--   0        0        0     5788 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_response.py
--rw-r--r--   0        0        0     3930 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_get_act_request.py
--rw-r--r--   0        0        0     5548 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_get_act_response.py
--rw-r--r--   0        0        0     3874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_package_label_request.py
--rw-r--r--   0        0        0     5644 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_package_label_response.py
--rw-r--r--   0        0        0     7141 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_cancel_request.py
--rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_cancel_response.py
--rw-r--r--   0        0        0     4751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_change_request.py
--rw-r--r--   0        0        0     3688 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_change_response.py
--rw-r--r--   0        0        0     4537 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_product_cancel_request_item.py
--rw-r--r--   0        0        0     4618 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/posting_product_change_request_item.py
--rw-r--r--   0        0        0     5072 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv1_get_carriage_available_list_request.py
--rw-r--r--   0        0        0     3849 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv1_get_carriage_available_list_response.py
--rw-r--r--   0        0        0     6727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_fbs_posting_with_params.py
--rw-r--r--   0        0        0     9573 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_fbs_posting_with_params_examplars.py
--rw-r--r--   0        0        0     7483 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_list_request.py
--rw-r--r--   0        0        0    11542 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_list_request_filter.py
--rw-r--r--   0        0        0     4569 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_request.py
--rw-r--r--   0        0        0     7780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request.py
--rw-r--r--   0        0        0    13515 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request_filter.py
--rw-r--r--   0        0        0     3766 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response.py
--rw-r--r--   0        0        0     4898 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response_result.py
--rw-r--r--   0        0        0     5023 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_request.py
--rw-r--r--   0        0        0     3711 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response.py
--rw-r--r--   0        0        0     4087 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response_result.py
--rw-r--r--   0        0        0     5012 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request.py
--rw-r--r--   0        0        0     5114 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product.py
--rw-r--r--   0        0        0     7214 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product_exemplar.py
--rw-r--r--   0        0        0     3893 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_response.py
--rw-r--r--   0        0        0     5450 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/premium_scores_score.py
--rw-r--r--   0        0        0     6026 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_external.py
--rw-r--r--   0        0        0     5912 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_ozon.py
--rw-r--r--   0        0        0     5940 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_self.py
--rw-r--r--   0        0        0     3729 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_boolean_response.py
--rw-r--r--   0        0        0     5073 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_certificate_products_list_response_product.py
--rw-r--r--   0        0        0     5699 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_certificate_unbind_response_item.py
--rw-r--r--   0        0        0     4978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_certification_list_response_certification.py
--rw-r--r--   0        0        0     5011 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_certification_list_response_certification_result.py
--rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_request.py
--rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_response.py
--rw-r--r--   0        0        0     4741 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_response_result.py
--rw-r--r--   0        0        0     6773 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_attribute.py
--rw-r--r--   0        0        0     4044 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_complex_attribute.py
--rw-r--r--   0        0        0     5053 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_dictionary_value.py
--rw-r--r--   0        0        0     4779 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_request.py
--rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_response.py
--rw-r--r--   0        0        0     6423 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_response_product.py
--rw-r--r--   0        0        0    11732 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_prices_v4_response_item.py
--rw-r--r--   0        0        0     6060 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_prices_v4_response_result.py
--rw-r--r--   0        0        0     3750 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_request.py
--rw-r--r--   0        0        0    12687 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_request_item.py
--rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_response.py
--rw-r--r--   0        0        0     4905 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_response_result.py
--rw-r--r--   0        0        0     3806 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_request.py
--rw-r--r--   0        0        0    17200 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_request_price.py
--rw-r--r--   0        0        0     3813 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response.py
--rw-r--r--   0        0        0     4479 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response_error.py
--rw-r--r--   0        0        0     7035 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response_process_result.py
--rw-r--r--   0        0        0     3824 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_request.py
--rw-r--r--   0        0        0     5634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_request_stock.py
--rw-r--r--   0        0        0     3813 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response.py
--rw-r--r--   0        0        0     8727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response_error.py
--rw-r--r--   0        0        0     7035 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response_process_result.py
--rw-r--r--   0        0        0     4991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_picking.py
--rw-r--r--   0        0        0     3894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_archive_request.py
--rw-r--r--   0        0        0     3995 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_accordance_types_response.py
--rw-r--r--   0        0        0     4639 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_accordance_types_response_type.py
--rw-r--r--   0        0        0     5109 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_bind_request.py
--rw-r--r--   0        0        0     3885 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_types_response.py
--rw-r--r--   0        0        0     4519 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_types_response_type.py
--rw-r--r--   0        0        0     4667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certification_list_request.py
--rw-r--r--   0        0        0     3718 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_certification_list_response.py
--rw-r--r--   0        0        0    10172 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_info_pictures_response_picture.py
--rw-r--r--   0        0        0     3910 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_product_unarchive_request.py
--rw-r--r--   0        0        0     4823 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/product_update_offer_id_request_update_offer_id.py
--rw-r--r--   0        0        0     5603 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_request.py
--rw-r--r--   0        0        0     3997 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response.py
--rw-r--r--   0        0        0    10380 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response_result.py
--rw-r--r--   0        0        0     7367 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_import_pictures_request.py
--rw-r--r--   0        0        0     3804 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_request.py
--rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_response.py
--rw-r--r--   0        0        0     3770 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_response_result.py
--rw-r--r--   0        0        0     3761 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_delete_products_request.py
--rw-r--r--   0        0        0     3761 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_delete_products_response.py
--rw-r--r--   0        0        0     6380 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_request.py
--rw-r--r--   0        0        0     3879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_response.py
--rw-r--r--   0        0        0     5628 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_discounted_stocks.py
--rw-r--r--   0        0        0     5748 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_request.py
--rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response.py
--rw-r--r--   0        0        0    44624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_item.py
--rw-r--r--   0        0        0     3794 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_result.py
--rw-r--r--   0        0        0     5633 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_source.py
--rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_stock.py
--rw-r--r--   0        0        0     7055 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_visibility_details.py
--rw-r--r--   0        0        0     5488 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_request.py
--rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response.py
--rw-r--r--   0        0        0     8461 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_commissions.py
--rw-r--r--   0        0        0    49953 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_result.py
--rw-r--r--   0        0        0     5565 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_source.py
--rw-r--r--   0        0        0     5370 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_stock.py
--rw-r--r--   0        0        0     5923 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_visibility_details.py
--rw-r--r--   0        0        0     5971 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request.py
--rw-r--r--   0        0        0     5899 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request_filter.py
--rw-r--r--   0        0        0     3876 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request_filter_filter_visibility.py
--rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response.py
--rw-r--r--   0        0        0     4731 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response_item.py
--rw-r--r--   0        0        0     5894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response_result.py
--rw-r--r--   0        0        0     3780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_request.py
--rw-r--r--   0        0        0     6663 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_request_stock.py
--rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response.py
--rw-r--r--   0        0        0     6341 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response_error.py
--rw-r--r--   0        0        0     7788 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response_result.py
--rw-r--r--   0        0        0    13864 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv2_status.py
--rw-r--r--   0        0        0     5563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_filter.py
--rw-r--r--   0        0        0     7900 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_request.py
--rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_response.py
--rw-r--r--   0        0        0    23310 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_response_result.py
--rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_request.py
--rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response.py
--rw-r--r--   0        0        0     5814 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_item.py
--rw-r--r--   0        0        0     6300 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_result.py
--rw-r--r--   0        0        0     5557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv4_filter.py
--rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv4_get_product_info_prices_v4_request.py
--rw-r--r--   0        0        0     3694 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/productv4_get_product_info_prices_v4_response.py
--rw-r--r--   0        0        0     4246 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/protobuf_any.py
--rw-r--r--   0        0        0     5299 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rating_item_change.py
--rw-r--r--   0        0        0     4526 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rating_summary_v1_response_group.py
--rw-r--r--   0        0        0     5744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rating_value.py
--rw-r--r--   0        0        0     4681 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/related_posting_cancel_reason.py
--rw-r--r--   0        0        0     6410 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/related_posting_cancel_reasons.py
--rw-r--r--   0        0        0     4513 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_postings_report_request.py
--rw-r--r--   0        0        0    12436 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_postings_report_request_filter.py
--rw-r--r--   0        0        0     7392 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_products_report_request.py
--rw-r--r--   0        0        0     2895 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_products_report_request_visibility.py
--rw-r--r--   0        0        0     4498 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_returns_report_request.py
--rw-r--r--   0        0        0     5812 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_returns_report_request_filter.py
--rw-r--r--   0        0        0     2811 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_discounted_request.py
--rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_discounted_response.py
--rw-r--r--   0        0        0     3533 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_create_report_response.py
--rw-r--r--   0        0        0     2751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_language.py
--rw-r--r--   0        0        0     2803 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_list_request_report_type.py
--rw-r--r--   0        0        0     4524 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_list_response_result.py
--rw-r--r--   0        0        0    10108 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_report.py
--rw-r--r--   0        0        0     3574 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_report_info_request.py
--rw-r--r--   0        0        0     3481 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_report_info_response.py
--rw-r--r--   0        0        0     5416 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_report_list_request.py
--rw-r--r--   0        0        0     3517 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/report_report_list_response.py
--rw-r--r--   0        0        0     4297 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/result_error.py
--rw-r--r--   0        0        0     3904 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/return_create_report_response_code.py
--rw-r--r--   0        0        0     3599 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returnreport_create_report_response.py
--rw-r--r--   0        0        0    19625 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_response_returns.py
--rw-r--r--   0        0        0     4427 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_available_action.py
--rw-r--r--   0        0        0     4443 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_client_return_method_type.py
--rw-r--r--   0        0        0     6512 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_rejection_reason.py
--rw-r--r--   0        0        0     5349 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_return_reason.py
--rw-r--r--   0        0        0     9839 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_list_response_returns.py
--rw-r--r--   0        0        0     4960 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rpc_status.py
--rw-r--r--   0        0        0     6060 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rpc_status_v1_polygon_bind.py
--rw-r--r--   0        0        0     6496 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/rpc_status_v1_polygon_create.py
--rw-r--r--   0        0        0     4629 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_activate_product_v1_request.py
--rw-r--r--   0        0        0     3765 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_actions_v1_response.py
--rw-r--r--   0        0        0     5838 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_request.py
--rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_response.py
--rw-r--r--   0        0        0     4750 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_response_result.py
--rw-r--r--   0        0        0     8936 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product.py
--rw-r--r--   0        0        0     4643 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_ids_v1_request.py
--rw-r--r--   0        0        0     5430 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_price.py
--rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response.py
--rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_deactivate.py
--rw-r--r--   0        0        0     4637 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_product.py
--rw-r--r--   0        0        0     4753 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_product_deactivate.py
--rw-r--r--   0        0        0     4985 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_result.py
--rw-r--r--   0        0        0     5131 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_result_deactivate.py
--rw-r--r--   0        0        0     2819 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/seller_serviceanalytics_dimension.py
--rw-r--r--   0        0        0     2743 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/sorting_order.py
--rw-r--r--   0        0        0     5680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_capacity.py
--rw-r--r--   0        0        0     4666 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_result.py
--rw-r--r--   0        0        0     5049 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_schedule.py
--rw-r--r--   0        0        0     4471 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_warehouse.py
--rw-r--r--   0        0        0     5002 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_activate_hot_sales_products_request.py
--rw-r--r--   0        0        0     5842 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_activate_hot_sales_products_request_activate_product.py
--rw-r--r--   0        0        0     3640 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_request.py
--rw-r--r--   0        0        0     3583 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_response.py
--rw-r--r--   0        0        0     5891 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_result.py
--rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_request.py
--rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_response.py
--rw-r--r--   0        0        0     4861 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_response_result.py
--rw-r--r--   0        0        0     3678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_decline_discount_tasks_response.py
--rw-r--r--   0        0        0     6176 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_decline_discount_tasks_response_result.py
--rw-r--r--   0        0        0     3680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_discount_tasks_request.py
--rw-r--r--   0        0        0     7994 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_discount_tasks_request_task.py
--rw-r--r--   0        0        0     4285 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_barcode.py
--rw-r--r--   0        0        0    12852 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_certificate.py
--rw-r--r--   0        0        0     4823 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_competitor.py
--rw-r--r--   0        0        0    16072 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_conditional_cancellation.py
--rw-r--r--   0        0        0     4811 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_conditional_cancellation_move_request.py
--rw-r--r--   0        0        0     3860 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_request.py
--rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_response.py
--rw-r--r--   0        0        0     3762 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_response_result.py
--rw-r--r--   0        0        0     4712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_request.py
--rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_response.py
--rw-r--r--   0        0        0     3796 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_response_result.py
--rw-r--r--   0        0        0     4619 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_create_stock_by_warehouse_report_request.py
--rw-r--r--   0        0        0     4933 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_deactivate_hot_sales_products_request.py
--rw-r--r--   0        0        0     3680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_decline_discount_tasks_request.py
--rw-r--r--   0        0        0     4591 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_decline_discount_tasks_request_task.py
--rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_delete_strategy_items_response.py
--rw-r--r--   0        0        0     3980 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_delete_strategy_items_response_result.py
--rw-r--r--   0        0        0     3070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_discount_task_status.py
--rw-r--r--   0        0        0     2723 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_empty.py
--rw-r--r--   0        0        0     3838 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_request.py
--rw-r--r--   0        0        0     3698 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_response.py
--rw-r--r--   0        0        0     6169 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_result.py
--rw-r--r--   0        0        0     8772 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_request.py
--rw-r--r--   0        0        0     5334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_response.py
--rw-r--r--   0        0        0     6331 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_response_dictionary_value.py
--rw-r--r--   0        0        0     5473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_request.py
--rw-r--r--   0        0        0     3665 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_response.py
--rw-r--r--   0        0        0    17668 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_response_attribute.py
--rw-r--r--   0        0        0     4735 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_competitors_request.py
--rw-r--r--   0        0        0     4570 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_competitors_response.py
--rw-r--r--   0        0        0     6681 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_list_request.py
--rw-r--r--   0        0        0     5621 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_list_response.py
--rw-r--r--   0        0        0     3978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_request.py
--rw-r--r--   0        0        0     3616 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_response.py
--rw-r--r--   0        0        0     5313 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_request.py
--rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_response.py
--rw-r--r--   0        0        0    39907 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_response_task.py
--rw-r--r--   0        0        0     3414 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_etgb_request.py
--rw-r--r--   0        0        0     3584 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_etgb_response.py
--rw-r--r--   0        0        0     2791 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_list_request.py
--rw-r--r--   0        0        0     3697 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_list_response.py
--rw-r--r--   0        0        0     5790 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_request.py
--rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_response.py
--rw-r--r--   0        0        0     4678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_response_result.py
--rw-r--r--   0        0        0     3956 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_request.py
--rw-r--r--   0        0        0     3524 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_response.py
--rw-r--r--   0        0        0     5770 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_response_result.py
--rw-r--r--   0        0        0     3872 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_request.py
--rw-r--r--   0        0        0     3827 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_response.py
--rw-r--r--   0        0        0    16340 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_response_item.py
--rw-r--r--   0        0        0     3736 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_request.py
--rw-r--r--   0        0        0     3821 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_response.py
--rw-r--r--   0        0        0     4633 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_response_result.py
--rw-r--r--   0        0        0     3748 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_rating_by_sku_request.py
--rw-r--r--   0        0        0     3821 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_rating_by_sku_response.py
--rw-r--r--   0        0        0     3981 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_restrictions_request.py
--rw-r--r--   0        0        0     3492 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_restrictions_response.py
--rw-r--r--   0        0        0     3634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response.py
--rw-r--r--   0        0        0     3969 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response_result.py
--rw-r--r--   0        0        0     3692 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_request.py
--rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_response.py
--rw-r--r--   0        0        0     9624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_response_result.py
--rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_items_response.py
--rw-r--r--   0        0        0     3742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_items_response_result.py
--rw-r--r--   0        0        0     4743 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_list_request.py
--rw-r--r--   0        0        0     4551 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_list_response.py
--rw-r--r--   0        0        0     3502 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_response.py
--rw-r--r--   0        0        0     7978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_response_result.py
--rw-r--r--   0        0        0     5843 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_items_request.py
--rw-r--r--   0        0        0     6329 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_items_response.py
--rw-r--r--   0        0        0     3890 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_request.py
--rw-r--r--   0        0        0    20230 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_response.py
--rw-r--r--   0        0        0     8173 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_orders_list_request.py
--rw-r--r--   0        0        0     6678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_orders_list_response.py
--rw-r--r--   0        0        0     3469 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_request.py
--rw-r--r--   0        0        0     3580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_response.py
--rw-r--r--   0        0        0     8332 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_response_item.py
--rw-r--r--   0        0        0     5550 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_barcode_reset_response.py
--rw-r--r--   0        0        0     2787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_delivery_schema.py
--rw-r--r--   0        0        0     3678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_barcode_response.py
--rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_pdf_response.py
--rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_png_response.py
--rw-r--r--   0        0        0     3636 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_info_request.py
--rw-r--r--   0        0        0     7290 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_info_response.py
--rw-r--r--   0        0        0     3769 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_is_enabled_response.py
--rw-r--r--   0        0        0     4449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_list_request.py
--rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_list_response.py
--rw-r--r--   0        0        0     2755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_status.py
--rw-r--r--   0        0        0     9047 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_hot_sale_product.py
--rw-r--r--   0        0        0     9894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_create_or_update_request.py
--rw-r--r--   0        0        0     3649 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_create_or_update_response.py
--rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_delete_request.py
--rw-r--r--   0        0        0     3585 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_delete_response.py
--rw-r--r--   0        0        0     3688 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_get_request.py
--rw-r--r--   0        0        0     3485 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_get_response.py
--rw-r--r--   0        0        0    10461 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_item_error.py
--rw-r--r--   0        0        0     3760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_item_ids_request.py
--rw-r--r--   0        0        0     4841 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_delivery_interval.py
--rw-r--r--   0        0        0     3896 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_request.py
--rw-r--r--   0        0        0     5264 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_response.py
--rw-r--r--   0        0        0     4580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_new_timeslot.py
--rw-r--r--   0        0        0     4678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_request.py
--rw-r--r--   0        0        0     3647 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_response.py
--rw-r--r--   0        0        0     4342 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_premium_scores.py
--rw-r--r--   0        0        0     3925 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_request.py
--rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_response.py
--rw-r--r--   0        0        0     4960 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_response_result.py
--rw-r--r--   0        0        0     3993 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_info_request.py
--rw-r--r--   0        0        0     3548 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_info_response.py
--rw-r--r--   0        0        0     8255 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_request.py
--rw-r--r--   0        0        0     3623 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_response.py
--rw-r--r--   0        0        0     4793 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_response_result.py
--rw-r--r--   0        0        0     2871 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_product_status_list_request.py
--rw-r--r--   0        0        0     3827 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_product_status_list_response.py
--rw-r--r--   0        0        0     7369 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_request.py
--rw-r--r--   0        0        0     3711 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_response.py
--rw-r--r--   0        0        0     4745 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_response_result.py
--rw-r--r--   0        0        0     2883 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_request.py
--rw-r--r--   0        0        0     3906 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_response.py
--rw-r--r--   0        0        0     2843 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_status_list_request.py
--rw-r--r--   0        0        0     3853 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_status_list_response.py
--rw-r--r--   0        0        0     5117 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_unbind_request.py
--rw-r--r--   0        0        0     3787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_unbind_response.py
--rw-r--r--   0        0        0     3532 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_request.py
--rw-r--r--   0        0        0     4608 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response.py
--rw-r--r--   0        0        0     5216 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response_error.py
--rw-r--r--   0        0        0     7725 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response_item.py
--rw-r--r--   0        0        0     3839 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request.py
--rw-r--r--   0        0        0     6134 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_attribute.py
--rw-r--r--   0        0        0     4747 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_item.py
--rw-r--r--   0        0        0     4873 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_value.py
--rw-r--r--   0        0        0     4148 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_response.py
--rw-r--r--   0        0        0     4607 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_discount_request.py
--rw-r--r--   0        0        0     3785 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_discount_response.py
--rw-r--r--   0        0        0     4037 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_request.py
--rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_response.py
--rw-r--r--   0        0        0     4651 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_response_error.py
--rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_request.py
--rw-r--r--   0        0        0     4070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_request_info.py
--rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response.py
--rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_info.py
--rw-r--r--   0        0        0     4132 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_info_result.py
--rw-r--r--   0        0        0     3762 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_result.py
--rw-r--r--   0        0        0     7682 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating.py
--rw-r--r--   0        0        0    12176 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_history_v1_request.py
--rw-r--r--   0        0        0     4778 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_history_v1_response.py
--rw-r--r--   0        0        0    10518 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_item.py
--rw-r--r--   0        0        0     5649 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_status.py
--rw-r--r--   0        0        0     5767 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_summary_v1_response.py
--rw-r--r--   0        0        0    10413 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_restriction.py
--rw-r--r--   0        0        0     5098 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_seller_warehouse.py
--rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result.py
--rw-r--r--   0        0        0     4733 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result_product.py
--rw-r--r--   0        0        0     3990 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result_result.py
--rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result.py
--rw-r--r--   0        0        0     4753 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_product.py
--rw-r--r--   0        0        0     4012 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_result.py
--rw-r--r--   0        0        0     4317 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair.py
--rw-r--r--   0        0        0     4475 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair_rejection.py
--rw-r--r--   0        0        0     4333 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair_statuses.py
--rw-r--r--   0        0        0     3636 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_strategy_request.py
--rw-r--r--   0        0        0     3826 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_supplier_available_warehouses_response.py
--rw-r--r--   0        0        0     4066 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_timeslot.py
--rw-r--r--   0        0        0     5639 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_update_pricing_strategy_request.py
--rw-r--r--   0        0        0     4682 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_update_status_strategy_request.py
--rw-r--r--   0        0        0     6177 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_vehicle_info.py
--rw-r--r--   0        0        0     5002 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v1_warehouse.py
--rw-r--r--   0        0        0     3991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_additional_data_item.py
--rw-r--r--   0        0        0     4786 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_history_response.py
--rw-r--r--   0        0        0     5589 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_list_response.py
--rw-r--r--   0        0        0     6648 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_message.py
--rw-r--r--   0        0        0     3730 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_read_response.py
--rw-r--r--   0        0        0    13045 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting.py
--rw-r--r--   0        0        0     3617 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting_list_response.py
--rw-r--r--   0        0        0     3449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting_response.py
--rw-r--r--   0        0        0    13676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting.py
--rw-r--r--   0        0        0     7709 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product.py
--rw-r--r--   0        0        0     3782 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_request.py
--rw-r--r--   0        0        0     3887 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_response.py
--rw-r--r--   0        0        0     4781 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_response_result.py
--rw-r--r--   0        0        0     6404 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_set_request.py
--rw-r--r--   0        0        0     5068 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_set_response.py
--rw-r--r--   0        0        0     3449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_response.py
--rw-r--r--   0        0        0     4904 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_get_geo_restrictions_by_filter_request_filter.py
--rw-r--r--   0        0        0     9676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_item_error.py
--rw-r--r--   0        0        0     3579 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_request.py
--rw-r--r--   0        0        0     3787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_response.py
--rw-r--r--   0        0        0    10330 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_result.py
--rw-r--r--   0        0        0     6906 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_products.py
--rw-r--r--   0        0        0     9003 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_filter.py
--rw-r--r--   0        0        0     5780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs.py
--rw-r--r--   0        0        0     5706 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_acceptance.py
--rw-r--r--   0        0        0     5084 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_excess.py
--rw-r--r--   0        0        0     5608 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_mismatch.py
--rw-r--r--   0        0        0     4465 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_request.py
--rw-r--r--   0        0        0     3676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_response.py
--rw-r--r--   0        0        0    17557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_result.py
--rw-r--r--   0        0        0     4010 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_request.py
--rw-r--r--   0        0        0     5289 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_response.py
--rw-r--r--   0        0        0     4799 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_request.py
--rw-r--r--   0        0        0     3720 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_response.py
--rw-r--r--   0        0        0     3552 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_request.py
--rw-r--r--   0        0        0     5566 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_response.py
--rw-r--r--   0        0        0     3676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_text_response.py
--rw-r--r--   0        0        0     5172 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_digital_act_request.py
--rw-r--r--   0        0        0     5580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_digital_act_response.py
--rw-r--r--   0        0        0     6520 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_financial_data.py
--rw-r--r--   0        0        0     9300 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_product.py
--rw-r--r--   0        0        0     7294 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_product.py
--rw-r--r--   0        0        0     3744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response.py
--rw-r--r--   0        0        0     5151 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response_result.py
--rw-r--r--   0        0        0     4703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response_type.py
--rw-r--r--   0        0        0     4879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_compensate_request.py
--rw-r--r--   0        0        0     6759 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_filter.py
--rw-r--r--   0        0        0     3720 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_request.py
--rw-r--r--   0        0        0     3552 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_response.py
--rw-r--r--   0        0        0     4485 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_v2_response_state.py
--rw-r--r--   0        0        0     5500 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_request.py
--rw-r--r--   0        0        0     3563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_response.py
--rw-r--r--   0        0        0     6699 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_v2_response_state.py
--rw-r--r--   0        0        0     3840 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_receive_return_request.py
--rw-r--r--   0        0        0     6674 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_reject_request.py
--rw-r--r--   0        0        0     5009 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_return_money_request.py
--rw-r--r--   0        0        0     4969 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_verify_request.py
--rw-r--r--   0        0        0     4435 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v2_user.py
--rw-r--r--   0        0        0     3991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_additional_data_item.py
--rw-r--r--   0        0        0    11268 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_address.py
--rw-r--r--   0        0        0     4123 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_addressee.py
--rw-r--r--   0        0        0     4359 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_addressee_fbs_lists.py
--rw-r--r--   0        0        0     4643 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_barcodes.py
--rw-r--r--   0        0        0     9471 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_cancellation.py
--rw-r--r--   0        0        0     6478 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_customer.py
--rw-r--r--   0        0        0     6810 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_customer_fbs_lists.py
--rw-r--r--   0        0        0     7721 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_delivery_method.py
--rw-r--r--   0        0        0     5621 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_dimensions.py
--rw-r--r--   0        0        0    32656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting.py
--rw-r--r--   0        0        0    14163 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_analytics_data.py
--rw-r--r--   0        0        0    37377 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_detail.py
--rw-r--r--   0        0        0     4070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_detail_related_postings.py
--rw-r--r--   0        0        0     4619 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_exemplar_product_v3.py
--rw-r--r--   0        0        0     9374 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product.py
--rw-r--r--   0        0        0     8797 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product_exemplar_info_v3.py
--rw-r--r--   0        0        0     3638 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product_exemplars_v3.py
--rw-r--r--   0        0        0    11742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_requirements_v3.py
--rw-r--r--   0        0        0     6742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_request.py
--rw-r--r--   0        0        0     3689 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response.py
--rw-r--r--   0        0        0     5274 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_period.py
--rw-r--r--   0        0        0     5805 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_result.py
--rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_list_response_v3.py
--rw-r--r--   0        0        0     5543 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_list_response_v3_result.py
--rw-r--r--   0        0        0     3507 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_response_v3.py
--rw-r--r--   0        0        0     5844 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbo_v3_request.py
--rw-r--r--   0        0        0     4697 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbo_v3_response.py
--rw-r--r--   0        0        0     5774 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbs_v3_request.py
--rw-r--r--   0        0        0     5019 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbs_v3_response.py
--rw-r--r--   0        0        0     3614 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request.py
--rw-r--r--   0        0        0     6377 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_attribute.py
--rw-r--r--   0        0        0     3759 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_complex_attribute.py
--rw-r--r--   0        0        0     4809 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_dictionary_value.py
--rw-r--r--   0        0        0    32162 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_item.py
--rw-r--r--   0        0        0     3535 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_response.py
--rw-r--r--   0        0        0     3694 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_response_result.py
--rw-r--r--   0        0        0     6520 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_posting_financial_data.py
--rw-r--r--   0        0        0    11308 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_posting_product_detail.py
--rw-r--r--   0        0        0     4903 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_returns_company_filter_fbo.py
--rw-r--r--   0        0        0     9024 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_returns_company_filter_fbs.py
--rw-r--r--   0        0        0     2868 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v3_service_type.py
--rw-r--r--   0        0        0     4902 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request.py
--rw-r--r--   0        0        0     5913 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request_product.py
--rw-r--r--   0        0        0     3752 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_response.py
--rw-r--r--   0        0        0     5256 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v4_get_upload_quota_response.py
--rw-r--r--   0        0        0     4005 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_request.py
--rw-r--r--   0        0        0     6110 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response.py
--rw-r--r--   0        0        0    10108 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product.py
--rw-r--r--   0        0        0    10780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product_exemplar.py
--rw-r--r--   0        0        0     6119 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request.py
--rw-r--r--   0        0        0     9918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product.py
--rw-r--r--   0        0        0    10582 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product_exemplar.py
--rw-r--r--   0        0        0     3867 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_response.py
--rw-r--r--   0        0        0     5760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/warehouse_delivery_method_list_request.py
--rw-r--r--   0        0        0     5351 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/warehouse_delivery_method_list_response.py
--rw-r--r--   0        0        0     7376 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/warehouse_first_mile_type.py
--rw-r--r--   0        0        0    20215 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/warehouse_list_response_warehouse.py
--rw-r--r--   0        0        0     3703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/models/warehouse_warehouse_list_response.py
--rw-r--r--   0        0        0    13320 2024-03-20 09:50:50.000000 ozon_api_client-0.0.4/ozon_api_client/rest.py
--rw-r--r--   0        0        0      403 2024-03-20 13:52:12.788868 ozon_api_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    92759 1970-01-01 00:00:00.000000 ozon_api_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    96029 2024-04-09 09:09:14.000000 ozon_api_client-0.0.5/README.md
+-rw-r--r--   0        0        0    70903 2024-03-20 13:08:55.232514 ozon_api_client-0.0.5/ozon_api_client/__init__.py
+-rw-r--r--   0        0        0     1540 2024-03-20 13:08:55.313909 ozon_api_client-0.0.5/ozon_api_client/api/__init__.py
+-rw-r--r--   0        0        0    12841 2024-03-20 13:08:55.732365 ozon_api_client-0.0.5/ozon_api_client/api/analytics_api_api.py
+-rw-r--r--   0        0        0    11016 2024-03-20 13:08:55.796024 ozon_api_client-0.0.5/ozon_api_client/api/barcode_api_api.py
+-rw-r--r--   0        0        0     7370 2024-03-20 13:08:55.138752 ozon_api_client-0.0.5/ozon_api_client/api/brand_api_api.py
+-rw-r--r--   0        0        0    24123 2024-03-20 13:08:54.933560 ozon_api_client-0.0.5/ozon_api_client/api/cancellation_api_api.py
+-rw-r--r--   0        0        0    19449 2024-03-20 13:08:55.736657 ozon_api_client-0.0.5/ozon_api_client/api/category_api_api.py
+-rw-r--r--   0        0        0    63927 2024-03-20 13:08:54.880946 ozon_api_client-0.0.5/ozon_api_client/api/certification_api_api.py
+-rw-r--r--   0        0        0    32367 2024-03-20 13:08:54.953498 ozon_api_client-0.0.5/ozon_api_client/api/chat_api_api.py
+-rw-r--r--   0        0        0    34465 2024-03-20 13:08:55.155750 ozon_api_client-0.0.5/ozon_api_client/api/fbo_api.py
+-rw-r--r--   0        0        0   218207 2024-03-20 13:08:54.852669 ozon_api_client-0.0.5/ozon_api_client/api/fbs_api.py
+-rw-r--r--   0        0        0    51898 2024-03-20 13:08:54.817343 ozon_api_client-0.0.5/ozon_api_client/api/fbsr_fbs_marks_api.py
+-rw-r--r--   0        0        0    19230 2024-03-20 13:08:55.590615 ozon_api_client-0.0.5/ozon_api_client/api/finance_api_api.py
+-rw-r--r--   0        0        0    11762 2024-03-20 13:08:55.131653 ozon_api_client-0.0.5/ozon_api_client/api/polygon_api_api.py
+-rw-r--r--   0        0        0    49168 2024-03-20 13:08:55.001110 ozon_api_client-0.0.5/ozon_api_client/api/prices_stocks_api_api.py
+-rw-r--r--   0        0        0    46970 2024-03-20 13:08:55.227205 ozon_api_client-0.0.5/ozon_api_client/api/pricing_strategy_api_api.py
+-rw-r--r--   0        0        0   140217 2024-03-20 13:08:55.302869 ozon_api_client-0.0.5/ozon_api_client/api/product_api_api.py
+-rw-r--r--   0        0        0    48513 2024-03-20 13:08:55.346639 ozon_api_client-0.0.5/ozon_api_client/api/promos_api.py
+-rw-r--r--   0        0        0    57166 2024-03-20 13:08:55.623046 ozon_api_client-0.0.5/ozon_api_client/api/report_api_api.py
+-rw-r--r--   0        0        0    37321 2024-03-20 13:08:55.218520 ozon_api_client-0.0.5/ozon_api_client/api/return_api_api.py
+-rw-r--r--   0        0        0     9794 2024-03-20 13:08:55.658984 ozon_api_client-0.0.5/ozon_api_client/api/returns_api_api.py
+-rw-r--r--   0        0        0    39878 2024-03-20 13:08:54.827228 ozon_api_client-0.0.5/ozon_api_client/api/rfbs_returns_api_api.py
+-rw-r--r--   0        0        0     8920 2024-03-20 13:08:55.733840 ozon_api_client-0.0.5/ozon_api_client/api/seller_rating_api.py
+-rw-r--r--   0        0        0    12746 2024-03-20 13:08:55.091479 ozon_api_client-0.0.5/ozon_api_client/api/supplier_api_api.py
+-rw-r--r--   0        0        0    10914 2024-03-20 13:08:55.158738 ozon_api_client-0.0.5/ozon_api_client/api/warehouse_api_api.py
+-rw-r--r--   0        0        0    25375 2024-03-20 13:08:55.340695 ozon_api_client-0.0.5/ozon_api_client/api_client.py
+-rw-r--r--   0        0        0     8388 2024-03-20 13:08:55.390475 ozon_api_client-0.0.5/ozon_api_client/configuration.py
+-rw-r--r--   0        0        0    69296 2024-03-20 13:08:54.869242 ozon_api_client-0.0.5/ozon_api_client/models/__init__.py
+-rw-r--r--   0        0        0     5190 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/add_strategy_items_response_error.py
+-rw-r--r--   0        0        0    15912 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_analytics_get_data_request.py
+-rw-r--r--   0        0        0     4496 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_analytics_get_data_response.py
+-rw-r--r--   0        0        0     4517 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_data_row.py
+-rw-r--r--   0        0        0     4187 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_data_row_dimension.py
+-rw-r--r--   0        0        0     5033 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_filter.py
+-rw-r--r--   0        0        0     4506 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_get_data_response_result.py
+-rw-r--r--   0        0        0     3048 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_get_stock_on_warehouses_request_warehouse_type.py
+-rw-r--r--   0        0        0     2755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_metric.py
+-rw-r--r--   0        0        0     4228 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_sorting.py
+-rw-r--r--   0        0        0     5918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_request.py
+-rw-r--r--   0        0        0     3634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_response.py
+-rw-r--r--   0        0        0     3812 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_response_result.py
+-rw-r--r--   0        0        0    10216 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_result_rows.py
+-rw-r--r--   0        0        0     4771 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/approve_decline_discount_tasks_response_fail_detail.py
+-rw-r--r--   0        0        0     4703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/brand_brand_company_certification_list_request.py
+-rw-r--r--   0        0        0     3772 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/brand_brand_company_certification_list_response.py
+-rw-r--r--   0        0        0     5246 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/brand_company_certification_list_response_brand_certification.py
+-rw-r--r--   0        0        0     5303 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/brand_company_certification_list_response_brand_certification_result.py
+-rw-r--r--   0        0        0    11334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/certificate_create_body.py
+-rw-r--r--   0        0        0     5308 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_file_request.py
+-rw-r--r--   0        0        0     3606 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_file_response.py
+-rw-r--r--   0        0        0     4405 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_message_request.py
+-rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_message_response.py
+-rw-r--r--   0        0        0     3728 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_start_request.py
+-rw-r--r--   0        0        0     3490 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_start_response.py
+-rw-r--r--   0        0        0     7093 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_history.py
+-rw-r--r--   0        0        0     9357 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_info.py
+-rw-r--r--   0        0        0     5404 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_list.py
+-rw-r--r--   0        0        0     4958 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_list_request_filter.py
+-rw-r--r--   0        0        0     4563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_read.py
+-rw-r--r--   0        0        0     3584 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/chat_start_response_result.py
+-rw-r--r--   0        0        0     3533 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/common_create_report_response.py
+-rw-r--r--   0        0        0     7329 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/common_price_indexes.py
+-rw-r--r--   0        0        0    15020 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/common_returns_company_item_fbo.py
+-rw-r--r--   0        0        0    30723 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/common_returns_company_item_fbs.py
+-rw-r--r--   0        0        0     4985 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/common_time_range_last_day.py
+-rw-r--r--   0        0        0     4495 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/conditional_cancellation_cancellation_reason.py
+-rw-r--r--   0        0        0     5620 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/conditional_cancellation_state.py
+-rw-r--r--   0        0        0     3582 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/create_report_response_code.py
+-rw-r--r--   0        0        0     4120 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/created_at.py
+-rw-r--r--   0        0        0     3760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/delete_products_request_product.py
+-rw-r--r--   0        0        0     5779 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/delete_products_response_delete_status.py
+-rw-r--r--   0        0        0     5834 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/delivery_method_list_request_filter.py
+-rw-r--r--   0        0        0    12629 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/delivery_method_list_response_delivery_method.py
+-rw-r--r--   0        0        0     5334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_delivery_details.py
+-rw-r--r--   0        0        0     4181 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_others.py
+-rw-r--r--   0        0        0     4335 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_payment.py
+-rw-r--r--   0        0        0     5263 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_return_details.py
+-rw-r--r--   0        0        0     4193 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_returns.py
+-rw-r--r--   0        0        0     9333 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_rfbs_details.py
+-rw-r--r--   0        0        0     4175 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_service.py
+-rw-r--r--   0        0        0     4211 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/details_services.py
+-rw-r--r--   0        0        0    10453 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbo_posting_fbo_posting_analytics_data.py
+-rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_barcodes.py
+-rw-r--r--   0        0        0     5955 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_detail_courier.py
+-rw-r--r--   0        0        0     6995 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_detail_prr_option.py
+-rw-r--r--   0        0        0     8525 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_fbs_posting_analytics_data.py
+-rw-r--r--   0        0        0     5605 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_move_status_response_move_status.py
+-rw-r--r--   0        0        0     4314 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result.py
+-rw-r--r--   0        0        0     7844 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product.py
+-rw-r--r--   0        0        0    10226 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product_exemplar.py
+-rw-r--r--   0        0        0     3816 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_package.py
+-rw-r--r--   0        0        0     4655 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_package_product.py
+-rw-r--r--   0        0        0     3917 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_with.py
+-rw-r--r--   0        0        0     4938 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_response_ship_additional_data.py
+-rw-r--r--   0        0        0     5025 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_tracking_number_set_request_tracking_number.py
+-rw-r--r--   0        0        0     5680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_request.py
+-rw-r--r--   0        0        0     4874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_response.py
+-rw-r--r--   0        0        0     3824 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_request.py
+-rw-r--r--   0        0        0     6179 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response.py
+-rw-r--r--   0        0        0     4934 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product.py
+-rw-r--r--   0        0        0    21322 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product_exemplar.py
+-rw-r--r--   0        0        0    10112 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_posting_product_detail_without_dimensions.py
+-rw-r--r--   0        0        0     4727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request.py
+-rw-r--r--   0        0        0     4899 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request_product.py
+-rw-r--r--   0        0        0     9179 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request_product_exemplar.py
+-rw-r--r--   0        0        0     3795 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_response.py
+-rw-r--r--   0        0        0     2727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/filter_op.py
+-rw-r--r--   0        0        0     4456 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/filter_period.py
+-rw-r--r--   0        0        0    10569 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_cash_flow.py
+-rw-r--r--   0        0        0     5735 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_delivery_service.py
+-rw-r--r--   0        0        0    12749 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_details.py
+-rw-r--r--   0        0        0     5897 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_details_others.py
+-rw-r--r--   0        0        0     5557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_return_service.py
+-rw-r--r--   0        0        0     7535 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_service.py
+-rw-r--r--   0        0        0     3675 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_get_realization_report_request.py
+-rw-r--r--   0        0        0     3755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_get_realization_report_response.py
+-rw-r--r--   0        0        0    15984 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_header.py
+-rw-r--r--   0        0        0     4573 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_result.py
+-rw-r--r--   0        0        0    24348 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_rows.py
+-rw-r--r--   0        0        0    15083 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_list_v3_request_filter.py
+-rw-r--r--   0        0        0    17234 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_list_v3_response_operation.py
+-rw-r--r--   0        0        0     4756 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_totals_v3_request_date.py
+-rw-r--r--   0        0        0     5522 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_request.py
+-rw-r--r--   0        0        0     3722 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_response.py
+-rw-r--r--   0        0        0     5876 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_response_result.py
+-rw-r--r--   0        0        0     6301 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_request.py
+-rw-r--r--   0        0        0     3744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_response.py
+-rw-r--r--   0        0        0    14909 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_response_result.py
+-rw-r--r--   0        0        0     4473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/financev3_period.py
+-rw-r--r--   0        0        0    21918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_carriage_available_list_response_result.py
+-rw-r--r--   0        0        0     4407 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_competitors_response_competitor_info.py
+-rw-r--r--   0        0        0     8136 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_request_filters.py
+-rw-r--r--   0        0        0     3931 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_request_with.py
+-rw-r--r--   0        0        0     5822 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_response_counters.py
+-rw-r--r--   0        0        0     4168 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_request_date.py
+-rw-r--r--   0        0        0     4383 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_response_result.py
+-rw-r--r--   0        0        0     5211 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_response_result_etgb.py
+-rw-r--r--   0        0        0     6938 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_geo_restrictions_by_filter_response_geo_restriction.py
+-rw-r--r--   0        0        0     9879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_hot_sales_list_response_hot_sale.py
+-rw-r--r--   0        0        0     7387 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_import_products_info_response_result_item.py
+-rw-r--r--   0        0        0     5301 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_image.py
+-rw-r--r--   0        0        0     4303 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_image360.py
+-rw-r--r--   0        0        0     5340 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_pdf.py
+-rw-r--r--   0        0        0     6640 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_v3_response_attribute.py
+-rw-r--r--   0        0        0     4967 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_v3_response_dictionary_value.py
+-rw-r--r--   0        0        0     4475 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_list_response_reason.py
+-rw-r--r--   0        0        0     3783 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_list_response_reasons.py
+-rw-r--r--   0        0        0     5282 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_stocks_v3_response_stock.py
+-rw-r--r--   0        0        0     5739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_product_rating.py
+-rw-r--r--   0        0        0     6618 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_condition.py
+-rw-r--r--   0        0        0    10309 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_group.py
+-rw-r--r--   0        0        0     4571 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_improve_attribute.py
+-rw-r--r--   0        0        0    19464 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_seller_actions_v1_response_action.py
+-rw-r--r--   0        0        0     4873 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_strategy_ids_by_item_ids_response_product_info.py
+-rw-r--r--   0        0        0    10790 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_strategy_list_response_strategy.py
+-rw-r--r--   0        0        0     6986 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_supply_order_items_response_item.py
+-rw-r--r--   0        0        0    19218 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_supply_orders_list_response_supply_order.py
+-rw-r--r--   0        0        0     5653 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_daily_create.py
+-rw-r--r--   0        0        0     5665 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_daily_update.py
+-rw-r--r--   0        0        0     4511 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_total.py
+-rw-r--r--   0        0        0     6338 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/giveout_info_response_article_details.py
+-rw-r--r--   0        0        0    10894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/giveout_list_response_giveout_details.py
+-rw-r--r--   0        0        0     5056 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/googlerpc_status.py
+-rw-r--r--   0        0        0     5242 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/import_products_request_pdf_list.py
+-rw-r--r--   0        0        0     3624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/invoice_get_response_result.py
+-rw-r--r--   0        0        0    25953 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/item_commissions.py
+-rw-r--r--   0        0        0     7518 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/item_marketing_actions.py
+-rw-r--r--   0        0        0    15056 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/item_price.py
+-rw-r--r--   0        0        0     2890 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/language_language.py
+-rw-r--r--   0        0        0     6473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/marketing_actions_marketing_action.py
+-rw-r--r--   0        0        0     4165 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/operation_item.py
+-rw-r--r--   0        0        0     6859 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/operation_posting.py
+-rw-r--r--   0        0        0    11115 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/operation_service.py
+-rw-r--r--   0        0        0     4565 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygon_bind_requestpolygon.py
+-rw-r--r--   0        0        0     4463 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygon_bind_requestwh_location.py
+-rw-r--r--   0        0        0     2751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_empty.py
+-rw-r--r--   0        0        0     5781 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_bind_request.py
+-rw-r--r--   0        0        0     3822 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_create_request.py
+-rw-r--r--   0        0        0     3716 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_create_response.py
+-rw-r--r--   0        0        0     3737 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_boolean_response.py
+-rw-r--r--   0        0        0     6226 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_fbs_posting_request.py
+-rw-r--r--   0        0        0     7656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason.py
+-rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_list_response.py
+-rw-r--r--   0        0        0     3946 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_request.py
+-rw-r--r--   0        0        0     3679 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_response.py
+-rw-r--r--   0        0        0     4981 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbo_posting_with_params.py
+-rw-r--r--   0        0        0    14274 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_act_check_status_response_status.py
+-rw-r--r--   0        0        0     3666 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_act_create_response_act.py
+-rw-r--r--   0        0        0     3850 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_delivered_request.py
+-rw-r--r--   0        0        0     3858 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_delivering_request.py
+-rw-r--r--   0        0        0     3842 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_last_mile_request.py
+-rw-r--r--   0        0        0     3801 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_move_status_response.py
+-rw-r--r--   0        0        0     3908 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_request.py
+-rw-r--r--   0        0        0     3826 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_response.py
+-rw-r--r--   0        0        0     5417 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_response_item.py
+-rw-r--r--   0        0        0     4195 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_tracking_number_set_request.py
+-rw-r--r--   0        0        0    17884 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_financial_data_product.py
+-rw-r--r--   0        0        0    19874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_financial_data_services.py
+-rw-r--r--   0        0        0     8557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_list_request.py
+-rw-r--r--   0        0        0     5836 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_list_request_filter.py
+-rw-r--r--   0        0        0     5492 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_request.py
+-rw-r--r--   0        0        0     3696 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbs_posting_by_barcode_request.py
+-rw-r--r--   0        0        0     3786 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_move_posting_request.py
+-rw-r--r--   0        0        0     3994 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_check_status_request.py
+-rw-r--r--   0        0        0     3679 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_check_status_response.py
+-rw-r--r--   0        0        0     6891 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_create_request.py
+-rw-r--r--   0        0        0     3615 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_create_response.py
+-rw-r--r--   0        0        0     4050 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_request.py
+-rw-r--r--   0        0        0     5788 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_response.py
+-rw-r--r--   0        0        0     3930 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_get_act_request.py
+-rw-r--r--   0        0        0     5548 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_get_act_response.py
+-rw-r--r--   0        0        0     3874 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_package_label_request.py
+-rw-r--r--   0        0        0     5644 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_package_label_response.py
+-rw-r--r--   0        0        0     7141 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_cancel_request.py
+-rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_cancel_response.py
+-rw-r--r--   0        0        0     4751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_change_request.py
+-rw-r--r--   0        0        0     3688 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_change_response.py
+-rw-r--r--   0        0        0     4537 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_product_cancel_request_item.py
+-rw-r--r--   0        0        0     4618 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/posting_product_change_request_item.py
+-rw-r--r--   0        0        0     5072 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv1_get_carriage_available_list_request.py
+-rw-r--r--   0        0        0     3849 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv1_get_carriage_available_list_response.py
+-rw-r--r--   0        0        0     6727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_fbs_posting_with_params.py
+-rw-r--r--   0        0        0     9573 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_fbs_posting_with_params_examplars.py
+-rw-r--r--   0        0        0     7483 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_list_request.py
+-rw-r--r--   0        0        0    11542 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_list_request_filter.py
+-rw-r--r--   0        0        0     4569 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_request.py
+-rw-r--r--   0        0        0     7780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request.py
+-rw-r--r--   0        0        0    13515 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request_filter.py
+-rw-r--r--   0        0        0     3766 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response.py
+-rw-r--r--   0        0        0     4898 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response_result.py
+-rw-r--r--   0        0        0     5023 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_request.py
+-rw-r--r--   0        0        0     3711 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response.py
+-rw-r--r--   0        0        0     4087 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response_result.py
+-rw-r--r--   0        0        0     5012 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request.py
+-rw-r--r--   0        0        0     5114 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product.py
+-rw-r--r--   0        0        0     7214 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product_exemplar.py
+-rw-r--r--   0        0        0     3893 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_response.py
+-rw-r--r--   0        0        0     5450 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/premium_scores_score.py
+-rw-r--r--   0        0        0     6026 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_external.py
+-rw-r--r--   0        0        0     5912 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_ozon.py
+-rw-r--r--   0        0        0     5940 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_self.py
+-rw-r--r--   0        0        0     3729 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_boolean_response.py
+-rw-r--r--   0        0        0     5073 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_certificate_products_list_response_product.py
+-rw-r--r--   0        0        0     5699 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_certificate_unbind_response_item.py
+-rw-r--r--   0        0        0     4978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_certification_list_response_certification.py
+-rw-r--r--   0        0        0     5011 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_certification_list_response_certification_result.py
+-rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_request.py
+-rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_response.py
+-rw-r--r--   0        0        0     4741 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_response_result.py
+-rw-r--r--   0        0        0     6773 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_attribute.py
+-rw-r--r--   0        0        0     4044 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_complex_attribute.py
+-rw-r--r--   0        0        0     5053 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_dictionary_value.py
+-rw-r--r--   0        0        0     4779 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_request.py
+-rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_response.py
+-rw-r--r--   0        0        0     6423 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_response_product.py
+-rw-r--r--   0        0        0    11732 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_prices_v4_response_item.py
+-rw-r--r--   0        0        0     6060 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_prices_v4_response_result.py
+-rw-r--r--   0        0        0     3750 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_request.py
+-rw-r--r--   0        0        0    12687 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_request_item.py
+-rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_response.py
+-rw-r--r--   0        0        0     4905 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_response_result.py
+-rw-r--r--   0        0        0     3806 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_request.py
+-rw-r--r--   0        0        0    17200 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_request_price.py
+-rw-r--r--   0        0        0     3813 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response.py
+-rw-r--r--   0        0        0     4479 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response_error.py
+-rw-r--r--   0        0        0     7035 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response_process_result.py
+-rw-r--r--   0        0        0     3824 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_request.py
+-rw-r--r--   0        0        0     5634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_request_stock.py
+-rw-r--r--   0        0        0     3813 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response.py
+-rw-r--r--   0        0        0     8727 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response_error.py
+-rw-r--r--   0        0        0     7035 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response_process_result.py
+-rw-r--r--   0        0        0     4991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_picking.py
+-rw-r--r--   0        0        0     3894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_archive_request.py
+-rw-r--r--   0        0        0     3995 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_accordance_types_response.py
+-rw-r--r--   0        0        0     4639 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_accordance_types_response_type.py
+-rw-r--r--   0        0        0     5109 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_bind_request.py
+-rw-r--r--   0        0        0     3885 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_types_response.py
+-rw-r--r--   0        0        0     4519 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_types_response_type.py
+-rw-r--r--   0        0        0     4667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certification_list_request.py
+-rw-r--r--   0        0        0     3718 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_certification_list_response.py
+-rw-r--r--   0        0        0    10172 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_info_pictures_response_picture.py
+-rw-r--r--   0        0        0     3910 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_product_unarchive_request.py
+-rw-r--r--   0        0        0     4823 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/product_update_offer_id_request_update_offer_id.py
+-rw-r--r--   0        0        0     5603 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_request.py
+-rw-r--r--   0        0        0     3997 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response.py
+-rw-r--r--   0        0        0    10380 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response_result.py
+-rw-r--r--   0        0        0     7367 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_import_pictures_request.py
+-rw-r--r--   0        0        0     3804 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_request.py
+-rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_response.py
+-rw-r--r--   0        0        0     3770 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_response_result.py
+-rw-r--r--   0        0        0     3761 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_delete_products_request.py
+-rw-r--r--   0        0        0     3761 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_delete_products_response.py
+-rw-r--r--   0        0        0     6380 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_request.py
+-rw-r--r--   0        0        0     3879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_response.py
+-rw-r--r--   0        0        0     5628 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_discounted_stocks.py
+-rw-r--r--   0        0        0     5748 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_request.py
+-rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response.py
+-rw-r--r--   0        0        0    44624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_item.py
+-rw-r--r--   0        0        0     3794 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_result.py
+-rw-r--r--   0        0        0     5633 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_source.py
+-rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_stock.py
+-rw-r--r--   0        0        0     7055 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_visibility_details.py
+-rw-r--r--   0        0        0     5488 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_request.py
+-rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response.py
+-rw-r--r--   0        0        0     8461 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_commissions.py
+-rw-r--r--   0        0        0    49953 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_result.py
+-rw-r--r--   0        0        0     5565 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_source.py
+-rw-r--r--   0        0        0     5370 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_stock.py
+-rw-r--r--   0        0        0     5923 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_visibility_details.py
+-rw-r--r--   0        0        0     5971 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request.py
+-rw-r--r--   0        0        0     5899 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request_filter.py
+-rw-r--r--   0        0        0     3876 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request_filter_filter_visibility.py
+-rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response.py
+-rw-r--r--   0        0        0     4731 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response_item.py
+-rw-r--r--   0        0        0     5894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response_result.py
+-rw-r--r--   0        0        0     3780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_request.py
+-rw-r--r--   0        0        0     6663 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_request_stock.py
+-rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response.py
+-rw-r--r--   0        0        0     6341 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response_error.py
+-rw-r--r--   0        0        0     7788 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response_result.py
+-rw-r--r--   0        0        0    13864 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv2_status.py
+-rw-r--r--   0        0        0     5563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_filter.py
+-rw-r--r--   0        0        0     7900 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_request.py
+-rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_response.py
+-rw-r--r--   0        0        0    23310 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_response_result.py
+-rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_request.py
+-rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response.py
+-rw-r--r--   0        0        0     5814 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_item.py
+-rw-r--r--   0        0        0     6300 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_result.py
+-rw-r--r--   0        0        0     5557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv4_filter.py
+-rw-r--r--   0        0        0     6036 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv4_get_product_info_prices_v4_request.py
+-rw-r--r--   0        0        0     3694 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/productv4_get_product_info_prices_v4_response.py
+-rw-r--r--   0        0        0     4246 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/protobuf_any.py
+-rw-r--r--   0        0        0     5299 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rating_item_change.py
+-rw-r--r--   0        0        0     4526 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rating_summary_v1_response_group.py
+-rw-r--r--   0        0        0     5744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rating_value.py
+-rw-r--r--   0        0        0     4681 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/related_posting_cancel_reason.py
+-rw-r--r--   0        0        0     6410 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/related_posting_cancel_reasons.py
+-rw-r--r--   0        0        0     4513 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_postings_report_request.py
+-rw-r--r--   0        0        0    12436 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_postings_report_request_filter.py
+-rw-r--r--   0        0        0     7392 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_products_report_request.py
+-rw-r--r--   0        0        0     2895 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_products_report_request_visibility.py
+-rw-r--r--   0        0        0     4498 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_returns_report_request.py
+-rw-r--r--   0        0        0     5812 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_returns_report_request_filter.py
+-rw-r--r--   0        0        0     2811 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_discounted_request.py
+-rw-r--r--   0        0        0     3630 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_discounted_response.py
+-rw-r--r--   0        0        0     3533 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_create_report_response.py
+-rw-r--r--   0        0        0     2751 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_language.py
+-rw-r--r--   0        0        0     2803 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_list_request_report_type.py
+-rw-r--r--   0        0        0     4524 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_list_response_result.py
+-rw-r--r--   0        0        0    10108 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_report.py
+-rw-r--r--   0        0        0     3574 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_report_info_request.py
+-rw-r--r--   0        0        0     3481 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_report_info_response.py
+-rw-r--r--   0        0        0     5416 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_report_list_request.py
+-rw-r--r--   0        0        0     3517 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/report_report_list_response.py
+-rw-r--r--   0        0        0     4297 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/result_error.py
+-rw-r--r--   0        0        0     3904 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/return_create_report_response_code.py
+-rw-r--r--   0        0        0     3599 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returnreport_create_report_response.py
+-rw-r--r--   0        0        0    19625 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_response_returns.py
+-rw-r--r--   0        0        0     4427 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_available_action.py
+-rw-r--r--   0        0        0     4443 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_client_return_method_type.py
+-rw-r--r--   0        0        0     6512 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_rejection_reason.py
+-rw-r--r--   0        0        0     5349 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_return_reason.py
+-rw-r--r--   0        0        0     9839 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_list_response_returns.py
+-rw-r--r--   0        0        0     4960 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rpc_status.py
+-rw-r--r--   0        0        0     6060 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rpc_status_v1_polygon_bind.py
+-rw-r--r--   0        0        0     6496 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/rpc_status_v1_polygon_create.py
+-rw-r--r--   0        0        0     4629 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_activate_product_v1_request.py
+-rw-r--r--   0        0        0     3765 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_actions_v1_response.py
+-rw-r--r--   0        0        0     5838 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_request.py
+-rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_response.py
+-rw-r--r--   0        0        0     4750 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_response_result.py
+-rw-r--r--   0        0        0     8936 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product.py
+-rw-r--r--   0        0        0     4643 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_ids_v1_request.py
+-rw-r--r--   0        0        0     5430 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_price.py
+-rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response.py
+-rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_deactivate.py
+-rw-r--r--   0        0        0     4637 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_product.py
+-rw-r--r--   0        0        0     4753 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_product_deactivate.py
+-rw-r--r--   0        0        0     4985 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_result.py
+-rw-r--r--   0        0        0     5131 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_result_deactivate.py
+-rw-r--r--   0        0        0     2819 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/seller_serviceanalytics_dimension.py
+-rw-r--r--   0        0        0     2743 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/sorting_order.py
+-rw-r--r--   0        0        0     5680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_capacity.py
+-rw-r--r--   0        0        0     4666 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_result.py
+-rw-r--r--   0        0        0     5049 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_schedule.py
+-rw-r--r--   0        0        0     4471 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_warehouse.py
+-rw-r--r--   0        0        0     5002 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_activate_hot_sales_products_request.py
+-rw-r--r--   0        0        0     5842 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_activate_hot_sales_products_request_activate_product.py
+-rw-r--r--   0        0        0     3640 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_request.py
+-rw-r--r--   0        0        0     3583 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_response.py
+-rw-r--r--   0        0        0     5891 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_result.py
+-rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_request.py
+-rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_response.py
+-rw-r--r--   0        0        0     4861 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_response_result.py
+-rw-r--r--   0        0        0     3678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_decline_discount_tasks_response.py
+-rw-r--r--   0        0        0     6176 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_decline_discount_tasks_response_result.py
+-rw-r--r--   0        0        0     3680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_discount_tasks_request.py
+-rw-r--r--   0        0        0     7994 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_discount_tasks_request_task.py
+-rw-r--r--   0        0        0     4285 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_barcode.py
+-rw-r--r--   0        0        0    12852 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_certificate.py
+-rw-r--r--   0        0        0     4823 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_competitor.py
+-rw-r--r--   0        0        0    16072 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_conditional_cancellation.py
+-rw-r--r--   0        0        0     4811 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_conditional_cancellation_move_request.py
+-rw-r--r--   0        0        0     3860 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_request.py
+-rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_response.py
+-rw-r--r--   0        0        0     3762 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_response_result.py
+-rw-r--r--   0        0        0     4712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_request.py
+-rw-r--r--   0        0        0     3612 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_response.py
+-rw-r--r--   0        0        0     3796 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_response_result.py
+-rw-r--r--   0        0        0     4619 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_create_stock_by_warehouse_report_request.py
+-rw-r--r--   0        0        0     4933 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_deactivate_hot_sales_products_request.py
+-rw-r--r--   0        0        0     3680 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_decline_discount_tasks_request.py
+-rw-r--r--   0        0        0     4591 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_decline_discount_tasks_request_task.py
+-rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_delete_strategy_items_response.py
+-rw-r--r--   0        0        0     3980 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_delete_strategy_items_response_result.py
+-rw-r--r--   0        0        0     3070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_discount_task_status.py
+-rw-r--r--   0        0        0     2723 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_empty.py
+-rw-r--r--   0        0        0     3838 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_request.py
+-rw-r--r--   0        0        0     3698 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_response.py
+-rw-r--r--   0        0        0     6169 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_result.py
+-rw-r--r--   0        0        0     8772 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_request.py
+-rw-r--r--   0        0        0     5334 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_response.py
+-rw-r--r--   0        0        0     6331 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_response_dictionary_value.py
+-rw-r--r--   0        0        0     5473 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_request.py
+-rw-r--r--   0        0        0     3665 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_response.py
+-rw-r--r--   0        0        0    17668 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_response_attribute.py
+-rw-r--r--   0        0        0     4735 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_competitors_request.py
+-rw-r--r--   0        0        0     4570 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_competitors_response.py
+-rw-r--r--   0        0        0     6681 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_list_request.py
+-rw-r--r--   0        0        0     5621 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_list_response.py
+-rw-r--r--   0        0        0     3978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_request.py
+-rw-r--r--   0        0        0     3616 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_response.py
+-rw-r--r--   0        0        0     5313 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_request.py
+-rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_response.py
+-rw-r--r--   0        0        0    39907 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_response_task.py
+-rw-r--r--   0        0        0     3414 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_etgb_request.py
+-rw-r--r--   0        0        0     3584 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_etgb_response.py
+-rw-r--r--   0        0        0     2791 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_list_request.py
+-rw-r--r--   0        0        0     3697 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_list_response.py
+-rw-r--r--   0        0        0     5790 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_request.py
+-rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_response.py
+-rw-r--r--   0        0        0     4678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_response_result.py
+-rw-r--r--   0        0        0     3956 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_request.py
+-rw-r--r--   0        0        0     3524 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_response.py
+-rw-r--r--   0        0        0     5770 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_response_result.py
+-rw-r--r--   0        0        0     3872 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_request.py
+-rw-r--r--   0        0        0     3827 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_response.py
+-rw-r--r--   0        0        0    16340 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_response_item.py
+-rw-r--r--   0        0        0     3736 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_request.py
+-rw-r--r--   0        0        0     3821 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_response.py
+-rw-r--r--   0        0        0     4633 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_response_result.py
+-rw-r--r--   0        0        0     3748 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_rating_by_sku_request.py
+-rw-r--r--   0        0        0     3821 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_rating_by_sku_response.py
+-rw-r--r--   0        0        0     3981 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_restrictions_request.py
+-rw-r--r--   0        0        0     3492 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_restrictions_response.py
+-rw-r--r--   0        0        0     3634 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response.py
+-rw-r--r--   0        0        0     3969 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response_result.py
+-rw-r--r--   0        0        0     3692 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_request.py
+-rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_response.py
+-rw-r--r--   0        0        0     9624 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_response_result.py
+-rw-r--r--   0        0        0     3557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_items_response.py
+-rw-r--r--   0        0        0     3742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_items_response_result.py
+-rw-r--r--   0        0        0     4743 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_list_request.py
+-rw-r--r--   0        0        0     4551 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_list_response.py
+-rw-r--r--   0        0        0     3502 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_response.py
+-rw-r--r--   0        0        0     7978 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_response_result.py
+-rw-r--r--   0        0        0     5843 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_items_request.py
+-rw-r--r--   0        0        0     6329 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_items_response.py
+-rw-r--r--   0        0        0     3890 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_request.py
+-rw-r--r--   0        0        0    20230 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_response.py
+-rw-r--r--   0        0        0     8173 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_orders_list_request.py
+-rw-r--r--   0        0        0     6678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_orders_list_response.py
+-rw-r--r--   0        0        0     3469 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_request.py
+-rw-r--r--   0        0        0     3580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_response.py
+-rw-r--r--   0        0        0     8332 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_response_item.py
+-rw-r--r--   0        0        0     5550 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_barcode_reset_response.py
+-rw-r--r--   0        0        0     2787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_delivery_schema.py
+-rw-r--r--   0        0        0     3678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_barcode_response.py
+-rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_pdf_response.py
+-rw-r--r--   0        0        0     5434 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_png_response.py
+-rw-r--r--   0        0        0     3636 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_info_request.py
+-rw-r--r--   0        0        0     7290 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_info_response.py
+-rw-r--r--   0        0        0     3769 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_is_enabled_response.py
+-rw-r--r--   0        0        0     4449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_list_request.py
+-rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_list_response.py
+-rw-r--r--   0        0        0     2755 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_status.py
+-rw-r--r--   0        0        0     9047 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_hot_sale_product.py
+-rw-r--r--   0        0        0     9894 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_create_or_update_request.py
+-rw-r--r--   0        0        0     3649 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_create_or_update_response.py
+-rw-r--r--   0        0        0     3712 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_delete_request.py
+-rw-r--r--   0        0        0     3585 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_delete_response.py
+-rw-r--r--   0        0        0     3688 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_get_request.py
+-rw-r--r--   0        0        0     3485 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_get_response.py
+-rw-r--r--   0        0        0    10461 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_item_error.py
+-rw-r--r--   0        0        0     3760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_item_ids_request.py
+-rw-r--r--   0        0        0     4841 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_delivery_interval.py
+-rw-r--r--   0        0        0     3896 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_request.py
+-rw-r--r--   0        0        0     5264 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_response.py
+-rw-r--r--   0        0        0     4580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_new_timeslot.py
+-rw-r--r--   0        0        0     4678 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_request.py
+-rw-r--r--   0        0        0     3647 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_response.py
+-rw-r--r--   0        0        0     4342 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_premium_scores.py
+-rw-r--r--   0        0        0     3925 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_request.py
+-rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_response.py
+-rw-r--r--   0        0        0     4960 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_response_result.py
+-rw-r--r--   0        0        0     3993 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_info_request.py
+-rw-r--r--   0        0        0     3548 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_info_response.py
+-rw-r--r--   0        0        0     8255 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_request.py
+-rw-r--r--   0        0        0     3623 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_response.py
+-rw-r--r--   0        0        0     4793 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_response_result.py
+-rw-r--r--   0        0        0     2871 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_product_status_list_request.py
+-rw-r--r--   0        0        0     3827 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_product_status_list_response.py
+-rw-r--r--   0        0        0     7369 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_request.py
+-rw-r--r--   0        0        0     3711 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_response.py
+-rw-r--r--   0        0        0     4745 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_response_result.py
+-rw-r--r--   0        0        0     2883 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_request.py
+-rw-r--r--   0        0        0     3906 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_response.py
+-rw-r--r--   0        0        0     2843 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_status_list_request.py
+-rw-r--r--   0        0        0     3853 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_status_list_response.py
+-rw-r--r--   0        0        0     5117 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_unbind_request.py
+-rw-r--r--   0        0        0     3787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_unbind_response.py
+-rw-r--r--   0        0        0     3532 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_request.py
+-rw-r--r--   0        0        0     4608 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response.py
+-rw-r--r--   0        0        0     5216 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response_error.py
+-rw-r--r--   0        0        0     7725 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response_item.py
+-rw-r--r--   0        0        0     3839 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request.py
+-rw-r--r--   0        0        0     6134 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_attribute.py
+-rw-r--r--   0        0        0     4747 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_item.py
+-rw-r--r--   0        0        0     4873 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_value.py
+-rw-r--r--   0        0        0     4148 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_response.py
+-rw-r--r--   0        0        0     4607 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_discount_request.py
+-rw-r--r--   0        0        0     3785 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_discount_response.py
+-rw-r--r--   0        0        0     4037 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_request.py
+-rw-r--r--   0        0        0     3714 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_response.py
+-rw-r--r--   0        0        0     4651 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_response_error.py
+-rw-r--r--   0        0        0     4739 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_request.py
+-rw-r--r--   0        0        0     4070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_request_info.py
+-rw-r--r--   0        0        0     3656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response.py
+-rw-r--r--   0        0        0     3700 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_info.py
+-rw-r--r--   0        0        0     4132 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_info_result.py
+-rw-r--r--   0        0        0     3762 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_result.py
+-rw-r--r--   0        0        0     7682 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating.py
+-rw-r--r--   0        0        0    12176 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_history_v1_request.py
+-rw-r--r--   0        0        0     4778 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_history_v1_response.py
+-rw-r--r--   0        0        0    10518 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_item.py
+-rw-r--r--   0        0        0     5649 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_status.py
+-rw-r--r--   0        0        0     5767 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_summary_v1_response.py
+-rw-r--r--   0        0        0    10413 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_restriction.py
+-rw-r--r--   0        0        0     5098 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_seller_warehouse.py
+-rw-r--r--   0        0        0     3645 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result.py
+-rw-r--r--   0        0        0     4733 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result_product.py
+-rw-r--r--   0        0        0     3990 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result_result.py
+-rw-r--r--   0        0        0     3667 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result.py
+-rw-r--r--   0        0        0     4753 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_product.py
+-rw-r--r--   0        0        0     4012 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_result.py
+-rw-r--r--   0        0        0     4317 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair.py
+-rw-r--r--   0        0        0     4475 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair_rejection.py
+-rw-r--r--   0        0        0     4333 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair_statuses.py
+-rw-r--r--   0        0        0     3636 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_strategy_request.py
+-rw-r--r--   0        0        0     3826 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_supplier_available_warehouses_response.py
+-rw-r--r--   0        0        0     4066 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_timeslot.py
+-rw-r--r--   0        0        0     5639 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_update_pricing_strategy_request.py
+-rw-r--r--   0        0        0     4682 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_update_status_strategy_request.py
+-rw-r--r--   0        0        0     6177 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_vehicle_info.py
+-rw-r--r--   0        0        0     5002 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v1_warehouse.py
+-rw-r--r--   0        0        0     3991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_additional_data_item.py
+-rw-r--r--   0        0        0     4786 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_history_response.py
+-rw-r--r--   0        0        0     5589 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_list_response.py
+-rw-r--r--   0        0        0     6648 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_message.py
+-rw-r--r--   0        0        0     3730 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_read_response.py
+-rw-r--r--   0        0        0    13045 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting.py
+-rw-r--r--   0        0        0     3617 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting_list_response.py
+-rw-r--r--   0        0        0     3449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting_response.py
+-rw-r--r--   0        0        0    13676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting.py
+-rw-r--r--   0        0        0     7709 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product.py
+-rw-r--r--   0        0        0     3782 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_request.py
+-rw-r--r--   0        0        0     3887 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_response.py
+-rw-r--r--   0        0        0     4781 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_response_result.py
+-rw-r--r--   0        0        0     6404 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_set_request.py
+-rw-r--r--   0        0        0     5068 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_set_response.py
+-rw-r--r--   0        0        0     3449 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_response.py
+-rw-r--r--   0        0        0     4904 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_get_geo_restrictions_by_filter_request_filter.py
+-rw-r--r--   0        0        0     9676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_item_error.py
+-rw-r--r--   0        0        0     3579 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_request.py
+-rw-r--r--   0        0        0     3787 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_response.py
+-rw-r--r--   0        0        0    10330 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_result.py
+-rw-r--r--   0        0        0     6906 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_products.py
+-rw-r--r--   0        0        0     9003 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_filter.py
+-rw-r--r--   0        0        0     5780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs.py
+-rw-r--r--   0        0        0     5706 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_acceptance.py
+-rw-r--r--   0        0        0     5084 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_excess.py
+-rw-r--r--   0        0        0     5608 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_mismatch.py
+-rw-r--r--   0        0        0     4465 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_request.py
+-rw-r--r--   0        0        0     3676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_response.py
+-rw-r--r--   0        0        0    17557 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_result.py
+-rw-r--r--   0        0        0     4010 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_request.py
+-rw-r--r--   0        0        0     5289 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_response.py
+-rw-r--r--   0        0        0     4799 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_request.py
+-rw-r--r--   0        0        0     3720 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_response.py
+-rw-r--r--   0        0        0     3552 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_request.py
+-rw-r--r--   0        0        0     5566 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_response.py
+-rw-r--r--   0        0        0     3676 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_text_response.py
+-rw-r--r--   0        0        0     5172 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_digital_act_request.py
+-rw-r--r--   0        0        0     5580 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_digital_act_response.py
+-rw-r--r--   0        0        0     6520 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_financial_data.py
+-rw-r--r--   0        0        0     9300 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_product.py
+-rw-r--r--   0        0        0     7294 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_product.py
+-rw-r--r--   0        0        0     3744 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response.py
+-rw-r--r--   0        0        0     5151 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response_result.py
+-rw-r--r--   0        0        0     4703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response_type.py
+-rw-r--r--   0        0        0     4879 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_compensate_request.py
+-rw-r--r--   0        0        0     6759 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_filter.py
+-rw-r--r--   0        0        0     3720 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_request.py
+-rw-r--r--   0        0        0     3552 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_response.py
+-rw-r--r--   0        0        0     4485 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_v2_response_state.py
+-rw-r--r--   0        0        0     5500 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_request.py
+-rw-r--r--   0        0        0     3563 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_response.py
+-rw-r--r--   0        0        0     6699 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_v2_response_state.py
+-rw-r--r--   0        0        0     3840 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_receive_return_request.py
+-rw-r--r--   0        0        0     6674 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_reject_request.py
+-rw-r--r--   0        0        0     5009 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_return_money_request.py
+-rw-r--r--   0        0        0     4969 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_verify_request.py
+-rw-r--r--   0        0        0     4435 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v2_user.py
+-rw-r--r--   0        0        0     3991 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_additional_data_item.py
+-rw-r--r--   0        0        0    11268 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_address.py
+-rw-r--r--   0        0        0     4123 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_addressee.py
+-rw-r--r--   0        0        0     4359 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_addressee_fbs_lists.py
+-rw-r--r--   0        0        0     4643 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_barcodes.py
+-rw-r--r--   0        0        0     9471 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_cancellation.py
+-rw-r--r--   0        0        0     6478 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_customer.py
+-rw-r--r--   0        0        0     6810 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_customer_fbs_lists.py
+-rw-r--r--   0        0        0     7721 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_delivery_method.py
+-rw-r--r--   0        0        0     5621 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_dimensions.py
+-rw-r--r--   0        0        0    32656 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting.py
+-rw-r--r--   0        0        0    14163 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_analytics_data.py
+-rw-r--r--   0        0        0    37377 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_detail.py
+-rw-r--r--   0        0        0     4070 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_detail_related_postings.py
+-rw-r--r--   0        0        0     4619 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_exemplar_product_v3.py
+-rw-r--r--   0        0        0     9374 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product.py
+-rw-r--r--   0        0        0     8797 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product_exemplar_info_v3.py
+-rw-r--r--   0        0        0     3638 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product_exemplars_v3.py
+-rw-r--r--   0        0        0    11742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_requirements_v3.py
+-rw-r--r--   0        0        0     6742 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_request.py
+-rw-r--r--   0        0        0     3689 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response.py
+-rw-r--r--   0        0        0     5274 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_period.py
+-rw-r--r--   0        0        0     5805 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_result.py
+-rw-r--r--   0        0        0     3590 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_list_response_v3.py
+-rw-r--r--   0        0        0     5543 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_list_response_v3_result.py
+-rw-r--r--   0        0        0     3507 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_response_v3.py
+-rw-r--r--   0        0        0     5844 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbo_v3_request.py
+-rw-r--r--   0        0        0     4697 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbo_v3_response.py
+-rw-r--r--   0        0        0     5774 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbs_v3_request.py
+-rw-r--r--   0        0        0     5019 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbs_v3_response.py
+-rw-r--r--   0        0        0     3614 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request.py
+-rw-r--r--   0        0        0     6377 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_attribute.py
+-rw-r--r--   0        0        0     3759 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_complex_attribute.py
+-rw-r--r--   0        0        0     4809 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_dictionary_value.py
+-rw-r--r--   0        0        0    32162 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_item.py
+-rw-r--r--   0        0        0     3535 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_response.py
+-rw-r--r--   0        0        0     3694 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_response_result.py
+-rw-r--r--   0        0        0     6520 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_posting_financial_data.py
+-rw-r--r--   0        0        0    11308 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_posting_product_detail.py
+-rw-r--r--   0        0        0     4903 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_returns_company_filter_fbo.py
+-rw-r--r--   0        0        0     9024 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_returns_company_filter_fbs.py
+-rw-r--r--   0        0        0     2868 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v3_service_type.py
+-rw-r--r--   0        0        0     4902 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request.py
+-rw-r--r--   0        0        0     5913 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request_product.py
+-rw-r--r--   0        0        0     3752 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_response.py
+-rw-r--r--   0        0        0     5256 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v4_get_upload_quota_response.py
+-rw-r--r--   0        0        0     4005 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_request.py
+-rw-r--r--   0        0        0     6110 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response.py
+-rw-r--r--   0        0        0    10108 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product.py
+-rw-r--r--   0        0        0    10780 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product_exemplar.py
+-rw-r--r--   0        0        0     6119 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request.py
+-rw-r--r--   0        0        0     9918 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product.py
+-rw-r--r--   0        0        0    10582 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product_exemplar.py
+-rw-r--r--   0        0        0     3867 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_response.py
+-rw-r--r--   0        0        0     5760 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/warehouse_delivery_method_list_request.py
+-rw-r--r--   0        0        0     5351 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/warehouse_delivery_method_list_response.py
+-rw-r--r--   0        0        0     7376 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/warehouse_first_mile_type.py
+-rw-r--r--   0        0        0    20215 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/warehouse_list_response_warehouse.py
+-rw-r--r--   0        0        0     3703 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/models/warehouse_warehouse_list_response.py
+-rw-r--r--   0        0        0    13320 2024-03-20 09:50:50.000000 ozon_api_client-0.0.5/ozon_api_client/rest.py
+-rw-r--r--   0        0        0      403 2024-04-09 11:50:50.383342 ozon_api_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    96720 1970-01-01 00:00:00.000000 ozon_api_client-0.0.5/PKG-INFO
```

### Comparing `ozon_api_client-0.0.4/README.md` & `ozon_api_client-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,61 +18,59 @@
 
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
-
 ```python
-import ozon_api_client 
+import swagger_client 
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
-
 ```python
-import ozon_api_client
+import swagger_client
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 from __future__ import print_function
 import time
-import ozon_api_client
-from ozon_api_client.rest import ApiException
+import swagger_client
+from swagger_client.rest import ApiException
 from pprint import pprint
 
 # create an instance of the API class
-api_instance = ozon_api_client.AnalyticsAPIApi(ozon_api_client.ApiClient(configuration))
-body = ozon_api_client.AnalyticsAnalyticsGetDataRequest() # AnalyticsAnalyticsGetDataRequest | 
+api_instance = swagger_client.AnalyticsAPIApi(swagger_client.ApiClient(configuration))
+body = swagger_client.AnalyticsAnalyticsGetDataRequest() # AnalyticsAnalyticsGetDataRequest | 
 client_id = 'client_id_example' # str | Идентификатор клиента.
 api_key = 'api_key_example' # str | API-ключ.
 
 try:
     # Данные аналитики
     api_response = api_instance.analytics_api_analytics_get_data(body, client_id, api_key)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AnalyticsAPIApi->analytics_api_analytics_get_data: %s\n" % e)
 
 # create an instance of the API class
-api_instance = ozon_api_client.AnalyticsAPIApi(ozon_api_client.ApiClient(configuration))
-body = ozon_api_client.AnalyticsStockOnWarehouseRequest() # AnalyticsStockOnWarehouseRequest | 
+api_instance = swagger_client.AnalyticsAPIApi(swagger_client.ApiClient(configuration))
+body = swagger_client.AnalyticsStockOnWarehouseRequest() # AnalyticsStockOnWarehouseRequest | 
 client_id = 'client_id_example' # str | Идентификатор клиента.
 api_key = 'api_key_example' # str | API-ключ.
 
 try:
     # Отчёт по остаткам и товарам
     api_response = api_instance.analytics_api_analytics_get_stock_on_warehouses_v2(body, client_id, api_key)
     pprint(api_response)
@@ -114,68 +112,76 @@
 *CertificationAPIApi* | [**rejection_reasons_list**](docs/CertificationAPIApi.md#rejection_reasons_list) | **POST** /v1/product/certificate/rejection_reasons/list | Возможные причины отклонения сертификата
 *ChatAPIApi* | [**chat_api_chat_history_v2**](docs/ChatAPIApi.md#chat_api_chat_history_v2) | **POST** /v2/chat/history | История чата
 *ChatAPIApi* | [**chat_api_chat_list_v2**](docs/ChatAPIApi.md#chat_api_chat_list_v2) | **POST** /v2/chat/list | Список чатов
 *ChatAPIApi* | [**chat_api_chat_read_v2**](docs/ChatAPIApi.md#chat_api_chat_read_v2) | **POST** /v2/chat/read | Отметить сообщения как прочитанные
 *ChatAPIApi* | [**chat_api_chat_send_file**](docs/ChatAPIApi.md#chat_api_chat_send_file) | **POST** /v1/chat/send/file | Отправить файл
 *ChatAPIApi* | [**chat_api_chat_send_message**](docs/ChatAPIApi.md#chat_api_chat_send_message) | **POST** /v1/chat/send/message | Отправить сообщение
 *ChatAPIApi* | [**chat_api_chat_start**](docs/ChatAPIApi.md#chat_api_chat_start) | **POST** /v1/chat/start | Создать новый чат
+*DeliveryFBSApi* | [**carriage_get**](docs/DeliveryFBSApi.md#carriage_get) | **POST** /v1/carriage/get | Информация о перевозке
+*DeliveryFBSApi* | [**posting_api_act_posting_list**](docs/DeliveryFBSApi.md#posting_api_act_posting_list) | **POST** /v2/posting/fbs/act/get-postings | Список отправлений в акте
+*DeliveryFBSApi* | [**posting_api_digital_act_document_sign**](docs/DeliveryFBSApi.md#posting_api_digital_act_document_sign) | **POST** /v2/posting/fbs/digital/act/document-sign | Подписать документы по отгрузке
+*DeliveryFBSApi* | [**posting_api_fbs_act_list**](docs/DeliveryFBSApi.md#posting_api_fbs_act_list) | **POST** /v2/posting/fbs/act/list | Список актов по отгрузкам
+*DeliveryFBSApi* | [**posting_api_get_carriage_available_list**](docs/DeliveryFBSApi.md#posting_api_get_carriage_available_list) | **POST** /v1/posting/carriage-available/list | Список доступных перевозок
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_check_status**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_check_status) | **POST** /v2/posting/fbs/act/check-status | Статус отгрузки и документов
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_create**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_create) | **POST** /v2/posting/fbs/act/create | Подтвердить отгрузку и создать документы
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_get_container_labels**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_get_container_labels) | **POST** /v2/posting/fbs/act/get-container-labels | Этикетки для грузового места
+*DeliveryFBSApi* | [**posting_api_posting_fbs_digital_act_check_status**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_digital_act_check_status) | **POST** /v2/posting/fbs/digital/act/check-status | Статус формирования накладной
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_act**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_act) | **POST** /v2/posting/fbs/act/get-pdf | Получить PDF c документами
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_barcode**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_barcode) | **POST** /v2/posting/fbs/act/get-barcode | Штрихкод для отгрузки отправления
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_barcode_text**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_barcode_text) | **POST** /v2/posting/fbs/act/get-barcode/text | Значение штрихкода для отгрузки отправления
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_digital_act**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_digital_act) | **POST** /v2/posting/fbs/digital/act/get-pdf | Получить лист отгрузки по перевозке
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_delivered**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_delivered) | **POST** /v2/fbs/posting/delivered | Изменить статус на «Доставлено»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_delivering**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_delivering) | **POST** /v2/fbs/posting/delivering | Изменить статус на «Доставляется»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_last_mile**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_last_mile) | **POST** /v2/fbs/posting/last-mile | Изменить статус на «Последняя миля»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_sentbyseller**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_sentbyseller) | **POST** /v2/fbs/posting/sent-by-seller | Изменить статус на «Отправлено продавцом»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_tracking_number_set**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_tracking_number_set) | **POST** /v2/fbs/posting/tracking-number/set | Добавить трек-номера
+*DeliveryrFBSApi* | [**posting_api_posting_timeslot_change_restrictions**](docs/DeliveryrFBSApi.md#posting_api_posting_timeslot_change_restrictions) | **POST** /v1/posting/fbs/timeslot/change-restrictions | Доступные даты для переноса доставки
+*DeliveryrFBSApi* | [**posting_api_set_posting_timeslot**](docs/DeliveryrFBSApi.md#posting_api_set_posting_timeslot) | **POST** /v1/posting/fbs/timeslot/set | Перенести дату доставки
 *FBOApi* | [**posting_api_get_fbo_posting**](docs/FBOApi.md#posting_api_get_fbo_posting) | **POST** /v2/posting/fbo/get | Информация об отправлении
 *FBOApi* | [**posting_api_get_fbo_posting_list**](docs/FBOApi.md#posting_api_get_fbo_posting_list) | **POST** /v2/posting/fbo/list | Список отправлений
 *FBOApi* | [**supplier_api_supplier_available_warehouses**](docs/FBOApi.md#supplier_api_supplier_available_warehouses) | **GET** /v1/supplier/available_warehouses | Загруженность складов Ozon
 *FBOApi* | [**supply_order_api_get_supply_order**](docs/FBOApi.md#supply_order_api_get_supply_order) | **POST** /v1/supply-order/get | Информация о заявке на поставку
 *FBOApi* | [**supply_order_api_get_supply_order_items**](docs/FBOApi.md#supply_order_api_get_supply_order_items) | **POST** /v1/supply-order/items | Список товаров в заявке на поставку
 *FBOApi* | [**supply_order_api_get_supply_orders_list**](docs/FBOApi.md#supply_order_api_get_supply_orders_list) | **POST** /v1/supply-order/list | Список заявок на поставку на склад Ozon
-*FBSApi* | [**posting_api_act_posting_list**](docs/FBSApi.md#posting_api_act_posting_list) | **POST** /v2/posting/fbs/act/get-postings | Список отправлений в акте
 *FBSApi* | [**posting_api_cancel_fbs_posting**](docs/FBSApi.md#posting_api_cancel_fbs_posting) | **POST** /v2/posting/fbs/cancel | Отменить отправление
 *FBSApi* | [**posting_api_cancel_fbs_posting_product**](docs/FBSApi.md#posting_api_cancel_fbs_posting_product) | **POST** /v2/posting/fbs/product/cancel | Отменить отправку некоторых товаров в отправлении
 *FBSApi* | [**posting_api_change_fbs_posting_product**](docs/FBSApi.md#posting_api_change_fbs_posting_product) | **POST** /v2/posting/fbs/product/change | Добавить вес для весовых товаров в отправлении
 *FBSApi* | [**posting_api_create_label_batch**](docs/FBSApi.md#posting_api_create_label_batch) | **POST** /v1/posting/fbs/package-label/create | Создать задание на выгрузку этикеток
-*FBSApi* | [**posting_api_digital_act_document_sign**](docs/FBSApi.md#posting_api_digital_act_document_sign) | **POST** /v2/posting/fbs/digital/act/document-sign | Подписать документы по отгрузке
-*FBSApi* | [**posting_api_fbs_act_list**](docs/FBSApi.md#posting_api_fbs_act_list) | **POST** /v2/posting/fbs/act/list | Список актов по отгрузкам
-*FBSApi* | [**posting_api_fbs_posting_delivered**](docs/FBSApi.md#posting_api_fbs_posting_delivered) | **POST** /v2/fbs/posting/delivered | Изменить статус на «Доставлено»
-*FBSApi* | [**posting_api_fbs_posting_delivering**](docs/FBSApi.md#posting_api_fbs_posting_delivering) | **POST** /v2/fbs/posting/delivering | Изменить статус на «Доставляется»
-*FBSApi* | [**posting_api_fbs_posting_last_mile**](docs/FBSApi.md#posting_api_fbs_posting_last_mile) | **POST** /v2/fbs/posting/last-mile | Изменить статус на «Последняя миля»
-*FBSApi* | [**posting_api_fbs_posting_sentbyseller**](docs/FBSApi.md#posting_api_fbs_posting_sentbyseller) | **POST** /v2/fbs/posting/sent-by-seller | Изменить статус на «Отправлено продавцом»
-*FBSApi* | [**posting_api_fbs_posting_tracking_number_set**](docs/FBSApi.md#posting_api_fbs_posting_tracking_number_set) | **POST** /v2/fbs/posting/tracking-number/set | Добавить трек-номера
-*FBSApi* | [**posting_api_get_carriage_available_list**](docs/FBSApi.md#posting_api_get_carriage_available_list) | **POST** /v1/posting/carriage-available/list | Список доступных перевозок
 *FBSApi* | [**posting_api_get_etgb**](docs/FBSApi.md#posting_api_get_etgb) | **POST** /v1/posting/global/etgb | Таможенные декларации ETGB
 *FBSApi* | [**posting_api_get_fbs_posting_by_barcode**](docs/FBSApi.md#posting_api_get_fbs_posting_by_barcode) | **POST** /v2/posting/fbs/get-by-barcode | Получить информацию об отправлении по штрихкоду
 *FBSApi* | [**posting_api_get_fbs_posting_list_v3**](docs/FBSApi.md#posting_api_get_fbs_posting_list_v3) | **POST** /v3/posting/fbs/list | Список отправлений (версия 3)
 *FBSApi* | [**posting_api_get_fbs_posting_unfulfilled_list**](docs/FBSApi.md#posting_api_get_fbs_posting_unfulfilled_list) | **POST** /v3/posting/fbs/unfulfilled/list | Список необработанных отправлений (версия 3)
 *FBSApi* | [**posting_api_get_fbs_posting_v3**](docs/FBSApi.md#posting_api_get_fbs_posting_v3) | **POST** /v3/posting/fbs/get | Получить информацию об отправлении по идентификатору
 *FBSApi* | [**posting_api_get_label_batch**](docs/FBSApi.md#posting_api_get_label_batch) | **POST** /v1/posting/fbs/package-label/get | Получить файл с этикетками
 *FBSApi* | [**posting_api_get_posting_fbs_cancel_reason_list**](docs/FBSApi.md#posting_api_get_posting_fbs_cancel_reason_list) | **POST** /v2/posting/fbs/cancel-reason/list | Причины отмены отправлений
 *FBSApi* | [**posting_api_get_posting_fbs_cancel_reason_v1**](docs/FBSApi.md#posting_api_get_posting_fbs_cancel_reason_v1) | **POST** /v1/posting/fbs/cancel-reason | Причины отмены отправления
 *FBSApi* | [**posting_api_get_restrictions**](docs/FBSApi.md#posting_api_get_restrictions) | **POST** /v1/posting/fbs/restrictions | Получить ограничения пункта приёма
 *FBSApi* | [**posting_api_list_country_product_fbs_posting_v2**](docs/FBSApi.md#posting_api_list_country_product_fbs_posting_v2) | **POST** /v2/posting/fbs/product/country/list | Список доступных стран-изготовителей
 *FBSApi* | [**posting_api_move_fbs_posting_to_arbitration**](docs/FBSApi.md#posting_api_move_fbs_posting_to_arbitration) | **POST** /v2/posting/fbs/arbitration | Открыть спор по отправлению
 *FBSApi* | [**posting_api_move_fbs_posting_to_awaiting_delivery**](docs/FBSApi.md#posting_api_move_fbs_posting_to_awaiting_delivery) | **POST** /v2/posting/fbs/awaiting-delivery | Передать отправление к отгрузке
-*FBSApi* | [**posting_api_posting_fbs_act_check_status**](docs/FBSApi.md#posting_api_posting_fbs_act_check_status) | **POST** /v2/posting/fbs/act/check-status | Статус отгрузки и документов
-*FBSApi* | [**posting_api_posting_fbs_act_create**](docs/FBSApi.md#posting_api_posting_fbs_act_create) | **POST** /v2/posting/fbs/act/create | Подтвердить отгрузку и создать документы
-*FBSApi* | [**posting_api_posting_fbs_act_get_container_labels**](docs/FBSApi.md#posting_api_posting_fbs_act_get_container_labels) | **POST** /v2/posting/fbs/act/get-container-labels | Этикетки для грузового места
-*FBSApi* | [**posting_api_posting_fbs_digital_act_check_status**](docs/FBSApi.md#posting_api_posting_fbs_digital_act_check_status) | **POST** /v2/posting/fbs/digital/act/check-status | Статус формирования накладной
-*FBSApi* | [**posting_api_posting_fbs_get_act**](docs/FBSApi.md#posting_api_posting_fbs_get_act) | **POST** /v2/posting/fbs/act/get-pdf | Получить PDF c документами
-*FBSApi* | [**posting_api_posting_fbs_get_barcode**](docs/FBSApi.md#posting_api_posting_fbs_get_barcode) | **POST** /v2/posting/fbs/act/get-barcode | Штрихкод для отгрузки отправления
-*FBSApi* | [**posting_api_posting_fbs_get_barcode_text**](docs/FBSApi.md#posting_api_posting_fbs_get_barcode_text) | **POST** /v2/posting/fbs/act/get-barcode/text | Значение штрихкода для отгрузки отправления
-*FBSApi* | [**posting_api_posting_fbs_get_digital_act**](docs/FBSApi.md#posting_api_posting_fbs_get_digital_act) | **POST** /v2/posting/fbs/digital/act/get-pdf | Получить лист отгрузки по перевозке
 *FBSApi* | [**posting_api_posting_fbs_package_label**](docs/FBSApi.md#posting_api_posting_fbs_package_label) | **POST** /v2/posting/fbs/package-label | Напечатать этикетку
 *FBSApi* | [**posting_api_posting_multi_box_qty_set_v3**](docs/FBSApi.md#posting_api_posting_multi_box_qty_set_v3) | **POST** /v3/posting/multiboxqty/set | Указать количество коробок для многокоробочных отправлений
-*FBSApi* | [**posting_api_posting_timeslot_change_restrictions**](docs/FBSApi.md#posting_api_posting_timeslot_change_restrictions) | **POST** /v1/posting/fbs/timeslot/change-restrictions | Доступные даты для переноса доставки
 *FBSApi* | [**posting_api_set_country_product_fbs_posting_v2**](docs/FBSApi.md#posting_api_set_country_product_fbs_posting_v2) | **POST** /v2/posting/fbs/product/country/set | Добавить информацию о стране-изготовителе товара
-*FBSApi* | [**posting_api_set_posting_timeslot**](docs/FBSApi.md#posting_api_set_posting_timeslot) | **POST** /v1/posting/fbs/timeslot/set | Перенести дату доставки
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_create_or_get**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_create_or_get) | **POST** /v5/fbs/posting/product/exemplar/create-or-get | Получить данные созданных экземпляров
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_set**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_set) | **POST** /v5/fbs/posting/product/exemplar/set | Проверить и сохранить данные экземпляров (версия 5)
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_validate**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_validate) | **POST** /v4/fbs/posting/product/exemplar/validate | Валидация кодов маркировки
 *FBSrFBSMarksApi* | [**posting_api_get_product_exemplar_status**](docs/FBSrFBSMarksApi.md#posting_api_get_product_exemplar_status) | **POST** /v4/fbs/posting/product/exemplar/status | Получить статус добавления экземпляров
 *FBSrFBSMarksApi* | [**posting_api_set_product_exemplar**](docs/FBSrFBSMarksApi.md#posting_api_set_product_exemplar) | **POST** /v4/fbs/posting/product/exemplar/set | Проверить и сохранить данные экземпляров
 *FBSrFBSMarksApi* | [**posting_api_ship_fbs_posting_package**](docs/FBSrFBSMarksApi.md#posting_api_ship_fbs_posting_package) | **POST** /v4/posting/fbs/ship/package | Частичная сборка отправления (версия 4)
 *FBSrFBSMarksApi* | [**posting_api_ship_fbs_posting_v4**](docs/FBSrFBSMarksApi.md#posting_api_ship_fbs_posting_v4) | **POST** /v4/posting/fbs/ship | Собрать заказ (версия 4)
 *FinanceAPIApi* | [**finance_api_finance_transaction_list_v3**](docs/FinanceAPIApi.md#finance_api_finance_transaction_list_v3) | **POST** /v3/finance/transaction/list | Список транзакций
 *FinanceAPIApi* | [**finance_api_finance_transaction_total_v3**](docs/FinanceAPIApi.md#finance_api_finance_transaction_total_v3) | **POST** /v3/finance/transaction/totals | Суммы транзакций
 *FinanceAPIApi* | [**finance_api_get_realization_report**](docs/FinanceAPIApi.md#finance_api_get_realization_report) | **POST** /v1/finance/realization | Отчёт о реализации товаров
+*PassApi* | [**carriage_pass_create**](docs/PassApi.md#carriage_pass_create) | **POST** /v1/carriage/pass/create | Создать пропуск
+*PassApi* | [**carriage_pass_delete**](docs/PassApi.md#carriage_pass_delete) | **POST** /v1/carriage/pass/delete | Удалить пропуск
+*PassApi* | [**carriage_pass_update**](docs/PassApi.md#carriage_pass_update) | **POST** /v1/carriage/pass/update | Обновить пропуск
+*PassApi* | [**pass_list**](docs/PassApi.md#pass_list) | **POST** /v1/pass/list | Список пропусков
+*PassApi* | [**return_pass_create**](docs/PassApi.md#return_pass_create) | **POST** /v1/return/pass/create | Создать пропуск для возврата
+*PassApi* | [**return_pass_delete**](docs/PassApi.md#return_pass_delete) | **POST** /v1/return/pass/delete | Удалить пропуск для возврата
+*PassApi* | [**return_pass_update**](docs/PassApi.md#return_pass_update) | **POST** /v1/return/pass/update | Обновить пропуск для возврата
 *PolygonAPIApi* | [**polygon_api_bind_polygon**](docs/PolygonAPIApi.md#polygon_api_bind_polygon) | **POST** /v1/polygon/bind | Свяжите метод доставки с полигоном доставки
 *PolygonAPIApi* | [**polygon_api_create_polygon**](docs/PolygonAPIApi.md#polygon_api_create_polygon) | **POST** /v1/polygon/create | Создайте полигон доставки
 *PricesStocksAPIApi* | [**product_api_get_product_info_discounted**](docs/PricesStocksAPIApi.md#product_api_get_product_info_discounted) | **POST** /v1/product/info/discounted | Узнать информацию об уценке и основном товаре по SKU уценённого товара
 *PricesStocksAPIApi* | [**product_api_get_product_info_prices_v4**](docs/PricesStocksAPIApi.md#product_api_get_product_info_prices_v4) | **POST** /v4/product/info/prices | Получить информацию о цене товара
 *PricesStocksAPIApi* | [**product_api_get_product_info_stocks_v3**](docs/PricesStocksAPIApi.md#product_api_get_product_info_stocks_v3) | **POST** /v3/product/info/stocks | Информация о количестве товаров
 *PricesStocksAPIApi* | [**product_api_import_products_prices**](docs/PricesStocksAPIApi.md#product_api_import_products_prices) | **POST** /v1/product/import/prices | Обновить цену
 *PricesStocksAPIApi* | [**product_api_import_products_stocks**](docs/PricesStocksAPIApi.md#product_api_import_products_stocks) | **POST** /v1/product/import/stocks | Обновить остатки
@@ -246,14 +252,15 @@
 *ReturnAPIApi* | [**return_api_giveout_barcode_reset**](docs/ReturnAPIApi.md#return_api_giveout_barcode_reset) | **POST** /v1/return/giveout/barcode-reset | Сгенерировать новый штрихкод
 *ReturnAPIApi* | [**return_api_giveout_get_barcode**](docs/ReturnAPIApi.md#return_api_giveout_get_barcode) | **POST** /v1/return/giveout/barcode | Значение штрихкода для возвратных отгрузок
 *ReturnAPIApi* | [**return_api_giveout_get_pdf**](docs/ReturnAPIApi.md#return_api_giveout_get_pdf) | **POST** /v1/return/giveout/get-pdf | Штрихкод для получения возвратной отгрузки в формате PDF
 *ReturnAPIApi* | [**return_api_giveout_get_png**](docs/ReturnAPIApi.md#return_api_giveout_get_png) | **POST** /v1/return/giveout/get-png | Штрихкод для получения возвратной отгрузки в формате PNG
 *ReturnAPIApi* | [**return_api_giveout_info**](docs/ReturnAPIApi.md#return_api_giveout_info) | **POST** /v1/return/giveout/info | Информация о возвратной отгрузке
 *ReturnAPIApi* | [**return_api_giveout_is_enabled**](docs/ReturnAPIApi.md#return_api_giveout_is_enabled) | **POST** /v1/return/giveout/is-enabled | Проверить возможность получения возвратных отгрузок по штрихкоду
 *ReturnAPIApi* | [**return_api_giveout_list**](docs/ReturnAPIApi.md#return_api_giveout_list) | **POST** /v1/return/giveout/list | Список возвратных отгрузок
+*ReturnAPIApi* | [**returns_company_fbs_info**](docs/ReturnAPIApi.md#returns_company_fbs_info) | **POST** /v1/returns/company/fbs/info | Количество возвратов FBS
 *ReturnsAPIApi* | [**returns_api_get_returns_company_fbo**](docs/ReturnsAPIApi.md#returns_api_get_returns_company_fbo) | **POST** /v3/returns/company/fbo | Получить информацию о возвратах FBO
 *ReturnsAPIApi* | [**returns_api_get_returns_company_fbsv3**](docs/ReturnsAPIApi.md#returns_api_get_returns_company_fbsv3) | **POST** /v3/returns/company/fbs | Получить информацию о возвратах FBS
 *SellerRatingApi* | [**rating_api_rating_history_v1**](docs/SellerRatingApi.md#rating_api_rating_history_v1) | **POST** /v1/rating/history | Получить информацию о рейтингах продавца за период
 *SellerRatingApi* | [**rating_api_rating_summary_v1**](docs/SellerRatingApi.md#rating_api_rating_summary_v1) | **POST** /v1/rating/summary | Получить информацию о текущих рейтингах продавца
 *SupplierAPIApi* | [**invoice_create**](docs/SupplierAPIApi.md#invoice_create) | **POST** /v1/invoice/create-or-update | Создать или изменить ссылку на счёт-фактуру
 *SupplierAPIApi* | [**invoice_delete**](docs/SupplierAPIApi.md#invoice_delete) | **POST** /v1/invoice/delete | Удалить ссылку на счёт-фактуру
 *SupplierAPIApi* | [**invoice_get**](docs/SupplierAPIApi.md#invoice_get) | **POST** /v1/invoice/get | Получить ссылку на счёт-фактуру
@@ -273,18 +280,31 @@
  - [AnalyticsMetric](docs/AnalyticsMetric.md)
  - [AnalyticsSorting](docs/AnalyticsSorting.md)
  - [AnalyticsStockOnWarehouseRequest](docs/AnalyticsStockOnWarehouseRequest.md)
  - [AnalyticsStockOnWarehouseResponse](docs/AnalyticsStockOnWarehouseResponse.md)
  - [AnalyticsStockOnWarehouseResponseResult](docs/AnalyticsStockOnWarehouseResponseResult.md)
  - [AnalyticsStockOnWarehouseResultRows](docs/AnalyticsStockOnWarehouseResultRows.md)
  - [ApproveDeclineDiscountTasksResponseFailDetail](docs/ApproveDeclineDiscountTasksResponseFailDetail.md)
+ - [ArrivalPassListRequestFilter](docs/ArrivalPassListRequestFilter.md)
+ - [ArrivalpassArrivalPassCreateRequest](docs/ArrivalpassArrivalPassCreateRequest.md)
+ - [ArrivalpassArrivalPassCreateRequestArrivalPass](docs/ArrivalpassArrivalPassCreateRequestArrivalPass.md)
+ - [ArrivalpassArrivalPassCreateResponse](docs/ArrivalpassArrivalPassCreateResponse.md)
+ - [ArrivalpassArrivalPassDeleteRequest](docs/ArrivalpassArrivalPassDeleteRequest.md)
+ - [ArrivalpassArrivalPassListRequest](docs/ArrivalpassArrivalPassListRequest.md)
+ - [ArrivalpassArrivalPassListResponse](docs/ArrivalpassArrivalPassListResponse.md)
+ - [ArrivalpassArrivalPassListResponseArrivalPass](docs/ArrivalpassArrivalPassListResponseArrivalPass.md)
+ - [ArrivalpassArrivalPassUpdateRequest](docs/ArrivalpassArrivalPassUpdateRequest.md)
+ - [ArrivalpassArrivalPassUpdateRequestArrivalPass](docs/ArrivalpassArrivalPassUpdateRequestArrivalPass.md)
  - [BrandBrandCompanyCertificationListRequest](docs/BrandBrandCompanyCertificationListRequest.md)
  - [BrandBrandCompanyCertificationListResponse](docs/BrandBrandCompanyCertificationListResponse.md)
  - [BrandCompanyCertificationListResponseBrandCertification](docs/BrandCompanyCertificationListResponseBrandCertification.md)
  - [BrandCompanyCertificationListResponseBrandCertificationResult](docs/BrandCompanyCertificationListResponseBrandCertificationResult.md)
+ - [CarriageCarriageGetRequest](docs/CarriageCarriageGetRequest.md)
+ - [CarriageCarriageGetResponse](docs/CarriageCarriageGetResponse.md)
+ - [CarriageCarriageGetResponseCancelAvailability](docs/CarriageCarriageGetResponseCancelAvailability.md)
  - [CertificateCreateBody](docs/CertificateCreateBody.md)
  - [ChatChatSendFileRequest](docs/ChatChatSendFileRequest.md)
  - [ChatChatSendFileResponse](docs/ChatChatSendFileResponse.md)
  - [ChatChatSendMessageRequest](docs/ChatChatSendMessageRequest.md)
  - [ChatChatSendMessageResponse](docs/ChatChatSendMessageResponse.md)
  - [ChatChatStartRequest](docs/ChatChatStartRequest.md)
  - [ChatChatStartResponse](docs/ChatChatStartResponse.md)
@@ -588,14 +608,17 @@
  - [ReportReportInfoRequest](docs/ReportReportInfoRequest.md)
  - [ReportReportInfoResponse](docs/ReportReportInfoResponse.md)
  - [ReportReportListRequest](docs/ReportReportListRequest.md)
  - [ReportReportListResponse](docs/ReportReportListResponse.md)
  - [ResultError](docs/ResultError.md)
  - [ReturnCreateReportResponseCode](docs/ReturnCreateReportResponseCode.md)
  - [ReturnreportCreateReportResponse](docs/ReturnreportCreateReportResponse.md)
+ - [ReturnsCompanyFbsInfoRequestPagination](docs/ReturnsCompanyFbsInfoRequestPagination.md)
+ - [ReturnsCompanyFbsInfoResponseDropOffPoints](docs/ReturnsCompanyFbsInfoResponseDropOffPoints.md)
+ - [ReturnsCompanyFbsInfoResponsePassInfo](docs/ReturnsCompanyFbsInfoResponsePassInfo.md)
  - [ReturnsRfbsGetResponseReturns](docs/ReturnsRfbsGetResponseReturns.md)
  - [ReturnsRfbsGetV2ResponseAvailableAction](docs/ReturnsRfbsGetV2ResponseAvailableAction.md)
  - [ReturnsRfbsGetV2ResponseClientReturnMethodType](docs/ReturnsRfbsGetV2ResponseClientReturnMethodType.md)
  - [ReturnsRfbsGetV2ResponseRejectionReason](docs/ReturnsRfbsGetV2ResponseRejectionReason.md)
  - [ReturnsRfbsGetV2ResponseReturnReason](docs/ReturnsRfbsGetV2ResponseReturnReason.md)
  - [ReturnsRfbsListResponseReturns](docs/ReturnsRfbsListResponseReturns.md)
  - [RpcStatus](docs/RpcStatus.md)
@@ -611,14 +634,20 @@
  - [SellerApiProductPrice](docs/SellerApiProductPrice.md)
  - [SellerApiProductV1Response](docs/SellerApiProductV1Response.md)
  - [SellerApiProductV1ResponseDeactivate](docs/SellerApiProductV1ResponseDeactivate.md)
  - [SellerApiProductV1ResponseProduct](docs/SellerApiProductV1ResponseProduct.md)
  - [SellerApiProductV1ResponseProductDeactivate](docs/SellerApiProductV1ResponseProductDeactivate.md)
  - [SellerApiProductV1ResponseResult](docs/SellerApiProductV1ResponseResult.md)
  - [SellerApiProductV1ResponseResultDeactivate](docs/SellerApiProductV1ResponseResultDeactivate.md)
+ - [SellerSellerAPIArrivalPassCreateRequest](docs/SellerSellerAPIArrivalPassCreateRequest.md)
+ - [SellerSellerAPIArrivalPassCreateRequestArrivalPass](docs/SellerSellerAPIArrivalPassCreateRequestArrivalPass.md)
+ - [SellerSellerAPIArrivalPassCreateResponse](docs/SellerSellerAPIArrivalPassCreateResponse.md)
+ - [SellerSellerAPIArrivalPassDeleteRequest](docs/SellerSellerAPIArrivalPassDeleteRequest.md)
+ - [SellerSellerAPIArrivalPassUpdateRequest](docs/SellerSellerAPIArrivalPassUpdateRequest.md)
+ - [SellerSellerAPIArrivalPassUpdateRequestArrivalPass](docs/SellerSellerAPIArrivalPassUpdateRequestArrivalPass.md)
  - [SellerServiceanalyticsDimension](docs/SellerServiceanalyticsDimension.md)
  - [SortingOrder](docs/SortingOrder.md)
  - [SupplierAvailableWarehousesResponseCapacity](docs/SupplierAvailableWarehousesResponseCapacity.md)
  - [SupplierAvailableWarehousesResponseResult](docs/SupplierAvailableWarehousesResponseResult.md)
  - [SupplierAvailableWarehousesResponseSchedule](docs/SupplierAvailableWarehousesResponseSchedule.md)
  - [SupplierAvailableWarehousesResponseWarehouse](docs/SupplierAvailableWarehousesResponseWarehouse.md)
  - [V1ActivateHotSalesProductsRequest](docs/V1ActivateHotSalesProductsRequest.md)
@@ -779,14 +808,17 @@
  - [V1Rating](docs/V1Rating.md)
  - [V1RatingHistoryV1Request](docs/V1RatingHistoryV1Request.md)
  - [V1RatingHistoryV1Response](docs/V1RatingHistoryV1Response.md)
  - [V1RatingItem](docs/V1RatingItem.md)
  - [V1RatingStatus](docs/V1RatingStatus.md)
  - [V1RatingSummaryV1Response](docs/V1RatingSummaryV1Response.md)
  - [V1Restriction](docs/V1Restriction.md)
+ - [V1ReturnsCompanyFbsInfoRequest](docs/V1ReturnsCompanyFbsInfoRequest.md)
+ - [V1ReturnsCompanyFbsInfoRequestFilter](docs/V1ReturnsCompanyFbsInfoRequestFilter.md)
+ - [V1ReturnsCompanyFbsInfoResponse](docs/V1ReturnsCompanyFbsInfoResponse.md)
  - [V1SellerWarehouse](docs/V1SellerWarehouse.md)
  - [V1SetActivateHotSaleProductsResult](docs/V1SetActivateHotSaleProductsResult.md)
  - [V1SetActivateHotSaleProductsResultProduct](docs/V1SetActivateHotSaleProductsResultProduct.md)
  - [V1SetActivateHotSaleProductsResultResult](docs/V1SetActivateHotSaleProductsResultResult.md)
  - [V1SetDeactivateHotSaleProductsResult](docs/V1SetDeactivateHotSaleProductsResult.md)
  - [V1SetDeactivateHotSaleProductsResultProduct](docs/V1SetDeactivateHotSaleProductsResultProduct.md)
  - [V1SetDeactivateHotSaleProductsResultResult](docs/V1SetDeactivateHotSaleProductsResultResult.md)
```

### Comparing `ozon_api_client-0.0.4/ozon_api_client/__init__.py` & `ozon_api_client-0.0.5/ozon_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/__init__.py` & `ozon_api_client-0.0.5/ozon_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/analytics_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/analytics_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/barcode_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/barcode_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/brand_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/brand_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/cancellation_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/cancellation_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/category_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/category_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/certification_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/certification_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/chat_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/chat_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/fbo_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/fbo_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/fbs_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/fbs_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/fbsr_fbs_marks_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/fbsr_fbs_marks_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/finance_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/finance_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/polygon_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/polygon_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/prices_stocks_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/prices_stocks_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/pricing_strategy_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/pricing_strategy_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/product_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/product_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/promos_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/promos_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/report_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/report_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/return_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/return_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/returns_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/returns_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/rfbs_returns_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/rfbs_returns_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/seller_rating_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/seller_rating_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/supplier_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/supplier_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api/warehouse_api_api.py` & `ozon_api_client-0.0.5/ozon_api_client/api/warehouse_api_api.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/api_client.py` & `ozon_api_client-0.0.5/ozon_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/configuration.py` & `ozon_api_client-0.0.5/ozon_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/__init__.py` & `ozon_api_client-0.0.5/ozon_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/add_strategy_items_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/add_strategy_items_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_analytics_get_data_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_analytics_get_data_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_analytics_get_data_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_analytics_get_data_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_data_row.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_data_row.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_data_row_dimension.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_data_row_dimension.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_get_data_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_get_data_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_get_stock_on_warehouses_request_warehouse_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_get_stock_on_warehouses_request_warehouse_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_metric.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_metric.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_sorting.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_sorting.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/analytics_stock_on_warehouse_result_rows.py` & `ozon_api_client-0.0.5/ozon_api_client/models/analytics_stock_on_warehouse_result_rows.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/approve_decline_discount_tasks_response_fail_detail.py` & `ozon_api_client-0.0.5/ozon_api_client/models/approve_decline_discount_tasks_response_fail_detail.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/brand_brand_company_certification_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/brand_brand_company_certification_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/brand_brand_company_certification_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/brand_brand_company_certification_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/brand_company_certification_list_response_brand_certification.py` & `ozon_api_client-0.0.5/ozon_api_client/models/brand_company_certification_list_response_brand_certification.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/brand_company_certification_list_response_brand_certification_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/brand_company_certification_list_response_brand_certification_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/certificate_create_body.py` & `ozon_api_client-0.0.5/ozon_api_client/models/certificate_create_body.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_file_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_file_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_file_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_file_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_message_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_message_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_send_message_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_send_message_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_start_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_start_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_chat_start_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_chat_start_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_history.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_history.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_list.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_list.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_read.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_read.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/chat_start_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/chat_start_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/common_create_report_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/common_create_report_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/common_price_indexes.py` & `ozon_api_client-0.0.5/ozon_api_client/models/common_price_indexes.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/common_returns_company_item_fbo.py` & `ozon_api_client-0.0.5/ozon_api_client/models/common_returns_company_item_fbo.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/common_returns_company_item_fbs.py` & `ozon_api_client-0.0.5/ozon_api_client/models/common_returns_company_item_fbs.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/common_time_range_last_day.py` & `ozon_api_client-0.0.5/ozon_api_client/models/common_time_range_last_day.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/conditional_cancellation_cancellation_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/conditional_cancellation_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/conditional_cancellation_state.py` & `ozon_api_client-0.0.5/ozon_api_client/models/conditional_cancellation_state.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/create_report_response_code.py` & `ozon_api_client-0.0.5/ozon_api_client/models/create_report_response_code.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/created_at.py` & `ozon_api_client-0.0.5/ozon_api_client/models/created_at.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/delete_products_request_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/delete_products_request_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/delete_products_response_delete_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/delete_products_response_delete_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/delivery_method_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/delivery_method_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/delivery_method_list_response_delivery_method.py` & `ozon_api_client-0.0.5/ozon_api_client/models/delivery_method_list_response_delivery_method.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_delivery_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_delivery_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_others.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_others.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_payment.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_payment.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_return_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_return_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_returns.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_returns.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_rfbs_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_rfbs_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_service.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_service.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/details_services.py` & `ozon_api_client-0.0.5/ozon_api_client/models/details_services.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbo_posting_fbo_posting_analytics_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbo_posting_fbo_posting_analytics_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_barcodes.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_barcodes.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_detail_courier.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_detail_courier.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_detail_prr_option.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_detail_prr_option.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_fbs_posting_analytics_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_fbs_posting_analytics_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_move_status_response_move_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_move_status_response_move_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_product_exemplar_validate_response_fbs_posting_product_exemplar_validate_result_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_package.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_package.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_package_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_package_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_request_with.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_request_with.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_ship_v4_response_ship_additional_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_ship_v4_response_ship_additional_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbs_posting_tracking_number_set_request_tracking_number.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbs_posting_tracking_number_set_request_tracking_number.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_fbs_posting_ship_v4_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_get_product_exemplar_status_response_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_posting_product_detail_without_dimensions.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_posting_product_detail_without_dimensions.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_request_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_request_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/fbsv4_set_product_exemplar_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/fbsv4_set_product_exemplar_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/filter_op.py` & `ozon_api_client-0.0.5/ozon_api_client/models/filter_op.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/filter_period.py` & `ozon_api_client-0.0.5/ozon_api_client/models/filter_period.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_cash_flow.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_cash_flow.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_delivery_service.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_delivery_service.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_details_others.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_details_others.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_return_service.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_return_service.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_cash_flow_statement_list_response_service.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_cash_flow_statement_list_response_service.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_get_realization_report_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_get_realization_report_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_get_realization_report_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_get_realization_report_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_header.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_header.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_realization_report_rows.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_realization_report_rows.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_list_v3_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_list_v3_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_list_v3_response_operation.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_list_v3_response_operation.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/finance_transaction_totals_v3_request_date.py` & `ozon_api_client-0.0.5/ozon_api_client/models/finance_transaction_totals_v3_request_date.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_list_v3_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_list_v3_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_finance_transaction_totals_v3_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_finance_transaction_totals_v3_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/financev3_period.py` & `ozon_api_client-0.0.5/ozon_api_client/models/financev3_period.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_carriage_available_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_carriage_available_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_competitors_response_competitor_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_competitors_response_competitor_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_request_filters.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_request_filters.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_request_with.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_request_with.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_conditional_cancellation_list_response_counters.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_conditional_cancellation_list_response_counters.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_request_date.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_request_date.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_etgb_response_result_etgb.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_etgb_response_result_etgb.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_geo_restrictions_by_filter_response_geo_restriction.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_geo_restrictions_by_filter_response_geo_restriction.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_hot_sales_list_response_hot_sale.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_hot_sales_list_response_hot_sale.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_import_products_info_response_result_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_import_products_info_response_result_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_image.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_image.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_image360.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_image360.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_response_pdf.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_response_pdf.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_v3_response_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_v3_response_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_attributes_v3_response_dictionary_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_attributes_v3_response_dictionary_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_list_response_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_list_response_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_list_response_reasons.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_list_response_reasons.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_info_stocks_v3_response_stock.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_info_stocks_v3_response_stock.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_product_rating.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_product_rating.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_condition.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_condition.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_group.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_group.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_product_rating_by_sku_response_rating_improve_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_product_rating_by_sku_response_rating_improve_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_seller_actions_v1_response_action.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_seller_actions_v1_response_action.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_strategy_ids_by_item_ids_response_product_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_strategy_ids_by_item_ids_response_product_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_strategy_list_response_strategy.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_strategy_list_response_strategy.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_supply_order_items_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_supply_order_items_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_supply_orders_list_response_supply_order.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_supply_orders_list_response_supply_order.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_daily_create.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_daily_create.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_daily_update.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_daily_update.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/get_upload_quota_response_total.py` & `ozon_api_client-0.0.5/ozon_api_client/models/get_upload_quota_response_total.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/giveout_info_response_article_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/giveout_info_response_article_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/giveout_list_response_giveout_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/giveout_list_response_giveout_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/googlerpc_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/import_products_request_pdf_list.py` & `ozon_api_client-0.0.5/ozon_api_client/models/import_products_request_pdf_list.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/invoice_get_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/invoice_get_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/item_commissions.py` & `ozon_api_client-0.0.5/ozon_api_client/models/item_commissions.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/item_marketing_actions.py` & `ozon_api_client-0.0.5/ozon_api_client/models/item_marketing_actions.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/item_price.py` & `ozon_api_client-0.0.5/ozon_api_client/models/item_price.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/language_language.py` & `ozon_api_client-0.0.5/ozon_api_client/models/language_language.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/marketing_actions_marketing_action.py` & `ozon_api_client-0.0.5/ozon_api_client/models/marketing_actions_marketing_action.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/operation_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/operation_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/operation_posting.py` & `ozon_api_client-0.0.5/ozon_api_client/models/operation_posting.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/operation_service.py` & `ozon_api_client-0.0.5/ozon_api_client/models/operation_service.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygon_bind_requestpolygon.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygon_bind_requestpolygon.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygon_bind_requestwh_location.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygon_bind_requestwh_location.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_empty.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_empty.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_bind_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_bind_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_create_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_create_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/polygonv1_polygon_create_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/polygonv1_polygon_create_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_boolean_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_boolean_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_fbs_posting_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_fbs_posting_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_cancel_reason_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_cancel_reason_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbo_posting_with_params.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbo_posting_with_params.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_act_check_status_response_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_act_check_status_response_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_act_create_response_act.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_act_create_response_act.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_delivered_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_delivered_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_delivering_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_delivering_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_last_mile_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_last_mile_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_move_status_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_move_status_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_sentbyseller_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_sentbyseller_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_fbs_posting_tracking_number_set_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_fbs_posting_tracking_number_set_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_financial_data_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_financial_data_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_financial_data_services.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_financial_data_services.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbo_posting_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbo_posting_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_get_fbs_posting_by_barcode_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_get_fbs_posting_by_barcode_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_move_posting_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_move_posting_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_check_status_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_check_status_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_check_status_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_check_status_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_create_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_create_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_create_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_create_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_act_get_container_labels_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_get_act_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_get_act_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_get_act_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_get_act_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_package_label_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_package_label_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_fbs_package_label_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_fbs_package_label_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_cancel_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_cancel_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_cancel_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_cancel_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_change_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_change_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_posting_product_change_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_posting_product_change_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_product_cancel_request_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_product_cancel_request_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/posting_product_change_request_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/posting_product_change_request_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv1_get_carriage_available_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv1_get_carriage_available_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv1_get_carriage_available_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv1_get_carriage_available_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_fbs_posting_with_params.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_fbs_posting_with_params.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_fbs_posting_with_params_examplars.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_fbs_posting_with_params_examplars.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_get_fbs_posting_unfulfilled_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv3_posting_multi_box_qty_set_v3_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_request_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/postingv4_fbs_posting_product_exemplar_validate_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/premium_scores_score.py` & `ozon_api_client-0.0.5/ozon_api_client/models/premium_scores_score.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_external.py` & `ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_external.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_ozon.py` & `ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_ozon.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/price_indexes_index_data_self.py` & `ozon_api_client-0.0.5/ozon_api_client/models/price_indexes_index_data_self.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_boolean_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_boolean_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_certificate_products_list_response_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_certificate_products_list_response_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_certificate_unbind_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_certificate_unbind_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_certification_list_response_certification.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_certification_list_response_certification.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_certification_list_response_certification_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_certification_list_response_certification_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_import_products_info_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_import_products_info_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_complex_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_complex_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_attributes_v3_response_dictionary_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_attributes_v3_response_dictionary_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_description_response_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_description_response_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_prices_v4_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_prices_v4_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_get_product_info_prices_v4_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_get_product_info_prices_v4_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_request_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_request_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_by_sku_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_by_sku_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_request_price.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_request_price.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_prices_response_process_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_prices_response_process_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_request_stock.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_request_stock.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_import_products_stocks_response_process_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_import_products_stocks_response_process_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_picking.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_picking.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_archive_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_archive_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_accordance_types_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_accordance_types_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_accordance_types_response_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_accordance_types_response_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_bind_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_bind_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_types_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_types_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certificate_types_response_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certificate_types_response_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certification_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certification_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_certification_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_certification_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_info_pictures_response_picture.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_info_pictures_response_picture.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_product_unarchive_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_product_unarchive_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/product_update_offer_id_request_update_offer_id.py` & `ozon_api_client-0.0.5/ozon_api_client/models/product_update_offer_id_request_update_offer_id.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productsv1_get_product_info_stocks_by_warehouse_fbs_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_import_pictures_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_import_pictures_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv1_product_info_pictures_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv1_product_info_pictures_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_delete_products_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_delete_products_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_delete_products_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_delete_products_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_geo_restrictions_by_filter_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_discounted_stocks.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_discounted_stocks.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_source.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_source.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_stock.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_stock.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_list_response_visibility_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_list_response_visibility_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_commissions.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_commissions.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_source.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_source.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_stock.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_stock.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_info_response_visibility_details.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_info_response_visibility_details.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_request_filter_filter_visibility.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_request_filter_filter_visibility.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_get_product_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_get_product_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_request_stock.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_request_stock.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_products_stocks_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_products_stocks_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv2_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv2_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_attributes_v3_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_attributes_v3_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv3_get_product_info_stocks_v3_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv4_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv4_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv4_get_product_info_prices_v4_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv4_get_product_info_prices_v4_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/productv4_get_product_info_prices_v4_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/productv4_get_product_info_prices_v4_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/protobuf_any.py` & `ozon_api_client-0.0.5/ozon_api_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rating_item_change.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rating_item_change.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rating_summary_v1_response_group.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rating_summary_v1_response_group.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rating_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rating_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/related_posting_cancel_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/related_posting_cancel_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/related_posting_cancel_reasons.py` & `ozon_api_client-0.0.5/ozon_api_client/models/related_posting_cancel_reasons.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_postings_report_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_postings_report_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_postings_report_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_postings_report_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_products_report_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_products_report_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_products_report_request_visibility.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_products_report_request_visibility.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_returns_report_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_returns_report_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_company_returns_report_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_company_returns_report_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_discounted_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_discounted_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_discounted_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_discounted_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_create_report_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_create_report_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_language.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_language.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_list_request_report_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_list_request_report_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_report.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_report.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_report_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_report_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_report_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_report_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_report_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_report_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/report_report_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/report_report_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/result_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/result_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/return_create_report_response_code.py` & `ozon_api_client-0.0.5/ozon_api_client/models/return_create_report_response_code.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returnreport_create_report_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returnreport_create_report_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_response_returns.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_response_returns.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_available_action.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_available_action.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_client_return_method_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_client_return_method_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_rejection_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_rejection_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_get_v2_response_return_reason.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_get_v2_response_return_reason.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/returns_rfbs_list_response_returns.py` & `ozon_api_client-0.0.5/ozon_api_client/models/returns_rfbs_list_response_returns.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rpc_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rpc_status_v1_polygon_bind.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rpc_status_v1_polygon_bind.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/rpc_status_v1_polygon_create.py` & `ozon_api_client-0.0.5/ozon_api_client/models/rpc_status_v1_polygon_create.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_activate_product_v1_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_activate_product_v1_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_actions_v1_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_actions_v1_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_get_seller_product_v1_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_get_seller_product_v1_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_ids_v1_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_ids_v1_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_price.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_price.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_deactivate.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_deactivate.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_product_deactivate.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_product_deactivate.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_api_product_v1_response_result_deactivate.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_api_product_v1_response_result_deactivate.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/seller_serviceanalytics_dimension.py` & `ozon_api_client-0.0.5/ozon_api_client/models/seller_serviceanalytics_dimension.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/sorting_order.py` & `ozon_api_client-0.0.5/ozon_api_client/models/sorting_order.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_capacity.py` & `ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_capacity.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_schedule.py` & `ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_schedule.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/supplier_available_warehouses_response_warehouse.py` & `ozon_api_client-0.0.5/ozon_api_client/models/supplier_available_warehouses_response_warehouse.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_activate_hot_sales_products_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_activate_hot_sales_products_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_activate_hot_sales_products_request_activate_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_activate_hot_sales_products_request_activate_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_barcode_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_barcode_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_add_strategy_items_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_add_strategy_items_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_decline_discount_tasks_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_decline_discount_tasks_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_decline_discount_tasks_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_decline_discount_tasks_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_discount_tasks_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_discount_tasks_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_approve_discount_tasks_request_task.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_approve_discount_tasks_request_task.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_barcode.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_barcode.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_certificate.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_certificate.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_competitor.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_competitor.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_conditional_cancellation.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_conditional_cancellation.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_conditional_cancellation_move_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_conditional_cancellation_move_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_label_batch_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_label_batch_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_pricing_strategy_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_pricing_strategy_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_create_stock_by_warehouse_report_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_create_stock_by_warehouse_report_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_deactivate_hot_sales_products_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_deactivate_hot_sales_products_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_decline_discount_tasks_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_decline_discount_tasks_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_decline_discount_tasks_request_task.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_decline_discount_tasks_request_task.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_delete_strategy_items_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_delete_strategy_items_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_delete_strategy_items_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_delete_strategy_items_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_discount_task_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_discount_task_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_empty.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_empty.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_generate_barcode_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_generate_barcode_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attribute_values_response_dictionary_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attribute_values_response_dictionary_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_attributes_response_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_attributes_response_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_competitors_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_competitors_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_competitors_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_competitors_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_conditional_cancellation_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_conditional_cancellation_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_discount_task_list_response_task.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_discount_task_list_response_task.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_etgb_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_etgb_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_etgb_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_etgb_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_hot_sales_products_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_hot_sales_products_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_label_batch_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_label_batch_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_discounted_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_discounted_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_info_subscription_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_info_subscription_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_rating_by_sku_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_rating_by_sku_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_product_rating_by_sku_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_product_rating_by_sku_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_restrictions_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_restrictions_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_restrictions_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_restrictions_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_ids_by_item_ids_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_item_info_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_item_info_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_items_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_items_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_items_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_items_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_strategy_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_strategy_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_items_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_items_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_items_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_items_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_order_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_order_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_orders_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_orders_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_supply_orders_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_supply_orders_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_get_tree_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_get_tree_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_barcode_reset_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_barcode_reset_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_delivery_schema.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_delivery_schema.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_barcode_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_barcode_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_pdf_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_pdf_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_get_png_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_get_png_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_is_enabled_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_is_enabled_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_giveout_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_giveout_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_hot_sale_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_hot_sale_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_create_or_update_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_create_or_update_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_create_or_update_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_delete_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_delete_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_delete_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_delete_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_get_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_get_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_invoice_get_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_invoice_get_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_item_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_item_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_item_ids_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_item_ids_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_delivery_interval.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_delivery_interval.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_change_restrictions_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_new_timeslot.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_new_timeslot.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_posting_fbs_timeslot_set_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_posting_fbs_timeslot_set_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_premium_scores.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_premium_scores.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_delete_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_delete_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_info_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_info_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_info_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_info_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_product_status_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_product_status_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_product_status_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_product_status_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_products_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_products_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_rejection_reasons_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_status_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_status_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_status_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_status_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_unbind_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_unbind_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_certificate_unbind_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_certificate_unbind_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_get_related_sku_response_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_get_related_sku_response_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_request_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_request_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_attributes_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_attributes_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_discount_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_discount_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_discount_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_discount_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_update_offer_id_response_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_update_offer_id_response_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_request_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_request_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_info_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_info_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_product_upload_digital_codes_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_product_upload_digital_codes_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_history_v1_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_history_v1_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_history_v1_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_history_v1_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_status.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_status.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_rating_summary_v1_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_rating_summary_v1_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_restriction.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_restriction.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_seller_warehouse.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_seller_warehouse.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_activate_hot_sale_products_result_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_activate_hot_sale_products_result_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_set_deactivate_hot_sale_products_result_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair_rejection.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair_rejection.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_status_code_name_pair_statuses.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_status_code_name_pair_statuses.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_strategy_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_strategy_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_supplier_available_warehouses_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_supplier_available_warehouses_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_timeslot.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_timeslot.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_update_pricing_strategy_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_update_pricing_strategy_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_update_status_strategy_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_update_status_strategy_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_vehicle_info.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_vehicle_info.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v1_warehouse.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v1_warehouse.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_additional_data_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_additional_data_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_history_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_history_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_message.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_message.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_chat_read_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_chat_read_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbo_posting_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbo_posting_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_set_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_set_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_product_country_set_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_product_country_set_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_fbs_posting_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_fbs_posting_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_get_geo_restrictions_by_filter_request_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_get_geo_restrictions_by_filter_request_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_item_error.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_item_error.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_postings_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_postings_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_get_products.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_get_products.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_acceptance.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_acceptance.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_excess.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_excess.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_mismatch.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_related_docs_act_of_mismatch.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_act_list_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_act_list_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_check_status_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_digital_act_document_sign_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_barcode_text_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_barcode_text_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_digital_act_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_digital_act_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_fbs_get_digital_act_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_fbs_get_digital_act_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_financial_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_financial_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_posting_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_posting_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_product_certificate_accordance_types_response_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_product_certificate_accordance_types_response_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_compensate_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_compensate_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_filter.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_filter.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_get_v2_response_state.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_get_v2_response_state.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_list_v2_response_state.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_list_v2_response_state.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_receive_return_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_receive_return_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_reject_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_reject_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_return_money_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_return_money_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_returns_rfbs_verify_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_returns_rfbs_verify_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v2_user.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v2_user.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_additional_data_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_additional_data_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_address.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_address.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_addressee.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_addressee.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_addressee_fbs_lists.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_addressee_fbs_lists.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_barcodes.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_barcodes.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_cancellation.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_cancellation.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_customer.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_customer.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_customer_fbs_lists.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_customer_fbs_lists.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_delivery_method.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_delivery_method.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_dimensions.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_dimensions.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_analytics_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_analytics_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_detail.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_detail.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_detail_related_postings.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_detail_related_postings.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_exemplar_product_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_exemplar_product_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product_exemplar_info_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product_exemplar_info_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_product_exemplars_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_product_exemplars_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_fbs_posting_requirements_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_fbs_posting_requirements_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_period.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_period.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_finance_cash_flow_statement_list_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_list_response_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_list_response_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_list_response_v3_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_list_response_v3_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_fbs_posting_response_v3.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_fbs_posting_response_v3.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbo_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbo_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbo_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbo_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbs_v3_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbs_v3_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_get_returns_company_fbs_v3_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_get_returns_company_fbs_v3_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_complex_attribute.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_complex_attribute.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_dictionary_value.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_dictionary_value.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_request_item.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_request_item.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_import_products_response_result.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_import_products_response_result.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_posting_financial_data.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_posting_financial_data.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_posting_product_detail.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_posting_product_detail.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_returns_company_filter_fbo.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_returns_company_filter_fbo.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_returns_company_filter_fbs.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_returns_company_filter_fbs.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v3_service_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v3_service_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_request_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v4_fbs_posting_ship_package_v4_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v4_fbs_posting_ship_package_v4_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v4_get_upload_quota_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v4_get_upload_quota_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_create_or_get_v5_response_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product_exemplar.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_request_product_exemplar.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/v5_fbs_posting_product_exemplar_set_v5_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/warehouse_delivery_method_list_request.py` & `ozon_api_client-0.0.5/ozon_api_client/models/warehouse_delivery_method_list_request.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/warehouse_delivery_method_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/warehouse_delivery_method_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/warehouse_first_mile_type.py` & `ozon_api_client-0.0.5/ozon_api_client/models/warehouse_first_mile_type.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/warehouse_list_response_warehouse.py` & `ozon_api_client-0.0.5/ozon_api_client/models/warehouse_list_response_warehouse.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/models/warehouse_warehouse_list_response.py` & `ozon_api_client-0.0.5/ozon_api_client/models/warehouse_warehouse_list_response.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/ozon_api_client/rest.py` & `ozon_api_client-0.0.5/ozon_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ozon_api_client-0.0.4/PKG-INFO` & `ozon_api_client-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozon-api-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: letby3
 Author-email: fvahit2@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,61 +38,59 @@
 
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
-
 ```python
-import ozon_api_client 
+import swagger_client 
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
-
 ```python
-import ozon_api_client
+import swagger_client
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 from __future__ import print_function
 import time
-import ozon_api_client
-from ozon_api_client.rest import ApiException
+import swagger_client
+from swagger_client.rest import ApiException
 from pprint import pprint
 
 # create an instance of the API class
-api_instance = ozon_api_client.AnalyticsAPIApi(ozon_api_client.ApiClient(configuration))
-body = ozon_api_client.AnalyticsAnalyticsGetDataRequest() # AnalyticsAnalyticsGetDataRequest | 
+api_instance = swagger_client.AnalyticsAPIApi(swagger_client.ApiClient(configuration))
+body = swagger_client.AnalyticsAnalyticsGetDataRequest() # AnalyticsAnalyticsGetDataRequest | 
 client_id = 'client_id_example' # str | Идентификатор клиента.
 api_key = 'api_key_example' # str | API-ключ.
 
 try:
     # Данные аналитики
     api_response = api_instance.analytics_api_analytics_get_data(body, client_id, api_key)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AnalyticsAPIApi->analytics_api_analytics_get_data: %s\n" % e)
 
 # create an instance of the API class
-api_instance = ozon_api_client.AnalyticsAPIApi(ozon_api_client.ApiClient(configuration))
-body = ozon_api_client.AnalyticsStockOnWarehouseRequest() # AnalyticsStockOnWarehouseRequest | 
+api_instance = swagger_client.AnalyticsAPIApi(swagger_client.ApiClient(configuration))
+body = swagger_client.AnalyticsStockOnWarehouseRequest() # AnalyticsStockOnWarehouseRequest | 
 client_id = 'client_id_example' # str | Идентификатор клиента.
 api_key = 'api_key_example' # str | API-ключ.
 
 try:
     # Отчёт по остаткам и товарам
     api_response = api_instance.analytics_api_analytics_get_stock_on_warehouses_v2(body, client_id, api_key)
     pprint(api_response)
@@ -134,68 +132,76 @@
 *CertificationAPIApi* | [**rejection_reasons_list**](docs/CertificationAPIApi.md#rejection_reasons_list) | **POST** /v1/product/certificate/rejection_reasons/list | Возможные причины отклонения сертификата
 *ChatAPIApi* | [**chat_api_chat_history_v2**](docs/ChatAPIApi.md#chat_api_chat_history_v2) | **POST** /v2/chat/history | История чата
 *ChatAPIApi* | [**chat_api_chat_list_v2**](docs/ChatAPIApi.md#chat_api_chat_list_v2) | **POST** /v2/chat/list | Список чатов
 *ChatAPIApi* | [**chat_api_chat_read_v2**](docs/ChatAPIApi.md#chat_api_chat_read_v2) | **POST** /v2/chat/read | Отметить сообщения как прочитанные
 *ChatAPIApi* | [**chat_api_chat_send_file**](docs/ChatAPIApi.md#chat_api_chat_send_file) | **POST** /v1/chat/send/file | Отправить файл
 *ChatAPIApi* | [**chat_api_chat_send_message**](docs/ChatAPIApi.md#chat_api_chat_send_message) | **POST** /v1/chat/send/message | Отправить сообщение
 *ChatAPIApi* | [**chat_api_chat_start**](docs/ChatAPIApi.md#chat_api_chat_start) | **POST** /v1/chat/start | Создать новый чат
+*DeliveryFBSApi* | [**carriage_get**](docs/DeliveryFBSApi.md#carriage_get) | **POST** /v1/carriage/get | Информация о перевозке
+*DeliveryFBSApi* | [**posting_api_act_posting_list**](docs/DeliveryFBSApi.md#posting_api_act_posting_list) | **POST** /v2/posting/fbs/act/get-postings | Список отправлений в акте
+*DeliveryFBSApi* | [**posting_api_digital_act_document_sign**](docs/DeliveryFBSApi.md#posting_api_digital_act_document_sign) | **POST** /v2/posting/fbs/digital/act/document-sign | Подписать документы по отгрузке
+*DeliveryFBSApi* | [**posting_api_fbs_act_list**](docs/DeliveryFBSApi.md#posting_api_fbs_act_list) | **POST** /v2/posting/fbs/act/list | Список актов по отгрузкам
+*DeliveryFBSApi* | [**posting_api_get_carriage_available_list**](docs/DeliveryFBSApi.md#posting_api_get_carriage_available_list) | **POST** /v1/posting/carriage-available/list | Список доступных перевозок
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_check_status**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_check_status) | **POST** /v2/posting/fbs/act/check-status | Статус отгрузки и документов
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_create**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_create) | **POST** /v2/posting/fbs/act/create | Подтвердить отгрузку и создать документы
+*DeliveryFBSApi* | [**posting_api_posting_fbs_act_get_container_labels**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_act_get_container_labels) | **POST** /v2/posting/fbs/act/get-container-labels | Этикетки для грузового места
+*DeliveryFBSApi* | [**posting_api_posting_fbs_digital_act_check_status**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_digital_act_check_status) | **POST** /v2/posting/fbs/digital/act/check-status | Статус формирования накладной
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_act**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_act) | **POST** /v2/posting/fbs/act/get-pdf | Получить PDF c документами
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_barcode**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_barcode) | **POST** /v2/posting/fbs/act/get-barcode | Штрихкод для отгрузки отправления
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_barcode_text**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_barcode_text) | **POST** /v2/posting/fbs/act/get-barcode/text | Значение штрихкода для отгрузки отправления
+*DeliveryFBSApi* | [**posting_api_posting_fbs_get_digital_act**](docs/DeliveryFBSApi.md#posting_api_posting_fbs_get_digital_act) | **POST** /v2/posting/fbs/digital/act/get-pdf | Получить лист отгрузки по перевозке
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_delivered**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_delivered) | **POST** /v2/fbs/posting/delivered | Изменить статус на «Доставлено»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_delivering**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_delivering) | **POST** /v2/fbs/posting/delivering | Изменить статус на «Доставляется»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_last_mile**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_last_mile) | **POST** /v2/fbs/posting/last-mile | Изменить статус на «Последняя миля»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_sentbyseller**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_sentbyseller) | **POST** /v2/fbs/posting/sent-by-seller | Изменить статус на «Отправлено продавцом»
+*DeliveryrFBSApi* | [**posting_api_fbs_posting_tracking_number_set**](docs/DeliveryrFBSApi.md#posting_api_fbs_posting_tracking_number_set) | **POST** /v2/fbs/posting/tracking-number/set | Добавить трек-номера
+*DeliveryrFBSApi* | [**posting_api_posting_timeslot_change_restrictions**](docs/DeliveryrFBSApi.md#posting_api_posting_timeslot_change_restrictions) | **POST** /v1/posting/fbs/timeslot/change-restrictions | Доступные даты для переноса доставки
+*DeliveryrFBSApi* | [**posting_api_set_posting_timeslot**](docs/DeliveryrFBSApi.md#posting_api_set_posting_timeslot) | **POST** /v1/posting/fbs/timeslot/set | Перенести дату доставки
 *FBOApi* | [**posting_api_get_fbo_posting**](docs/FBOApi.md#posting_api_get_fbo_posting) | **POST** /v2/posting/fbo/get | Информация об отправлении
 *FBOApi* | [**posting_api_get_fbo_posting_list**](docs/FBOApi.md#posting_api_get_fbo_posting_list) | **POST** /v2/posting/fbo/list | Список отправлений
 *FBOApi* | [**supplier_api_supplier_available_warehouses**](docs/FBOApi.md#supplier_api_supplier_available_warehouses) | **GET** /v1/supplier/available_warehouses | Загруженность складов Ozon
 *FBOApi* | [**supply_order_api_get_supply_order**](docs/FBOApi.md#supply_order_api_get_supply_order) | **POST** /v1/supply-order/get | Информация о заявке на поставку
 *FBOApi* | [**supply_order_api_get_supply_order_items**](docs/FBOApi.md#supply_order_api_get_supply_order_items) | **POST** /v1/supply-order/items | Список товаров в заявке на поставку
 *FBOApi* | [**supply_order_api_get_supply_orders_list**](docs/FBOApi.md#supply_order_api_get_supply_orders_list) | **POST** /v1/supply-order/list | Список заявок на поставку на склад Ozon
-*FBSApi* | [**posting_api_act_posting_list**](docs/FBSApi.md#posting_api_act_posting_list) | **POST** /v2/posting/fbs/act/get-postings | Список отправлений в акте
 *FBSApi* | [**posting_api_cancel_fbs_posting**](docs/FBSApi.md#posting_api_cancel_fbs_posting) | **POST** /v2/posting/fbs/cancel | Отменить отправление
 *FBSApi* | [**posting_api_cancel_fbs_posting_product**](docs/FBSApi.md#posting_api_cancel_fbs_posting_product) | **POST** /v2/posting/fbs/product/cancel | Отменить отправку некоторых товаров в отправлении
 *FBSApi* | [**posting_api_change_fbs_posting_product**](docs/FBSApi.md#posting_api_change_fbs_posting_product) | **POST** /v2/posting/fbs/product/change | Добавить вес для весовых товаров в отправлении
 *FBSApi* | [**posting_api_create_label_batch**](docs/FBSApi.md#posting_api_create_label_batch) | **POST** /v1/posting/fbs/package-label/create | Создать задание на выгрузку этикеток
-*FBSApi* | [**posting_api_digital_act_document_sign**](docs/FBSApi.md#posting_api_digital_act_document_sign) | **POST** /v2/posting/fbs/digital/act/document-sign | Подписать документы по отгрузке
-*FBSApi* | [**posting_api_fbs_act_list**](docs/FBSApi.md#posting_api_fbs_act_list) | **POST** /v2/posting/fbs/act/list | Список актов по отгрузкам
-*FBSApi* | [**posting_api_fbs_posting_delivered**](docs/FBSApi.md#posting_api_fbs_posting_delivered) | **POST** /v2/fbs/posting/delivered | Изменить статус на «Доставлено»
-*FBSApi* | [**posting_api_fbs_posting_delivering**](docs/FBSApi.md#posting_api_fbs_posting_delivering) | **POST** /v2/fbs/posting/delivering | Изменить статус на «Доставляется»
-*FBSApi* | [**posting_api_fbs_posting_last_mile**](docs/FBSApi.md#posting_api_fbs_posting_last_mile) | **POST** /v2/fbs/posting/last-mile | Изменить статус на «Последняя миля»
-*FBSApi* | [**posting_api_fbs_posting_sentbyseller**](docs/FBSApi.md#posting_api_fbs_posting_sentbyseller) | **POST** /v2/fbs/posting/sent-by-seller | Изменить статус на «Отправлено продавцом»
-*FBSApi* | [**posting_api_fbs_posting_tracking_number_set**](docs/FBSApi.md#posting_api_fbs_posting_tracking_number_set) | **POST** /v2/fbs/posting/tracking-number/set | Добавить трек-номера
-*FBSApi* | [**posting_api_get_carriage_available_list**](docs/FBSApi.md#posting_api_get_carriage_available_list) | **POST** /v1/posting/carriage-available/list | Список доступных перевозок
 *FBSApi* | [**posting_api_get_etgb**](docs/FBSApi.md#posting_api_get_etgb) | **POST** /v1/posting/global/etgb | Таможенные декларации ETGB
 *FBSApi* | [**posting_api_get_fbs_posting_by_barcode**](docs/FBSApi.md#posting_api_get_fbs_posting_by_barcode) | **POST** /v2/posting/fbs/get-by-barcode | Получить информацию об отправлении по штрихкоду
 *FBSApi* | [**posting_api_get_fbs_posting_list_v3**](docs/FBSApi.md#posting_api_get_fbs_posting_list_v3) | **POST** /v3/posting/fbs/list | Список отправлений (версия 3)
 *FBSApi* | [**posting_api_get_fbs_posting_unfulfilled_list**](docs/FBSApi.md#posting_api_get_fbs_posting_unfulfilled_list) | **POST** /v3/posting/fbs/unfulfilled/list | Список необработанных отправлений (версия 3)
 *FBSApi* | [**posting_api_get_fbs_posting_v3**](docs/FBSApi.md#posting_api_get_fbs_posting_v3) | **POST** /v3/posting/fbs/get | Получить информацию об отправлении по идентификатору
 *FBSApi* | [**posting_api_get_label_batch**](docs/FBSApi.md#posting_api_get_label_batch) | **POST** /v1/posting/fbs/package-label/get | Получить файл с этикетками
 *FBSApi* | [**posting_api_get_posting_fbs_cancel_reason_list**](docs/FBSApi.md#posting_api_get_posting_fbs_cancel_reason_list) | **POST** /v2/posting/fbs/cancel-reason/list | Причины отмены отправлений
 *FBSApi* | [**posting_api_get_posting_fbs_cancel_reason_v1**](docs/FBSApi.md#posting_api_get_posting_fbs_cancel_reason_v1) | **POST** /v1/posting/fbs/cancel-reason | Причины отмены отправления
 *FBSApi* | [**posting_api_get_restrictions**](docs/FBSApi.md#posting_api_get_restrictions) | **POST** /v1/posting/fbs/restrictions | Получить ограничения пункта приёма
 *FBSApi* | [**posting_api_list_country_product_fbs_posting_v2**](docs/FBSApi.md#posting_api_list_country_product_fbs_posting_v2) | **POST** /v2/posting/fbs/product/country/list | Список доступных стран-изготовителей
 *FBSApi* | [**posting_api_move_fbs_posting_to_arbitration**](docs/FBSApi.md#posting_api_move_fbs_posting_to_arbitration) | **POST** /v2/posting/fbs/arbitration | Открыть спор по отправлению
 *FBSApi* | [**posting_api_move_fbs_posting_to_awaiting_delivery**](docs/FBSApi.md#posting_api_move_fbs_posting_to_awaiting_delivery) | **POST** /v2/posting/fbs/awaiting-delivery | Передать отправление к отгрузке
-*FBSApi* | [**posting_api_posting_fbs_act_check_status**](docs/FBSApi.md#posting_api_posting_fbs_act_check_status) | **POST** /v2/posting/fbs/act/check-status | Статус отгрузки и документов
-*FBSApi* | [**posting_api_posting_fbs_act_create**](docs/FBSApi.md#posting_api_posting_fbs_act_create) | **POST** /v2/posting/fbs/act/create | Подтвердить отгрузку и создать документы
-*FBSApi* | [**posting_api_posting_fbs_act_get_container_labels**](docs/FBSApi.md#posting_api_posting_fbs_act_get_container_labels) | **POST** /v2/posting/fbs/act/get-container-labels | Этикетки для грузового места
-*FBSApi* | [**posting_api_posting_fbs_digital_act_check_status**](docs/FBSApi.md#posting_api_posting_fbs_digital_act_check_status) | **POST** /v2/posting/fbs/digital/act/check-status | Статус формирования накладной
-*FBSApi* | [**posting_api_posting_fbs_get_act**](docs/FBSApi.md#posting_api_posting_fbs_get_act) | **POST** /v2/posting/fbs/act/get-pdf | Получить PDF c документами
-*FBSApi* | [**posting_api_posting_fbs_get_barcode**](docs/FBSApi.md#posting_api_posting_fbs_get_barcode) | **POST** /v2/posting/fbs/act/get-barcode | Штрихкод для отгрузки отправления
-*FBSApi* | [**posting_api_posting_fbs_get_barcode_text**](docs/FBSApi.md#posting_api_posting_fbs_get_barcode_text) | **POST** /v2/posting/fbs/act/get-barcode/text | Значение штрихкода для отгрузки отправления
-*FBSApi* | [**posting_api_posting_fbs_get_digital_act**](docs/FBSApi.md#posting_api_posting_fbs_get_digital_act) | **POST** /v2/posting/fbs/digital/act/get-pdf | Получить лист отгрузки по перевозке
 *FBSApi* | [**posting_api_posting_fbs_package_label**](docs/FBSApi.md#posting_api_posting_fbs_package_label) | **POST** /v2/posting/fbs/package-label | Напечатать этикетку
 *FBSApi* | [**posting_api_posting_multi_box_qty_set_v3**](docs/FBSApi.md#posting_api_posting_multi_box_qty_set_v3) | **POST** /v3/posting/multiboxqty/set | Указать количество коробок для многокоробочных отправлений
-*FBSApi* | [**posting_api_posting_timeslot_change_restrictions**](docs/FBSApi.md#posting_api_posting_timeslot_change_restrictions) | **POST** /v1/posting/fbs/timeslot/change-restrictions | Доступные даты для переноса доставки
 *FBSApi* | [**posting_api_set_country_product_fbs_posting_v2**](docs/FBSApi.md#posting_api_set_country_product_fbs_posting_v2) | **POST** /v2/posting/fbs/product/country/set | Добавить информацию о стране-изготовителе товара
-*FBSApi* | [**posting_api_set_posting_timeslot**](docs/FBSApi.md#posting_api_set_posting_timeslot) | **POST** /v1/posting/fbs/timeslot/set | Перенести дату доставки
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_create_or_get**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_create_or_get) | **POST** /v5/fbs/posting/product/exemplar/create-or-get | Получить данные созданных экземпляров
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_set**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_set) | **POST** /v5/fbs/posting/product/exemplar/set | Проверить и сохранить данные экземпляров (версия 5)
 *FBSrFBSMarksApi* | [**posting_api_fbs_posting_product_exemplar_validate**](docs/FBSrFBSMarksApi.md#posting_api_fbs_posting_product_exemplar_validate) | **POST** /v4/fbs/posting/product/exemplar/validate | Валидация кодов маркировки
 *FBSrFBSMarksApi* | [**posting_api_get_product_exemplar_status**](docs/FBSrFBSMarksApi.md#posting_api_get_product_exemplar_status) | **POST** /v4/fbs/posting/product/exemplar/status | Получить статус добавления экземпляров
 *FBSrFBSMarksApi* | [**posting_api_set_product_exemplar**](docs/FBSrFBSMarksApi.md#posting_api_set_product_exemplar) | **POST** /v4/fbs/posting/product/exemplar/set | Проверить и сохранить данные экземпляров
 *FBSrFBSMarksApi* | [**posting_api_ship_fbs_posting_package**](docs/FBSrFBSMarksApi.md#posting_api_ship_fbs_posting_package) | **POST** /v4/posting/fbs/ship/package | Частичная сборка отправления (версия 4)
 *FBSrFBSMarksApi* | [**posting_api_ship_fbs_posting_v4**](docs/FBSrFBSMarksApi.md#posting_api_ship_fbs_posting_v4) | **POST** /v4/posting/fbs/ship | Собрать заказ (версия 4)
 *FinanceAPIApi* | [**finance_api_finance_transaction_list_v3**](docs/FinanceAPIApi.md#finance_api_finance_transaction_list_v3) | **POST** /v3/finance/transaction/list | Список транзакций
 *FinanceAPIApi* | [**finance_api_finance_transaction_total_v3**](docs/FinanceAPIApi.md#finance_api_finance_transaction_total_v3) | **POST** /v3/finance/transaction/totals | Суммы транзакций
 *FinanceAPIApi* | [**finance_api_get_realization_report**](docs/FinanceAPIApi.md#finance_api_get_realization_report) | **POST** /v1/finance/realization | Отчёт о реализации товаров
+*PassApi* | [**carriage_pass_create**](docs/PassApi.md#carriage_pass_create) | **POST** /v1/carriage/pass/create | Создать пропуск
+*PassApi* | [**carriage_pass_delete**](docs/PassApi.md#carriage_pass_delete) | **POST** /v1/carriage/pass/delete | Удалить пропуск
+*PassApi* | [**carriage_pass_update**](docs/PassApi.md#carriage_pass_update) | **POST** /v1/carriage/pass/update | Обновить пропуск
+*PassApi* | [**pass_list**](docs/PassApi.md#pass_list) | **POST** /v1/pass/list | Список пропусков
+*PassApi* | [**return_pass_create**](docs/PassApi.md#return_pass_create) | **POST** /v1/return/pass/create | Создать пропуск для возврата
+*PassApi* | [**return_pass_delete**](docs/PassApi.md#return_pass_delete) | **POST** /v1/return/pass/delete | Удалить пропуск для возврата
+*PassApi* | [**return_pass_update**](docs/PassApi.md#return_pass_update) | **POST** /v1/return/pass/update | Обновить пропуск для возврата
 *PolygonAPIApi* | [**polygon_api_bind_polygon**](docs/PolygonAPIApi.md#polygon_api_bind_polygon) | **POST** /v1/polygon/bind | Свяжите метод доставки с полигоном доставки
 *PolygonAPIApi* | [**polygon_api_create_polygon**](docs/PolygonAPIApi.md#polygon_api_create_polygon) | **POST** /v1/polygon/create | Создайте полигон доставки
 *PricesStocksAPIApi* | [**product_api_get_product_info_discounted**](docs/PricesStocksAPIApi.md#product_api_get_product_info_discounted) | **POST** /v1/product/info/discounted | Узнать информацию об уценке и основном товаре по SKU уценённого товара
 *PricesStocksAPIApi* | [**product_api_get_product_info_prices_v4**](docs/PricesStocksAPIApi.md#product_api_get_product_info_prices_v4) | **POST** /v4/product/info/prices | Получить информацию о цене товара
 *PricesStocksAPIApi* | [**product_api_get_product_info_stocks_v3**](docs/PricesStocksAPIApi.md#product_api_get_product_info_stocks_v3) | **POST** /v3/product/info/stocks | Информация о количестве товаров
 *PricesStocksAPIApi* | [**product_api_import_products_prices**](docs/PricesStocksAPIApi.md#product_api_import_products_prices) | **POST** /v1/product/import/prices | Обновить цену
 *PricesStocksAPIApi* | [**product_api_import_products_stocks**](docs/PricesStocksAPIApi.md#product_api_import_products_stocks) | **POST** /v1/product/import/stocks | Обновить остатки
@@ -266,14 +272,15 @@
 *ReturnAPIApi* | [**return_api_giveout_barcode_reset**](docs/ReturnAPIApi.md#return_api_giveout_barcode_reset) | **POST** /v1/return/giveout/barcode-reset | Сгенерировать новый штрихкод
 *ReturnAPIApi* | [**return_api_giveout_get_barcode**](docs/ReturnAPIApi.md#return_api_giveout_get_barcode) | **POST** /v1/return/giveout/barcode | Значение штрихкода для возвратных отгрузок
 *ReturnAPIApi* | [**return_api_giveout_get_pdf**](docs/ReturnAPIApi.md#return_api_giveout_get_pdf) | **POST** /v1/return/giveout/get-pdf | Штрихкод для получения возвратной отгрузки в формате PDF
 *ReturnAPIApi* | [**return_api_giveout_get_png**](docs/ReturnAPIApi.md#return_api_giveout_get_png) | **POST** /v1/return/giveout/get-png | Штрихкод для получения возвратной отгрузки в формате PNG
 *ReturnAPIApi* | [**return_api_giveout_info**](docs/ReturnAPIApi.md#return_api_giveout_info) | **POST** /v1/return/giveout/info | Информация о возвратной отгрузке
 *ReturnAPIApi* | [**return_api_giveout_is_enabled**](docs/ReturnAPIApi.md#return_api_giveout_is_enabled) | **POST** /v1/return/giveout/is-enabled | Проверить возможность получения возвратных отгрузок по штрихкоду
 *ReturnAPIApi* | [**return_api_giveout_list**](docs/ReturnAPIApi.md#return_api_giveout_list) | **POST** /v1/return/giveout/list | Список возвратных отгрузок
+*ReturnAPIApi* | [**returns_company_fbs_info**](docs/ReturnAPIApi.md#returns_company_fbs_info) | **POST** /v1/returns/company/fbs/info | Количество возвратов FBS
 *ReturnsAPIApi* | [**returns_api_get_returns_company_fbo**](docs/ReturnsAPIApi.md#returns_api_get_returns_company_fbo) | **POST** /v3/returns/company/fbo | Получить информацию о возвратах FBO
 *ReturnsAPIApi* | [**returns_api_get_returns_company_fbsv3**](docs/ReturnsAPIApi.md#returns_api_get_returns_company_fbsv3) | **POST** /v3/returns/company/fbs | Получить информацию о возвратах FBS
 *SellerRatingApi* | [**rating_api_rating_history_v1**](docs/SellerRatingApi.md#rating_api_rating_history_v1) | **POST** /v1/rating/history | Получить информацию о рейтингах продавца за период
 *SellerRatingApi* | [**rating_api_rating_summary_v1**](docs/SellerRatingApi.md#rating_api_rating_summary_v1) | **POST** /v1/rating/summary | Получить информацию о текущих рейтингах продавца
 *SupplierAPIApi* | [**invoice_create**](docs/SupplierAPIApi.md#invoice_create) | **POST** /v1/invoice/create-or-update | Создать или изменить ссылку на счёт-фактуру
 *SupplierAPIApi* | [**invoice_delete**](docs/SupplierAPIApi.md#invoice_delete) | **POST** /v1/invoice/delete | Удалить ссылку на счёт-фактуру
 *SupplierAPIApi* | [**invoice_get**](docs/SupplierAPIApi.md#invoice_get) | **POST** /v1/invoice/get | Получить ссылку на счёт-фактуру
@@ -293,18 +300,31 @@
  - [AnalyticsMetric](docs/AnalyticsMetric.md)
  - [AnalyticsSorting](docs/AnalyticsSorting.md)
  - [AnalyticsStockOnWarehouseRequest](docs/AnalyticsStockOnWarehouseRequest.md)
  - [AnalyticsStockOnWarehouseResponse](docs/AnalyticsStockOnWarehouseResponse.md)
  - [AnalyticsStockOnWarehouseResponseResult](docs/AnalyticsStockOnWarehouseResponseResult.md)
  - [AnalyticsStockOnWarehouseResultRows](docs/AnalyticsStockOnWarehouseResultRows.md)
  - [ApproveDeclineDiscountTasksResponseFailDetail](docs/ApproveDeclineDiscountTasksResponseFailDetail.md)
+ - [ArrivalPassListRequestFilter](docs/ArrivalPassListRequestFilter.md)
+ - [ArrivalpassArrivalPassCreateRequest](docs/ArrivalpassArrivalPassCreateRequest.md)
+ - [ArrivalpassArrivalPassCreateRequestArrivalPass](docs/ArrivalpassArrivalPassCreateRequestArrivalPass.md)
+ - [ArrivalpassArrivalPassCreateResponse](docs/ArrivalpassArrivalPassCreateResponse.md)
+ - [ArrivalpassArrivalPassDeleteRequest](docs/ArrivalpassArrivalPassDeleteRequest.md)
+ - [ArrivalpassArrivalPassListRequest](docs/ArrivalpassArrivalPassListRequest.md)
+ - [ArrivalpassArrivalPassListResponse](docs/ArrivalpassArrivalPassListResponse.md)
+ - [ArrivalpassArrivalPassListResponseArrivalPass](docs/ArrivalpassArrivalPassListResponseArrivalPass.md)
+ - [ArrivalpassArrivalPassUpdateRequest](docs/ArrivalpassArrivalPassUpdateRequest.md)
+ - [ArrivalpassArrivalPassUpdateRequestArrivalPass](docs/ArrivalpassArrivalPassUpdateRequestArrivalPass.md)
  - [BrandBrandCompanyCertificationListRequest](docs/BrandBrandCompanyCertificationListRequest.md)
  - [BrandBrandCompanyCertificationListResponse](docs/BrandBrandCompanyCertificationListResponse.md)
  - [BrandCompanyCertificationListResponseBrandCertification](docs/BrandCompanyCertificationListResponseBrandCertification.md)
  - [BrandCompanyCertificationListResponseBrandCertificationResult](docs/BrandCompanyCertificationListResponseBrandCertificationResult.md)
+ - [CarriageCarriageGetRequest](docs/CarriageCarriageGetRequest.md)
+ - [CarriageCarriageGetResponse](docs/CarriageCarriageGetResponse.md)
+ - [CarriageCarriageGetResponseCancelAvailability](docs/CarriageCarriageGetResponseCancelAvailability.md)
  - [CertificateCreateBody](docs/CertificateCreateBody.md)
  - [ChatChatSendFileRequest](docs/ChatChatSendFileRequest.md)
  - [ChatChatSendFileResponse](docs/ChatChatSendFileResponse.md)
  - [ChatChatSendMessageRequest](docs/ChatChatSendMessageRequest.md)
  - [ChatChatSendMessageResponse](docs/ChatChatSendMessageResponse.md)
  - [ChatChatStartRequest](docs/ChatChatStartRequest.md)
  - [ChatChatStartResponse](docs/ChatChatStartResponse.md)
@@ -608,14 +628,17 @@
  - [ReportReportInfoRequest](docs/ReportReportInfoRequest.md)
  - [ReportReportInfoResponse](docs/ReportReportInfoResponse.md)
  - [ReportReportListRequest](docs/ReportReportListRequest.md)
  - [ReportReportListResponse](docs/ReportReportListResponse.md)
  - [ResultError](docs/ResultError.md)
  - [ReturnCreateReportResponseCode](docs/ReturnCreateReportResponseCode.md)
  - [ReturnreportCreateReportResponse](docs/ReturnreportCreateReportResponse.md)
+ - [ReturnsCompanyFbsInfoRequestPagination](docs/ReturnsCompanyFbsInfoRequestPagination.md)
+ - [ReturnsCompanyFbsInfoResponseDropOffPoints](docs/ReturnsCompanyFbsInfoResponseDropOffPoints.md)
+ - [ReturnsCompanyFbsInfoResponsePassInfo](docs/ReturnsCompanyFbsInfoResponsePassInfo.md)
  - [ReturnsRfbsGetResponseReturns](docs/ReturnsRfbsGetResponseReturns.md)
  - [ReturnsRfbsGetV2ResponseAvailableAction](docs/ReturnsRfbsGetV2ResponseAvailableAction.md)
  - [ReturnsRfbsGetV2ResponseClientReturnMethodType](docs/ReturnsRfbsGetV2ResponseClientReturnMethodType.md)
  - [ReturnsRfbsGetV2ResponseRejectionReason](docs/ReturnsRfbsGetV2ResponseRejectionReason.md)
  - [ReturnsRfbsGetV2ResponseReturnReason](docs/ReturnsRfbsGetV2ResponseReturnReason.md)
  - [ReturnsRfbsListResponseReturns](docs/ReturnsRfbsListResponseReturns.md)
  - [RpcStatus](docs/RpcStatus.md)
@@ -631,14 +654,20 @@
  - [SellerApiProductPrice](docs/SellerApiProductPrice.md)
  - [SellerApiProductV1Response](docs/SellerApiProductV1Response.md)
  - [SellerApiProductV1ResponseDeactivate](docs/SellerApiProductV1ResponseDeactivate.md)
  - [SellerApiProductV1ResponseProduct](docs/SellerApiProductV1ResponseProduct.md)
  - [SellerApiProductV1ResponseProductDeactivate](docs/SellerApiProductV1ResponseProductDeactivate.md)
  - [SellerApiProductV1ResponseResult](docs/SellerApiProductV1ResponseResult.md)
  - [SellerApiProductV1ResponseResultDeactivate](docs/SellerApiProductV1ResponseResultDeactivate.md)
+ - [SellerSellerAPIArrivalPassCreateRequest](docs/SellerSellerAPIArrivalPassCreateRequest.md)
+ - [SellerSellerAPIArrivalPassCreateRequestArrivalPass](docs/SellerSellerAPIArrivalPassCreateRequestArrivalPass.md)
+ - [SellerSellerAPIArrivalPassCreateResponse](docs/SellerSellerAPIArrivalPassCreateResponse.md)
+ - [SellerSellerAPIArrivalPassDeleteRequest](docs/SellerSellerAPIArrivalPassDeleteRequest.md)
+ - [SellerSellerAPIArrivalPassUpdateRequest](docs/SellerSellerAPIArrivalPassUpdateRequest.md)
+ - [SellerSellerAPIArrivalPassUpdateRequestArrivalPass](docs/SellerSellerAPIArrivalPassUpdateRequestArrivalPass.md)
  - [SellerServiceanalyticsDimension](docs/SellerServiceanalyticsDimension.md)
  - [SortingOrder](docs/SortingOrder.md)
  - [SupplierAvailableWarehousesResponseCapacity](docs/SupplierAvailableWarehousesResponseCapacity.md)
  - [SupplierAvailableWarehousesResponseResult](docs/SupplierAvailableWarehousesResponseResult.md)
  - [SupplierAvailableWarehousesResponseSchedule](docs/SupplierAvailableWarehousesResponseSchedule.md)
  - [SupplierAvailableWarehousesResponseWarehouse](docs/SupplierAvailableWarehousesResponseWarehouse.md)
  - [V1ActivateHotSalesProductsRequest](docs/V1ActivateHotSalesProductsRequest.md)
@@ -799,14 +828,17 @@
  - [V1Rating](docs/V1Rating.md)
  - [V1RatingHistoryV1Request](docs/V1RatingHistoryV1Request.md)
  - [V1RatingHistoryV1Response](docs/V1RatingHistoryV1Response.md)
  - [V1RatingItem](docs/V1RatingItem.md)
  - [V1RatingStatus](docs/V1RatingStatus.md)
  - [V1RatingSummaryV1Response](docs/V1RatingSummaryV1Response.md)
  - [V1Restriction](docs/V1Restriction.md)
+ - [V1ReturnsCompanyFbsInfoRequest](docs/V1ReturnsCompanyFbsInfoRequest.md)
+ - [V1ReturnsCompanyFbsInfoRequestFilter](docs/V1ReturnsCompanyFbsInfoRequestFilter.md)
+ - [V1ReturnsCompanyFbsInfoResponse](docs/V1ReturnsCompanyFbsInfoResponse.md)
  - [V1SellerWarehouse](docs/V1SellerWarehouse.md)
  - [V1SetActivateHotSaleProductsResult](docs/V1SetActivateHotSaleProductsResult.md)
  - [V1SetActivateHotSaleProductsResultProduct](docs/V1SetActivateHotSaleProductsResultProduct.md)
  - [V1SetActivateHotSaleProductsResultResult](docs/V1SetActivateHotSaleProductsResultResult.md)
  - [V1SetDeactivateHotSaleProductsResult](docs/V1SetDeactivateHotSaleProductsResult.md)
  - [V1SetDeactivateHotSaleProductsResultProduct](docs/V1SetDeactivateHotSaleProductsResultProduct.md)
  - [V1SetDeactivateHotSaleProductsResultResult](docs/V1SetDeactivateHotSaleProductsResultResult.md)
```

