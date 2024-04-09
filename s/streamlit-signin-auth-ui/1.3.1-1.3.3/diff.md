# Comparing `tmp/streamlit_signin_auth_ui-1.3.1.tar.gz` & `tmp/streamlit_signin_auth_ui-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_signin_auth_ui-1.3.1.tar", last modified: Fri Mar 29 12:28:21 2024, max compression
+gzip compressed data, was "streamlit_signin_auth_ui-1.3.3.tar", last modified: Tue Apr  9 17:21:44 2024, max compression
```

## Comparing `streamlit_signin_auth_ui-1.3.1.tar` & `streamlit_signin_auth_ui-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 12:28:21.322330 streamlit_signin_auth_ui-1.3.1/
--rw-rw-rw-   0        0        0     1074 2024-03-18 19:49:12.000000 streamlit_signin_auth_ui-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7210 2024-03-29 12:28:21.311333 streamlit_signin_auth_ui-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6149 2024-03-29 12:27:14.000000 streamlit_signin_auth_ui-1.3.1/README.md
--rw-rw-rw-   0        0        0     1059 2024-03-29 12:26:13.000000 streamlit_signin_auth_ui-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 12:28:21.324329 streamlit_signin_auth_ui-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 12:28:21.118335 streamlit_signin_auth_ui-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 12:28:21.176329 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/
--rw-rw-rw-   0        0        0        0 2024-03-02 14:48:05.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/__init__.py
--rw-rw-rw-   0        0        0     6216 2024-03-24 19:27:18.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/utils.py
--rw-rw-rw-   0        0        0    13697 2024-03-20 23:09:05.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/widgets.py
-drwxrwxrwx   0        0        0        0 2024-03-29 12:28:21.308331 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/
--rw-rw-rw-   0        0        0     7210 2024-03-29 12:28:21.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2024-03-29 12:28:21.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 12:28:21.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-03-29 12:28:21.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-03-29 12:28:21.000000 streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 17:21:44.454764 streamlit_signin_auth_ui-1.3.3/
+-rw-rw-rw-   0        0        0     1074 2024-03-18 19:49:12.000000 streamlit_signin_auth_ui-1.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     7225 2024-04-09 17:21:44.451766 streamlit_signin_auth_ui-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6164 2024-04-09 17:20:13.000000 streamlit_signin_auth_ui-1.3.3/README.md
+-rw-rw-rw-   0        0        0     1059 2024-04-09 17:19:41.000000 streamlit_signin_auth_ui-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:21:44.454764 streamlit_signin_auth_ui-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 17:21:44.368183 streamlit_signin_auth_ui-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 17:21:44.404752 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/
+-rw-rw-rw-   0        0        0        0 2024-03-02 14:48:05.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/__init__.py
+-rw-rw-rw-   0        0        0     6216 2024-03-24 19:27:18.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/utils.py
+-rw-rw-rw-   0        0        0    13723 2024-04-09 17:18:33.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:21:44.447764 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/
+-rw-rw-rw-   0        0        0     7225 2024-04-09 17:21:44.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-04-09 17:21:44.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:21:44.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-09 17:21:44.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-09 17:21:44.000000 streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/top_level.txt
```

### Comparing `streamlit_signin_auth_ui-1.3.1/LICENSE.txt` & `streamlit_signin_auth_ui-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_signin_auth_ui-1.3.1/PKG-INFO` & `streamlit_signin_auth_ui-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: streamlit_signin_auth_ui
-Version: 1.3.1
-Summary: Login/Sign-up page with Streamlit,the user's data are stored in a Google Sheets file as database,also the lables of widgets are in frensh language.
+Version: 1.3.3
+Summary: Login/Sign-up page with Streamlit,the user's data are stored in a Google Sheets file as database,also the lables of widgets are in Frensh language.
 Author-email: TAOUFIQ ABDESSAMAD <samadtaoufik@gmail.com>
 Project-URL: Homepage, https://github.com/GitSamad88/streamlit-signin-ui
 Project-URL: Issues, https://github.com/GitSamad88/streamlit-signin-ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,15 +18,15 @@
 Requires-Dist: oauth2client>=4.1.3
 Requires-Dist: google_api_python_client>=2.119.0
 Requires-Dist: argon2-cffi
 Requires-Dist: streamlit_lottie
 Requires-Dist: streamlit_option_menu
 Requires-Dist: streamlit-cookies-manager-hotpatched==0.2.1
 
-# Login page with Streamlit (Lables in frensh language)
+# Login page with Streamlit (Lables of widgets are in Frensh language)
 
 # Update of https://github.com/GitSamad88
 
 
 
 #Version 2024-3-29 : this version is an update of streamlit-login-auth-ui-23
 
@@ -160,11 +160,11 @@
 Generated in the sidebar only if the user is logged in, allows users to logout. \
 
 <img width="919" alt="loggin" src="https://github.com/GitSamad88/streamlit-signin-ui/assets/110288424/034ff583-0e81-437a-a5ae-33ca7e6f521f">
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
-v1.3.1
+v1.3.3
 
 ## License
 [MIT](https://github.com/GitSamad88/streamlit_signin_ui/blob/main/LICENSE)
```

### Comparing `streamlit_signin_auth_ui-1.3.1/README.md` & `streamlit_signin_auth_ui-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Login page with Streamlit (Lables in frensh language)
+# Login page with Streamlit (Lables of widgets are in Frensh language)
 
 # Update of https://github.com/GitSamad88
 
 
 
 #Version 2024-3-29 : this version is an update of streamlit-login-auth-ui-23
 
@@ -136,11 +136,11 @@
 Generated in the sidebar only if the user is logged in, allows users to logout. \
 
 <img width="919" alt="loggin" src="https://github.com/GitSamad88/streamlit-signin-ui/assets/110288424/034ff583-0e81-437a-a5ae-33ca7e6f521f">
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
-v1.3.1
+v1.3.3
 
 ## License
 [MIT](https://github.com/GitSamad88/streamlit_signin_ui/blob/main/LICENSE)
```

### Comparing `streamlit_signin_auth_ui-1.3.1/pyproject.toml` & `streamlit_signin_auth_ui-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 5d0d  uptools>=61.0"].
 00000030: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b70 726f  ld_meta"....[pro
 00000060: 6a65 6374 5d0d 0a6e 616d 6520 3d20 2273  ject]..name = "s
 00000070: 7472 6561 6d6c 6974 5f73 6967 6e69 6e5f  treamlit_signin_
 00000080: 6175 7468 5f75 6922 0d0a 7665 7273 696f  auth_ui"..versio
-00000090: 6e20 3d20 2231 2e33 2e31 220d 0a61 7574  n = "1.3.1"..aut
+00000090: 6e20 3d20 2231 2e33 2e33 220d 0a61 7574  n = "1.3.3"..aut
 000000a0: 686f 7273 203d 205b 0d0a 2020 7b20 6e61  hors = [..  { na
 000000b0: 6d65 3d22 5441 4f55 4649 5120 4142 4445  me="TAOUFIQ ABDE
 000000c0: 5353 414d 4144 222c 2065 6d61 696c 3d22  SSAMAD", email="
 000000d0: 7361 6d61 6474 616f 7566 696b 4067 6d61  samadtaoufik@gma
 000000e0: 696c 2e63 6f6d 2220 7d2c 0d0a 5d0d 0a64  il.com" },..]..d
 000000f0: 6573 6372 6970 7469 6f6e 203d 2022 4c6f  escription = "Lo
 00000100: 6769 6e2f 5369 676e 2d75 7020 7061 6765  gin/Sign-up page
 00000110: 2077 6974 6820 5374 7265 616d 6c69 742c   with Streamlit,
 00000120: 7468 6520 7573 6572 2773 2064 6174 6120  the user's data 
 00000130: 6172 6520 7374 6f72 6564 2069 6e20 6120  are stored in a 
 00000140: 476f 6f67 6c65 2053 6865 6574 7320 6669  Google Sheets fi
 00000150: 6c65 2061 7320 6461 7461 6261 7365 2c61  le as database,a
 00000160: 6c73 6f20 7468 6520 6c61 626c 6573 206f  lso the lables o
 00000170: 6620 7769 6467 6574 7320 6172 6520 696e  f widgets are in
-00000180: 2066 7265 6e73 6820 6c61 6e67 7561 6765   frensh language
+00000180: 2046 7265 6e73 6820 6c61 6e67 7561 6765   Frensh language
 00000190: 2e22 0d0a 7265 6164 6d65 203d 2022 5245  ."..readme = "RE
 000001a0: 4144 4d45 2e6d 6422 0d0a 7265 7175 6972  ADME.md"..requir
 000001b0: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
 000001c0: 2e31 3022 0d0a 636c 6173 7369 6669 6572  .10"..classifier
 000001d0: 7320 3d20 5b0d 0a20 2020 2022 5072 6f67  s = [..    "Prog
 000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
```

### Comparing `streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/utils.py` & `streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui/widgets.py` & `streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     def reset_password(self) -> None:
         """
         Creates the reset password widget and after user authentication (email and the password shared over that email),
         resets the password and updates the same in the Google sheet file (database).
         """
         with st.form(key="form0003"):
-            email_reset_passwd = st.text_input("Email", placeholder='Entrez votre email')
+            email_reset_passwd = st.text_input("Email",value='example@gmail.com', placeholder='Entrez votre email')
             email_exists_check, username_reset_passwd = check_email_exists(self.credentials,email_reset_passwd)
 
             current_passwd = st.text_input("Mot de passe temporaire",
                                            placeholder='Svp entrez le mot de passe que vous avez reçu par email!')
             current_passwd_check = check_current_passwd(self.credentials,email_reset_passwd, current_passwd)
 
             new_passwd = st.text_input("Nouveau mot de passe", placeholder='Svp entrez un mot de passe nouveau et fort!',
```

### Comparing `streamlit_signin_auth_ui-1.3.1/src/streamlit_signin_auth_ui.egg-info/PKG-INFO` & `streamlit_signin_auth_ui-1.3.3/src/streamlit_signin_auth_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: streamlit_signin_auth_ui
-Version: 1.3.1
-Summary: Login/Sign-up page with Streamlit,the user's data are stored in a Google Sheets file as database,also the lables of widgets are in frensh language.
+Version: 1.3.3
+Summary: Login/Sign-up page with Streamlit,the user's data are stored in a Google Sheets file as database,also the lables of widgets are in Frensh language.
 Author-email: TAOUFIQ ABDESSAMAD <samadtaoufik@gmail.com>
 Project-URL: Homepage, https://github.com/GitSamad88/streamlit-signin-ui
 Project-URL: Issues, https://github.com/GitSamad88/streamlit-signin-ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,15 +18,15 @@
 Requires-Dist: oauth2client>=4.1.3
 Requires-Dist: google_api_python_client>=2.119.0
 Requires-Dist: argon2-cffi
 Requires-Dist: streamlit_lottie
 Requires-Dist: streamlit_option_menu
 Requires-Dist: streamlit-cookies-manager-hotpatched==0.2.1
 
-# Login page with Streamlit (Lables in frensh language)
+# Login page with Streamlit (Lables of widgets are in Frensh language)
 
 # Update of https://github.com/GitSamad88
 
 
 
 #Version 2024-3-29 : this version is an update of streamlit-login-auth-ui-23
 
@@ -160,11 +160,11 @@
 Generated in the sidebar only if the user is logged in, allows users to logout. \
 
 <img width="919" alt="loggin" src="https://github.com/GitSamad88/streamlit-signin-ui/assets/110288424/034ff583-0e81-437a-a5ae-33ca7e6f521f">
 
 __Cookies are automatically created and destroyed depending on the user authentication status.__
 
 ## Version
-v1.3.1
+v1.3.3
 
 ## License
 [MIT](https://github.com/GitSamad88/streamlit_signin_ui/blob/main/LICENSE)
```

