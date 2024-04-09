# Comparing `tmp/gocodeo-0.0.9.tar.gz` & `tmp/gocodeo-0.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocodeo-0.0.9.tar", last modified: Tue Mar 26 08:16:26 2024, max compression
+gzip compressed data, was "gocodeo-0.0.9.1.tar", last modified: Tue Apr  9 03:06:10 2024, max compression
```

## Comparing `gocodeo-0.0.9.tar` & `gocodeo-0.0.9.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 08:16:26.800686 gocodeo-0.0.9/
--rw-rw-rw-   0        0        0      746 2024-03-26 08:16:26.799677 gocodeo-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-03 14:58:55.000000 gocodeo-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 08:16:26.770816 gocodeo-0.0.9/gocodeo/
--rw-rw-rw-   0        0        0       41 2024-03-11 01:58:56.000000 gocodeo-0.0.9/gocodeo/__init__.py
--rw-rw-rw-   0        0        0    22077 2024-03-26 08:12:41.000000 gocodeo-0.0.9/gocodeo/generator.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:16:26.798472 gocodeo-0.0.9/gocodeo.egg-info/
--rw-rw-rw-   0        0        0      746 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-26 08:16:26.000000 gocodeo-0.0.9/gocodeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2024-03-03 14:59:37.000000 gocodeo-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 08:16:26.800686 gocodeo-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-03-26 08:13:36.000000 gocodeo-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.587958 gocodeo-0.0.9.1/
+-rw-rw-rw-   0        0        0      809 2024-04-09 03:06:10.582716 gocodeo-0.0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-03 14:58:55.000000 gocodeo-0.0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.549568 gocodeo-0.0.9.1/gocodeo/
+-rw-rw-rw-   0        0        0       67 2024-04-04 07:06:34.000000 gocodeo-0.0.9.1/gocodeo/__init__.py
+-rw-rw-rw-   0        0        0    27750 2024-04-08 05:16:56.000000 gocodeo-0.0.9.1/gocodeo/generator.py
+-rw-rw-rw-   0        0        0     7224 2024-04-08 18:54:13.000000 gocodeo-0.0.9.1/gocodeo/train.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:06:10.582716 gocodeo-0.0.9.1/gocodeo.egg-info/
+-rw-rw-rw-   0        0        0      809 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 03:06:10.000000 gocodeo-0.0.9.1/gocodeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2024-03-03 14:59:37.000000 gocodeo-0.0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 03:06:10.587958 gocodeo-0.0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2024-04-09 03:05:44.000000 gocodeo-0.0.9.1/setup.py
```

### Comparing `gocodeo-0.0.9/PKG-INFO` & `gocodeo-0.0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: gocodeo
-Version: 0.0.9
+Version: 0.0.9.1
 Summary: A package to generate unit tests for a file
 Author: GoCodeo AI
 Description-Content-Type: text/markdown
 Requires-Dist: vertexai
 Requires-Dist: requests
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: google-auth
 Requires-Dist: python-dotenv
+Requires-Dist: google-cloud-storage
+Requires-Dist: pymongo
 
         gocodeo is a  package that provides a command-line interface (CLI) to generate unit tests for files. 
         To use gocodeo , simply run the command:
         
             gocodeo generate <file_path>
             
         For example:
```

### Comparing `gocodeo-0.0.9/gocodeo/generator.py` & `gocodeo-0.0.9.1/gocodeo/generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -62,18 +62,19 @@
 client = MongoClient(connection_url,tlsCAFile=ca)
 
 # Access the CLI database
 db = client["CLI"]
 
 def update_client_1(private_key, total_lines, total_functions):
     # Access the client_1 collection
-    collection = db["client_1"]
+    # collection = db["client_1"]
+    collection=db["Local_1"]
 
     # Check if private_key matches
-    if private_key == "gc_spgrXSnfZqYSVqqhQiVjlYApSQofFXIUtF":
+    if private_key == "gc_local":
         # Find the document with the private_key
         document = collection.find_one({"private_key": private_key})
 
         # If document exists, update the lines and functions values
         if document:
             previous_lines = document.get("lines", 0)
             previous_functions = document.get("functions", 0)
@@ -214,16 +215,17 @@
 
     if len(choices) == 0:
         raise Exception("Prompt did not return any answer")   
     message = choices[0].get("message", {}).get("content", "")
     # print(message, "message")
  
     return message
-def generate_api_request(code, context, type, number):
-    prompt = f"You are angularjs unit testing expert. Your job is to write {number} numbers high quality unit test code using jasmine and karma framework only, for given angular code: {code} for the given {type} scenarios in the context: {context}. Strictly go through the context and generate at least {number} numbers high quality unit test code with description including assertions cvoering all scenarios in one file. Please mock all the services and data where ever necessary. Please Make sure to import all the dependencies at the top for execution of tests."
+def generate_api_request(code, context, type, number,import_lines,imported_code):
+    prompt = f"You are angularjs unit testing expert. Your job is to write {number} numbers high quality unit test code using jasmine and karma framework only, for given angular code: {code} for the given {type} scenarios in the context: {context}. Strictly go through the context and generate at least {number} numbers high quality unit test code with description including assertions covering all scenarios in one file. Please mock all the services and data where ever necessary. Please Make sure to import all the dependencies at the top for execution of tests & the imports are {import_lines}.Import all these dependencies as per given if they are present.{imported_code}these are the code of imported classes or functions.Take context from here also & try to generate more accurate & executable unit test cases."
+
     payload = {
         "model": "gpt-3.5-turbo-16k",
         "messages": [
             {
                 "role": "user",
                 "content": prompt
             }
@@ -274,16 +276,165 @@
 
     # Extract the filename from the file path
     filename = os.path.basename(file_path)
 
     # Remove the file extension if present
     filename_without_extension = os.path.splitext(filename)[0]
 
+    
+
     return filename_without_extension    
 
+def extract_imports_from_file(file_path):
+    try:
+        with open(file_path, 'r') as file:
+            typescript_code = file.read()
+            
+            # Regular expression pattern to match import statements
+            import_pattern = r'import\s+{[^}]+}\s+from\s+[\'"].+?[\'"];'
+
+            # Find all import statements using regex
+            import_lines = re.findall(import_pattern, typescript_code)
+
+            if not import_lines:
+                return ""  # Return empty string if no import lines found
+
+            # Concatenate import lines into a single string with newline characters
+            import_string = '\n'.join(import_lines)
+            
+            return import_string
+    except FileNotFoundError:
+        return "File not found"
+    except Exception as e:
+        return f"Error: {e}"
+    
+# Handle user defined imports
+def extract_user_defined_imports(typescript_code):
+    if not typescript_code.strip():
+        return ''  # Return empty string if no imports found
+
+    # Regular expression pattern to match import blocks
+    import_pattern = r'(import\s+{[^}]+}\s+from\s+[\'"][^\'"]+[\'"];)+'
+
+    # Find all import blocks using regex
+    import_blocks = re.findall(import_pattern, typescript_code)
+
+    user_defined_imports = []
+
+    # Iterate through import blocks
+    for import_block in import_blocks:
+        # Regular expression pattern to match individual import statements within the block
+        import_statement_pattern = r'import\s+{([^}]+)}\s+from\s+[\'"]([^\'"]+)[\'"];'
+
+        # Find all import statements within the block
+        import_statements = re.findall(import_statement_pattern, import_block)
+
+        # Iterate through import statements within the block
+        for import_statement in import_statements:
+            import_symbols, import_path = import_statement
+
+            # Check if the import path is a relative path (starts with './' or '../')
+            if import_path.startswith('./'):
+                # Replace './' with '../'
+                import_path = '../' + import_path[2:]
+            elif import_path.startswith('../'):
+                # Add an extra '../' to the import path
+                import_path = '../' + import_path
+
+            # Construct the new import statement
+            new_import_statement = f"import {{ {import_symbols} }} from '{import_path}';"
+
+            # Append the new import statement to the list
+            user_defined_imports.append(new_import_statement)
+
+    # Join the user-defined imports into a single string
+    user_defined_imports_string = '\n'.join(user_defined_imports)
+
+    return user_defined_imports_string
+
+
+
+
+# Replace the updated imports 
+def replace_string_imports(original_code, updated_imports):
+    if not original_code.strip() or not updated_imports.strip():
+        return original_code  # Return original code if no imports found
+
+    try:
+        # Regular expression pattern to match import statements
+        import_pattern = r'import\s+{[^}]+}\s+from\s+[\'"][^\'"]+[\'"];\n*'
+
+        # Find and remove existing imports
+        existing_imports = re.findall(import_pattern, original_code)
+        original_code = re.sub(import_pattern, '', original_code)
+
+        # Prepend new imports before the remaining code
+        updated_code = '\n'.join([import_line.strip() for import_line in updated_imports.split('\n')]) + '\n\n' + original_code.strip()
+
+        return updated_code
+    except Exception as e:
+        return f"Error: {e}"
+
+# Context retrival from file
+def fetch_imported_code(import_statement_string, base_path):
+    # Regular expression pattern to match user-defined import statements
+    user_import_statement_pattern = r'import\s+{([^}]+)}\s+from\s+[\'"](\.\./[^\'"]+)[\'"];'
+
+    # Find all user-defined import statements using regex
+    user_import_statements = re.findall(user_import_statement_pattern, import_statement_string)
+    user_import_statements = [(import_symbols.strip(), import_path.strip()) for import_symbols, import_path in user_import_statements]
+    
+    imported_code = []
+
+    # Iterate through user-defined import statements
+    for import_symbols, import_path in user_import_statements:
+        # Construct the file path based on the base path and the import path
+        file_path = os.path.abspath(os.path.join(base_path, import_path + '.ts'))
+
+        # Check if the file exists
+        if not os.path.exists(file_path):
+            print(f"File not found: {file_path}")
+            continue
+
+        # Read the content of the file
+        with open(file_path, 'r') as file:
+            file_content = file.read()
+
+            # Split import symbols into individual imports
+            import_symbols_list = [symbol.strip() for symbol in import_symbols.split(',')]
+
+            # Iterate through individual imports
+            for symbol in import_symbols_list:
+                # Check if the imported item is a class or a function
+                is_class = re.search(rf'\bclass\s+{symbol}\b', file_content)
+                is_function = re.search(rf'\bfunction\s+{symbol}\b', file_content)
+
+                # Extract the code of the imported item
+                imported_item_code = None
+                if is_class:
+                    class_code_pattern = rf'\bexport\s+class\s+{symbol}\b[\s\S]*?(?=export\s+class|\Z)'
+                    class_code_match = re.search(class_code_pattern, file_content)
+                    if class_code_match:
+                        imported_item_code = class_code_match.group(0).strip()
+                elif is_function:
+                    function_code_pattern = rf'\bexport\s+function\s+{symbol}\b[\s\S]*?(?=export\s+function|\Z)'
+                    function_code_match = re.search(function_code_pattern, file_content)
+                    if function_code_match:
+                        imported_item_code = function_code_match.group(0).strip()
+
+                if imported_item_code:
+                    imported_code.append(imported_item_code)
+                else:
+                    print(f"Class or function '{symbol}' not found in file: {file_path}")
+
+    # Join all the imported code strings into a single string
+    all_imported_code = '\n\n'.join(imported_code)
+
+    return all_imported_code
+
 # for gettting code of happy path & negative cases scenarios
 def generate_tests(file_name):
     try:
         with open(file_name, 'r', encoding='utf-8') as file:
             file_content = file.read()
 
             file_size = os.path.getsize(file_name)
@@ -291,20 +442,23 @@
             function_names = extract_function_names(file_content)
             total_line=[]
             
 
             # Prompt user for private key
             private_key = input("Enter your private key: ")
             
-            if private_key == "gc_spgrXSnfZqYSVqqhQiVjlYApSQofFXIUtF":
+            if private_key == "gc_local":
 
             
                 function_names = extract_function_names(file_content)
                 # print("Function Names:", function_names)
 
+                import_lines=extract_imports_from_file(file_name)
+                new_imports = extract_user_defined_imports(import_lines)
+                # print(new_imports)
                 
                 # Extract function code for each function name
                 for function_name in function_names:
                     function_code,lines = extract_function_code(file_content, function_name)
                     lines=lines-1
                     # print("\nFunction:", function_name)
                     # print("Code:\n", function_code)
@@ -313,14 +467,15 @@
 
 
              
 
                 # Check if the provided private key matches the expected key
                 if file_size >= 20000:
                     print("Function Names:", function_names)
+
                     # Extract function code for each function name
                     for function_name in function_names:
                         function_code = extract_function_code(file_content, function_name)
                         # print("\nFunction:", function_name)
                         # print("Code:\n", function_code)
 
                         behaviour_type = [{"type": "HappyPath", "number": 6}, {"type": "EdgeCase", "number":18 }, {"type": "NegativeCase", "number": 8}]
@@ -328,127 +483,110 @@
                         explain_response = explain_api_request(function_code)
 
                         for obj in behaviour_type:
                             
                             type = obj['type']
                             print(f"Generating tests on '{type}' scenarios for '{function_name}' function")
                             api_response = open_api_request(function_code, obj['type'], obj['number'], explain_response)
-                            test_response = generate_api_request(function_code, api_response, obj['type'], obj['number'])
+
+                            directory_path = os.path.dirname(file_name)
+                            test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
+                            function_test_folder_path = os.path.join(test_folder_path, function_name)
+                            output_file_path = os.path.join(function_test_folder_path, f'test_{function_name}_{type}.spec.ts')
+
+                            retrived_context=fetch_imported_code(new_imports,function_test_folder_path)
+                            # print(retrived_context)
+                                
+
+                            test_response = generate_api_request(function_code, api_response, obj['type'], obj['number'],import_lines,retrived_context)
                             test_response1 = generate_api_request1(function_code, test_response,obj['type'], obj['number'])
         
                         
-                            if test_response:
+                            if test_response1:
                                 directory_path = os.path.dirname(file_name)
                                 test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                                 os.makedirs(test_folder_path,exist_ok=True)
                                 function_test_folder_path = os.path.join(test_folder_path, function_name)
                                 os.makedirs(function_test_folder_path,exist_ok=True)
                                 
                                 # Write API response (test cases) to a test.py file in the same directory
                                 output_file_path = os.path.join(function_test_folder_path, f'test_{function_name}_{type}.spec.ts')
                                 
-                                if (test_response1.startswith("```typescript") or test_response1.startswith("```javascript") or test_response1.startswith("```ts") or test_response1.startswith("```")):
-        
-                                    start_markers = ["```typescript", "```javascript", "```", "ts"]
-                                    end_marker = "```"
-                                    start_index = -1
-                                    end_index = -1
+                                pattern1 = r'(?:\s*```(?:typescript|javascript|ts)?\n)?(.*?)(?:```|$)'
+                                pattern2 = r'```(?:typescript|javascript|ts)?\n(.*?)```|\b(?:typescript|javascript|ts)?\n(.*?)(?=$|```)'
+                                combined_pattern = f"{pattern1}|{pattern2}"
 
 
-                                    end_index = test_response1.rfind(end_marker)
-
-                                    for marker in start_markers:
-                                        start_index = test_response1.find(marker)
-                                        if start_index != -1:
-                                            break
-        
-                                    if start_index != -1:
-                                        start_index = min(filter(lambda x: x != -1, [test_response1.find(marker) for marker in start_markers]))
-                                        # Extract content between start and end markers
-                                        if end_index != -1:
-                                            start_marker_length = len(start_markers[start_index])
-                                            content = test_response1[start_index + start_marker_length:end_index].strip()
-                                        else:
-                                            content = test_response1[start_index:].strip()
-                                    else:
-                                        content = test_response1
+                                match = re.search(combined_pattern, test_response1, re.DOTALL)
+
+                                if match:
+                                    content = match.group(1) or match.group(2) or match.group(3) or match.group(4)
+                                    content=content.strip()
                                 else:
-                                    content = test_response1
+                                    content=test_response1
+                                updated_code=replace_string_imports(content, new_imports)
                                 with open(output_file_path, 'w') as output_file:
-                                    output_file.write(content)
+                                    output_file.write(updated_code)
                                     print(f"Test cases for '{function_name}' written to {output_file_path}")
                             else:
                                 print(f"Failed to fetch test cases from API for function '{function_name}'.")        
                             
                     total_lines=sum(total_line) 
                  
                     total_functions=len(function_names)
                 
-                    update_client_1(private_key, total_lines,total_functions)
+                    # update_client_1(private_key, total_lines,total_functions)
                 else:
                     explain_response = explain_api_request(file_content)
                     File_name=extract_filename(file_name)
+                    
                     behaviour_type = [{"type": "HappyPath", "number": 6}, {"type": "EdgeCase", "number":12 }, {"type": "NegativeCase", "number": 8}]
                     for obj in behaviour_type:
                         type = obj['type']
 
                         print(f"Generating tests on '{type}' scenarios for file : {file_name} ")
                         api_response = open_api_request(file_content, obj['type'], obj['number'], explain_response)
                     
-                        test_response = generate_api_request(file_content, api_response, obj['type'], obj['number'])
+                        directory_path = os.path.dirname(file_name)
+                        test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
+                        output_file_path = os.path.join(test_folder_path, f'test_{File_name}_{type}.spec.ts')
+
+                        retrived_context=fetch_imported_code(new_imports,test_folder_path)
+                        # print(retrived_context)
+
+                        test_response = generate_api_request(file_content, api_response, obj['type'], obj['number'],import_lines,retrived_context)
                         
                         test_response1 = generate_api_request1(file_content, test_response,obj['type'], obj['number'])  
                         if test_response1:
 
                             directory_path = os.path.dirname(file_name)
                             test_folder_path = os.path.join(directory_path, 'gocodeo_tests')
                             os.makedirs(test_folder_path,exist_ok=True)
                             
                             # Write API response (test cases) to a test.py file in the same directory
                             output_file_path = os.path.join(test_folder_path, f'test_{File_name}_{type}.spec.ts')
                             
-                            if (test_response1.startswith("```typescript") or test_response1.startswith("```javascript") or test_response1.startswith("```ts") or test_response1.startswith("```")):
-    
-                                start_markers = ["```typescript", "```javascript", "```", "ts"]
-                                end_marker = "```"
-                                start_index = -1
-                                end_index = -1
-
-                                end_index = test_response1.rfind(end_marker)
-
-                                for marker in start_markers:
-                                    start_index = test_response1.find(marker)
-                                    if start_index != -1:
-                                        break
-
-                                if start_index != -1:
-                                    # Find the minimum start index
-                                    start_index = min(filter(lambda x: x != -1, [test_response1.find(marker) for marker in start_markers]))
-                                
-                                    # Extract content between start and end markers if end marker is found
-                                    if end_index != -1:
-                                        start_marker_length = len(start_markers[start_index])
-                                        content = test_response1[start_index + start_marker_length:end_index].strip()
-                                    else:
-                                        # If end marker is not found, trim content from the first start marker found
-                                        content = test_response1[start_index:].strip()
-                                else:
-                                    content = test_response1
+                            pattern1 = r'(?:\s*```(?:typescript|javascript|ts)?\n)?(.*?)(?:```|$)'
+                            pattern2 = r'```(?:typescript|javascript|ts)?\n(.*?)```|\b(?:typescript|javascript|ts)?\n(.*?)(?=$|```)'
+                            combined_pattern = f"{pattern1}|{pattern2}"
+
+
+                            match = re.search(combined_pattern, test_response1, re.DOTALL)
+
+                            if match:
+                                content = match.group(1) or match.group(2) or match.group(3) or match.group(4)
+                                content=content.strip()
                             else:
-                                content = test_response1
+                                content=test_response1
+                            updated_code=replace_string_imports(content, new_imports)
                             with open(output_file_path, 'w') as output_file:
-                                output_file.write(content)
+                                output_file.write(updated_code)
                                 print(f"Test cases on '{type}' scenarios written to file:{output_file_path}")
                         else:
                             print(f"Failed to fetch test cases from API for function '{function_name}'.")        
-                    total_lines=sum(total_line) 
-                 
-                    total_functions=len(function_names)
-                
-                    update_client_1(private_key, total_lines,total_functions)
             else:
                 print("Invalid private key. Access denied.")
 
     except FileNotFoundError:
         print(f"Error: File '{file_name}' not found.")
 
 def generate_tests_cli():
```

### Comparing `gocodeo-0.0.9/gocodeo.egg-info/PKG-INFO` & `gocodeo-0.0.9.1/gocodeo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: gocodeo
-Version: 0.0.9
+Version: 0.0.9.1
 Summary: A package to generate unit tests for a file
 Author: GoCodeo AI
 Description-Content-Type: text/markdown
 Requires-Dist: vertexai
 Requires-Dist: requests
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: google-auth
 Requires-Dist: python-dotenv
+Requires-Dist: google-cloud-storage
+Requires-Dist: pymongo
 
         gocodeo is a  package that provides a command-line interface (CLI) to generate unit tests for files. 
         To use gocodeo , simply run the command:
         
             gocodeo generate <file_path>
             
         For example:
```

### Comparing `gocodeo-0.0.9/setup.py` & `gocodeo-0.0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gocodeo',
-    version='0.0.9',
+    version='0.0.9.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'gocodeo = gocodeo.generator:generate_tests_cli'
+            'gocodeo-generate = gocodeo.generator:generate_tests_cli',
+            'gocodeo-train = gocodeo.train:start'
+        
         ]
     },
     install_requires= ['vertexai',
                        'requests',
                        'google-cloud-aiplatform',
                        'google-auth',
-                       'python-dotenv'],
+                       'python-dotenv',
+                       'google-cloud-storage',
+                       'pymongo',
+                       ],
 
     author='GoCodeo AI',
     description='A package to generate unit tests for a file',
     long_description='''\
         gocodeo is a  package that provides a command-line interface (CLI) to generate unit tests for files. 
         To use gocodeo , simply run the command:
```

