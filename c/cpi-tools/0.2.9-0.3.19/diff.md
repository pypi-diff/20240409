# Comparing `tmp/cpi_tools-0.2.9.tar.gz` & `tmp/cpi_tools-0.3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.2.9.tar", last modified: Thu Sep  7 10:09:10 2023, max compression
+gzip compressed data, was "cpi_tools-0.3.19.tar", last modified: Mon Apr  8 22:14:53 2024, max compression
```

## Comparing `cpi_tools-0.2.9.tar` & `cpi_tools-0.3.19.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-07 10:09:10.244489 cpi_tools-0.2.9/
--rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0      956 2023-09-07 10:09:10.244489 cpi_tools-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-09-07 10:09:10.231225 cpi_tools-0.2.9/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/cpi_tools/aws_tools.py
--rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/cpi_tools/cpi_validation.py
--rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/cpi_tools/fuzzy_matching_cpi.py
--rw-rw-rw-   0        0        0    16144 2023-07-07 16:13:31.000000 cpi_tools-0.2.9/cpi_tools/tracking_processing_tools.py
-drwxrwxrwx   0        0        0        0 2023-09-07 10:09:10.244489 cpi_tools-0.2.9/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      956 2023-09-07 10:09:10.000000 cpi_tools-0.2.9/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-09-07 10:09:10.000000 cpi_tools-0.2.9/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-07 10:09:10.000000 cpi_tools-0.2.9/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-09-07 10:09:10.000000 cpi_tools-0.2.9/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0      581 2023-09-07 10:09:10.244489 cpi_tools-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.849841 cpi_tools-0.3.19/
+-rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.3.19/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-01-27 16:40:16.000000 cpi_tools-0.3.19/MANIFEST.in
+-rw-rw-rw-   0        0        0      957 2024-04-08 22:14:53.841828 cpi_tools-0.3.19/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-01-27 16:58:15.000000 cpi_tools-0.3.19/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.809827 cpi_tools-0.3.19/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.3.19/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-01-27 16:56:14.000000 cpi_tools-0.3.19/cpi_tools/aws_tools.py
+-rw-rw-rw-   0        0        0     5403 2023-09-18 18:36:57.000000 cpi_tools-0.3.19/cpi_tools/cpi_validation.py
+-rw-rw-rw-   0        0        0     9747 2024-04-08 21:06:40.000000 cpi_tools-0.3.19/cpi_tools/fuzzy_matching_cpi.py
+-rw-rw-rw-   0        0        0    16524 2024-04-08 21:06:40.000000 cpi_tools-0.3.19/cpi_tools/tracking_processing_tools.py
+-rw-rw-rw-   0        0        0    15367 2024-04-08 22:14:01.000000 cpi_tools-0.3.19/cpi_tools/tracking_processing_tools_v2.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.833839 cpi_tools-0.3.19/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      957 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-01-27 16:46:45.000000 cpi_tools-0.3.19/pyproject.toml
+-rw-rw-rw-   0        0        0      582 2024-04-08 22:14:53.849841 cpi_tools-0.3.19/setup.cfg
```

### Comparing `cpi_tools-0.2.9/PKG-INFO` & `cpi_tools-0.3.19/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpi_tools
-Version: 0.2.9
+Version: 0.3.19
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.9/cpi_tools/aws_tools.py` & `cpi_tools-0.3.19/cpi_tools/aws_tools.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import pandas as pd
-import boto3
-import s3fs
-from io import StringIO
-
-from dotenv import load_dotenv, find_dotenv
-
-def read_from_s3(s3_bucket: str, s3_file_path:str, file_name: str, file_type = 'csv', sheet_name=None, skip_rows=0) -> pd.DataFrame:
-    """
-    This function reads data from an S3 bucket and returns it as a pandas DataFrame.
-
-    Inputs:
-
-    s3_bucket (str): The name of the S3 bucket where the file is located.
-    s3_file_path (str): The file path within the S3 bucket.
-    file_name (str): The name of the file to be read.
-    file_type (str, optional): The file type of the file to be read. Defaults to 'csv'.
-    sheet_name (str, optional): The sheet name to be read from the excel file. Only used if file_type is 'xlsx'.
-    skip_rows (int, optional): The number of rows to skip when reading the file. Defaults to 0.
-    Returns:
-
-    df (pd.DataFrame): The data read from the file.
-    """
-
-    if load_dotenv(find_dotenv()):
-
-        if file_type == 'csv':
-            df = pd.read_csv(f's3://{s3_bucket}/{s3_file_path}/{file_name}.csv',skiprows=skip_rows, encoding='utf-8')
-
-        elif file_type == 'xlsx':
-            if sheet_name:
-                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', sheet_name=sheet_name, skiprows=skip_rows)
-            else:
-                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', skiprows=skip_rows)
-    else:
-        print('No AWS account variables found. Please add account variables to the .env file in your local directory')
-
-    return df
-
-
-def write_to_s3(df: pd.DataFrame, s3_bucket: str, s3_file_path:str, file_name: str):
-
-    '''
-    This function takes a processed reference dataframe and the filename for it to be saved as within S3 
-    and uploads the dataframe as a CSV
-
-    Inputs:
-
-    df (pd.DataFrame): The dataframe to be written to s3
-    s3_bucket (str): The name of the S3 bucket where the file will ve saved.
-    s3_file_path (str): The file path within the S3 bucket.
-    file_name (str): The name of the file to be saved.
-
-    Returns:
-    None
-    '''
-    
-    #Filepath to processed cpi reference folder
-    csv_buffer = StringIO()
-    df.to_csv(csv_buffer, index=False, encoding="utf-8")
-    s3_resource = boto3.resource('s3')
+import pandas as pd
+import boto3
+import s3fs
+from io import StringIO
+
+from dotenv import load_dotenv, find_dotenv
+
+def read_from_s3(s3_bucket: str, s3_file_path:str, file_name: str, file_type = 'csv', sheet_name=None, skip_rows=0) -> pd.DataFrame:
+    """
+    This function reads data from an S3 bucket and returns it as a pandas DataFrame.
+
+    Inputs:
+
+    s3_bucket (str): The name of the S3 bucket where the file is located.
+    s3_file_path (str): The file path within the S3 bucket.
+    file_name (str): The name of the file to be read.
+    file_type (str, optional): The file type of the file to be read. Defaults to 'csv'.
+    sheet_name (str, optional): The sheet name to be read from the excel file. Only used if file_type is 'xlsx'.
+    skip_rows (int, optional): The number of rows to skip when reading the file. Defaults to 0.
+    Returns:
+
+    df (pd.DataFrame): The data read from the file.
+    """
+
+    if load_dotenv(find_dotenv()):
+
+        if file_type == 'csv':
+            df = pd.read_csv(f's3://{s3_bucket}/{s3_file_path}/{file_name}.csv',skiprows=skip_rows, encoding='utf-8')
+
+        elif file_type == 'xlsx':
+            if sheet_name:
+                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', sheet_name=sheet_name, skiprows=skip_rows)
+            else:
+                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', skiprows=skip_rows)
+    else:
+        print('No AWS account variables found. Please add account variables to the .env file in your local directory')
+
+    return df
+
+
+def write_to_s3(df: pd.DataFrame, s3_bucket: str, s3_file_path:str, file_name: str):
+
+    '''
+    This function takes a processed reference dataframe and the filename for it to be saved as within S3 
+    and uploads the dataframe as a CSV
+
+    Inputs:
+
+    df (pd.DataFrame): The dataframe to be written to s3
+    s3_bucket (str): The name of the S3 bucket where the file will ve saved.
+    s3_file_path (str): The file path within the S3 bucket.
+    file_name (str): The name of the file to be saved.
+
+    Returns:
+    None
+    '''
+    
+    #Filepath to processed cpi reference folder
+    csv_buffer = StringIO()
+    df.to_csv(csv_buffer, index=False, encoding="utf-8")
+    s3_resource = boto3.resource('s3')
     s3_resource.Object(s3_bucket, f'{s3_file_path}/{file_name}.csv').put(Body=csv_buffer.getvalue())
```

### Comparing `cpi_tools-0.2.9/cpi_tools/cpi_validation.py` & `cpi_tools-0.3.19/cpi_tools/cpi_validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from operator import ge
+from webbrowser import get
 import pandas as pd
 import pandera as pa
 from cpi_tools import aws_tools
 import boto3
 import s3fs
 
 def get_valid_ref_values(ref_file, ref_column) -> list[str]:
@@ -28,61 +30,67 @@
     The function uses the validate method from the pandas_schema library to validate the DataFrame against the schema, 
     and raises an exception if the validation fails. If the validation is successful, the function prints a message 
     indicating that the DataFrame is GLCF compatible.
         
     '''
 
     # Get or define valid column values
+
+    valid_data_source_values = get_valid_ref_values('ref_data_source', 'data_source')
     valid_sector_values = get_valid_ref_values('ref_project_type', 'sector')
     valid_sub_sector_values = get_valid_ref_values('ref_project_type', 'sub_sector')
     valid_solution_values = get_valid_ref_values('ref_project_type', 'solution')
     valid_country_values = get_valid_ref_values('ref_geog_list_cpi', 'country_cpi')
     valid_region_values = get_valid_ref_values('ref_geog_list_cpi', 'region_cpi')
+    valid_oecd_values = get_valid_ref_values('ref_geog_list_cpi', 'oecd_membership')
+    valid_r3_ipcc_values = get_valid_ref_values('ref_geog_list_cpi', 'r3_ipcc')
+    valid_instrument_values = get_valid_ref_values('ref_instr', 'instrument_type')
     
     valid_institution_type_layer2_values =  ["Bilateral DFI", "Commercial FI", 'Corporation', 'Export Credit Agency (ECA)',
                             'Funds','Government', 'Household/Individual', 'Institutional Investors', 
                             'Multilateral Climate Funds','Multilateral DFI','National DFI', 'Public Fund',
                             'SOE', 'State-owned FI', 'Unknown']
     
-    valid_institution_type_layer1_values = ['Public', 'Private']
-
+    valid_institution_type_layer1_values = ['Public', 'Private', 'Unknown']
     valid_domestic_international_values = ['Domestic', 'International']
-
     valid_use_values = ['Mitigation', 'Adaptation', 'Multiple Objectives']
+    valid_exclusion_values = ['Include', 'Exclude']
 
 
     # Define GLCF Schema
     schema = pa.DataFrameSchema({
         "id_glcf": pa.Column(str),
-        "data_source_id": pa.Column(str, required=False),
+        "id_original": pa.Column(str, required=False),
         "data_source": pa.Column(str),
         "year": pa.Column(int, checks=pa.Check.in_range(min_date, max_date)),
         "project_name": pa.Column(str),
         "project_description": pa.Column(str, nullable=True),
         "country_origin_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
         "region_origin_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_origin_cpi": pa.Column(str),
+        "oecd_origin_cpi": pa.Column(str, pa.Check.isin(valid_oecd_values)),
+        "r3_ipcc_origin_cpi": pa.Column(str, pa.Check.isin(valid_r3_ipcc_values)),
         "country_destination_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
         "region_destination_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_destination_cpi": pa.Column(str),
+        "oecd_destination_cpi": pa.Column(str, pa.Check.isin(valid_oecd_values)),
+        "r3_ipcc_destination_cpi": pa.Column(str, pa.Check.isin(valid_r3_ipcc_values)),
         "institution_cpi": pa.Column(str),
         "institution_type_layer1": pa.Column(str, pa.Check.isin(valid_institution_type_layer1_values)),
         "institution_type_layer2": pa.Column(str, pa.Check.isin(valid_institution_type_layer2_values)),
         "recipient_type_layer1": pa.Column(str),
         "domestic_international": pa.Column(str, pa.Check.isin(valid_domestic_international_values)),
         "value_USDm": pa.Column(float, pa.Check.ge(0)), #Greater than or equal to 0
-        "instrument_cpi": pa.Column(str),
+        "instrument_cpi": pa.Column(str, pa.Check.isin(valid_instrument_values)),
         "sector_original": pa.Column(str),
         "sector_key_cpi": pa.Column(str),
         "sector_cpi": pa.Column(str, checks=pa.Check.isin(valid_sector_values)),
         "sub_sector_cpi": pa.Column(str, pa.Check.isin(valid_sub_sector_values)),
         "solution_cpi": pa.Column(str, pa.Check.isin(valid_solution_values)),
         "use_cpi": pa.Column(str, pa.Check.isin(valid_use_values)),
         "gender_cpi": pa.Column(str),
-        "exclude_include": pa.Column(str)
+        "exclude_include": pa.Column(str, pa.Check.isin(valid_exclusion_values))
     })
 
     # Attempt Validation
     try:
         schema.validate(df, lazy=True)
         print('Dataframe GLCF Compatible')
     except pa.errors.SchemaErrors as e:
```

### Comparing `cpi_tools-0.2.9/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.3.19/cpi_tools/tracking_processing_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,395 +1,395 @@
-import dropbox
-from dropbox.exceptions import AuthError
-from dropbox import DropboxOAuth2FlowNoRedirect
-import os
-import pandas as pd
-import numpy as np
-import io
-import unicodedata
-from datetime import date
-import uuid
-from dotenv import load_dotenv, find_dotenv
-import s3fs
-import boto3
-load_dotenv(find_dotenv())
-from cpi_tools import aws_tools
-
-S3_REFERENCE_BUCKET = 'cpi-reference-data'
-
-"""
-######################################################################################################
-######################## Dropbox and reference table processing functions ############################
-######################################################################################################
-
-"""
-
-
-def dropbox_authorisation(app_key:str, secret_key:str):
-    """
-    This function initiates an authorization process for a Dropbox App. 
-
-    Parameters:
-    app_key (str): The app key for your Dropbox app. You get this when you create an app on the Dropbox developers' site.
-    secret_key (str): The secret key for your Dropbox app. This is also provided when you create an app.
-
-    Returns:
-    oauth_result: A DropboxOAuth2FlowNoRedirect result object which contains access token and other information.
-    """
-
-    # Creating an instance of DropboxOAuth2FlowNoRedirect using app_key and secret_key.
-    # This class performs the second half of the OAuth2 'code' flow, where a code is exchanged for a token.
-    auth_flow = DropboxOAuth2FlowNoRedirect(app_key, secret_key)
-
-    # Starting the OAuth2 flow and getting the authorization URL.
-    authorize_url = auth_flow.start()
-
-    # Printing instructions for the user.
-    print ("1. Go to: " + authorize_url)
-    print ("2. Click 'Allow' (you might have to log in first).")
-    print ("3. Copy the authorization code.")
-
-    # Taking the authorization code input from the user.
-    auth_code = input("Enter the authorization code here: ").strip()
-
-    # Trying to finish the OAuth2 flow using the authorization code and obtaining the result.
-    try:
-        oauth_result = auth_flow.finish(auth_code)
-    except Exception as e:
-        print("Error: %s" % (e,))
-
-    # Return the result which can be used for making Dropbox API calls.
-    return oauth_result
-
-
-
-def export_dropbox_file_to_s3(dropbox_file_path:str, s3_bucket:str, s3_path:str, s3_file_name:str):
-    """
-    This function exports a file from Dropbox to an Amazon S3 bucket.
-
-    Parameters:
-    dropbox_file_path (str): The path of the file in Dropbox.
-    s3_bucket (str): The name of the S3 bucket to which the file is to be uploaded.
-    s3_path (str): The path in the S3 bucket where the file should be placed.
-    s3_file_name (str): The name with which the file should be stored in the S3 bucket.
-
-    Returns:
-    None
-    """
-    
-    # Attempt to load environment variables for Dropbox app key and secret key
-    try:
-        app_key = os.getenv('DROPBOX_APP_KEY')
-        secret_key = os.getenv('DROPBOX_SECRET_KEY')
-    except Exception as e:
-        print('Error Loading Dropbox app and secret key. Ensure variables are in your .env file: ' + str(e))
-
-    # Authorize Dropbox API usage with the app key and secret key
-    oauth = dropbox_authorisation(app_key=app_key, secret_key=secret_key)
-    
-    # Attempt to download the file from Dropbox and upload to S3
-    try:
-        # Set up Dropbox client with OAuth credentials
-        with dropbox.Dropbox(oauth2_access_token=oauth.access_token,
-                             oauth2_access_token_expiration=oauth.expires_at,
-                             oauth2_refresh_token=oauth.refresh_token,
-                             app_key=app_key,
-                             app_secret=secret_key) as dbx:
-
-            print("Successfully set up client!")
-
-            # Download the file from Dropbox
-            metadata, result = dbx.files_download(path=dropbox_file_path)
-
-            try: 
-                # Set up S3 client
-                s3 = boto3.resource('s3')
-                # Upload the file to S3
-                s3.Bucket(s3_bucket).put_object(Key=f'{s3_path}/{s3_file_name}', Body=result.content)
-            except Exception as e:
-                print('Error uploading dropbox data to S3: ' + str(e))
-
-    except Exception as e:
-        print('Error downloading file from Dropbox: ' + str(e))
-
-    return None
-
-
-def process_reference_data(base_data, file_name=None, sql_field_name=None, col_name_row=0, start_row=3, project_type=False): 
-    '''
-    This function takes an unprocessed reference dataframe taken from the master reference table excel and converts it
-    into a format useable within processing code
-    
-    If a filename is provided, it then writes this processed data to an s3 bucket 
-    
-    Parameters:
-    base_data: Pandas Dataframe
-    file_name: String
-    sql_field_name: String - If the reference table has a SQL Field name column, this is dropped
-    col_name_row: Int - selects the row that is used as the column names for the processed data
-    start_row: Int - Selects the row to start from, drops the rows prior to this one
-    project_type: Boolean - If project_type reference data, apply additional processing steps
-    
-    Returns
-    df: Pandas Dataframe - processed reference data
-    '''
-    
-    df = base_data.copy()
-
-    #Set the column names to the correct rows
-    df.columns = df.iloc[col_name_row]
-    
-    #If the ref table has a sql field, drop it
-    if sql_field_name:
-
-        df.drop(columns = sql_field_name, inplace=True)
-    
-    #Select the row to start from
-    df = df.iloc[start_row:]
-    
-    #Drop columns called nan
-    df = df.loc[:, df.columns.notna()]
-    
-    #If ref_project_type reference data, create a use column
-    if project_type:
-            df['use'] = df.apply(lambda x: generate_project_type_use(x['MI'], x['AD']), axis=1)
-        
-    
-    #Drop rows where all values are nan
-    df.dropna(axis = 0, how = 'all', inplace = True)
-
-    #Remove whitespace from strings and column names
-    df.rename(columns=lambda x: x.strip(), inplace=True)
-    df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
-
-    #Enforce unicode conversion
-    df = df.applymap(lambda x: unicodedata.normalize("NFKD",x) if isinstance(x, str) else x)
-    
-    #Write to S3 if filename is provided
-    if file_name:
-            
-        aws_tools.write_to_s3(df, S3_REFERENCE_BUCKET, 'cpi/processed', file_name)
-        
-def generate_project_type_use(mi, ad):
-    '''
-    This function generates a Use column in the project type reference data using the MI and AD columns
-    
-    mi: Boolean Column
-    ad: Boolean Column
-    
-    Returns
-    use: String Column
-    
-    '''
-
-    if ((mi == 1) & (ad == 1)):
-        use = 'Multiple Objectives'
-    elif mi == 1:
-        use = 'Mitigation'
-    elif ad == 1:
-        use = 'Adaptation'
-    else:
-        use = np.nan
-
-    return use
-
-def extract_reference_sheets():
-    """
-    This function extracts multiple reference sheets from an Excel file stored in an Amazon S3 bucket.
-    It then processes each sheet using the 'process_reference_data' function.
-
-    Parameters: None
-
-    Returns: None
-    """
-    # Define the path to the file in the S3 bucket
-    s3_file_path = 'cpi/raw'
-    # Define the name of the file
-    file_name = 'master_ref.xlsm'
-    
-    # For each sheet in the Excel file, read the data into a pandas DataFrame
-    # and then process that data using the 'process_reference_data' function.
-    # The arguments passed to 'process_reference_data' vary depending on the specific sheet being processed.
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='coeff'),
-                           'ref_coef', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='double_counting'),
-                           'ref_double_counting', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='fx'),
-                           'ref_fx', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gearing'),
-                           'ref_gearing')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gender'),
-                           'ref_gender', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_all'),
-                           'ref_geog_list_all', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_cpi'),
-                           'ref_geog_list_cpi', 'SQL Field Name', 1,4)
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_all'),
-                           'ref_institution_list_all', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_cpi'),
-                           'ref_institution_list_cpi','SQL Field Name', start_row=4)
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='instr'),
-                           'ref_instr', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='multiplier'),
-                           'ref_multiplier')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='recipient'),
-                           'ref_recipient')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='project_type'),
-                           'ref_project_type', 'SQL Field Name', project_type=True)
-        
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='ownership'),
-                           'ref_ownership')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='sector'),
-                           'ref_sector', 'SQL Field Name')
-
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='soe'),
-                           'ref_soe', 'SQL Field Name')
-    
-    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='data_source'),
-                           'ref_data_source')
-
-    return None
-
-
-def update_ref_tables():
-    """
-    This function updates reference tables by reading a master reference table from Dropbox,
-    exporting it to an Amazon S3 bucket, and then extracting reference data from the table.
-
-    Parameters: None
-
-    Returns: None
-    """
-
-    # Output status update
-    print('Reading Master Reference Table...')
-
-    # Define the path to the file in Dropbox
-    reference_metadata_dropbox_path = '/CF-Program/1.Workstreams/Tracking/GLCF/GLCF MASTER/3. Reference Tables Excel/Reference Tables_v1_MASTER_2022.xlsm'
-    
-    # Export the file from Dropbox to an S3 bucket
-    export_dropbox_file_to_s3(reference_metadata_dropbox_path, s3_bucket='cpi-reference-data',
-                              s3_path='cpi/raw', s3_file_name='master_ref.xlsm')
-    
-    # Output status update
-    print('Extracting reference data')
-
-    # Extract reference data from the master reference table
-    extract_reference_sheets()
-
-    return None
-
-
-
-def get_reference_tables(update=False):
-    """
-    This function retrieves various reference tables stored in an Amazon S3 bucket as pandas DataFrames.
-    If the 'update' parameter is set to True, it will first update the reference tables
-    by calling the 'update_ref_tables' function.
-
-    Parameters:
-    update (bool): If True, the reference tables are updated before being retrieved.
-
-    Returns:
-    tuple: A tuple of pandas DataFrames, each one representing a reference table.
-    """
-    
-    # If the 'update' parameter is set to True, update the reference tables
-    if update:
-        update_ref_tables()
-
-    # Define the path to the folder in the S3 bucket where the reference tables are stored
-    cpi_reference_folder = 'cpi/processed'
-
-    # Retrieve each reference table from the S3 bucket and read it into a pandas DataFrame.
-    # Note that each file is read with 'utf-8' encoding.
-    # Each DataFrame is stored in a separate variable.
-
-    # Data Source Geography Names
-    ref_geog_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_all.csv', encoding='utf-8')
-    
-    # Coefficient table
-    ref_coeff =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_coef.csv', encoding='utf-8')
-    
-    # Foreign exchange rates
-    ref_fx =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_fx.csv', encoding='utf-8')
-    
-    # Gender table
-    ref_gender =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gender.csv', encoding='utf-8')
-    
-    # Gearing table
-    ref_gearing =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gearing.csv', encoding='utf-8')
-    
-    # CPI Geography Names
-    ref_geog_list_cpi =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_cpi.csv', encoding='utf-8')
-    
-    # Data Source Institution names
-    ref_institution_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_all.csv', encoding='utf-8')
-    
-    # CPI Institution names
-    ref_institution_list_cpi = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_cpi.csv', encoding='utf-8')
-
-    # Ownership table
-    ref_ownership = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_ownership.csv', encoding='utf-8')
-    
-    # Project type table
-    ref_project_type = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_project_type.csv')
-    
-    # Sector table
-    ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
-    
-    # Instrument table
-    ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
-    
-    # Capacity multiplier tables
-    ref_multiplier = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_multiplier.csv', encoding='utf-8')
-    
-    # Recipient table
-    ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
-    
-    # Data source
-    ref_data_source = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_data_source.csv', encoding='utf-8')
-
-    # Return all the DataFrames as a tuple
-    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_gearing, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
-    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_multiplier, ref_recipient, ref_data_source
-
-
-def generate_glcf_id(df:pd.DataFrame, year:int):
-    '''
-    This function generates a unique ID for each entry in the dataset processed. 
-    
-    Parameters:
-    df(pd.DataFrame): the dataset being processed. 
-    Note that it is important that this dataset has already been cleaned and most
-    importantly subset to only the relevant row entries, as the final data ID will
-    include the row number of each observation. 
-    year(int): the year of the GLCF publication (e.g., 2023 for data relating to
-    2021 and 2022).
-    
-    Returns:
-    df(pd.DataFrame): the inputted dataframe, with the addition of the column 'data_source_id'.
-    '''
-    
-    df['data_source_id'] = df.data_source_code.map(lambda x: str(x).zfill(3)) + '-' + \
-                           str(year) + '-' + \
-                           df.index.map(lambda x: str(x+1).zfill(9))
-
-    return df
-    
-    
-    
+import dropbox
+from dropbox.exceptions import AuthError
+from dropbox import DropboxOAuth2FlowNoRedirect
+import os
+import pandas as pd
+import numpy as np
+import io
+import unicodedata
+from datetime import date
+import uuid
+from dotenv import load_dotenv, find_dotenv
+import s3fs
+import boto3
+load_dotenv(find_dotenv())
+from cpi_tools import aws_tools
+
+S3_REFERENCE_BUCKET = 'cpi-reference-data'
+
+"""
+######################################################################################################
+######################## Dropbox and reference table processing functions ############################
+######################################################################################################
+
+"""
+
+
+def dropbox_authorisation(app_key:str, secret_key:str):
+    """
+    This function initiates an authorization process for a Dropbox App. 
+
+    Parameters:
+    app_key (str): The app key for your Dropbox app. You get this when you create an app on the Dropbox developers' site.
+    secret_key (str): The secret key for your Dropbox app. This is also provided when you create an app.
+
+    Returns:
+    oauth_result: A DropboxOAuth2FlowNoRedirect result object which contains access token and other information.
+    """
+
+    # Creating an instance of DropboxOAuth2FlowNoRedirect using app_key and secret_key.
+    # This class performs the second half of the OAuth2 'code' flow, where a code is exchanged for a token.
+    auth_flow = DropboxOAuth2FlowNoRedirect(app_key, secret_key)
+
+    # Starting the OAuth2 flow and getting the authorization URL.
+    authorize_url = auth_flow.start()
+
+    # Printing instructions for the user.
+    print ("1. Go to: " + authorize_url)
+    print ("2. Click 'Allow' (you might have to log in first).")
+    print ("3. Copy the authorization code.")
+
+    # Taking the authorization code input from the user.
+    auth_code = input("Enter the authorization code here: ").strip()
+
+    # Trying to finish the OAuth2 flow using the authorization code and obtaining the result.
+    try:
+        oauth_result = auth_flow.finish(auth_code)
+    except Exception as e:
+        print("Error: %s" % (e,))
+
+    # Return the result which can be used for making Dropbox API calls.
+    return oauth_result
+
+
+
+def export_dropbox_file_to_s3(dropbox_file_path:str, s3_bucket:str, s3_path:str, s3_file_name:str):
+    """
+    This function exports a file from Dropbox to an Amazon S3 bucket.
+
+    Parameters:
+    dropbox_file_path (str): The path of the file in Dropbox.
+    s3_bucket (str): The name of the S3 bucket to which the file is to be uploaded.
+    s3_path (str): The path in the S3 bucket where the file should be placed.
+    s3_file_name (str): The name with which the file should be stored in the S3 bucket.
+
+    Returns:
+    None
+    """
+    
+    # Attempt to load environment variables for Dropbox app key and secret key
+    try:
+        app_key = os.getenv('DROPBOX_APP_KEY')
+        secret_key = os.getenv('DROPBOX_SECRET_KEY')
+    except Exception as e:
+        print('Error Loading Dropbox app and secret key. Ensure variables are in your .env file: ' + str(e))
+
+    # Authorize Dropbox API usage with the app key and secret key
+    oauth = dropbox_authorisation(app_key=app_key, secret_key=secret_key)
+    
+    # Attempt to download the file from Dropbox and upload to S3
+    try:
+        # Set up Dropbox client with OAuth credentials
+        with dropbox.Dropbox(oauth2_access_token=oauth.access_token,
+                             oauth2_access_token_expiration=oauth.expires_at,
+                             oauth2_refresh_token=oauth.refresh_token,
+                             app_key=app_key,
+                             app_secret=secret_key) as dbx:
+
+            print("Successfully set up client!")
+
+            # Download the file from Dropbox
+            metadata, result = dbx.files_download(path=dropbox_file_path)
+
+            try: 
+                # Set up S3 client
+                s3 = boto3.resource('s3')
+                # Upload the file to S3
+                s3.Bucket(s3_bucket).put_object(Key=f'{s3_path}/{s3_file_name}', Body=result.content)
+            except Exception as e:
+                print('Error uploading dropbox data to S3: ' + str(e))
+
+    except Exception as e:
+        print('Error downloading file from Dropbox: ' + str(e))
+
+    return None
+
+
+def process_reference_data(base_data, file_name=None, sql_field_name=None, col_name_row=0, start_row=3, project_type=False): 
+    '''
+    This function takes an unprocessed reference dataframe taken from the master reference table excel and converts it
+    into a format useable within processing code
+    
+    If a filename is provided, it then writes this processed data to an s3 bucket 
+    
+    Parameters:
+    base_data: Pandas Dataframe
+    file_name: String
+    sql_field_name: String - If the reference table has a SQL Field name column, this is dropped
+    col_name_row: Int - selects the row that is used as the column names for the processed data
+    start_row: Int - Selects the row to start from, drops the rows prior to this one
+    project_type: Boolean - If project_type reference data, apply additional processing steps
+    
+    Returns
+    df: Pandas Dataframe - processed reference data
+    '''
+    
+    df = base_data.copy()
+
+    #Set the column names to the correct rows
+    df.columns = df.iloc[col_name_row]
+    
+    #If the ref table has a sql field, drop it
+    if sql_field_name:
+
+        df.drop(columns = sql_field_name, inplace=True)
+    
+    #Select the row to start from
+    df = df.iloc[start_row:]
+    
+    #Drop columns called nan
+    df = df.loc[:, df.columns.notna()]
+    
+    #If ref_project_type reference data, create a use column
+    if project_type:
+            df['use'] = df.apply(lambda x: generate_project_type_use(x['MI'], x['AD']), axis=1)
+        
+    
+    #Drop rows where all values are nan
+    df.dropna(axis = 0, how = 'all', inplace = True)
+
+    #Remove whitespace from strings and column names
+    df.rename(columns=lambda x: x.strip(), inplace=True)
+    df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
+
+    #Enforce unicode conversion
+    df = df.applymap(lambda x: unicodedata.normalize("NFKD",x) if isinstance(x, str) else x)
+    
+    #Write to S3 if filename is provided
+    if file_name:
+            
+        aws_tools.write_to_s3(df, S3_REFERENCE_BUCKET, 'cpi/processed', file_name)
+        
+def generate_project_type_use(mi, ad):
+    '''
+    This function generates a Use column in the project type reference data using the MI and AD columns
+    
+    mi: Boolean Column
+    ad: Boolean Column
+    
+    Returns
+    use: String Column
+    
+    '''
+
+    if ((mi == 1) & (ad == 1)):
+        use = 'Multiple Objectives'
+    elif mi == 1:
+        use = 'Mitigation'
+    elif ad == 1:
+        use = 'Adaptation'
+    else:
+        use = np.nan
+
+    return use
+
+def extract_reference_sheets():
+    """
+    This function extracts multiple reference sheets from an Excel file stored in an Amazon S3 bucket.
+    It then processes each sheet using the 'process_reference_data' function.
+
+    Parameters: None
+
+    Returns: None
+    """
+    # Define the path to the file in the S3 bucket
+    s3_file_path = 'cpi/raw'
+    # Define the name of the file
+    file_name = 'master_ref.xlsm'
+    
+    # For each sheet in the Excel file, read the data into a pandas DataFrame
+    # and then process that data using the 'process_reference_data' function.
+    # The arguments passed to 'process_reference_data' vary depending on the specific sheet being processed.
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='coeff'),
+                           'ref_coef', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='double_counting'),
+                           'ref_double_counting', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='fx'),
+                           'ref_fx', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gearing'),
+                           'ref_gearing')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='gender'),
+                           'ref_gender', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_all'),
+                           'ref_geog_list_all', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='geog_list_cpi'),
+                           'ref_geog_list_cpi', 'SQL Field Name', 1,4)
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_all'),
+                           'ref_institution_list_all', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='institution_list_cpi'),
+                           'ref_institution_list_cpi','SQL Field Name', start_row=4)
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='instr'),
+                           'ref_instr', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='multiplier'),
+                           'ref_multiplier')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='recipient'),
+                           'ref_recipient')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='project_type'),
+                           'ref_project_type', 'SQL Field Name', project_type=True)
+        
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='ownership'),
+                           'ref_ownership')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='sector'),
+                           'ref_sector', 'SQL Field Name')
+
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='soe'),
+                           'ref_soe', 'SQL Field Name')
+    
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='data_source'),
+                           'ref_data_source')
+
+    return None
+
+
+def update_ref_tables():
+    """
+    This function updates reference tables by reading a master reference table from Dropbox,
+    exporting it to an Amazon S3 bucket, and then extracting reference data from the table.
+
+    Parameters: None
+
+    Returns: None
+    """
+
+    # Output status update
+    print('Reading Master Reference Table...')
+
+    # Define the path to the file in Dropbox
+    reference_metadata_dropbox_path = '/CF-Program/1.Workstreams/Tracking/GLCF/GLCF MASTER/3. Reference Tables Excel/Reference Tables_v1_MASTER_2022.xlsm'
+    
+    # Export the file from Dropbox to an S3 bucket
+    export_dropbox_file_to_s3(reference_metadata_dropbox_path, s3_bucket='cpi-reference-data',
+                              s3_path='cpi/raw', s3_file_name='master_ref.xlsm')
+    
+    # Output status update
+    print('Extracting reference data')
+
+    # Extract reference data from the master reference table
+    extract_reference_sheets()
+
+    return None
+
+
+
+def get_reference_tables(update=False):
+    """
+    This function retrieves various reference tables stored in an Amazon S3 bucket as pandas DataFrames.
+    If the 'update' parameter is set to True, it will first update the reference tables
+    by calling the 'update_ref_tables' function.
+
+    Parameters:
+    update (bool): If True, the reference tables are updated before being retrieved.
+
+    Returns:
+    tuple: A tuple of pandas DataFrames, each one representing a reference table.
+    """
+    
+    # If the 'update' parameter is set to True, update the reference tables
+    if update:
+        update_ref_tables()
+
+    # Define the path to the folder in the S3 bucket where the reference tables are stored
+    cpi_reference_folder = 'cpi/processed'
+
+    # Retrieve each reference table from the S3 bucket and read it into a pandas DataFrame.
+    # Note that each file is read with 'utf-8' encoding.
+    # Each DataFrame is stored in a separate variable.
+
+    # Data Source Geography Names
+    ref_geog_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_all.csv', encoding='utf-8')
+    
+    # Coefficient table
+    ref_coeff =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_coef.csv', encoding='utf-8')
+    
+    # Foreign exchange rates
+    ref_fx =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_fx.csv', encoding='utf-8')
+    
+    # Gender table
+    ref_gender =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gender.csv', encoding='utf-8')
+    
+    # Gearing table
+    ref_gearing =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gearing.csv', encoding='utf-8')
+    
+    # CPI Geography Names
+    ref_geog_list_cpi =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_cpi.csv', encoding='utf-8')
+    
+    # Data Source Institution names
+    ref_institution_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_all.csv', encoding='utf-8')
+    
+    # CPI Institution names
+    ref_institution_list_cpi = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_cpi.csv', encoding='utf-8')
+
+    # Ownership table
+    ref_ownership = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_ownership.csv', encoding='utf-8')
+    
+    # Project type table
+    ref_project_type = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_project_type.csv')
+    
+    # Sector table
+    ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
+    
+    # Instrument table
+    ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
+    
+    # Capacity multiplier tables
+    ref_multiplier = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_multiplier.csv', encoding='utf-8')
+    
+    # Recipient table
+    ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
+    
+    # Data source
+    ref_data_source = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_data_source.csv', encoding='utf-8')
+
+    # Return all the DataFrames as a tuple
+    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_gearing, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
+    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_multiplier, ref_recipient, ref_data_source
+
+
+def generate_glcf_id(df:pd.DataFrame, year:int):
+    '''
+    This function generates a unique ID for each entry in the dataset processed. 
+    
+    Parameters:
+    df(pd.DataFrame): the dataset being processed. 
+    Note that it is important that this dataset has already been cleaned and most
+    importantly subset to only the relevant row entries, as the final data ID will
+    include the row number of each observation. 
+    year(int): the year of the GLCF publication (e.g., 2023 for data relating to
+    2021 and 2022).
+    
+    Returns:
+    df(pd.DataFrame): the inputted dataframe, with the addition of the column 'id_glcf'.
+    '''
+    
+    df['id_glcf'] = df.data_source_code.map(lambda x: str(x).zfill(3)) + '-' + \
+                           str(year) + '-' + \
+                           df.index.map(lambda x: str(x+1).zfill(9))
+
+    return df
+    
+    
+
```

### Comparing `cpi_tools-0.2.9/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.3.19/cpi_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi-tools
-Version: 0.2.9
+Name: cpi_tools
+Version: 0.3.19
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.9/setup.cfg` & `cpi_tools-0.3.19/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7069 5f74 6f6f 6c73 0d0a 7665   = cpi_tools..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 390d 0a61  rsion = 0.2.9..a
-00000030: 7574 686f 7220 3d20 4a61 6b65 2043 6f6e  uthor = Jake Con
-00000040: 6e6f 6c6c 792c 204e 696b 6974 6120 4d61  nolly, Nikita Ma
-00000050: 7269 6e69 0d0a 6175 7468 6f72 5f65 6d61  rini..author_ema
-00000060: 696c 203d 2064 6174 6173 6369 656e 6365  il = datascience
-00000070: 4063 7069 676c 6f62 616c 2e6f 7267 0d0a  @cpiglobal.org..
-00000080: 6465 7363 7269 7074 696f 6e20 3d20 5265  description = Re
-00000090: 706f 7369 746f 7279 206f 6620 6675 6e63  pository of func
-000000a0: 7469 6f6e 7320 7573 6564 2061 6372 6f73  tions used acros
-000000b0: 7320 4350 490d 0a6c 6f6e 675f 6465 7363  s CPI..long_desc
-000000c0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000d0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-000000e0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000f0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-00000100: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-00000110: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000120: 6f6d 2f63 6c69 6d61 7465 706f 6c69 6379  om/climatepolicy
-00000130: 6461 7461 2f63 7069 5f74 6f6f 6c73 0d0a  data/cpi_tools..
-00000140: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000150: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000160: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000170: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
-00000180: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000190: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001c0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-000001d0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000001e0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-000001f0: 6573 203d 203e 3d33 2e37 0d0a 696e 636c  es = >=3.7..incl
-00000200: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000210: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
-00000220: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000230: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000240: 300d 0a0d 0a                             0....
+00000020: 7273 696f 6e20 3d20 302e 332e 3139 0d0a  rsion = 0.3.19..
+00000030: 6175 7468 6f72 203d 204a 616b 6520 436f  author = Jake Co
+00000040: 6e6e 6f6c 6c79 2c20 4e69 6b69 7461 204d  nnolly, Nikita M
+00000050: 6172 696e 690d 0a61 7574 686f 725f 656d  arini..author_em
+00000060: 6169 6c20 3d20 6461 7461 7363 6965 6e63  ail = datascienc
+00000070: 6540 6370 6967 6c6f 6261 6c2e 6f72 670d  e@cpiglobal.org.
+00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2052  .description = R
+00000090: 6570 6f73 6974 6f72 7920 6f66 2066 756e  epository of fun
+000000a0: 6374 696f 6e73 2075 7365 6420 6163 726f  ctions used acro
+000000b0: 7373 2043 5049 0d0a 6c6f 6e67 5f64 6573  ss CPI..long_des
+000000c0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000d0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+000000e0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000f0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000100: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
+00000110: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000120: 636f 6d2f 636c 696d 6174 6570 6f6c 6963  com/climatepolic
+00000130: 7964 6174 612f 6370 695f 746f 6f6c 730d  ydata/cpi_tools.
+00000140: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000150: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000160: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000170: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+00000180: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000190: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000001a0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001c0: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+000001d0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+000001e0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+000001f0: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
+00000200: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000210: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
+00000220: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000230: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000240: 2030 0d0a 0d0a                            0....
```

