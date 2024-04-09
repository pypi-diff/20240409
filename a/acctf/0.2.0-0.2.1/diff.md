# Comparing `tmp/acctf-0.2.0.tar.gz` & `tmp/acctf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acctf-0.2.0.tar", last modified: Sun Mar 24 07:47:45 2024, max compression
+gzip compressed data, was "acctf-0.2.1.tar", last modified: Tue Apr  9 13:00:35 2024, max compression
```

## Comparing `acctf-0.2.0.tar` & `acctf-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-01-06 03:12:47.000000 acctf-0.2.0/LICENSE
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-03-24 07:47:45.657934 acctf-0.2.0/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3085 2024-03-24 07:39:30.000000 acctf-0.2.0/README.md
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      662 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/bank/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      620 2024-03-17 12:13:36.000000 acctf-0.2.0/acctf/bank/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/bank/mizuho/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     5523 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/bank/mizuho/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:36.000000 acctf-0.2.0/acctf/bank/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/bank/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     7888 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/bank/sbi/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/other/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/other/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/other/wealthnavi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2120 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/other/wealthnavi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/other/wealthnavi/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/securities/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      739 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/securities/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/securities/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/securities/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3881 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/securities/sbi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/securities/sbi/utils.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf/utils/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:32:41.000000 acctf-0.2.0/acctf/utils/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:36.000000 acctf-0.2.0/acctf/utils/format.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-03-24 07:39:30.000000 acctf-0.2.0/acctf/utils/totp.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-03-24 07:47:45.657934 acctf-0.2.0/acctf.egg-info/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-03-24 07:47:45.000000 acctf-0.2.0/acctf.egg-info/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-03-24 07:47:45.000000 acctf-0.2.0/acctf.egg-info/SOURCES.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-03-24 07:47:45.000000 acctf-0.2.0/acctf.egg-info/dependency_links.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-03-24 07:47:45.000000 acctf-0.2.0/acctf.egg-info/requires.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-03-24 07:47:45.000000 acctf-0.2.0/acctf.egg-info/top_level.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-03-24 07:47:45.657934 acctf-0.2.0/setup.cfg
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      940 2024-03-24 07:41:27.000000 acctf-0.2.0/setup.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.2.1/LICENSE
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-04-09 13:00:35.975093 acctf-0.2.1/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3085 2024-04-06 13:38:11.000000 acctf-0.2.1/README.md
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      819 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      680 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/mizuho/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     5583 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/mizuho/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.2.1/acctf/bank/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/bank/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     7948 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/bank/sbi/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/other/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/other/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/other/wealthnavi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2180 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/other/wealthnavi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/other/wealthnavi/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/securities/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      799 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/securities/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/securities/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.965093 acctf-0.2.1/acctf/securities/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3941 2024-04-09 12:55:27.000000 acctf-0.2.1/acctf/securities/sbi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/securities/sbi/utils.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/acctf/utils/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.2.1/acctf/utils/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.2.1/acctf/utils/format.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.2.1/acctf/utils/totp.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-09 13:00:35.975093 acctf-0.2.1/acctf.egg-info/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3742 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/SOURCES.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/dependency_links.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/requires.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-04-09 13:00:35.000000 acctf-0.2.1/acctf.egg-info/top_level.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-09 13:00:35.975093 acctf-0.2.1/setup.cfg
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      940 2024-04-09 12:57:35.000000 acctf-0.2.1/setup.py
```

### Comparing `acctf-0.2.0/LICENSE` & `acctf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acctf-0.2.0/PKG-INFO` & `acctf-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.2.0
+Version: 0.2.1
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.2.0/README.md` & `acctf-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `acctf-0.2.0/acctf/__init__.py` & `acctf-0.2.1/acctf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from abc import abstractmethod
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.webdriver import WebDriver
 
 class Base:
     driver: WebDriver
 
-    def __init__(self):
+    def __init__(self, executable_path: str=None):
         options = Options()
         options.add_argument('--headless')
-        self.driver = webdriver.Chrome(options=options)
+        service = Service(executable_path=executable_path)
+        self.driver = webdriver.Chrome(options=options, service=service)
         self.driver.implicitly_wait(10)
 
     @abstractmethod
     def login(self, user_id: str, password: str, totp: str | None = None):
         raise NotImplementedError()
 
     @abstractmethod
```

### Comparing `acctf-0.2.0/acctf/bank/mizuho/__init__.py` & `acctf-0.2.1/acctf/bank/mizuho/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from selenium.webdriver.support.select import Select
 
 from acctf.bank import Bank, Balance, Transaction
 from acctf.bank.model import str_to_deposit_type, CurrencyType
 
 
 class Mizuho(Bank, ABC):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, executable_path: str = None):
+        super().__init__(executable_path=executable_path)
         self.driver.get('https://web.ib.mizuhobank.co.jp/servlet/LOGBNK0000000B.do')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.NAME, 'txbCustNo')
         user_id_elem.send_keys(user_id)
         self.driver.find_element(By.NAME, 'N00000-next').click()
```

### Comparing `acctf-0.2.0/acctf/bank/model.py` & `acctf-0.2.1/acctf/bank/model.py`

 * *Files identical despite different names*

### Comparing `acctf-0.2.0/acctf/bank/sbi/__init__.py` & `acctf-0.2.1/acctf/bank/sbi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from acctf.utils.format import format_displayed_money
 
 
 class SBI(Bank, ABC):
     account_number = ""
     branch_name = ""
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, executable_path: str = None):
+        super().__init__(executable_path=executable_path)
         self.driver.get('https://www.netbk.co.jp/contents/pages/wpl010101/i010101CT/DI01010210')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.ID, 'userNameNewLogin')
         user_id_elem.send_keys(user_id)
```

### Comparing `acctf-0.2.0/acctf/other/wealthnavi/__init__.py` & `acctf-0.2.1/acctf/other/wealthnavi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from acctf import Base
 from acctf.other.wealthnavi.model import Asset
 from acctf.utils.format import format_displayed_money
 from acctf.utils.totp import get_code
 
 
 class WealthNavi(Base):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, executable_path: str = None):
+        super().__init__(executable_path=executable_path)
         self.driver.get('https://invest.wealthnavi.com/login')
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.ID, 'username')
         user_id_elem.send_keys(user_id)
 
         user_pw_elem = self.driver.find_element(By.ID, 'password')
```

### Comparing `acctf-0.2.0/acctf/securities/__init__.py` & `acctf-0.2.1/acctf/securities/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABCMeta, abstractmethod
 
 from acctf import Base
 from acctf.securities.model import Value
 
 
 class Securities(Base, metaclass=ABCMeta):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, executable_path: str = None):
+        super().__init__(executable_path=executable_path)
 
     @abstractmethod
     def get_stock_specific(self) -> list[Value]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_stock_specific_us(self) -> list[Value]:
```

### Comparing `acctf-0.2.0/acctf/securities/sbi/__init__.py` & `acctf-0.2.1/acctf/securities/sbi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class SBI(Securities, ABC):
     _df_fund_specific: pd.DataFrame = None
     _df_fund_nisa_accum: pd.DataFrame = None
     _df_fund_old_nisa_accum: pd.DataFrame = None
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, executable_path: str = None):
+        super().__init__(executable_path=executable_path)
         self.driver.get('https://www.sbisec.co.jp/ETGate')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
         user_id_elem = self.driver.find_element(By.NAME, 'user_id')
         user_id_elem.send_keys(user_id)
         user_pw_elem = self.driver.find_element(By.NAME, 'user_password')
```

### Comparing `acctf-0.2.0/acctf/securities/sbi/utils.py` & `acctf-0.2.1/acctf/securities/sbi/utils.py`

 * *Files identical despite different names*

### Comparing `acctf-0.2.0/acctf.egg-info/PKG-INFO` & `acctf-0.2.1/acctf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.2.0
+Version: 0.2.1
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.2.0/acctf.egg-info/SOURCES.txt` & `acctf-0.2.1/acctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acctf-0.2.0/setup.py` & `acctf-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="acctf",
-    version="0.2.0",
+    version="0.2.1",
     description="library that scrapes the data from an account such as securities, bank",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hirano00o/acctf",
     author="hirano00o",
     classifiers=[
         "Programming Language :: Python :: 3",
```

