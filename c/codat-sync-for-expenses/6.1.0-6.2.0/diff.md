# Comparing `tmp/codat-sync-for-expenses-6.1.0.tar.gz` & `tmp/codat-sync-for-expenses-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-6.1.0.tar", last modified: Wed Mar 20 17:32:28 2024, max compression
+gzip compressed data, was "codat-sync-for-expenses-6.2.0.tar", last modified: Tue Apr  9 16:29:32 2024, max compression
```

## Comparing `codat-sync-for-expenses-6.1.0.tar` & `codat-sync-for-expenses-6.2.0.tar`

### file list

```diff
@@ -1,183 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.800522 codat-sync-for-expenses-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-03-20 17:32:28.800522 codat-sync-for-expenses-6.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    11779 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 17:32:28.800522 codat-sync-for-expenses-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.772522 codat-sync-for-expenses-6.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.772522 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-03-20 17:32:28.000000 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-03-20 17:32:28.000000 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 17:32:28.000000 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-20 17:32:28.000000 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-20 17:32:28.000000 codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.776522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.776522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/companies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13613 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    26705 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/manage_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.776522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.776522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.784522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_expense_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/delete_company.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/delete_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_create_chartofaccounts_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_data_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_pull_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_push_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/initiate_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_companies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_pull_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_push_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_suppliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_syncs.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/refresh_all_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/refresh_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/set_company_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/unlink_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_expense_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/upload_expense_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.796522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountingaddresstype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountprototype.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accounttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/attachmentupload.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/bankaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/codatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/company.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companyrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/contactref.py
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createaccountresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createcustomerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createsupplierresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customerdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customerstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/datastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/errorvalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/errorvalidationitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/expensetransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/group_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/halref.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/initiatesync.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/integrationtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/invoiceto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/mappingoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/phonenumbertype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pulloperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pulloperations.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushchangetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushfieldvalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperationchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperationref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperations.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoptionchoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoptionproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoptiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushvalidationinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/recordref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/schema_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplementaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplierdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/suppliers.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplierstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/synccompletewebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/synccompletewebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncfailedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncfailedwebhookdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncinitiated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncstartedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/trackingref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/transactionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updatecustomerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updateexpenserequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updateexpenseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updatesupplierresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/validationitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.796522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reached.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/push_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20723 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/suppliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:32:28.796522 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29900 2024-03-20 17:32:12.000000 codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.840696 codat-sync-for-expenses-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18819 2024-04-09 16:29:32.840696 codat-sync-for-expenses-6.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12191 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:29:32.840696 codat-sync-for-expenses-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.808696 codat-sync-for-expenses-6.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.808696 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18819 2024-04-09 16:29:32.000000 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-09 16:29:32.000000 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:29:32.000000 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 16:29:32.000000 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 16:29:32.000000 codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.812696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.812696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24893 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27036 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/manage_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.812696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.812696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.820696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_expense_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_reimbursable_expense_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_transfer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/delete_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/delete_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_create_chartofaccounts_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_pull_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_push_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/initiate_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_pull_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_push_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_suppliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_syncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/refresh_all_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/refresh_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/set_company_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/unlink_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_expense_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_reimbursable_expense_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/upload_expense_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.836696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountingaddresstype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountprototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accounttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/attachmentupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/bankaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/codatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companyrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/contactref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createaccountresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createcustomerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createreimbursableexpenserequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createreimbursableexpenseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createsupplierresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createtransferrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createtransferresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customerdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customerstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/datastatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/errorvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/errorvalidationitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/group_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/halref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/initiatesync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/integrationtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/invoiceto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/phonenumbertype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pulloperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pulloperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushchangetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushfieldvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperationchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperationref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoptionchoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoptionproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoptiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushvalidationinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/recordref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/reimbursableexpensetransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/reimbursableexpensetransactionline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/schema_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplementaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplierdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/suppliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplierstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/synccompletewebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/synccompletewebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncfailedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncfailedwebhookdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncstartedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/trackingref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transferdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updatecustomerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updateexpenserequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updateexpenseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updatesupplierresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/validationitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.836696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reached.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/push_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/reimbursements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/suppliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/transaction_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/transfers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:32.836696 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-09 16:29:24.000000 codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-6.1.0/PKG-INFO` & `codat-sync-for-expenses-6.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,368 +1,369 @@
-Metadata-Version: 2.1
-Name: codat-sync-for-expenses
-Version: 6.1.0
-Summary: Push expenses to accounting platforms.
-Home-page: UNKNOWN
-Author: Codat
-License: UNKNOWN
-Description: # Sync for Expenses
-        
-        <!-- Start Codat Library Description -->
-        ﻿Embedded accounting integrations for corporate card providers.
-        <!-- End Codat Library Description -->
-        
-        <!-- Start SDK Installation [installation] -->
-        ## SDK Installation
-        
-        ```bash
-        pip install codat-sync-for-expenses
-        ```
-        <!-- End SDK Installation [installation] -->
-        
-        ## Example Usage
-        <!-- Start SDK Example Usage [usage] -->
-        ## SDK Example Usage
-        
-        ### Example
-        
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End SDK Example Usage [usage] -->
-        
-        <!-- Start Available Resources and Operations [operations] -->
-        ## Available Resources and Operations
-        
-        ### [companies](docs/sdks/companies/README.md)
-        
-        * [create](docs/sdks/companies/README.md#create) - Create company
-        * [delete](docs/sdks/companies/README.md#delete) - Delete a company
-        * [get](docs/sdks/companies/README.md#get) - Get company
-        * [list](docs/sdks/companies/README.md#list) - List companies
-        * [update](docs/sdks/companies/README.md#update) - Update company
-        
-        ### [connections](docs/sdks/connections/README.md)
-        
-        * [create](docs/sdks/connections/README.md#create) - Create connection
-        * [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create partner expense connection
-        * [delete](docs/sdks/connections/README.md#delete) - Delete connection
-        * [get](docs/sdks/connections/README.md#get) - Get connection
-        * [list](docs/sdks/connections/README.md#list) - List connections
-        * [unlink](docs/sdks/connections/README.md#unlink) - Unlink connection
-        
-        ### [accounts](docs/sdks/accounts/README.md)
-        
-        * [create](docs/sdks/accounts/README.md#create) - Create account
-        * [get_create_model](docs/sdks/accounts/README.md#get_create_model) - Get create account model
-        
-        ### [customers](docs/sdks/customers/README.md)
-        
-        * [create](docs/sdks/customers/README.md#create) - Create customer
-        * [get](docs/sdks/customers/README.md#get) - Get customer
-        * [list](docs/sdks/customers/README.md#list) - List customers
-        * [update](docs/sdks/customers/README.md#update) - Update customer
-        
-        ### [suppliers](docs/sdks/suppliers/README.md)
-        
-        * [create](docs/sdks/suppliers/README.md#create) - Create supplier
-        * [get](docs/sdks/suppliers/README.md#get) - Get supplier
-        * [list](docs/sdks/suppliers/README.md#list) - List suppliers
-        * [update](docs/sdks/suppliers/README.md#update) - Update supplier
-        
-        ### [manage_data](docs/sdks/managedata/README.md)
-        
-        * [get](docs/sdks/managedata/README.md#get) - Get data status
-        * [get_pull_operation](docs/sdks/managedata/README.md#get_pull_operation) - Get pull operation
-        * [list_pull_operations](docs/sdks/managedata/README.md#list_pull_operations) - List pull operations
-        * [refresh_all_data_types](docs/sdks/managedata/README.md#refresh_all_data_types) - Refresh all data
-        * [refresh_data_type](docs/sdks/managedata/README.md#refresh_data_type) - Refresh data type
-        
-        ### [push_operations](docs/sdks/pushoperations/README.md)
-        
-        * [get](docs/sdks/pushoperations/README.md#get) - Get push operation
-        * [list](docs/sdks/pushoperations/README.md#list) - List push operations
-        
-        ### [configuration](docs/sdks/configuration/README.md)
-        
-        * [get](docs/sdks/configuration/README.md#get) - Get company configuration
-        * [get_mapping_options](docs/sdks/configuration/README.md#get_mapping_options) - Mapping options
-        * [set](docs/sdks/configuration/README.md#set) - Set company configuration
-        
-        ### [expenses](docs/sdks/expenses/README.md)
-        
-        * [create](docs/sdks/expenses/README.md#create) - Create expense transaction
-        * [update](docs/sdks/expenses/README.md#update) - Update expense transactions
-        * [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
-        
-        ### [sync](docs/sdks/sync/README.md)
-        
-        * [get](docs/sdks/sync/README.md#get) - Get sync status
-        * [get_last_successful_sync](docs/sdks/sync/README.md#get_last_successful_sync) - Last successful sync
-        * [get_latest_sync](docs/sdks/sync/README.md#get_latest_sync) - Latest sync status
-        * [initiate_sync](docs/sdks/sync/README.md#initiate_sync) - Initiate sync
-        * [list](docs/sdks/sync/README.md#list) - List sync statuses
-        
-        ### [transaction_status](docs/sdks/transactionstatus/README.md)
-        
-        * [get](docs/sdks/transactionstatus/README.md#get) - Get sync transaction
-        * [list](docs/sdks/transactionstatus/README.md#list) - List sync transactions
-        <!-- End Available Resources and Operations [operations] -->
-        
-        
-        
-        <!-- Start Retries [retries] -->
-        ## Retries
-        
-        Some of the endpoints in this SDK support retries. If you use the SDK without any configuration, it will fall back to the default retry strategy provided by the API. However, the default retry strategy can be overridden on a per-operation basis, or across the entire SDK.
-        
-        To change the default retry strategy for a single API call, simply provide a `RetryConfig` object to the call:
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        from codatsyncexpenses.utils import BackoffStrategy, RetryConfig
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req,
-            RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        
-        If you'd like to override the default retry strategy for all operations that support retries, you can use the `retry_config` optional parameter when initializing the SDK:
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        from codatsyncexpenses.utils import BackoffStrategy, RetryConfig
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False)
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Retries [retries] -->
-        
-        <!-- Start Error Handling [errors] -->
-        ## Error Handling
-        
-        Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
-        
-        | Error Object                | Status Code                 | Content Type                |
-        | --------------------------- | --------------------------- | --------------------------- |
-        | errors.ErrorMessage         | 400,401,402,403,429,500,503 | application/json            |
-        | errors.SDKError             | 4x-5xx                      | */*                         |
-        
-        ### Example
-        
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import errors, shared
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = None
-        try:
-            res = s.companies.create(req)
-        except errors.ErrorMessage as e:
-            # handle exception
-            raise(e)
-        except errors.SDKError as e:
-            # handle exception
-            raise(e)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Error Handling [errors] -->
-        
-        <!-- Start Server Selection [server] -->
-        ## Server Selection
-        
-        ### Select Server by Index
-        
-        You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
-        
-        | # | Server | Variables |
-        | - | ------ | --------- |
-        | 0 | `https://api.codat.io` | None |
-        
-        #### Example
-        
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            server_idx=0,
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        
-        
-        ### Override Server URL Per-Client
-        
-        The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            server_url="https://api.codat.io",
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Server Selection [server] -->
-        
-        <!-- Start Custom HTTP Client [http-client] -->
-        ## Custom HTTP Client
-        
-        The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
-        
-        For example, you could specify a header for every request that this sdk makes as follows:
-        ```python
-        import codatsyncexpenses
-        import requests
-        
-        http_client = requests.Session()
-        http_client.headers.update({'x-custom-header': 'someValue'})
-        s = codatsyncexpenses.CodatSyncExpenses(client: http_client)
-        ```
-        <!-- End Custom HTTP Client [http-client] -->
-        
-        <!-- Start Authentication [security] -->
-        ## Authentication
-        
-        ### Per-Client Security Schemes
-        
-        This SDK supports the following security scheme globally:
-        
-        | Name          | Type          | Scheme        |
-        | ------------- | ------------- | ------------- |
-        | `auth_header` | apiKey        | API key       |
-        
-        You can set the security parameters through the `security` optional parameter when initializing the SDK client instance. For example:
-        ```python
-        import codatsyncexpenses
-        from codatsyncexpenses.models import shared
-        
-        s = codatsyncexpenses.CodatSyncExpenses(
-            security=shared.Security(
-                auth_header="Basic BASE_64_ENCODED(API_KEY)",
-            ),
-        )
-        
-        req = shared.CompanyRequestBody(
-            name='Bank of Dave',
-            description='Requested early access to the new financing scheme.',
-        )
-        
-        res = s.companies.create(req)
-        
-        if res.company is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Authentication [security] -->
-        
-        <!-- Placeholder for Future Speakeasy SDK Sections -->
-        
-        <!-- Start Codat Support Notes -->
-        ### Support
-        
-        If you encounter any challenges while utilizing our SDKs, please don't hesitate to reach out for assistance. 
-        You can raise any issues by contacting your dedicated Codat representative or reaching out to our [support team](mailto:support@codat.io).
-        We're here to help ensure a smooth experience for you.
-        <!-- End Codat Support Notes -->
-        
-        <!-- Start Codat Generated By -->
-        ### Library generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-        <!-- End Codat Generated By -->
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# Sync for Expenses
+
+<!-- Start Codat Library Description -->
+﻿Embedded accounting integrations for corporate card providers.
+<!-- End Codat Library Description -->
+
+<!-- Start SDK Installation [installation] -->
+## SDK Installation
+
+```bash
+pip install codat-sync-for-expenses
+```
+<!-- End SDK Installation [installation] -->
+
+## Example Usage
+<!-- Start SDK Example Usage [usage] -->
+## SDK Example Usage
+
+### Example
+
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+<!-- End SDK Example Usage [usage] -->
+
+<!-- Start Available Resources and Operations [operations] -->
+## Available Resources and Operations
+
+### [companies](docs/sdks/companies/README.md)
+
+* [create](docs/sdks/companies/README.md#create) - Create company
+* [delete](docs/sdks/companies/README.md#delete) - Delete a company
+* [get](docs/sdks/companies/README.md#get) - Get company
+* [list](docs/sdks/companies/README.md#list) - List companies
+* [update](docs/sdks/companies/README.md#update) - Update company
+
+### [connections](docs/sdks/connections/README.md)
+
+* [create](docs/sdks/connections/README.md#create) - Create connection
+* [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create partner expense connection
+* [delete](docs/sdks/connections/README.md#delete) - Delete connection
+* [get](docs/sdks/connections/README.md#get) - Get connection
+* [list](docs/sdks/connections/README.md#list) - List connections
+* [unlink](docs/sdks/connections/README.md#unlink) - Unlink connection
+
+### [accounts](docs/sdks/accounts/README.md)
+
+* [create](docs/sdks/accounts/README.md#create) - Create account
+* [get_create_model](docs/sdks/accounts/README.md#get_create_model) - Get create account model
+
+### [customers](docs/sdks/customers/README.md)
+
+* [create](docs/sdks/customers/README.md#create) - Create customer
+* [get](docs/sdks/customers/README.md#get) - Get customer
+* [list](docs/sdks/customers/README.md#list) - List customers
+* [update](docs/sdks/customers/README.md#update) - Update customer
+
+### [suppliers](docs/sdks/suppliers/README.md)
+
+* [create](docs/sdks/suppliers/README.md#create) - Create supplier
+* [get](docs/sdks/suppliers/README.md#get) - Get supplier
+* [list](docs/sdks/suppliers/README.md#list) - List suppliers
+* [update](docs/sdks/suppliers/README.md#update) - Update supplier
+
+### [manage_data](docs/sdks/managedata/README.md)
+
+* [get](docs/sdks/managedata/README.md#get) - Get data status
+* [get_pull_operation](docs/sdks/managedata/README.md#get_pull_operation) - Get pull operation
+* [list_pull_operations](docs/sdks/managedata/README.md#list_pull_operations) - List pull operations
+* [refresh_all_data_types](docs/sdks/managedata/README.md#refresh_all_data_types) - Refresh all data
+* [refresh_data_type](docs/sdks/managedata/README.md#refresh_data_type) - Refresh data type
+
+### [push_operations](docs/sdks/pushoperations/README.md)
+
+* [get](docs/sdks/pushoperations/README.md#get) - Get push operation
+* [list](docs/sdks/pushoperations/README.md#list) - List push operations
+
+### [configuration](docs/sdks/configuration/README.md)
+
+* [get](docs/sdks/configuration/README.md#get) - Get company configuration
+* [get_mapping_options](docs/sdks/configuration/README.md#get_mapping_options) - Mapping options
+* [set](docs/sdks/configuration/README.md#set) - Set company configuration
+
+### [expenses](docs/sdks/expenses/README.md)
+
+* [create](docs/sdks/expenses/README.md#create) - Create expense transaction
+* [update](docs/sdks/expenses/README.md#update) - Update expense transactions
+
+### [reimbursements](docs/sdks/reimbursements/README.md)
+
+* [create](docs/sdks/reimbursements/README.md#create) - Create reimbursable expense transaction
+* [update](docs/sdks/reimbursements/README.md#update) - Update reimbursable expense transaction
+
+### [sync](docs/sdks/sync/README.md)
+
+* [get](docs/sdks/sync/README.md#get) - Get sync status
+* [get_last_successful_sync](docs/sdks/sync/README.md#get_last_successful_sync) - Last successful sync
+* [get_latest_sync](docs/sdks/sync/README.md#get_latest_sync) - Latest sync status
+* [initiate_sync](docs/sdks/sync/README.md#initiate_sync) - Initiate sync
+* [list](docs/sdks/sync/README.md#list) - List sync statuses
+
+### [transaction_status](docs/sdks/transactionstatus/README.md)
+
+* [get](docs/sdks/transactionstatus/README.md#get) - Get sync transaction
+* [list](docs/sdks/transactionstatus/README.md#list) - List sync transactions
+
+### [attachments](docs/sdks/attachments/README.md)
+
+* [upload](docs/sdks/attachments/README.md#upload) - Upload attachment
+
+### [transfers](docs/sdks/transfers/README.md)
+
+* [create](docs/sdks/transfers/README.md#create) - Create transfer transaction
+<!-- End Available Resources and Operations [operations] -->
+
+
+
+<!-- Start Retries [retries] -->
+## Retries
+
+Some of the endpoints in this SDK support retries. If you use the SDK without any configuration, it will fall back to the default retry strategy provided by the API. However, the default retry strategy can be overridden on a per-operation basis, or across the entire SDK.
+
+To change the default retry strategy for a single API call, simply provide a `RetryConfig` object to the call:
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+from codatsyncexpenses.utils import BackoffStrategy, RetryConfig
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req,
+    RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+
+If you'd like to override the default retry strategy for all operations that support retries, you can use the `retry_config` optional parameter when initializing the SDK:
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+from codatsyncexpenses.utils import BackoffStrategy, RetryConfig
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False)
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+<!-- End Retries [retries] -->
+
+<!-- Start Error Handling [errors] -->
+## Error Handling
+
+Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
+
+| Error Object                | Status Code                 | Content Type                |
+| --------------------------- | --------------------------- | --------------------------- |
+| errors.ErrorMessage         | 400,401,402,403,429,500,503 | application/json            |
+| errors.SDKError             | 4xx-5xx                     | */*                         |
+
+### Example
+
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import errors, shared
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = None
+try:
+    res = s.companies.create(req)
+except errors.ErrorMessage as e:
+    # handle exception
+    raise(e)
+except errors.SDKError as e:
+    # handle exception
+    raise(e)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+<!-- End Error Handling [errors] -->
+
+<!-- Start Server Selection [server] -->
+## Server Selection
+
+### Select Server by Index
+
+You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
+
+| # | Server | Variables |
+| - | ------ | --------- |
+| 0 | `https://api.codat.io` | None |
+
+#### Example
+
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    server_idx=0,
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+
+
+### Override Server URL Per-Client
+
+The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    server_url="https://api.codat.io",
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+<!-- End Server Selection [server] -->
+
+<!-- Start Custom HTTP Client [http-client] -->
+## Custom HTTP Client
+
+The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
+
+For example, you could specify a header for every request that this sdk makes as follows:
+```python
+import codatsyncexpenses
+import requests
+
+http_client = requests.Session()
+http_client.headers.update({'x-custom-header': 'someValue'})
+s = codatsyncexpenses.CodatSyncExpenses(client=http_client)
+```
+<!-- End Custom HTTP Client [http-client] -->
+
+<!-- Start Authentication [security] -->
+## Authentication
+
+### Per-Client Security Schemes
+
+This SDK supports the following security scheme globally:
+
+| Name          | Type          | Scheme        |
+| ------------- | ------------- | ------------- |
+| `auth_header` | apiKey        | API key       |
+
+You can set the security parameters through the `security` optional parameter when initializing the SDK client instance. For example:
+```python
+import codatsyncexpenses
+from codatsyncexpenses.models import shared
+
+s = codatsyncexpenses.CodatSyncExpenses(
+    security=shared.Security(
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
+    ),
+)
+
+req = shared.CompanyRequestBody(
+    name='Bank of Dave',
+    description='Requested early access to the new financing scheme.',
+)
+
+res = s.companies.create(req)
+
+if res.company is not None:
+    # handle response
+    pass
+
+```
+<!-- End Authentication [security] -->
+
+<!-- Placeholder for Future Speakeasy SDK Sections -->
+
+<!-- Start Codat Support Notes -->
+### Support
+
+If you encounter any challenges while utilizing our SDKs, please don't hesitate to reach out for assistance. 
+You can raise any issues by contacting your dedicated Codat representative or reaching out to our [support team](mailto:support@codat.io).
+We're here to help ensure a smooth experience for you.
+<!-- End Codat Support Notes -->
+
+<!-- Start Codat Generated By -->
+### Library generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+<!-- End Codat Generated By -->
```

### Comparing `codat-sync-for-expenses-6.1.0/setup.py` & `codat-sync-for-expenses-6.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import setuptools
+import re
 
 try:
-    with open("README.md", "r") as fh:
+    with open('README.md', 'r') as fh:
         long_description = fh.read()
+        GITHUB_URL = 'https://github.com/codatio/client-sdk-python.git'
+        GITHUB_URL = GITHUB_URL[: -len('.git')] if GITHUB_URL.endswith('.git') else GITHUB_URL
+        # links on PyPI should have absolute URLs
+        long_description = re.sub(
+            r'(\[[^\]]+\]\()((?!https?:)[^\)]+)(\))',
+            lambda m: m.group(1) + GITHUB_URL + '/blob/master/' + m.group(2) + m.group(3),
+            long_description,
+        )
 except FileNotFoundError:
-    long_description = ""
+    long_description = ''
 
 setuptools.setup(
-    name="codat-sync-for-expenses",
-    version="6.1.0",
-    author="Codat",
-    description="Push expenses to accounting platforms.",
+    name='codat-sync-for-expenses',
+    version='6.2.0',
+    author='Codat',
+    description='Push expenses to accounting platforms.',
+    url='https://github.com/codatio/client-sdk-python.git',
     long_description=long_description,
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(where="src"),
+    long_description_content_type='text/markdown',
+    packages=setuptools.find_packages(where='src'),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
         "idna>=3.4",
         "jsonpath-python>=1.0.6",
         "marshmallow>=3.19.0",
@@ -30,14 +40,16 @@
         "six>=1.16.0",
         "typing-inspect>=0.9.0",
         "typing_extensions>=4.7.1",
         "urllib3>=1.26.18",
     ],
     extras_require={
         "dev": [
-            "pylint==2.16.2",
+            "pylint==3.1.0",
         ],
     },
     package_dir={'': 'src'},
     python_requires='>=3.8',
-    package_data={"codat-sync-for-expenses": ["py.typed"]},
+    package_data={
+        'codat-sync-for-expenses': ['py.typed']
+    },
 )
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-6.2.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 src/codat_sync_for_expenses.egg-info/PKG-INFO
 src/codat_sync_for_expenses.egg-info/SOURCES.txt
 src/codat_sync_for_expenses.egg-info/dependency_links.txt
 src/codat_sync_for_expenses.egg-info/requires.txt
 src/codat_sync_for_expenses.egg-info/top_level.txt
 src/codatsyncexpenses/__init__.py
 src/codatsyncexpenses/accounts.py
+src/codatsyncexpenses/attachments.py
 src/codatsyncexpenses/companies.py
 src/codatsyncexpenses/configuration.py
 src/codatsyncexpenses/connections.py
 src/codatsyncexpenses/customers.py
 src/codatsyncexpenses/expenses.py
 src/codatsyncexpenses/manage_data.py
 src/codatsyncexpenses/push_operations.py
+src/codatsyncexpenses/reimbursements.py
 src/codatsyncexpenses/sdk.py
 src/codatsyncexpenses/sdkconfiguration.py
 src/codatsyncexpenses/suppliers.py
 src/codatsyncexpenses/sync.py
 src/codatsyncexpenses/transaction_status.py
+src/codatsyncexpenses/transfers.py
 src/codatsyncexpenses/_hooks/__init__.py
 src/codatsyncexpenses/_hooks/registration.py
 src/codatsyncexpenses/_hooks/sdkhooks.py
 src/codatsyncexpenses/_hooks/types.py
 src/codatsyncexpenses/models/__init__.py
 src/codatsyncexpenses/models/errors/__init__.py
 src/codatsyncexpenses/models/errors/errormessage.py
@@ -30,15 +33,17 @@
 src/codatsyncexpenses/models/operations/__init__.py
 src/codatsyncexpenses/models/operations/create_account.py
 src/codatsyncexpenses/models/operations/create_company.py
 src/codatsyncexpenses/models/operations/create_connection.py
 src/codatsyncexpenses/models/operations/create_customer.py
 src/codatsyncexpenses/models/operations/create_expense_transaction.py
 src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+src/codatsyncexpenses/models/operations/create_reimbursable_expense_transaction.py
 src/codatsyncexpenses/models/operations/create_supplier.py
+src/codatsyncexpenses/models/operations/create_transfer_transaction.py
 src/codatsyncexpenses/models/operations/delete_company.py
 src/codatsyncexpenses/models/operations/delete_connection.py
 src/codatsyncexpenses/models/operations/get_company.py
 src/codatsyncexpenses/models/operations/get_company_configuration.py
 src/codatsyncexpenses/models/operations/get_connection.py
 src/codatsyncexpenses/models/operations/get_create_chartofaccounts_model.py
 src/codatsyncexpenses/models/operations/get_customer.py
@@ -63,20 +68,22 @@
 src/codatsyncexpenses/models/operations/refresh_all_data_types.py
 src/codatsyncexpenses/models/operations/refresh_data_type.py
 src/codatsyncexpenses/models/operations/set_company_configuration.py
 src/codatsyncexpenses/models/operations/unlink_connection.py
 src/codatsyncexpenses/models/operations/update_company.py
 src/codatsyncexpenses/models/operations/update_customer.py
 src/codatsyncexpenses/models/operations/update_expense_transaction.py
+src/codatsyncexpenses/models/operations/update_reimbursable_expense_transaction.py
 src/codatsyncexpenses/models/operations/update_supplier.py
 src/codatsyncexpenses/models/operations/upload_expense_attachment.py
 src/codatsyncexpenses/models/shared/__init__.py
 src/codatsyncexpenses/models/shared/accountingaddresstype.py
 src/codatsyncexpenses/models/shared/accountmappinginfo.py
 src/codatsyncexpenses/models/shared/accountprototype.py
+src/codatsyncexpenses/models/shared/accountref.py
 src/codatsyncexpenses/models/shared/accountstatus.py
 src/codatsyncexpenses/models/shared/accounttype.py
 src/codatsyncexpenses/models/shared/attachment.py
 src/codatsyncexpenses/models/shared/attachmentupload.py
 src/codatsyncexpenses/models/shared/bankaccount.py
 src/codatsyncexpenses/models/shared/clientratelimitreachedwebhook.py
 src/codatsyncexpenses/models/shared/clientratelimitreachedwebhookdata.py
@@ -92,15 +99,19 @@
 src/codatsyncexpenses/models/shared/connections.py
 src/codatsyncexpenses/models/shared/contact.py
 src/codatsyncexpenses/models/shared/contactref.py
 src/codatsyncexpenses/models/shared/createaccountresponse.py
 src/codatsyncexpenses/models/shared/createcustomerresponse.py
 src/codatsyncexpenses/models/shared/createexpenserequest.py
 src/codatsyncexpenses/models/shared/createexpenseresponse.py
+src/codatsyncexpenses/models/shared/createreimbursableexpenserequest.py
+src/codatsyncexpenses/models/shared/createreimbursableexpenseresponse.py
 src/codatsyncexpenses/models/shared/createsupplierresponse.py
+src/codatsyncexpenses/models/shared/createtransferrequest.py
+src/codatsyncexpenses/models/shared/createtransferresponse.py
 src/codatsyncexpenses/models/shared/customer.py
 src/codatsyncexpenses/models/shared/customerdetails.py
 src/codatsyncexpenses/models/shared/customers.py
 src/codatsyncexpenses/models/shared/customerstatus.py
 src/codatsyncexpenses/models/shared/dataconnectionerror.py
 src/codatsyncexpenses/models/shared/dataconnectionstatus.py
 src/codatsyncexpenses/models/shared/datastatus.py
@@ -130,14 +141,16 @@
 src/codatsyncexpenses/models/shared/pushoperationstatus.py
 src/codatsyncexpenses/models/shared/pushoption.py
 src/codatsyncexpenses/models/shared/pushoptionchoice.py
 src/codatsyncexpenses/models/shared/pushoptionproperty.py
 src/codatsyncexpenses/models/shared/pushoptiontype.py
 src/codatsyncexpenses/models/shared/pushvalidationinfo.py
 src/codatsyncexpenses/models/shared/recordref.py
+src/codatsyncexpenses/models/shared/reimbursableexpensetransaction.py
+src/codatsyncexpenses/models/shared/reimbursableexpensetransactionline.py
 src/codatsyncexpenses/models/shared/schema_datatype.py
 src/codatsyncexpenses/models/shared/security.py
 src/codatsyncexpenses/models/shared/supplementaldata.py
 src/codatsyncexpenses/models/shared/supplier.py
 src/codatsyncexpenses/models/shared/supplierdetails.py
 src/codatsyncexpenses/models/shared/suppliers.py
 src/codatsyncexpenses/models/shared/supplierstatus.py
@@ -149,14 +162,15 @@
 src/codatsyncexpenses/models/shared/syncstartedwebhook.py
 src/codatsyncexpenses/models/shared/taxratemappinginfo.py
 src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
 src/codatsyncexpenses/models/shared/trackingref.py
 src/codatsyncexpenses/models/shared/transaction.py
 src/codatsyncexpenses/models/shared/transactions.py
 src/codatsyncexpenses/models/shared/transactionstatus.py
+src/codatsyncexpenses/models/shared/transferdetails.py
 src/codatsyncexpenses/models/shared/updatecustomerresponse.py
 src/codatsyncexpenses/models/shared/updateexpenserequest.py
 src/codatsyncexpenses/models/shared/updateexpenseresponse.py
 src/codatsyncexpenses/models/shared/updatesupplierresponse.py
 src/codatsyncexpenses/models/shared/validation.py
 src/codatsyncexpenses/models/shared/validationitem.py
 src/codatsyncexpenses/models/webhooks/__init__.py
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/registration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/sdkhooks.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/sdkhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
 from .registration import init_hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -27,27 +27,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/_hooks/types.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/_hooks/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -38,21 +42,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/accounts.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/expenses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
-class Accounts:
-    r"""Accounts"""
+class Expenses:
+    r"""Create expense transactions."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: operations.CreateAccountRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateAccountResponse:
-        r"""Create account
-        The *Create account* endpoint creates a new [account](https://docs.codat.io/sync-for-expenses-api#/schemas/Account) for a given company's connection.
+    def create(self, request: operations.CreateExpenseTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseTransactionResponse:
+        r"""Create expense transaction
+        The *Create expense* endpoint creates an [expense transaction](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) in the accounting platform for a given company's connection. 
+
+        [Expense transactions](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) represent transactions made with a company debit or credit card. 
 
-        [Accounts](https://docs.codat.io/sync-for-expenses-api#/schemas/Account) are the categories a business uses to record accounting transactions.
 
         **Integration-specific behaviour**
 
-        Required data may vary by integration. To see what data to post, first call [Get create account model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-chartOfAccounts-model).
+        Some accounting platforms support the option of pushing transactions to a draft state. This can be done by setting the postAsDraft property on the transaction to true. For platforms without this feature, the postAsDraft property should be ignored or set to false.
 
-        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts) for integrations that support creating an account.
+        | Integration | Draft State | Details                                                                                                      |  
+        |-------------|-------------|--------------------------------------------------------------------------------------------------------------|
+        | Dynamics 365 Business Central | Yes   | Setting postAsDraft to true will push the transactions to a drafted state rather than posting directly to the ledger. For transactions in a draft state, they can then be approved and posted within the accounting platform. |
+        | Quickbooks Online | No | -  |
+        | Xero | No | - |
+        | NetSuite | No | - |
         """
-        hook_ctx = HookContext(operation_id='create-account', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-expense-transaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/accounts', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountRequest, "account_prototype", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateExpenseTransactionRequest, "create_expense_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.CreateAccountRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -54,89 +59,89 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateExpenseTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateAccountResponse])
-                res.create_account_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateExpenseResponse])
+                res.create_expense_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_create_model(self, request: operations.GetCreateChartOfAccountsModelRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCreateChartOfAccountsModelResponse:
-        r"""Get create account model
-        The *Get create account model* endpoint returns the expected data for the request payload when creating an [account](https://docs.codat.io/sync-for-expenses-api#/schemas/Account) for a given company and integration.
+    def update(self, request: operations.UpdateExpenseTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateExpenseTransactionResponse:
+        r"""Update expense transactions
+        The *Update expense* endpoint updates an existing [expense transaction](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) in the accounting platform for a given company's connection. 
 
-        [Accounts](https://docs.codat.io/sync-for-expenses-api#/schemas/Account) are the categories a business uses to record accounting transactions.
+        [Expense transactions](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) represent transactions made with a company debit or credit card. 
 
-        **Integration-specific behaviour**
 
-        See the *response examples* for integration-specific indicative models.
+        **Integration-specific behaviour**
 
-        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts) for integrations that support creating an account.
+        At the moment you can update expenses only for Xero ([Payment](https://docs.codat.io/expenses/sync-process/expense-transactions#transaction-types) transaction type only).
         """
-        hook_ctx = HookContext(operation_id='get-create-chartOfAccounts-model', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='update-expense-transaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCreateChartOfAccountsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/chartOfAccounts', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/expense-transactions/{transactionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateExpenseTransactionRequest, "update_expense_request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -145,59 +150,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','422','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetCreateChartOfAccountsModelResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdateExpenseTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
-                res.push_option = out
+        if http_res.status_code == 202:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateExpenseResponse])
+                res.update_expense_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [400, 401, 402, 403, 404, 422, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/companies.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
-from typing import Optional
+from typing import List, Optional
 
-class Companies:
-    r"""Create and manage your Codat companies."""
+class Sync:
+    r"""Trigger and monitor expense syncs to accounting software."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: Optional[shared.CompanyRequestBody], retries: Optional[utils.RetryConfig] = None) -> operations.CreateCompanyResponse:
-        r"""Create company
-        Use the *Create company* endpoint to create a new [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) that represents your customer in Codat. 
-
-        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
-        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
-
-        If forbidden characters (see `name` pattern) are present in the request, a company will be created with the forbidden characters removed. For example, `Company (Codat[1])` with be created as `Company Codat1`.
+    def get(self, request: operations.GetSyncByIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncByIDResponse:
+        r"""Get sync status
+        Get the sync status for a specified sync
         """
-        hook_ctx = HookContext(operation_id='create-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-sync-by-id', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/companies'
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CompanyRequestBody], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -50,78 +42,73 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetSyncByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
+                res.company_sync_status = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def delete(self, request: operations.DeleteCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteCompanyResponse:
-        r"""Delete a company
-        The *Delete company* endpoint permanently deletes a [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company), its [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) and any cached data. This operation is irreversible.
-
-        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
-        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
+    def get_last_successful_sync(self, request: operations.GetLastSuccessfulSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLastSuccessfulSyncResponse:
+        r"""Last successful sync
+        Gets the status of the last successful sync
         """
-        hook_ctx = HookContext(operation_id='delete-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-last-successful-sync', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteCompanyRequest, base_url, '/companies/{companyId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -136,73 +123,73 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLastSuccessfulSyncResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 204:
-            pass
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
+                res.company_sync_status = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, request: operations.GetCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyResponse:
-        r"""Get company
-        The *Get company* endpoint returns a single company for a given `companyId`.
-
-        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
-        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
+    def get_latest_sync(self, request: operations.GetLatestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLatestSyncResponse:
+        r"""Latest sync status
+        Gets the latest sync status
         """
-        hook_ctx = HookContext(operation_id='get-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-latest-sync', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCompanyRequest, base_url, '/companies/{companyId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -217,85 +204,82 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetLatestSyncResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
+                res.company_sync_status = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
-        r"""List companies
-        The *List companies* endpoint returns a list of [companies] associated to your instances.
-
-        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
-        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
+    def initiate_sync(self, request: operations.InitiateSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.InitiateSyncResponse:
+        r"""Initiate sync
+        Initiate sync of pending transactions.
         """
-        hook_ctx = HookContext(operation_id='list-companies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='initiate-sync', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/companies'
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCompaniesRequest, request), **query_params }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.InitiateSyncRequest, "initiate_sync", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -304,88 +288,79 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','422','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.InitiateSyncResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
-                res.companies = out
+        if http_res.status_code == 202:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SyncInitiated])
+                res.sync_initiated = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [400, 401, 402, 403, 404, 422, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update(self, request: operations.UpdateCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateCompanyResponse:
-        r"""Update company
-        Use the *Update company* endpoint to update both the name and description of the company. 
-        If you use [groups](https://docs.codat.io/sync-for-expenses-api#/schemas/Group) to manage a set of companies, use the [Add company](https://docs.codat.io/sync-for-expenses-api#/operations/add-company-to-group) or [Remove company](https://docs.codat.io/sync-for-expenses-api#/operations/remove-company-from-group) endpoints to add or remove a company from a group.
-
-        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
-        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
+    def list(self, request: operations.ListSyncsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncsResponse:
+        r"""List sync statuses
+        Gets a list of sync statuses
         """
-        hook_ctx = HookContext(operation_id='update-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-syncs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCompanyRequest, base_url, '/companies/{companyId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCompanyRequest, "company_request_body", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -394,59 +369,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListSyncsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.CompanySyncStatus]])
+                res.classes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
 class Configuration:
     r"""Manage mapping options and sync configuration."""
     sdk_configuration: SDKConfiguration
 
@@ -19,15 +19,15 @@
     def get(self, request: operations.GetCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyConfigurationResponse:
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
         hook_ctx = HookContext(operation_id='get-company-configuration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/config', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -42,53 +42,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetCompanyConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetCompanyConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyConfiguration])
                 res.company_configuration = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,15 +100,15 @@
     def get_mapping_options(self, request: operations.GetMappingOptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetMappingOptionsResponse:
         r"""Mapping options
         Gets the expense mapping options for a companies accounting software
         """
         hook_ctx = HookContext(operation_id='get-mapping-options', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -125,53 +123,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetMappingOptionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetMappingOptionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MappingOptions])
                 res.mapping_options = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -185,15 +181,15 @@
     def set(self, request: operations.SetCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SetCompanyConfigurationResponse:
         r"""Set company configuration
         Sets a companies expense sync configuration
         """
         hook_ctx = HookContext(operation_id='set-company-configuration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.SetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/config', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.SetCompanyConfigurationRequest, "company_configuration", False, True, 'json')
@@ -211,59 +207,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.SetCompanyConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.SetCompanyConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyConfiguration])
                 res.company_configuration = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/connections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
 class Connections:
     r"""Create and manage partner expense connection."""
     sdk_configuration: SDKConfiguration
 
@@ -21,15 +21,15 @@
         Creates a connection for the company by providing a valid `platformKey`. 
 
         Use the [List Integrations](https://docs.codat.io/sync-for-expenses-api#/operations/list-integrations) endpoint to access valid platform keys.
         """
         hook_ctx = HookContext(operation_id='create-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateConnectionRequest, base_url, '/companies/{companyId}/connections', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateConnectionRequest, "request_body", False, True, 'json')
@@ -47,53 +47,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -107,15 +105,15 @@
     def create_partner_expense_connection(self, request: operations.CreatePartnerExpenseConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreatePartnerExpenseConnectionResponse:
         r"""Create partner expense connection
         Creates a partner expense data connection
         """
         hook_ctx = HookContext(operation_id='create-partner-expense-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -130,53 +128,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreatePartnerExpenseConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreatePartnerExpenseConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -191,15 +187,15 @@
         r"""Delete connection
         Revoke and remove a connection from a company.
         This operation is not reversible. The end user would need to reauthorize a new data connection if you wish to view new data for this company.
         """
         hook_ctx = HookContext(operation_id='delete-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -214,48 +210,46 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -269,15 +263,15 @@
     def get(self, request: operations.GetConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetConnectionResponse:
         r"""Get connection
         Returns a specific connection for a company when valid identifiers are provided. If the identifiers are for a deleted company and/or connection, a not found response is returned.
         """
         hook_ctx = HookContext(operation_id='get-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -292,53 +286,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -352,22 +344,22 @@
     def list(self, request: operations.ListConnectionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListConnectionsResponse:
         r"""List connections
         List the connections for a company.
         """
         hook_ctx = HookContext(operation_id='list-connections', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListConnectionsRequest, base_url, '/companies/{companyId}/connections', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListConnectionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -376,53 +368,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListConnectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListConnectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
                 res.connections = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -436,15 +426,15 @@
     def unlink(self, request: operations.UnlinkConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UnlinkConnectionResponse:
         r"""Unlink connection
         This allows you to deauthorize a connection, without deleting it from Codat. This means you can still view any data that has previously been pulled into Codat, and also lets you re-authorize in future if your customer wishes to resume sharing their data.
         """
         hook_ctx = HookContext(operation_id='unlink-connection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UnlinkConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UnlinkConnectionRequest, "request_body", False, True, 'json')
@@ -462,59 +452,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UnlinkConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UnlinkConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/customers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/customers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
 class Customers:
     r"""Customers"""
     sdk_configuration: SDKConfiguration
 
@@ -27,25 +27,25 @@
         Required data may vary by integration. To see what data to post, first call [Get create/update customer model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-customers-model).
 
         Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support creating an account.
         """
         hook_ctx = HookContext(operation_id='create-customer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCustomerRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/customers', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/push/customers', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomerRequest, "customer", True, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.CreateCustomerRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -54,53 +54,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateCustomerResponse])
                 res.create_customer_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -120,15 +118,15 @@
         Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support getting a specific customer.
 
         Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
         """
         hook_ctx = HookContext(operation_id='get-customer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomerRequest, base_url, '/companies/{companyId}/data/customers/{customerId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/customers/{customerId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -143,53 +141,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
                 res.customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 409, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -207,22 +203,22 @@
         [Customers](https://docs.codat.io/sync-for-expenses-api#/schemas/Customer) are people or organizations that buy goods or services from the SMB.
 
         Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
         """
         hook_ctx = HookContext(operation_id='list-customers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCustomersRequest, base_url, '/companies/{companyId}/data/customers', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/customers', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCustomersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -231,53 +227,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListCustomersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListCustomersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Customers])
                 res.customers = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 409, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -299,25 +293,25 @@
         Required data may vary by integration. To see what data to post, first call [Get create/update customer model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-customers-model).
 
         Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support creating an account.
         """
         hook_ctx = HookContext(operation_id='update-customer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCustomerRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/customers/{customerId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/push/customers/{customerId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCustomerRequest, "customer", True, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.UpdateCustomerRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -326,59 +320,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UpdateCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdateCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateCustomerResponse])
                 res.update_customer_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/suppliers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
-class Expenses:
-    r"""Create expense datasets and upload receipts."""
+class Suppliers:
+    r"""Suppliers"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: operations.CreateExpenseTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseTransactionResponse:
-        r"""Create expense transaction
-        The *Create expense* endpoint creates an [expense transaction](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) in the accounting platform for a given company's connection. 
-
-        [Expense transactions](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) represent transactions made with a company debit or credit card. 
+    def create(self, request: operations.CreateSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateSupplierResponse:
+        r"""Create supplier
+        The *Create supplier* endpoint creates a new [supplier](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
 
+        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
 
         **Integration-specific behaviour**
 
-        Some accounting platforms support the option of pushing transactions to a draft state. This can be done by setting the postAsDraft property on the transaction to true. For platforms without this feature, the postAsDraft property should be ignored or set to false.
+        Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-suppliers-model).
 
-        | Integration | Draft State | Details                                                                                                      |  
-        |-------------|-------------|--------------------------------------------------------------------------------------------------------------|
-        | Dynamics 365 Business Central | Yes   | Setting postAsDraft to true will push the transactions to a drafted state rather than posting directly to the ledger. For transactions in a draft state, they can then be approved and posted within the accounting platform. |
-        | Quickbooks Online | No | -  |
-        | Xero | No | - |
-        | NetSuite | No | - |
+        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating an account.
         """
-        hook_ctx = HookContext(operation_id='create-expense-transaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateExpenseTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateExpenseTransactionRequest, "create_expense_request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateSupplierRequest, "supplier", True, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -59,91 +54,171 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateExpenseTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateExpenseResponse])
-                res.create_expense_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateSupplierResponse])
+                res.create_supplier_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update(self, request: operations.UpdateExpenseTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateExpenseTransactionResponse:
-        r"""Update expense transactions
-        The *Update expense* endpoint updates an existing [expense transaction](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) in the accounting platform for a given company's connection. 
+    def get(self, request: operations.GetSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSupplierResponse:
+        r"""Get supplier
+        The *Get supplier* endpoint returns a single supplier for a given supplierId.
 
-        [Expense transactions](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) represent transactions made with a company debit or credit card. 
+        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
 
+        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support getting a specific supplier.
 
-        **Integration-specific behaviour**
+        Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
+        """
+        hook_ctx = HookContext(operation_id='get-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/suppliers/{supplierId}', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        global_retry_config = self.sdk_configuration.retry_config
+        retry_config = retries
+        if retry_config is None:
+            if global_retry_config:
+                retry_config = global_retry_config
+            else:
+                retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+
+        req = None
+        def do_request():
+            nonlocal req
+            try:
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+                http_res = client.send(req)
+            except Exception as e:
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
+
+            if utils.match_status_codes(['401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
+                    raise e
+                if result is not None:
+                    http_res = result
+            else:
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+
+            return http_res
 
-        At the moment you can update expenses only for Xero ([Payment](https://docs.codat.io/expenses/sync-process/expense-transactions#transaction-types) transaction type only).
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
+        
+        
+        res = operations.GetSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Supplier])
+                res.supplier = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code in [401, 402, 403, 404, 409, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
+    def list(self, request: operations.ListSuppliersRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSuppliersResponse:
+        r"""List suppliers
+        The *List suppliers* endpoint returns a list of [suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
+
+        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
+
+        Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
         """
-        hook_ctx = HookContext(operation_id='update-expense-transaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-suppliers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateExpenseTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/expense-transactions/{transactionId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/suppliers', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateExpenseTransactionRequest, "update_expense_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -152,97 +227,91 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','422','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UpdateExpenseTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListSuppliersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 202:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateExpenseResponse])
-                res.update_expense_response = out
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Suppliers])
+                res.suppliers = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 422, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [400, 401, 402, 403, 404, 409, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def upload_attachment(self, request: operations.UploadExpenseAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadExpenseAttachmentResponse:
-        r"""Upload attachment
-        The *Upload attachment* endpoint uploads an attachment in the accounting software against the given transactionId. 
+    def update(self, request: operations.UpdateSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateSupplierResponse:
+        r"""Update supplier
+        The *Update supplier* endpoint updates an existing [supplier](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
 
-        [Expense transactions](https://docs.codat.io/sync-for-expenses-api#/schemas/ExpenseTransaction) represent transactions made with a company debit or credit card. 
+        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
 
         **Integration-specific behaviour**
 
-        Each accounting software supports different file formats and sizes.
+        Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-suppliers-model).
 
-        | Integration | File Size | File Extension                                                                                                      |  
-        |-------------|-------------|--------------------------------------------------------------------------------------------------------------|
-        | Xero | 4MB  | 7Z, BMP, CSV, DOC, DOCX, EML, GIF, JPEG, JPG, KEYNOTE, MSG, NUMBERS, ODF, ODS, ODT, PAGES, PDF, PNG, PPT, PPTX, RAR, RTF, TIF, TIFF, TXT, XLS, XLSX, ZIP |
-        | QuickBooks Online | 100MB | AI, CSV, DOC, DOCX, EPS, GIF, JPEG, JPG, ODS, PAGES, PDF, PNG, RTF, TIF, TXT, XLS, XLSX, XML  |
-        | NetSuite | 100MB | BMP, CSV, XLS, XLSX, JSON, PDF, PJPG, PJPEG, PNG, TXT, SVG, TIF, TIFF, DOC, DOCX, ZIP |
-        | Dynamics 365 Business Central | 350 MB | Dynamics do not explicitly outline which file types are supported but they do state <a className=\"external\" href=\"https://learn.microsoft.com/en-gb/dynamics365/business-central/ui-how-add-link-to-record#to-attach-a-file-to-a-purchase-invoice\" target=\"_blank\">here</a> that \"You can attach any type of file, such as text, image, or video files\". |
+        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating an account.
         """
-        hook_ctx = HookContext(operation_id='upload-expense-attachment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='update-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UploadExpenseAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers/{supplierId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UploadExpenseAttachmentRequest, "attachment_upload", False, True, 'multipart')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateSupplierRequest, "supplier", True, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -251,59 +320,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UploadExpenseAttachmentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdateSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
-                res.attachment = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateSupplierResponse])
+                res.update_supplier_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/manage_data.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/manage_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Dict, Optional
 
 class ManageData:
     r"""Asynchronously retrieve data from an integration to refresh data in Codat."""
     sdk_configuration: SDKConfiguration
 
@@ -19,15 +19,15 @@
     def get(self, request: operations.GetDataStatusRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetDataStatusResponse:
         r"""Get data status
         Get the state of each data type for a company
         """
         hook_ctx = HookContext(operation_id='get-data-status', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetDataStatusRequest, base_url, '/companies/{companyId}/dataStatus', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/dataStatus', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -42,53 +42,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetDataStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetDataStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, shared.DataStatus]])
                 res.data_statuses = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,15 +100,15 @@
     def get_pull_operation(self, request: operations.GetPullOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPullOperationResponse:
         r"""Get pull operation
         Retrieve information about a single dataset or pull operation.
         """
         hook_ctx = HookContext(operation_id='get-pull-operation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPullOperationRequest, base_url, '/companies/{companyId}/data/history/{datasetId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/history/{datasetId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -125,53 +123,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetPullOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPullOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
                 res.pull_operation = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -185,22 +181,22 @@
     def list_pull_operations(self, request: operations.ListPullOperationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListPullOperationsResponse:
         r"""List pull operations
         Gets the pull operation history (datasets) for a given company.
         """
         hook_ctx = HookContext(operation_id='list-pull-operations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPullOperationsRequest, base_url, '/companies/{companyId}/data/history', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/history', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPullOperationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -209,53 +205,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListPullOperationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListPullOperationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperations])
                 res.pull_operations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -273,15 +267,15 @@
         This is an asynchronous operation, and will bring updated data into Codat from the linked integration for you to view.
 
         [Read more](https://docs.codat.io/core-concepts/data-type-settings) about data type settings and `fetch on first link`.
         """
         hook_ctx = HookContext(operation_id='refresh-all-data-types', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshAllDataTypesRequest, base_url, '/companies/{companyId}/data/all', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/all', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -296,48 +290,46 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.RefreshAllDataTypesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.RefreshAllDataTypesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -353,22 +345,22 @@
         Refreshes a given data type for a given company.
 
         This is an asynchronous operation, and will bring updated data into Codat from the linked integration for you to view.
         """
         hook_ctx = HookContext(operation_id='refresh-data-type', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshDataTypeRequest, base_url, '/companies/{companyId}/data/queue/{dataType}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/data/queue/{dataType}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.RefreshDataTypeRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -377,59 +369,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.RefreshDataTypeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.RefreshDataTypeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
                 res.pull_operation = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/errormessage.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/errormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/errors/sdkerror.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from .create_account import *
 from .create_company import *
 from .create_connection import *
 from .create_customer import *
 from .create_expense_transaction import *
 from .create_partner_expense_connection import *
+from .create_reimbursable_expense_transaction import *
 from .create_supplier import *
+from .create_transfer_transaction import *
 from .delete_company import *
 from .delete_connection import *
 from .get_company import *
 from .get_company_configuration import *
 from .get_connection import *
 from .get_create_chartofaccounts_model import *
 from .get_customer import *
@@ -35,11 +37,12 @@
 from .refresh_all_data_types import *
 from .refresh_data_type import *
 from .set_company_configuration import *
 from .unlink_connection import *
 from .update_company import *
 from .update_customer import *
 from .update_expense_transaction import *
+from .update_reimbursable_expense_transaction import *
 from .update_supplier import *
 from .upload_expense_attachment import *
 
-__all__ = ["CreateAccountRequest","CreateAccountResponse","CreateCompanyResponse","CreateConnectionRequest","CreateConnectionRequestBody","CreateConnectionResponse","CreateCustomerRequest","CreateCustomerResponse","CreateExpenseTransactionRequest","CreateExpenseTransactionResponse","CreatePartnerExpenseConnectionRequest","CreatePartnerExpenseConnectionResponse","CreateSupplierRequest","CreateSupplierResponse","DeleteCompanyRequest","DeleteCompanyResponse","DeleteConnectionRequest","DeleteConnectionResponse","GetCompanyConfigurationRequest","GetCompanyConfigurationResponse","GetCompanyRequest","GetCompanyResponse","GetConnectionRequest","GetConnectionResponse","GetCreateChartOfAccountsModelRequest","GetCreateChartOfAccountsModelResponse","GetCustomerRequest","GetCustomerResponse","GetDataStatusRequest","GetDataStatusResponse","GetLastSuccessfulSyncRequest","GetLastSuccessfulSyncResponse","GetLatestSyncRequest","GetLatestSyncResponse","GetMappingOptionsRequest","GetMappingOptionsResponse","GetPullOperationRequest","GetPullOperationResponse","GetPushOperationRequest","GetPushOperationResponse","GetSupplierRequest","GetSupplierResponse","GetSyncByIDRequest","GetSyncByIDResponse","GetSyncTransactionRequest","GetSyncTransactionResponse","InitiateSyncRequest","InitiateSyncResponse","ListCompaniesRequest","ListCompaniesResponse","ListConnectionsRequest","ListConnectionsResponse","ListCustomersRequest","ListCustomersResponse","ListPullOperationsRequest","ListPullOperationsResponse","ListPushOperationsRequest","ListPushOperationsResponse","ListSuppliersRequest","ListSuppliersResponse","ListSyncTransactionsRequest","ListSyncTransactionsResponse","ListSyncsRequest","ListSyncsResponse","RefreshAllDataTypesRequest","RefreshAllDataTypesResponse","RefreshDataTypeRequest","RefreshDataTypeResponse","SetCompanyConfigurationRequest","SetCompanyConfigurationResponse","UnlinkConnectionRequest","UnlinkConnectionResponse","UnlinkConnectionUpdateConnection","UpdateCompanyRequest","UpdateCompanyResponse","UpdateCustomerRequest","UpdateCustomerResponse","UpdateExpenseTransactionRequest","UpdateExpenseTransactionResponse","UpdateSupplierRequest","UpdateSupplierResponse","UploadExpenseAttachmentRequest","UploadExpenseAttachmentResponse"]
+__all__ = ["CreateAccountRequest","CreateAccountResponse","CreateCompanyResponse","CreateConnectionRequest","CreateConnectionRequestBody","CreateConnectionResponse","CreateCustomerRequest","CreateCustomerResponse","CreateExpenseTransactionRequest","CreateExpenseTransactionResponse","CreatePartnerExpenseConnectionRequest","CreatePartnerExpenseConnectionResponse","CreateReimbursableExpenseTransactionRequest","CreateReimbursableExpenseTransactionResponse","CreateSupplierRequest","CreateSupplierResponse","CreateTransferTransactionRequest","CreateTransferTransactionResponse","DeleteCompanyRequest","DeleteCompanyResponse","DeleteConnectionRequest","DeleteConnectionResponse","GetCompanyConfigurationRequest","GetCompanyConfigurationResponse","GetCompanyRequest","GetCompanyResponse","GetConnectionRequest","GetConnectionResponse","GetCreateChartOfAccountsModelRequest","GetCreateChartOfAccountsModelResponse","GetCustomerRequest","GetCustomerResponse","GetDataStatusRequest","GetDataStatusResponse","GetLastSuccessfulSyncRequest","GetLastSuccessfulSyncResponse","GetLatestSyncRequest","GetLatestSyncResponse","GetMappingOptionsRequest","GetMappingOptionsResponse","GetPullOperationRequest","GetPullOperationResponse","GetPushOperationRequest","GetPushOperationResponse","GetSupplierRequest","GetSupplierResponse","GetSyncByIDRequest","GetSyncByIDResponse","GetSyncTransactionRequest","GetSyncTransactionResponse","InitiateSyncRequest","InitiateSyncResponse","ListCompaniesRequest","ListCompaniesResponse","ListConnectionsRequest","ListConnectionsResponse","ListCustomersRequest","ListCustomersResponse","ListPullOperationsRequest","ListPullOperationsResponse","ListPushOperationsRequest","ListPushOperationsResponse","ListSuppliersRequest","ListSuppliersResponse","ListSyncTransactionsRequest","ListSyncTransactionsResponse","ListSyncsRequest","ListSyncsResponse","RefreshAllDataTypesRequest","RefreshAllDataTypesResponse","RefreshDataTypeRequest","RefreshDataTypeResponse","SetCompanyConfigurationRequest","SetCompanyConfigurationResponse","UnlinkConnectionRequest","UnlinkConnectionResponse","UnlinkConnectionUpdateConnection","UpdateCompanyRequest","UpdateCompanyResponse","UpdateCustomerRequest","UpdateCustomerResponse","UpdateExpenseTransactionRequest","UpdateExpenseTransactionResponse","UpdateReimbursableExpenseTransactionRequest","UpdateReimbursableExpenseTransactionResponse","UpdateSupplierRequest","UpdateSupplierResponse","UploadExpenseAttachmentRequest","UploadExpenseAttachmentResponse"]
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_account.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_account.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_company.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_company.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_customer.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_expense_transaction.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_expense_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/create_supplier.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/create_supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/delete_company.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/delete_company.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/delete_connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/delete_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_company.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_company.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_create_chartofaccounts_model.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_create_chartofaccounts_model.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_customer.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_data_status.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_data_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_pull_operation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_pull_operation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_push_operation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_push_operation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_supplier.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/initiate_sync.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/initiate_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
     sync_initiated: Optional[shared_syncinitiated.SyncInitiated] = dataclasses.field(default=None)
-    r"""Returns the newly created SyncId"""
+    r"""Returns the newly created syncId"""
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_companies.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_companies.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_connections.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_connections.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_customers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_customers.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_pull_operations.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_pull_operations.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_push_operations.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_push_operations.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_suppliers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_suppliers.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/refresh_all_data_types.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/refresh_all_data_types.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/refresh_data_type.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/refresh_data_type.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/set_company_configuration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/set_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/unlink_connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/unlink_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_company.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_company.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_customer.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_expense_transaction.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_expense_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/update_supplier.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/update_supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/operations/upload_expense_attachment.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/operations/upload_expense_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .accountingaddresstype import *
 from .accountmappinginfo import *
 from .accountprototype import *
+from .accountref import *
 from .accountstatus import *
 from .accounttype import *
 from .attachment import *
 from .attachmentupload import *
 from .bankaccount import *
 from .clientratelimitreachedwebhook import *
 from .clientratelimitreachedwebhookdata import *
@@ -22,15 +23,19 @@
 from .connections import *
 from .contact import *
 from .contactref import *
 from .createaccountresponse import *
 from .createcustomerresponse import *
 from .createexpenserequest import *
 from .createexpenseresponse import *
+from .createreimbursableexpenserequest import *
+from .createreimbursableexpenseresponse import *
 from .createsupplierresponse import *
+from .createtransferrequest import *
+from .createtransferresponse import *
 from .customer import *
 from .customerdetails import *
 from .customers import *
 from .customerstatus import *
 from .dataconnectionerror import *
 from .dataconnectionstatus import *
 from .datastatus import *
@@ -60,14 +65,16 @@
 from .pushoperationstatus import *
 from .pushoption import *
 from .pushoptionchoice import *
 from .pushoptionproperty import *
 from .pushoptiontype import *
 from .pushvalidationinfo import *
 from .recordref import *
+from .reimbursableexpensetransaction import *
+from .reimbursableexpensetransactionline import *
 from .schema_datatype import *
 from .security import *
 from .supplementaldata import *
 from .supplier import *
 from .supplierdetails import *
 from .suppliers import *
 from .supplierstatus import *
@@ -79,15 +86,16 @@
 from .syncstartedwebhook import *
 from .taxratemappinginfo import *
 from .trackingcategorymappinginfo import *
 from .trackingref import *
 from .transaction import *
 from .transactions import *
 from .transactionstatus import *
+from .transferdetails import *
 from .updatecustomerresponse import *
 from .updateexpenserequest import *
 from .updateexpenseresponse import *
 from .updatesupplierresponse import *
 from .validation import *
 from .validationitem import *
 
-__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountPrototype","AccountStatus","AccountType","AccountingAccount","AccountingAddress","AccountingAddressType","AccountingCustomer","AccountingSupplier","Attachment","AttachmentUpload","BankAccount","BankAccountReference","ClientRateLimitReachedWebhook","ClientRateLimitReachedWebhookData","ClientRateLimitResetWebhook","ClientRateLimitResetWebhookData","CodatFile","Companies","Company","CompanyConfiguration","CompanyRequestBody","CompanySyncStatus","Connection","Connections","Contact","ContactRef","CreateAccountResponse","CreateAccountResponseMetadata","CreateAccountResponseValidDataTypeLinks","CreateCustomerResponse","CreateCustomerResponseAccountingAddress","CreateExpenseRequest","CreateExpenseResponse","CreateSupplierResponse","Customer","CustomerDetails","CustomerStatus","Customers","Data","DataConnectionError","DataConnectionStatus","DataStatus","DataType","DataTypes","ErrorValidation","ErrorValidationItem","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","GroupItems","GroupReference","HalRef","InitiateSync","IntegrationType","InvoiceTo","InvoiceToDataType","Items","Links","MappingOptions","Metadata","Phone","PhoneNumberType","PullOperation","PullOperations","PushChangeType","PushFieldValidation","PushOperation","PushOperationChange","PushOperationRef","PushOperationStatus","PushOperations","PushOption","PushOptionChoice","PushOptionProperty","PushOptionType","PushValidationInfo","RecordRef","SchemaDataType","Security","SourceType","Status","SupplementalData","Supplier","SupplierDetails","SupplierStatus","Suppliers","SyncCompleteWebhook","SyncCompleteWebhookData","SyncFailedWebhook","SyncFailedWebhookData","SyncInitiated","SyncStartedWebhook","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TrackingRef","TrackingRefDataType","Transaction","TransactionStatus","Transactions","Type","UpdateCustomerResponse","UpdateCustomerResponseAccountingAddress","UpdateCustomerResponseAccountingCustomer","UpdateExpenseRequest","UpdateExpenseRequestBankAccountReference","UpdateExpenseResponse","UpdateSupplierResponse","UpdateSupplierResponseAccountingSupplier","ValidDataTypeLinks","ValidTransactionTypes","Validation","ValidationItem"]
+__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountPrototype","AccountRef","AccountStatus","AccountType","AccountingAccount","AccountingAddress","AccountingAddressType","AccountingCustomer","AccountingSupplier","Attachment","AttachmentUpload","BankAccount","BankAccountReference","ClientRateLimitReachedWebhook","ClientRateLimitReachedWebhookData","ClientRateLimitResetWebhook","ClientRateLimitResetWebhookData","CodatFile","Companies","Company","CompanyConfiguration","CompanyRequestBody","CompanySyncStatus","Connection","Connections","Contact","ContactRef","CreateAccountResponse","CreateAccountResponseMetadata","CreateAccountResponseValidDataTypeLinks","CreateCustomerResponse","CreateCustomerResponseAccountingAddress","CreateExpenseRequest","CreateExpenseResponse","CreateReimbursableExpenseRequest","CreateReimbursableExpenseResponse","CreateSupplierResponse","CreateTransferRequest","CreateTransferResponse","Customer","CustomerDetails","CustomerStatus","Customers","Data","DataConnectionError","DataConnectionStatus","DataStatus","DataType","DataTypes","ErrorValidation","ErrorValidationItem","ExpenseTransaction","ExpenseTransactionBankAccountReference","ExpenseTransactionLine","ExpenseTransactionType","GroupItems","GroupReference","HalRef","InitiateSync","IntegrationType","InvoiceTo","InvoiceToDataType","Items","Links","MappingOptions","Metadata","Phone","PhoneNumberType","PullOperation","PullOperations","PushChangeType","PushFieldValidation","PushOperation","PushOperationChange","PushOperationRef","PushOperationStatus","PushOperations","PushOption","PushOptionChoice","PushOptionProperty","PushOptionType","PushValidationInfo","RecordRef","ReimbursableExpenseTransaction","ReimbursableExpenseTransactionLine","SchemaDataType","Security","SourceType","Status","SupplementalData","Supplier","SupplierDetails","SupplierStatus","Suppliers","SyncCompleteWebhook","SyncCompleteWebhookData","SyncFailedWebhook","SyncFailedWebhookData","SyncInitiated","SyncStartedWebhook","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TrackingRef","TrackingRefDataType","Transaction","TransactionStatus","Transactions","TransferDetails","Type","UpdateCustomerResponse","UpdateCustomerResponseAccountingAddress","UpdateCustomerResponseAccountingCustomer","UpdateExpenseRequest","UpdateExpenseRequestBankAccountReference","UpdateExpenseResponse","UpdateSupplierResponse","UpdateSupplierResponseAccountingSupplier","ValidDataTypeLinks","ValidTransactionTypes","Validation","ValidationItem"]
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/accountprototype.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/accountprototype.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhook.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhook.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhookdata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitreachedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhook.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhook.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhookdata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/clientratelimitresetwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companies.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companies.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/company.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/company.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companyrequestbody.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companyrequestbody.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/connection.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/connections.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/connections.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/contact.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/contact.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/contactref.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/contactref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createaccountresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createaccountresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createcustomerresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createcustomerresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/createsupplierresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/createsupplierresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customerdetails.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customerdetails.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/customers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/customers.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/datastatus.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/datastatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/datatype.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/datatype.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/errorvalidation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/errorvalidation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/errorvalidationitem.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/errorvalidationitem.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BankAccountReference:
+class ExpenseTransactionBankAccountReference:
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Identifier of the bank account."""
     
 
 
 class ExpenseTransactionType(str, Enum):
     r"""The type of transaction."""
@@ -58,15 +58,15 @@
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     type: ExpenseTransactionType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of transaction."""
-    bank_account_ref: Optional[BankAccountReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccountRef'), 'exclude': lambda f: f is None }})
+    bank_account_ref: Optional[ExpenseTransactionBankAccountReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccountRef'), 'exclude': lambda f: f is None }})
     contact_ref: Optional[ContactRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactRef'), 'exclude': lambda f: f is None }})
     currency_rate: Optional[Decimal] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'encoder': utils.decimalencoder(True, False), 'decoder': utils.decimaldecoder, 'exclude': lambda f: f is ExpenseTransaction.UNSET }})
     r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
 
     Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
 
     It is not possible to perform the currency conversion with two or more non-base currencies participating in the transaction. For example, if a company's base currency is USD, and it has a bill issued in EUR, then the bill payment must happen in USD or EUR.
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/group_items.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/group_items.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/halref.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/halref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/initiatesync.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/initiatesync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/invoiceto.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/invoiceto.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/items.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/items.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/links.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/links.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/metadata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/metadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pulloperation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pulloperation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pulloperations.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pulloperations.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushfieldvalidation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushfieldvalidation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperationchange.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperationchange.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperationref.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperationref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoperations.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoperations.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoption.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoption.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoptionchoice.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoptionchoice.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushoptionproperty.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushoptionproperty.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/pushvalidationinfo.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/pushvalidationinfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RecordRef:
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""identifier of linked reference from mapping options."""
+    r"""Identifier of linked reference from mapping options."""
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/schema_datatype.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/schema_datatype.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplementaldata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplementaldata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/supplierdetails.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/supplierdetails.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/suppliers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/suppliers.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/synccompletewebhook.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/synccompletewebhook.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/synccompletewebhookdata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/synccompletewebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncfailedwebhook.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncfailedwebhook.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncfailedwebhookdata.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncfailedwebhookdata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/syncstartedwebhook.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/syncstartedwebhook.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/trackingref.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/trackingref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/transaction.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/transactions.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updatecustomerresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updatecustomerresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updateexpenserequest.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updateexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updateexpenseresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updateexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/updatesupplierresponse.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/updatesupplierresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/validation.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/validation.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/shared/validationitem.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/shared/validationitem.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reached.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reached.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reset.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/client_rate_limit_reset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_complete.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_complete.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_failed.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_failed.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/models/webhooks/sync_started.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/models/webhooks/sync_started.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/push_operations.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/push_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
 class PushOperations:
     r"""Access create, update and delete operations made to an SMB's data connection."""
     sdk_configuration: SDKConfiguration
 
@@ -19,15 +19,15 @@
     def get(self, request: operations.GetPushOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPushOperationResponse:
         r"""Get push operation
         Retrieve push operation.
         """
         hook_ctx = HookContext(operation_id='get-push-operation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPushOperationRequest, base_url, '/companies/{companyId}/push/{pushOperationKey}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/push/{pushOperationKey}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -42,53 +42,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetPushOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetPushOperationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperation])
                 res.push_operation = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,22 +100,22 @@
     def list(self, request: operations.ListPushOperationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListPushOperationsResponse:
         r"""List push operations
         List push operation records.
         """
         hook_ctx = HookContext(operation_id='list-push-operations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPushOperationsRequest, base_url, '/companies/{companyId}/push', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/push', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPushOperationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -126,59 +124,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListPushOperationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListPushOperationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperations])
                 res.push_operations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sdk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .accounts import Accounts
+from .attachments import Attachments
 from .companies import Companies
 from .configuration import Configuration
 from .connections import Connections
 from .customers import Customers
 from .expenses import Expenses
 from .manage_data import ManageData
 from .push_operations import PushOperations
+from .reimbursements import Reimbursements
 from .sdkconfiguration import SDKConfiguration
 from .suppliers import Suppliers
 from .sync import Sync
 from .transaction_status import TransactionStatus
+from .transfers import Transfers
+from .utils.retries import RetryConfig
 from codatsyncexpenses import utils
 from codatsyncexpenses._hooks import SDKHooks
 from codatsyncexpenses.models import shared
 from typing import Callable, Dict, Optional, Union
 
 class CodatSyncExpenses:
     r"""Sync for Expenses: The API for Sync for Expenses.
@@ -44,51 +48,58 @@
     manage_data: ManageData
     r"""Asynchronously retrieve data from an integration to refresh data in Codat."""
     push_operations: PushOperations
     r"""Access create, update and delete operations made to an SMB's data connection."""
     configuration: Configuration
     r"""Manage mapping options and sync configuration."""
     expenses: Expenses
-    r"""Create expense datasets and upload receipts."""
+    r"""Create expense transactions."""
+    reimbursements: Reimbursements
+    r"""Create reimbursable expense transactions."""
     sync: Sync
     r"""Trigger and monitor expense syncs to accounting software."""
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
+    attachments: Attachments
+    r"""Upload attachmens to expenses, transfers and reimbursable expense transactions."""
+    transfers: Transfers
+    r"""Create transfer transactions."""
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  security: Union[shared.Security,Callable[[], shared.Security]] = None,
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param security: The security details required for authentication
         :type security: Union[shared.Security,Callable[[], shared.Security]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+    
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             retry_config=retry_config
@@ -98,24 +109,27 @@
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.companies = Companies(self.sdk_configuration)
         self.connections = Connections(self.sdk_configuration)
         self.accounts = Accounts(self.sdk_configuration)
         self.customers = Customers(self.sdk_configuration)
         self.suppliers = Suppliers(self.sdk_configuration)
         self.manage_data = ManageData(self.sdk_configuration)
         self.push_operations = PushOperations(self.sdk_configuration)
         self.configuration = Configuration(self.sdk_configuration)
         self.expenses = Expenses(self.sdk_configuration)
+        self.reimbursements = Reimbursements(self.sdk_configuration)
         self.sync = Sync(self.sdk_configuration)
         self.transaction_status = TransactionStatus(self.sdk_configuration)
+        self.attachments = Attachments(self.sdk_configuration)
+        self.transfers = Transfers(self.sdk_configuration)
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/sdkconfiguration.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/sdkconfiguration.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from codatsyncexpenses.models import shared
 from dataclasses import dataclass
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.codat.io',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'prealpha'
-    sdk_version: str = '6.1.0'
-    gen_version: str = '2.286.2'
-    user_agent: str = 'speakeasy-sdk/python 6.1.0 2.286.2 prealpha codat-sync-for-expenses'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '6.2.0'
+    gen_version: str = '2.301.3'
+    user_agent: str = 'speakeasy-sdk/python 6.2.0 2.301.3 prealpha codat-sync-for-expenses'
+    retry_config: Optional[RetryConfig] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/suppliers.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/companies.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import Optional
 
-class Suppliers:
-    r"""Suppliers"""
+class Companies:
+    r"""Create and manage your Codat companies."""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: operations.CreateSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateSupplierResponse:
-        r"""Create supplier
-        The *Create supplier* endpoint creates a new [supplier](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
+    def create(self, request: Optional[shared.CompanyRequestBody], retries: Optional[utils.RetryConfig] = None) -> operations.CreateCompanyResponse:
+        r"""Create company
+        Use the *Create company* endpoint to create a new [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) that represents your customer in Codat. 
 
-        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
+        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
+        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
 
-        **Integration-specific behaviour**
-
-        Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-suppliers-model).
-
-        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating an account.
+        If forbidden characters (see `name` pattern) are present in the request, a company will be created with the forbidden characters removed. For example, `Company (Codat[1])` with be created as `Company Codat1`.
         """
-        hook_ctx = HookContext(operation_id='create-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='create-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateSupplierRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers', request)
+        url = base_url + '/companies'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateSupplierRequest, "supplier", True, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Optional[shared.CompanyRequestBody], "request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.CreateSupplierRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -54,81 +50,155 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.CreateSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateSupplierResponse])
-                res.create_supplier_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [400, 401, 402, 403, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get(self, request: operations.GetSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSupplierResponse:
-        r"""Get supplier
-        The *Get supplier* endpoint returns a single supplier for a given supplierId.
+    def delete(self, request: operations.DeleteCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteCompanyResponse:
+        r"""Delete a company
+        The *Delete company* endpoint permanently deletes a [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company), its [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) and any cached data. This operation is irreversible.
 
-        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
+        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
+        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
+        """
+        hook_ctx = HookContext(operation_id='delete-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        global_retry_config = self.sdk_configuration.retry_config
+        retry_config = retries
+        if retry_config is None:
+            if global_retry_config:
+                retry_config = global_retry_config
+            else:
+                retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
+
+        req = None
+        def do_request():
+            nonlocal req
+            try:
+                req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+                http_res = client.send(req)
+            except Exception as e:
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support getting a specific supplier.
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
+                    raise e
+                if result is not None:
+                    http_res = result
+            else:
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+
+            return http_res
 
-        Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
+        
+        
+        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 204:
+            pass
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
+    def get(self, request: operations.GetCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyResponse:
+        r"""Get company
+        The *Get company* endpoint returns a single company for a given `companyId`.
+
+        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
+        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
-        hook_ctx = HookContext(operation_id='get-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='get-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSupplierRequest, base_url, '/companies/{companyId}/data/suppliers/{supplierId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -143,86 +213,83 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Supplier])
-                res.supplier = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [401, 402, 403, 404, 409, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list(self, request: operations.ListSuppliersRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSuppliersResponse:
-        r"""List suppliers
-        The *List suppliers* endpoint returns a list of [suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
-
-        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
+    def list(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
+        r"""List companies
+        The *List companies* endpoint returns a list of [companies] associated to your instances.
 
-        Before using this endpoint, you must have [retrieved data for the company](https://docs.codat.io/sync-for-expenses-api#/operations/refresh-company-data).
+        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
+        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
-        hook_ctx = HookContext(operation_id='list-suppliers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='list-companies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListSuppliersRequest, base_url, '/companies/{companyId}/data/suppliers', request)
+        url = base_url + '/companies'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListSuppliersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -231,93 +298,86 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','409','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListSuppliersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Suppliers])
-                res.suppliers = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
+                res.companies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 409, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update(self, request: operations.UpdateSupplierRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateSupplierResponse:
-        r"""Update supplier
-        The *Update supplier* endpoint updates an existing [supplier](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) for a given company's connection.
-
-        [Suppliers](https://docs.codat.io/sync-for-expenses-api#/schemas/Supplier) are people or organizations that provide something, such as a product or service.
-
-        **Integration-specific behaviour**
+    def update(self, request: operations.UpdateCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateCompanyResponse:
+        r"""Update company
+        Use the *Update company* endpoint to update both the name and description of the company. 
+        If you use [groups](https://docs.codat.io/sync-for-expenses-api#/schemas/Group) to manage a set of companies, use the [Add company](https://docs.codat.io/sync-for-expenses-api#/operations/add-company-to-group) or [Remove company](https://docs.codat.io/sync-for-expenses-api#/operations/remove-company-from-group) endpoints to add or remove a company from a group.
 
-        Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/sync-for-expenses-api#/operations/get-create-update-suppliers-model).
-
-        Check out our [coverage explorer](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating an account.
+        A [company](https://docs.codat.io/sync-for-expenses-api#/schemas/Company) represents a business sharing access to their data.
+        Each company can have multiple [connections](https://docs.codat.io/sync-for-expenses-api#/schemas/Connection) to different data sources, such as one connection to Xero for accounting data, two connections to Plaid for two bank accounts, and a connection to Zettle for POS data.
         """
-        hook_ctx = HookContext(operation_id='update-supplier', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='update-company', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateSupplierRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers/{supplierId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateSupplierRequest, "supplier", True, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCompanyRequest, "company_request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.UpdateSupplierRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -326,59 +386,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
-            if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+            if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.UpdateSupplierResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateSupplierResponse])
-                res.update_supplier_response = out
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+        elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/transaction_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from codatsyncexpenses import utils
-from codatsyncexpenses._hooks import HookContext
+from codatsyncexpenses._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from codatsyncexpenses.models import errors, operations, shared
 from typing import List, Optional
 
 class TransactionStatus:
     r"""Retrieve the status of transactions within a sync."""
     sdk_configuration: SDKConfiguration
 
@@ -19,15 +19,15 @@
     def get(self, request: operations.GetSyncTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncTransactionResponse:
         r"""Get sync transaction
         Gets the status of a transaction for a sync
         """
         hook_ctx = HookContext(operation_id='get-sync-transaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -42,53 +42,51 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.GetSyncTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetSyncTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Transaction]])
                 res.transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,22 +100,22 @@
     def list(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
         r"""List sync transactions
         Gets the transactions and status for a sync
         """
         hook_ctx = HookContext(operation_id='list-sync-transactions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
+        url = utils.generate_url(base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListSyncTransactionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
@@ -126,59 +124,58 @@
             else:
                 retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         req = None
         def do_request():
             nonlocal req
             try:
-                req = self.sdk_configuration.get_hooks().before_request(
-                    hook_ctx, 
-                    requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-                )
+                req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+                req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
                 http_res = client.send(req)
             except Exception as e:
-                _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-                raise e
+                _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+                if e is not None:
+                    raise e
 
             if utils.match_status_codes(['400','401','402','403','404','429','4XX','500','503','5XX'], http_res.status_code):
-                http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-                if e:
+                result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+                if e is not None:
                     raise e
+                if result is not None:
+                    http_res = result
             else:
-                result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-                if isinstance(result, Exception):
-                    raise result
-                http_res = result
+                http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
 
             return http_res
 
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         
         
-        res = operations.ListSyncTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListSyncTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Transactions])
                 res.transactions = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code in [400, 401, 402, 403, 404, 429, 500, 503]:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorMessage)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `codat-sync-for-expenses-6.1.0/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-6.2.0/src/codatsyncexpenses/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.shared'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.shared"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

