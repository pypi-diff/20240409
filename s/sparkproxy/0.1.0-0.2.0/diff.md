# Comparing `tmp/sparkproxy-0.1.0.tar.gz` & `tmp/sparkproxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.1.0.tar", last modified: Tue Apr  9 00:29:20 2024, max compression
+gzip compressed data, was "sparkproxy-0.2.0.tar", last modified: Tue Apr  9 03:20:31 2024, max compression
```

## Comparing `sparkproxy-0.1.0.tar` & `sparkproxy-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.596260 sparkproxy-0.1.0/
--rw-r--r--   0 huanghy    (501) staff       (20)     1104 2024-04-08 13:44:36.000000 sparkproxy-0.1.0/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1161 2024-04-09 00:29:20.596143 sparkproxy-0.1.0/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     1641 2024-04-09 00:00:54.000000 sparkproxy-0.1.0/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-09 00:29:20.596303 sparkproxy-0.1.0/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2393 2024-04-08 17:01:43.000000 sparkproxy-0.1.0/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.592912 sparkproxy-0.1.0/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-08 17:01:20.000000 sparkproxy-0.1.0/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2716 2024-04-08 17:00:19.000000 sparkproxy-0.1.0/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.1.0/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.1.0/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.594380 sparkproxy-0.1.0/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.1.0/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.1.0/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.595328 sparkproxy-0.1.0/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.1.0/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.1.0/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.1.0/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.1.0/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.1.0/sparkproxy/http/response.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.595580 sparkproxy-0.1.0/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.1.0/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.595794 sparkproxy-0.1.0/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.1.0/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5101 2024-04-08 17:00:19.000000 sparkproxy-0.1.0/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 00:29:20.593777 sparkproxy-0.1.0/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1161 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      659 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       55 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-09 00:29:20.000000 sparkproxy-0.1.0/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.384274 sparkproxy-0.2.0/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.2.0/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1130 2024-04-09 03:20:31.384146 sparkproxy-0.2.0/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     3719 2024-04-09 03:20:05.000000 sparkproxy-0.2.0/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-09 03:20:31.384339 sparkproxy-0.2.0/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.2.0/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.380857 sparkproxy-0.2.0/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-09 03:18:58.000000 sparkproxy-0.2.0/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2877 2024-04-09 03:14:04.000000 sparkproxy-0.2.0/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.2.0/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.382286 sparkproxy-0.2.0/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.2.0/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.2.0/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383243 sparkproxy-0.2.0/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.2.0/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.2.0/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1555 2024-04-09 02:53:50.000000 sparkproxy-0.2.0/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383576 sparkproxy-0.2.0/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.383802 sparkproxy-0.2.0/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.2.0/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5916 2024-04-09 03:16:16.000000 sparkproxy-0.2.0/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-09 03:20:31.381702 sparkproxy-0.2.0/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1130 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       55 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-09 03:20:31.000000 sparkproxy-0.2.0/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.1.0/LICENSE` & `sparkproxy-0.2.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2014 Sparkproxy, Ltd.<sdk@sparkproxy.com>
+Copyright (c) 2024 yungoo
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `sparkproxy-0.1.0/PKG-INFO` & `sparkproxy-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.1.0
-Summary: Sparkproxy OpenApi SDK
-Home-page: https://github.com/yungoo/spark-proxy/sdk/spark-sdk-python
+Version: 0.2.0
+Summary: Spark proxy OpenApi SDK
+Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,10 +23,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 License-File: LICENSE
 
 see:
-https://github.com/yungoo/spark-proxy/sdk/spark-sdk-python
+https://github.com/yungoo/spark-sdk-python
```

### Comparing `sparkproxy-0.1.0/setup.py` & `sparkproxy-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
 setup(
     name='sparkproxy',
     version=find_version("sparkproxy/__init__.py"),
-    description='Sparkproxy OpenApi SDK',
-    long_description='see:\nhttps://github.com/yungoo/spark-proxy/sdk/spark-sdk-python\n',
+    description='Spark proxy OpenApi SDK',
+    long_description='see:\nhttps://github.com/yungoo/spark-sdk-python\n',
     author='Spark Proxy Co., Ltd.',
     author_email='sdk@sparkproxy.com',
     maintainer_email='support@sparkproxy.com',
     license='MIT',
-    url='https://github.com/yungoo/spark-proxy/sdk/spark-sdk-python',
+    url='https://github.com/yungoo/spark-sdk-python',
     platforms='any',
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `sparkproxy-0.1.0/sparkproxy/auth.py` & `sparkproxy-0.2.0/sparkproxy/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # -*- coding: utf-8 -*-
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding
+import time
+
+from cryptography.exceptions import InvalidSignature
+
+from sparkproxy.rsa import rsa_load_pem_private_key, rsa_sign, rsa_decrypt, rsa_verify, rsa_load_pem_public_key
 
 
 class Auth(object):
     """安全机制类
 
     该类主要内容是凭证的签名接口的实现，以及回调验证。
 
     Attributes:
         __supplier_no: 供应商编号，双方协商获得
         __private_key: RSA私匙，公钥交给SparkProxy，调用接口时使用私钥签名，sparkproxy使用公钥验签
+        __public_key: RSA公钥，SparkProxy提供的公钥
     """
 
-    def __init__(self, supplier_no, private_key, disable_timestamp_signature=None):
+    def __init__(self, supplier_no, private_key, public_key = None):
         """初始化Auth类"""
         self.__checkKey(supplier_no, private_key)
         self.__supplier_no = supplier_no
-        self.__private_key = self.__load_rsa_private_key(private_key)
-        self.disable_timestamp_signature = disable_timestamp_signature
-
-    @staticmethod
-    def __load_rsa_private_key(private_key):
-        private_key = serialization.load_pem_private_key(
-            private_key.encode(),
-            password=None,
-            backend=default_backend()
-        )
-        return private_key
+        self.__private_key = rsa_load_pem_private_key(private_key)
+        if public_key is not None:
+            self.__public_key = rsa_load_pem_public_key(public_key)
 
     def get_supplier_no(self):
         return self.__supplier_no
 
     def get_private_key(self):
         return self.__private_key
 
@@ -43,39 +38,47 @@
             req:         待签名请求的参数
         Returns:
             签名凭证
         """
         message = 'supplierNo={0}&timestamp={1}'.format(req["supplierNo"], req["timestamp"])
 
         # 使用私钥对哈希值进行签名
-        signature = self.__private_key.sign(
-            message.encode(),
-            padding.PKCS1v15(),
-            hashes.SHA256()
-        )
-        return signature.hex()
+        return rsa_sign(message, self.__private_key)
 
     @staticmethod
     def __checkKey(access_key, secret_key):
         if not (access_key and secret_key):
             raise ValueError('invalid key')
 
+    def decrypt(self, encrypt_msg):
+        return rsa_decrypt(encrypt_msg, self.__private_key)
+
     def verify_callback(
             self,
-            origin_authorization,
-            url,
-            body,
-            content_type='application/x-www-form-urlencoded'):
+            supplier_no, sign, req_id, timestamp):
         """回调验证
 
         Args:
-            origin_authorization: 回调时请求Header中的Authorization字段
-            url:                  回调请求的url
-            body:                 回调请求的body
-            content_type:         回调请求body的Content-Type
+            supplier_no:        回调请求中供应商NO
+            sign:              回调请求的签名
+            req_id:            回调请求的请求ID
+            timestamp:         回调请求的时间戳
 
         Returns:
-            返回true表示验证成功，返回false表示验证失败
+            返回ValueError异常表示验证失败
         """
-        token = self.token_of_request(url, body, content_type)
-        authorization = 'QBox {0}'.format(token)
-        return origin_authorization == authorization
+        if not supplier_no:
+            raise ValueError(f"签名参数supplierNo未提供。reqId: {req_id}")
+        if not sign:
+            raise ValueError(f"签名参数sign未提供。reqId: {req_id}")
+
+        if time.time() - timestamp > 600:
+            raise ValueError(f"签名已过期。reqId: {req_id}")
+
+        str_to_sign = f"supplierNo={supplier_no}&timestamp={timestamp}"
+
+        try:
+            rsa_verify(sign, str_to_sign, self.__public_key)
+        except InvalidSignature:
+            raise ValueError(f"签名校验错误。reqId: {req_id}")
+        except Exception as e:
+            raise ValueError(f"签名验证过程中出现问题: {e}")
```

### Comparing `sparkproxy-0.1.0/sparkproxy/compat.py` & `sparkproxy-0.2.0/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/config.py` & `sparkproxy-0.2.0/sparkproxy/config.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/__init__.py` & `sparkproxy-0.2.0/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/client.py` & `sparkproxy-0.2.0/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/middleware/base.py` & `sparkproxy-0.2.0/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.2.0/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.2.0/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/http/response.py` & `sparkproxy-0.2.0/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.1.0/sparkproxy/services/openapi/client.py` & `sparkproxy-0.2.0/sparkproxy/services/openapi/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,26 @@
     def __init__(self, auth, host=None):
         self.auth = auth
         if host is None:
             self.host = config.get_default("default_api_host")
         else:
             self.host = host
 
-    def get_product_stock(self, proxy_type, country_code = None, city_code = None):
+    def get_product_stock(self, proxy_type, country_code=None, city_code=None):
         """获取商品库存
 
         列出当前所有在售的商品及其库存信息。
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回服务组列表[<product1>, <product1>, ...]，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
-        return self.__post('GetProductStock', {"proxyType": proxy_type, "countryCode": country_code, "cityCode": city_code})
+        return self.__post('GetProductStock',
+                           {"proxyType": proxy_type, "countryCode": country_code, "cityCode": city_code})
 
     def create_proxy(self, req_order_no, sku, amount, duration, unit, country_code, city_code):
         """创建代理实例
 
         创建新代理实例，返回订单信息
 
         Args:
@@ -61,30 +62,37 @@
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
         return self.__post('CreateProxy', {"reqOrderNo": req_order_no, "sku": sku, "amount": amount,
-                                           "duration": duration, "unit": unit, "countryCode": country_code, "cityCode": city_code})
+                                           "duration": duration, "unit": unit, "countryCode": country_code,
+                                           "cityCode": city_code})
 
     def renew_proxy(self, req_order_no, instances):
         """续费代理实例
 
         续费新代理实例，返回新订单信息
 
         Args:
             - args:  订单&实例描述
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
-        return self.__post('RenewProxy', {"reqOrderNo": req_order_no, "instances": instances})
+        ret, info = self.__post('RenewProxy', {"reqOrderNo": req_order_no, "instances": instances})
+        if ret is not None:
+            for ipInfo in ret['data']['ipInfo']:
+                password = ipInfo["password"]
+                if len(password) > 0:
+                    ipInfo["password"] = self.auth.decrypt(password)
+        return ret, info
 
     def delete_proxy(self, req_order_no, instances):
         """删除代理实例
 
         删除代理实例，删除即时生效
 
         Args:
@@ -106,30 +114,41 @@
             - req_order_no:  请求方订单ID
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
-        return self.__post('GetOrder', {"reqOrderNo": req_order_no})
+        ret, info = self.__post('GetOrder', {"reqOrderNo": req_order_no})
+        if ret is not None:
+            for ipInfo in ret['data']['ipInfo']:
+                password = ipInfo["password"]
+                if len(password) > 0:
+                    ipInfo["password"] = self.auth.decrypt(password)
+        return ret, info
 
     def get_instance(self, instance_id):
         """获取订单信息
 
         获取订单信息
 
         Args:
             - instance_id:  实例ID
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
-        return self.__post('GetInstance', {"instanceId": instance_id})
+        ret, info = self.__post('GetInstance', {"instanceId": instance_id})
+        if ret is not None:
+            password = ret['data']['IpInfo']["password"]
+            if len(password) > 0:
+                ret['data']['IpInfo']["password"] = self.auth.decrypt(password)
+        return ret, info
 
     def __request_params(self, method, args):
         base_params = {
             "method": method,
             "version": "2024-04-08",
             "reqId": str(uuid.uuid4()),
             "timestamp": int(time.time()),
```

### Comparing `sparkproxy-0.1.0/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.2.0/sparkproxy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.1.0
-Summary: Sparkproxy OpenApi SDK
-Home-page: https://github.com/yungoo/spark-proxy/sdk/spark-sdk-python
+Version: 0.2.0
+Summary: Spark proxy OpenApi SDK
+Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,10 +23,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 License-File: LICENSE
 
 see:
-https://github.com/yungoo/spark-proxy/sdk/spark-sdk-python
+https://github.com/yungoo/spark-sdk-python
```

### Comparing `sparkproxy-0.1.0/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.2.0/sparkproxy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 sparkproxy/__init__.py
 sparkproxy/auth.py
 sparkproxy/compat.py
 sparkproxy/config.py
+sparkproxy/rsa.py
 sparkproxy.egg-info/PKG-INFO
 sparkproxy.egg-info/SOURCES.txt
 sparkproxy.egg-info/dependency_links.txt
 sparkproxy.egg-info/entry_points.txt
 sparkproxy.egg-info/requires.txt
 sparkproxy.egg-info/top_level.txt
 sparkproxy/http/__init__.py
```

