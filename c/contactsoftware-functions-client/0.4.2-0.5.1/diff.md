# Comparing `tmp/contactsoftware_functions_client-0.4.2.tar.gz` & `tmp/contactsoftware_functions_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactsoftware_functions_client-0.4.2.tar", max compression
+gzip compressed data, was "contactsoftware_functions_client-0.5.1.tar", max compression
```

## Comparing `contactsoftware_functions_client-0.4.2.tar` & `contactsoftware_functions_client-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1543 2024-02-26 14:48:56.099624 contactsoftware_functions_client-0.4.2/README.md
--rw-r--r--   0        0        0       85 2024-02-02 10:04:30.766488 contactsoftware_functions_client-0.4.2/cfc/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-02 10:04:30.766488 contactsoftware_functions_client-0.4.2/cfc/app.py
--rw-r--r--   0        0        0     1183 2024-02-02 10:04:30.766488 contactsoftware_functions_client-0.4.2/cfc/auth.py
--rw-r--r--   0        0        0     3526 2024-02-27 07:30:58.654783 contactsoftware_functions_client-0.4.2/cfc/config.py
--rw-r--r--   0        0        0     6679 2024-02-27 07:30:58.770776 contactsoftware_functions_client-0.4.2/cfc/environment.py
--rw-r--r--   0        0        0      622 2024-02-27 07:33:08.712885 contactsoftware_functions_client-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 contactsoftware_functions_client-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-09 13:16:14.496368 contactsoftware_functions_client-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1927 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/README.md
+-rw-r--r--   0        0        0       85 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/app.py
+-rw-r--r--   0        0        0     1264 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/auth.py
+-rw-r--r--   0        0        0     3548 2024-04-09 13:47:16.015817 contactsoftware_functions_client-0.5.1/cfc/config.py
+-rw-r--r--   0        0        0     6807 2024-04-09 13:16:14.500368 contactsoftware_functions_client-0.5.1/cfc/environment.py
+-rw-r--r--   0        0        0      622 2024-04-09 13:47:27.664183 contactsoftware_functions_client-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 contactsoftware_functions_client-0.5.1/PKG-INFO
```

### Comparing `contactsoftware_functions_client-0.4.2/README.md` & `contactsoftware_functions_client-0.5.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,175 @@
-00000000: 203c 6831 3e3c 6120 6872 6566 3d22 6874   <h1><a href="ht
-00000010: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000020: 2f63 736c 6162 2f66 756e 6374 696f 6e73  /cslab/functions
-00000030: 2d73 646b 223e 3c69 6d67 2073 7263 3d22  -sdk"><img src="
-00000040: 6874 7470 733a 2f2f 7777 772e 636f 6e74  https://www.cont
-00000050: 6163 742d 736f 6674 7761 7265 2e63 6f6d  act-software.com
-00000060: 2f64 6573 6967 6e2f 696d 672f 6c6f 676f  /design/img/logo
-00000070: 2d69 636f 6e2e 7376 6722 2077 6964 7468  -icon.svg" width
-00000080: 3d22 3530 2220 616c 743d 2243 4f4e 5441  ="50" alt="CONTA
-00000090: 4354 204c 6f67 6f22 3e3c 2f61 3e20 4675  CT Logo"></a> Fu
-000000a0: 6e63 7469 6f6e 732d 436c 6965 6e74 3c2f  nctions-Client</
-000000b0: 6831 3e0a 0a54 6869 7320 434c 4920 746f  h1>..This CLI to
-000000c0: 6f6c 2069 7320 7573 6564 2066 6f72 2075  ol is used for u
-000000d0: 706c 6f61 6469 6e67 2061 6e64 206d 616e  ploading and man
-000000e0: 6167 696e 6720 4675 6e63 7469 6f6e 7320  aging Functions 
-000000f0: 696e 2043 494d 2044 6174 6162 6173 6520  in CIM Database 
-00000100: 436c 6f75 642e 0a0a 2323 2320 496e 7374  Cloud...### Inst
-00000110: 616c 6c61 7469 6f6e 0a0a 6060 6063 6f6e  allation..```con
-00000120: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
-00000130: 6c6c 2063 6f6e 7461 6374 736f 6674 7761  ll contactsoftwa
-00000140: 7265 2d66 756e 6374 696f 6e73 2d63 6c69  re-functions-cli
-00000150: 656e 740a 6060 600a 0a23 2323 204c 6f67  ent.```..### Log
-00000160: 696e 0a42 6566 6f72 6520 796f 7520 6361  in.Before you ca
-00000170: 6e20 6372 6561 7465 2065 6e76 6972 6f6e  n create environ
-00000180: 6d65 6e74 7320 6f72 2064 6570 6c6f 7920  ments or deploy 
-00000190: 4675 6e63 7469 6f6e 7320 796f 7520 6e65  Functions you ne
-000001a0: 6564 2074 6f20 6c6f 6769 6e20 7573 696e  ed to login usin
-000001b0: 6720 796f 7572 2063 6c69 656e 742d 6964  g your client-id
-000001c0: 2061 6e64 2073 6563 7265 742e 204f 6274   and secret. Obt
-000001d0: 6169 6e20 796f 7572 2063 6c69 656e 7420  ain your client 
-000001e0: 6372 6564 656e 7469 616c 7320 7669 6120  credentials via 
-000001f0: 7468 6520 434f 4e54 4143 5420 506f 7274  the CONTACT Port
-00000200: 616c 2e0a 0a60 6060 636f 6e73 6f6c 650a  al...```console.
-00000210: 2420 6366 6320 6c6f 6769 6e20 2d2d 636c  $ cfc login --cl
-00000220: 6965 6e74 2d69 6420 3c63 6c69 656e 745f  ient-id <client_
-00000230: 6964 3e20 2d2d 636c 6965 6e74 2d73 6563  id> --client-sec
-00000240: 7265 7420 3c63 6c69 656e 745f 7365 6372  ret <client_secr
-00000250: 6574 3e0a 6060 600a 0a0a 2323 2320 5573  et>.```...### Us
-00000260: 6167 650a 4669 7273 7420 796f 7520 6e65  age.First you ne
-00000270: 6564 2074 6f20 6861 7665 2061 6e20 656e  ed to have an en
-00000280: 7669 726f 6e6d 656e 7420 7468 6174 2079  vironment that y
-00000290: 6f75 2063 616e 2064 6570 6c6f 7920 796f  ou can deploy yo
-000002a0: 7572 2063 6f64 6520 696e 746f 2e0a 0a43  ur code into...C
-000002b0: 6865 636b 2069 6620 796f 7520 616c 7265  heck if you alre
-000002c0: 6164 7920 6861 7665 2065 6e76 6972 6f6e  ady have environ
-000002d0: 6d65 6e74 7320 6176 6169 6c61 626c 653a  ments available:
-000002e0: 0a0a 6060 6063 6f6e 736f 6c65 0a24 2063  ..```console.$ c
-000002f0: 6663 2065 6e76 206c 6973 740a 6060 600a  fc env list.```.
-00000300: 0a6f 7220 6372 6561 7465 2061 206e 6577  .or create a new
-00000310: 206f 6e65 3a0a 0a60 6060 636f 6e73 6f6c   one:..```consol
-00000320: 650a 2420 6366 6320 656e 7620 6372 6561  e.$ cfc env crea
-00000330: 7465 203c 656e 7669 726f 6e6d 656e 745f  te <environment_
-00000340: 6e61 6d65 3e0a 6060 600a 0a59 6f75 206e  name>.```..You n
-00000350: 6565 6420 746f 2063 7265 6174 6520 616e  eed to create an
-00000360: 2060 656e 7669 726f 6e6d 656e 742e 7961   `environment.ya
-00000370: 6d6c 6020 6669 6c65 2074 6861 7420 6c69  ml` file that li
-00000380: 7374 7320 7468 6520 4675 6e63 7469 6f6e  sts the Function
-00000390: 7320 796f 7572 2065 6e76 6972 6f6e 6d65  s your environme
-000003a0: 6e74 2073 686f 756c 6420 636f 6e74 6169  nt should contai
-000003b0: 6e3a 0a0a 6060 6079 616d 6c0a 7275 6e74  n:..```yaml.runt
-000003c0: 696d 653a 2070 7974 686f 6e33 2e31 300a  ime: python3.10.
-000003d0: 7665 7273 696f 6e3a 2076 310a 6675 6e63  version: v1.func
-000003e0: 7469 6f6e 733a 0a20 202d 206e 616d 653a  tions:.  - name:
-000003f0: 206d 795f 6675 6e63 7469 6f6e 0a20 2020   my_function.   
-00000400: 2065 6e74 7279 706f 696e 743a 206d 6169   entrypoint: mai
-00000410: 6e2e 6d79 5f66 756e 6374 696f 6e0a 6060  n.my_function.``
-00000420: 600a 0a61 6e64 206f 6620 636f 7572 7365  `..and of course
-00000430: 2074 6865 2063 6f64 6520 6f66 2079 6f75   the code of you
-00000440: 7220 4675 6e63 7469 6f6e 3a0a 0a60 6060  r Function:..```
-00000450: 7079 7468 6f6e 0a23 206d 6169 6e2e 7079  python.# main.py
-00000460: 0a64 6566 206d 795f 6675 6e63 7469 6f6e  .def my_function
-00000470: 286d 6574 6164 6174 612c 2065 7665 6e74  (metadata, event
-00000480: 2c20 7365 7276 6963 6529 3a0a 2020 2e2e  , service):.  ..
-00000490: 2e0a 6060 600a 0a3e 205b 214e 4f54 455d  ..```..> [!NOTE]
-000004a0: 0a3e 2059 6f75 2063 616e 2073 7065 6369  .> You can speci
-000004b0: 6679 2065 7874 7261 2072 6571 7569 7265  fy extra require
-000004c0: 6d65 6e74 7320 796f 7572 2063 6f64 6520  ments your code 
-000004d0: 6861 7320 696e 2061 2072 6571 7569 7265  has in a require
-000004e0: 6d65 6e74 732e 7478 742e 0a0a 3e20 5b21  ments.txt...> [!
-000004f0: 494d 504f 5254 414e 545d 0a3e 2054 6865  IMPORTANT].> The
-00000500: 2070 7974 686f 6e33 2e31 3020 7275 6e74   python3.10 runt
-00000510: 696d 6520 7265 7175 6972 6573 2079 6f75  ime requires you
-00000520: 2074 6f20 6164 6420 2a2a 636f 6e74 6163   to add **contac
-00000530: 7473 6f66 7477 6172 652d 6675 6e63 7469  tsoftware-functi
-00000540: 6f6e 732a 2a20 746f 2074 6865 2072 6571  ons** to the req
-00000550: 7569 7265 6d65 6e74 732e 7478 7420 756e  uirements.txt un
-00000560: 6c65 7373 2079 6f75 2073 7065 6369 6679  less you specify
-00000570: 2079 6f75 7220 6f77 6e20 6d61 696e 5f65   your own main_e
-00000580: 6e74 7279 706f 696e 7420 6861 6e64 6c65  ntrypoint handle
-00000590: 722e 2028 7365 6520 646f 6375 6d65 6e74  r. (see document
-000005a0: 6174 696f 6e29 0a0a 4e6f 7720 796f 7520  ation)..Now you 
-000005b0: 6361 6e20 6465 706c 6f79 2079 6f75 7220  can deploy your 
-000005c0: 636f 6465 2069 6e74 6f20 616e 2065 6e76  code into an env
-000005d0: 6972 6f6e 6d65 6e74 3a0a 0a60 6060 0a24  ironment:..```.$
-000005e0: 2063 6663 2065 6e76 2064 6570 6c6f 7920   cfc env deploy 
-000005f0: 3c65 6e76 6972 6f6e 6d65 6e74 5f6e 616d  <environment_nam
-00000600: 653e 0a60 6060 0a                        e>.```.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6e74  : 2.1.Name: cont
+00000020: 6163 7473 6f66 7477 6172 652d 6675 6e63  actsoftware-func
+00000030: 7469 6f6e 732d 636c 6965 6e74 0a56 6572  tions-client.Ver
+00000040: 7369 6f6e 3a20 302e 352e 310a 5375 6d6d  sion: 0.5.1.Summ
+00000050: 6172 793a 2043 6c69 656e 7420 666f 7220  ary: Client for 
+00000060: 7570 6c6f 6164 696e 6720 616e 6420 6d61  uploading and ma
+00000070: 6e61 6769 6e67 2046 756e 6374 696f 6e73  naging Functions
+00000080: 2069 6e20 4349 4d20 4461 7461 6261 7365   in CIM Database
+00000090: 2043 6c6f 7564 2e0a 4c69 6365 6e73 653a   Cloud..License:
+000000a0: 204d 4954 0a41 7574 686f 723a 204a 656e   MIT.Author: Jen
+000000b0: 7320 4bc3 bc72 7465 6e0a 4175 7468 6f72  s K..rten.Author
+000000c0: 2d65 6d61 696c 3a20 6a6b 7540 636f 6e74  -email: jku@cont
+000000d0: 6163 742e 6465 0a52 6571 7569 7265 732d  act.de.Requires-
+000000e0: 5079 7468 6f6e 3a20 3e3d 332e 392c 3c34  Python: >=3.9,<4
+000000f0: 2e30 0a43 6c61 7373 6966 6965 723a 204c  .0.Classifier: L
+00000100: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000110: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000120: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+00000130: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000140: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000150: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+00000160: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000170: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000180: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000190: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000001a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001b0: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+000001c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+000001f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000200: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000210: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+00000220: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000230: 5079 5941 4d4c 2028 3e3d 362e 302c 3c37  PyYAML (>=6.0,<7
+00000240: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+00000250: 743a 2061 7070 6469 7273 2028 3e3d 312e  t: appdirs (>=1.
+00000260: 342e 342c 3c32 2e30 2e30 290a 5265 7175  4.4,<2.0.0).Requ
+00000270: 6972 6573 2d44 6973 743a 2063 6c69 636b  ires-Dist: click
+00000280: 2028 3e3d 382e 302e 342c 3c39 2e30 2e30   (>=8.0.4,<9.0.0
+00000290: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+000002a0: 2072 6571 7565 7374 7320 283e 3d32 2e32   requests (>=2.2
+000002b0: 372e 312c 3c33 2e30 2e30 290a 5265 7175  7.1,<3.0.0).Requ
+000002c0: 6972 6573 2d44 6973 743a 2072 6963 6820  ires-Dist: rich 
+000002d0: 283e 3d31 322e 302e 312c 3c31 332e 302e  (>=12.0.1,<13.0.
+000002e0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000002f0: 3a20 7479 7065 7220 283e 3d30 2e34 2e30  : typer (>=0.4.0
+00000300: 2c3c 302e 352e 3029 0a52 6571 7569 7265  ,<0.5.0).Require
+00000310: 732d 4469 7374 3a20 7572 6c6c 6962 3320  s-Dist: urllib3 
+00000320: 283e 3d31 2e32 362e 3136 2c3c 322e 302e  (>=1.26.16,<2.0.
+00000330: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
+00000340: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000350: 742f 6d61 726b 646f 776e 0a0a 203c 6831  t/markdown.. <h1
+00000360: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00000370: 2f2f 6769 7468 7562 2e63 6f6d 2f63 736c  //github.com/csl
+00000380: 6162 2f66 756e 6374 696f 6e73 2d73 646b  ab/functions-sdk
+00000390: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000003a0: 733a 2f2f 7777 772e 636f 6e74 6163 742d  s://www.contact-
+000003b0: 736f 6674 7761 7265 2e63 6f6d 2f64 6573  software.com/des
+000003c0: 6967 6e2f 696d 672f 6c6f 676f 2d69 636f  ign/img/logo-ico
+000003d0: 6e2e 7376 6722 2077 6964 7468 3d22 3530  n.svg" width="50
+000003e0: 2220 616c 743d 2243 4f4e 5441 4354 204c  " alt="CONTACT L
+000003f0: 6f67 6f22 3e3c 2f61 3e20 4675 6e63 7469  ogo"></a> Functi
+00000400: 6f6e 732d 436c 6965 6e74 3c2f 6831 3e0a  ons-Client</h1>.
+00000410: 0a54 6869 7320 434c 4920 746f 6f6c 2069  .This CLI tool i
+00000420: 7320 7573 6564 2066 6f72 2075 706c 6f61  s used for uploa
+00000430: 6469 6e67 2061 6e64 206d 616e 6167 696e  ding and managin
+00000440: 6720 4675 6e63 7469 6f6e 7320 696e 2043  g Functions in C
+00000450: 494d 2044 6174 6162 6173 6520 436c 6f75  IM Database Clou
+00000460: 642e 0a0a 496e 666f 726d 6174 696f 6e20  d...Information 
+00000470: 6f6e 2068 6f77 2062 7569 6c64 2046 756e  on how build Fun
+00000480: 6374 696f 6e73 2063 616e 2062 6520 666f  ctions can be fo
+00000490: 756e 6420 696e 2074 6865 2046 756e 6374  und in the Funct
+000004a0: 696f 6e73 2d53 444b 2064 6f63 756d 656e  ions-SDK documen
+000004b0: 7461 7469 6f6e 3a20 6874 7470 733a 2f2f  tation: https://
+000004c0: 6373 6c61 622e 6769 7468 7562 2e69 6f2f  cslab.github.io/
+000004d0: 6675 6e63 7469 6f6e 732d 7364 6b2d 7079  functions-sdk-py
+000004e0: 7468 6f6e 2f0a 0a23 2320 5265 7175 6972  thon/..## Requir
+000004f0: 656d 656e 7473 0a0a 5079 7468 6f6e 2033  ements..Python 3
+00000500: 2e31 302b 0a0a 2323 2049 6e73 7461 6c6c  .10+..## Install
+00000510: 6174 696f 6e0a 0a60 6060 636f 6e73 6f6c  ation..```consol
+00000520: 650a 2420 7069 7020 696e 7374 616c 6c20  e.$ pip install 
+00000530: 636f 6e74 6163 7473 6f66 7477 6172 652d  contactsoftware-
+00000540: 6675 6e63 7469 6f6e 732d 636c 6965 6e74  functions-client
+00000550: 0a60 6060 0a0a 2323 204c 6f67 696e 0a42  .```..## Login.B
+00000560: 6566 6f72 6520 796f 7520 6361 6e20 6372  efore you can cr
+00000570: 6561 7465 2065 6e76 6972 6f6e 6d65 6e74  eate environment
+00000580: 7320 6f72 2064 6570 6c6f 7920 4675 6e63  s or deploy Func
+00000590: 7469 6f6e 7320 796f 7520 6e65 6564 2074  tions you need t
+000005a0: 6f20 6c6f 6769 6e20 7573 696e 6720 796f  o login using yo
+000005b0: 7572 2063 6c69 656e 742d 6964 2061 6e64  ur client-id and
+000005c0: 2073 6563 7265 742e 204f 6274 6169 6e20   secret. Obtain 
+000005d0: 796f 7572 2063 6c69 656e 7420 6372 6564  your client cred
+000005e0: 656e 7469 616c 7320 7669 6120 7468 6520  entials via the 
+000005f0: 434f 4e54 4143 5420 506f 7274 616c 2e0a  CONTACT Portal..
+00000600: 0a60 6060 636f 6e73 6f6c 650a 2420 6366  .```console.$ cf
+00000610: 6320 6c6f 6769 6e20 2d2d 636c 6965 6e74  c login --client
+00000620: 2d69 6420 3c63 6c69 656e 745f 6964 3e20  -id <client_id> 
+00000630: 2d2d 636c 6965 6e74 2d73 6563 7265 7420  --client-secret 
+00000640: 3c63 6c69 656e 745f 7365 6372 6574 3e0a  <client_secret>.
+00000650: 6060 600a 0a54 6865 2063 7265 6465 6e74  ```..The credent
+00000660: 6961 6c73 2077 696c 6c20 6265 2073 746f  ials will be sto
+00000670: 7265 6420 696e 2061 2063 6f6e 6669 6775  red in a configu
+00000680: 7261 7469 6f6e 2066 696c 652e 2054 6865  ration file. The
+00000690: 2073 746f 7261 6765 206c 6f63 6174 696f   storage locatio
+000006a0: 6e20 6f66 2074 6865 2063 6f6e 6669 6775  n of the configu
+000006b0: 7261 7469 6f6e 2066 696c 6520 6465 7065  ration file depe
+000006c0: 6e64 7320 6f6e 2074 6865 204f 533a 0a0a  nds on the OS:..
+000006d0: 2d20 5769 6e64 6f77 733a 2060 433a 5c55  - Windows: `C:\U
+000006e0: 7365 7273 5c3c 7573 6572 6e61 6d65 3e5c  sers\<username>\
+000006f0: 4170 7044 6174 615c 4c6f 6361 6c5c 436f  AppData\Local\Co
+00000700: 6e74 6163 745c 6366 635c 636f 6e66 6967  ntact\cfc\config
+00000710: 2e69 6e69 600a 2d20 4c69 6e75 783a 2060  .ini`.- Linux: `
+00000720: 7e2f 2e63 6f6e 6669 672f 6366 632f 636f  ~/.config/cfc/co
+00000730: 6e66 6967 2e69 6e69 600a 0a0a 2323 2046  nfig.ini`...## F
+00000740: 6561 7475 7265 730a 2323 2320 4d61 6e61  eatures.### Mana
+00000750: 6765 2046 756e 6374 696f 6e20 656e 7669  ge Function envi
+00000760: 726f 6e6d 656e 7473 0a46 756e 6374 696f  ronments.Functio
+00000770: 6e73 2061 7265 2067 726f 7570 6564 2069  ns are grouped i
+00000780: 6e74 6f20 2a2a 656e 7669 726f 6e6d 656e  nto **environmen
+00000790: 7473 2a2a 2c20 7768 6963 6820 6172 6520  ts**, which are 
+000007a0: 7468 6520 2844 6f63 6b65 7229 2063 6f6e  the (Docker) con
+000007b0: 7461 696e 6572 2074 6865 2063 6f64 6520  tainer the code 
+000007c0: 7275 6e73 2069 6e2e 2041 6e20 656e 7669  runs in. An envi
+000007d0: 726f 6e6d 656e 7420 636f 6e74 6169 6e73  ronment contains
+000007e0: 2061 2072 756e 7469 6d65 2066 6f72 2069   a runtime for i
+000007f0: 7473 2073 7065 6369 6669 6320 7072 6f67  ts specific prog
+00000800: 7261 6d6d 696e 6720 6c61 6e67 7561 6765  ramming language
+00000810: 2c20 7468 6520 4675 6e63 7469 6f6e 2063  , the Function c
+00000820: 6f64 6520 616e 6420 6120 636f 6e66 6967  ode and a config
+00000830: 7572 6174 696f 6e20 6669 6c65 2064 6573  uration file des
+00000840: 6372 6962 696e 6720 7468 6520 656e 7669  cribing the envi
+00000850: 726f 6e6d 656e 742e 0a0a 4372 6561 7465  ronment...Create
+00000860: 2061 206e 6577 2065 6e76 6972 6f6e 6d65   a new environme
+00000870: 6e74 3a0a 0a60 6060 636f 6e73 6f6c 650a  nt:..```console.
+00000880: 2420 6366 6320 656e 7620 6372 6561 7465  $ cfc env create
+00000890: 203c 656e 7669 726f 6e6d 656e 745f 6e61   <environment_na
+000008a0: 6d65 3e0a 6060 600a 0a44 6973 706c 6179  me>.```..Display
+000008b0: 2061 206c 6973 7420 6f66 2061 6c6c 2065   a list of all e
+000008c0: 6e76 6972 6f6e 6d65 6e74 733a 0a0a 6060  nvironments:..``
+000008d0: 6063 6f6e 736f 6c65 0a24 2063 6663 2065  `console.$ cfc e
+000008e0: 6e76 206c 6973 740a 6060 600a 0a44 6973  nv list.```..Dis
+000008f0: 706c 6179 2074 6865 2064 6574 6169 6c73  play the details
+00000900: 206f 6620 616e 2065 6e76 6972 6f6e 6d65   of an environme
+00000910: 6e74 3a0a 0a60 6060 636f 6e73 6f6c 650a  nt:..```console.
+00000920: 2420 6366 6320 656e 7620 6465 7363 7269  $ cfc env descri
+00000930: 6265 203c 656e 7669 726f 6e6d 656e 745f  be <environment_
+00000940: 6e61 6d65 3e0a 6060 600a 0a0a 2323 2320  name>.```...### 
+00000950: 4465 706c 6f79 2046 756e 6374 696f 6e20  Deploy Function 
+00000960: 636f 6465 2069 6e74 6f20 616e 2065 6e76  code into an env
+00000970: 6972 6f6e 6d65 6e74 0a54 6f20 6465 706c  ironment.To depl
+00000980: 6f79 2046 756e 6374 696f 6e20 636f 6465  oy Function code
+00000990: 2069 6e74 6f20 616e 2065 7869 7374 696e   into an existin
+000009a0: 6720 656e 7669 726f 6e6d 656e 7420 7275  g environment ru
+000009b0: 6e3a 0a0a 6060 600a 2420 6366 6320 656e  n:..```.$ cfc en
+000009c0: 7620 6465 706c 6f79 203c 656e 7669 726f  v deploy <enviro
+000009d0: 6e6d 656e 745f 6e61 6d65 3e0a 6060 600a  nment_name>.```.
+000009e0: 0a4d 616b 6520 7375 7265 2079 6f75 2072  .Make sure you r
+000009f0: 756e 2074 6865 2063 6f6d 6d61 6e64 2066  un the command f
+00000a00: 726f 6d20 7769 7468 696e 2074 6865 2064  rom within the d
+00000a10: 6972 6563 746f 7279 2074 6861 7420 636f  irectory that co
+00000a20: 6e74 6169 6e73 2074 6865 2060 656e 7669  ntains the `envi
+00000a30: 726f 6e6d 656e 742e 7961 6d6c 6020 636f  ronment.yaml` co
+00000a40: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00000a50: 2e0a 0a49 6e66 6f72 6d61 7469 6f6e 206f  ...Information o
+00000a60: 6e20 686f 7720 746f 2062 7569 6c64 2046  n how to build F
+00000a70: 756e 6374 696f 6e20 636f 6465 2063 616e  unction code can
+00000a80: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
+00000a90: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
+00000aa0: 6620 7468 6520 4675 6e63 7469 6f6e 732d  f the Functions-
+00000ab0: 5344 4b3a 2068 7474 7073 3a2f 2f63 736c  SDK: https://csl
+00000ac0: 6162 2e67 6974 6875 622e 696f 2f66 756e  ab.github.io/fun
+00000ad0: 6374 696f 6e73 2d73 646b 2d70 7974 686f  ctions-sdk-pytho
+00000ae0: 6e2f 0a0a                                n/..
```

### Comparing `contactsoftware_functions_client-0.4.2/cfc/app.py` & `contactsoftware_functions_client-0.5.1/cfc/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,33 @@
 app.add_typer(env_app, name="env")
 
 
 def get_environment(source_path: str):
     envfile = os.path.join(source_path, "environment.yaml")
 
     if not os.path.exists(envfile):
-        raise typer.BadParameter("Directory is not a valid environment", param_hint="source_path")
+        raise typer.BadParameter(
+            "Directory is not a valid environment", param_hint="source_path"
+        )
 
     with open(envfile, "rb") as f:
         return yaml.safe_load(f)
 
 
 @app.command(name="login")
 def login(
     client_id: str = typer.Option(..., prompt=True),
     client_secret: str = typer.Option(..., prompt=True, hide_input=True),
     service_url: str = typer.Option(default=config.service_url),
 ):
     """Login to function backend using client ID and client secret"""
 
-    if service_url != config.service_url and typer.confirm("There is already another service url saved. Override?"):
+    if service_url != config.service_url and typer.confirm(
+        "There is already another service url saved. Override?"
+    ):
         config.service_url = service_url
         config.save()
 
     config.client_id = client_id
     config.client_secret = client_secret
 
     try:
```

### Comparing `contactsoftware_functions_client-0.4.2/cfc/auth.py` & `contactsoftware_functions_client-0.5.1/cfc/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,30 @@
 
 
 def authenticate_keycloak(client_id: str, client_secret: str) -> (str, int):
     """
     Connects with the given credentials to KeyCloak and fetch an access token
     return: a jwt token and unix timestamp when the token will expire
     """
-    payload = {"grant_type": "client_credentials", "scope": FUNCTION_CONTROLLER_DEV_TOKEN_SCOPE}
+    payload = {
+        "grant_type": "client_credentials",
+        "scope": FUNCTION_CONTROLLER_DEV_TOKEN_SCOPE,
+    }
     headers = {"Content-Type": "application/x-www-form-urlencoded"}
     response = requests.post(
-        TOKEN_ISSUER + TOKEN_URL_EXTENSION, headers=headers, data=payload, auth=(client_id, client_secret), timeout=60
+        TOKEN_ISSUER + TOKEN_URL_EXTENSION,
+        headers=headers,
+        data=payload,
+        auth=(client_id, client_secret),
+        timeout=60,
     )
 
     if response.status_code == 401:
         raise CredentialsInvalid
     if response.status_code != 200:
         raise ValueError(f"Token endpoint returned status code {response.status_code}")
 
     response_content = response.json()
-    return response_content["access_token"], int(response_content["expires_in"]) + time.time()
+    return (
+        response_content["access_token"],
+        int(response_content["expires_in"]) + time.time(),
+    )
```

### Comparing `contactsoftware_functions_client-0.4.2/cfc/config.py` & `contactsoftware_functions_client-0.5.1/cfc/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from appdirs import user_config_dir
 
 from .auth import authenticate_keycloak
 
 
 class Config:  # pylint: disable=too-many-instance-attributes
     config_path: Path = Path()
-    service_url: str = "https://functions.cs-0a.contact-cloud.com"
+    service_url: str = "https://functions.cs-0b.contact-cloud.com"
     _conf: configparser.ConfigParser | None = None
     _client_id: str = ""
     _client_secret: str = ""
     _access_token: str = ""
     token_valid_until: int = 0
 
     def __init__(self, config_directory=None):
@@ -92,15 +92,17 @@
             "default", "service_url", fallback=self.service_url
         )
         self._access_token = os.getenv("CFC_TOKEN") or self._conf.get(
             "default", "_access_token", fallback=self._access_token
         )
         self._client_id = self._conf.get("default", "client_id", fallback="")
         self._client_secret = self._conf.get("default", "client_secret", fallback="")
-        self.token_valid_until = self._conf.get("default", "token_valid_until", fallback=0)
+        self.token_valid_until = self._conf.get(
+            "default", "token_valid_until", fallback=0
+        )
 
     def save(self):
         self._set_conf()
         with open(self.config_path, "w", encoding="utf-8") as f:
             self._conf.write(f)
```

### Comparing `contactsoftware_functions_client-0.4.2/cfc/environment.py` & `contactsoftware_functions_client-0.5.1/cfc/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 env_app = typer.Typer()
 console = Console()
 
 
 def name_callback(name: str) -> str:
     if not re.fullmatch(NAME_PATTERN, name) or len(name) > 50:
-        raise typer.BadParameter(f"Name must match pattern {NAME_PATTERN} and must not be longer than 50 characters")
+        raise typer.BadParameter(
+            f"Name must match pattern {NAME_PATTERN} and must not be longer than 50 characters"
+        )
     return name
 
 
 def tag_callback(name: str) -> str:
     if not name:
         return name
 
@@ -61,15 +63,17 @@
         headers={"Authorization": f"Bearer {config.access_token}"},
     )
 
     if response.status_code == 201:
         console.print("Environment successfully created")
 
     elif response.status_code in (400, 500):
-        console.print("Error while creating environment: " + response.json()["detail"]["msg"])
+        console.print(
+            "Error while creating environment: " + response.json()["detail"]["msg"]
+        )
         raise typer.Exit(code=1)
 
     else:
         console.print("Unknown error while creating environment")
         raise typer.Exit(code=1)
 
 
@@ -119,27 +123,33 @@
             "\n".join(str(e) for e in env["functions"]),
         )
 
     console.print(table)
 
 
 @env_app.command(name="describe")
-def describe_env(environment_name: str = typer.Argument(..., callback=name_callback, envvar=ENVIRONMENT_ENVVAR_NAME)):
+def describe_env(
+    environment_name: str = typer.Argument(
+        ..., callback=name_callback, envvar=ENVIRONMENT_ENVVAR_NAME
+    )
+):
     """describes an environment"""
     _ensure_token_set()
     result = requests.get(  # nosec pylint: disable=missing-timeout
         config.service_url + "/api/environments/" + environment_name,
         headers={"Authorization": f"Bearer {config.access_token}"},
     )
     console.print(result.json())
 
 
 @env_app.command(name="deploy")
 def deploy_env(
-    environment_name: str = typer.Argument(..., callback=name_callback, envvar=ENVIRONMENT_ENVVAR_NAME),
+    environment_name: str = typer.Argument(
+        ..., callback=name_callback, envvar=ENVIRONMENT_ENVVAR_NAME
+    ),
     source_path: str = typer.Option("."),
     tag: str = typer.Option("", callback=tag_callback),
     environment_variables: str = typer.Option("", callback=env_var_callback),
 ):
     """deploy code into an environment"""
     _ensure_token_set()
 
@@ -153,15 +163,18 @@
     data = tag_info
     if environment_variables:
         data["environment_variables"] = environment_variables
 
     with open("source.tar.gz", "rb") as codepackage:
         console.print("Uploading code (This can take a while)")
         response = requests.post(  # nosec pylint: disable=missing-timeout
-            config.service_url + "/api/environments/" + environment_name + "/upload_code",
+            config.service_url
+            + "/api/environments/"
+            + environment_name
+            + "/upload_code",
             files={"codepackage": codepackage},
             data=data,
             headers={"Authorization": f"Bearer {config.access_token}"},
         )
 
     if response.status_code in (200, 202):
         console.print("Waiting for build job to complete")
@@ -175,15 +188,17 @@
         console.print(f"Error: received status code {response.status_code}")
         print(response.text)
 
     os.unlink("source.tar.gz")
 
 
 def _get_new_logs(old_logs: list[str], current_logs: str) -> list[str]:
-    current_logs_list = current_logs.rstrip("\n").split("\n")  # rstrip \n, to prevent empty lines
+    current_logs_list = current_logs.rstrip("\n").split(
+        "\n"
+    )  # rstrip \n, to prevent empty lines
     common_index = len(old_logs)
     return current_logs_list[common_index:]
 
 
 def _wait_for_job(job_id: str, sleep_time: int = 5) -> bool:
     log_lines: list[str] = []
     while True:
```

### Comparing `contactsoftware_functions_client-0.4.2/pyproject.toml` & `contactsoftware_functions_client-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "contactsoftware-functions-client"
-version = "0.4.2"
+version = "0.5.1"
 readme = "README.md"
 license = "MIT"
 authors = [
-    "Julian Alberts <jal@contact.de>",
-    "Jens Kürten <jku@contact.de>"
+    "Jens Kürten <jku@contact.de>",
+    "Julian Alberts <jal@contact.de>"
 ]
 description = "Client for uploading and managing Functions in CIM Database Cloud."
 
 packages = [
     { include = "cfc"}
    ]
```

