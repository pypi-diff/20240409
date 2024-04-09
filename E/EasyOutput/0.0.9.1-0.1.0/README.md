# Comparing `tmp/easyoutput-0.0.9.1.tar.gz` & `tmp/easyoutput-0.1.0.tar.gz`

## Comparing `easyoutput-0.0.9.1.tar` & `easyoutput-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/README.MD
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/.github/ISSUE_TEMPLATE/🐞-bug-report.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/.github/ISSUE_TEMPLATE/🚀feature-request.md
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/img/EasyOutputSmallLogo.png
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/src/EasyOutput/EasyOutput.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/src/EasyOutput/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/tests/test.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 easyoutput-0.0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.0/README.MD
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🚀feature-request.md
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 easyoutput-0.1.0/img/EasyOutputSmallLogo.png
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 easyoutput-0.1.0/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.1.0/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 easyoutput-0.1.0/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 easyoutput-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 easyoutput-0.1.0/PKG-INFO
```

### Comparing `easyoutput-0.0.9.1/README.MD` & `easyoutput-0.1.0/README.MD`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,68 @@
 # Easy Output 
 ```py 
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
-![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&color=55%2C%20117%2C%20169)
+![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)
+> [!IMPORTANT]
+> I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
-![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
+## Information
+**EasyOutput** consists of easy colored print options without the extra work.
+
+```py
+# You can now highlight your message aswell! 
+Success_Message("New Highlight!", highlight=True)
+
+# Or keep it og 😄
+Success_Message("No Highlight!")
+# Same as
+Success_Message("No Highlight!", highlight=False)
+
+# As of v0.1.0 you can now change the color of your text.
+from EasyOutput.EasyOutput import Colors, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green)
+```
+
+In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+```py
+from colorama import Fore, Style
+
+def Success(message):
+    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+
+print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+# and calling it like so
+
+Success("Your Success Message")
+```
+
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+
+## Important Information 🥇
+[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
+
+[Jonathan Hartley](https://github.com/tartley)\
+[colorama repo](https://github.com/tartley/colorama)
+
+## PYPI
+
+[EasyOutput](https://pypi.org/project/EasyOutput/)
+
+
+Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
 [comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
@@ -127,67 +176,7 @@
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
 </details>
 
 </details>
-
-# Information
-**EasyOutput** consists of easy colored print options without the hassle of doing
-```py
-from colorama import Fore, Style
-
-def Success(message):
-    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
-
-# and calling it like so
-
-Success("Your Success Message")
-
-
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-```
-
-In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
-
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
-Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
-
-[Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
-[Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
-
-**Updating as much as I can!**
-# Functions
-
-### Success
-**Use:**
-```py
-Success_Message("EasyOutput")
-
-```
-**Shows:**
-
-Success: EasyOutput 
-
-### Error
-**Use:**
-```py
-Error_Message("EasyOutput")
-
-```
-**Shows:**
-
-Error: EasyOutput 
-
-## PYPI
-
-[EasyOutput](https://pypi.org/project/EasyOutput/)
-
-
-Badges from: [Shields.io](https://shields.io/badges)
```

### Comparing `easyoutput-0.0.9.1/.github/ISSUE_TEMPLATE/🚀feature-request.md` & `easyoutput-0.1.0/.github/ISSUE_TEMPLATE/🚀feature-request.md`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.9.1/img/EasyOutputSmallLogo.png` & `easyoutput-0.1.0/img/EasyOutputSmallLogo.png`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.9.1/LICENSE.txt` & `easyoutput-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.9.1/README.md` & `easyoutput-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,68 @@
 # Easy Output 
 ```py 
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
-![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&color=55%2C%20117%2C%20169)
+![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)
+> [!IMPORTANT]
+> I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
-![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
+## Information
+**EasyOutput** consists of easy colored print options without the extra work.
+
+```py
+# You can now highlight your message aswell! 
+Success_Message("New Highlight!", highlight=True)
+
+# Or keep it og 😄
+Success_Message("No Highlight!")
+# Same as
+Success_Message("No Highlight!", highlight=False)
+
+# As of v0.1.0 you can now change the color of your text.
+from EasyOutput.EasyOutput import Colors, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green)
+```
+
+In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+```py
+from colorama import Fore, Style
+
+def Success(message):
+    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+
+print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+# and calling it like so
+
+Success("Your Success Message")
+```
+
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+
+## Important Information 🥇
+[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
+
+[Jonathan Hartley](https://github.com/tartley)\
+[colorama repo](https://github.com/tartley/colorama)
+
+## PYPI
+
+[EasyOutput](https://pypi.org/project/EasyOutput/)
+
+
+Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
 [comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
@@ -127,67 +176,7 @@
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
 </details>
 
 </details>
-
-# Information
-**EasyOutput** consists of easy colored print options without the hassle of doing
-```py
-from colorama import Fore, Style
-
-def Success(message):
-    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
-
-# and calling it like so
-
-Success("Your Success Message")
-
-
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-```
-
-In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
-
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
-Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
-
-[Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
-[Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
-
-**Updating as much as I can!**
-# Functions
-
-### Success
-**Use:**
-```py
-Success_Message("EasyOutput")
-
-```
-**Shows:**
-
-Success: EasyOutput 
-
-### Error
-**Use:**
-```py
-Error_Message("EasyOutput")
-
-```
-**Shows:**
-
-Error: EasyOutput 
-
-## PYPI
-
-[EasyOutput](https://pypi.org/project/EasyOutput/)
-
-
-Badges from: [Shields.io](https://shields.io/badges)
```

### Comparing `easyoutput-0.0.9.1/pyproject.toml` & `easyoutput-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyOutput"
-version = "0.0.9.1"
+version = "0.1.0"
 authors = [
   { name="FrankAustin", email="frankaustindev808@gmail.com" },
 ]
 description = "Colored messages in the palm of your hand"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 keywords = [
-  "Error Message", "Success Message", "Warning Message", "Easy"
+  "Error Message", "Success Message", "Warning Message", "Easy", "Colored Messages"
 ]
 maintainers = [
   {name = "FrankAustin", email="frankaustindev808@gmail.com"}
 ]
 requires-python = ">=3.12"
 install_requires= ['colorama']
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
+    "License :: Freeware",
     "Operating System :: Unix",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
   "colorama"
 ]
```

### Comparing `easyoutput-0.0.9.1/PKG-INFO` & `easyoutput-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: EasyOutput
-Version: 0.0.9.1
+Version: 0.1.0
 Summary: Colored messages in the palm of your hand
 Project-URL: Homepage, https://github.com/FrankAustin808/EasyOut/
 Project-URL: Issues, https://github.com/FrankAustin808/EasyOut/issues/new/choose
 Project-URL: Feature Request, https://github.com/FrankAustin808/EasyOut/issues/new/choose
 Author-email: FrankAustin <frankaustindev808@gmail.com>
 Maintainer-email: FrankAustin <frankaustindev808@gmail.com>
 License: MIT License
@@ -25,37 +25,87 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE.txt
-Keywords: Easy,Error Message,Success Message,Warning Message
+Keywords: Colored Messages,Easy,Error Message,Success Message,Warning Message
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: Freeware
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Requires-Dist: colorama
 Description-Content-Type: text/markdown
 
 # Easy Output 
 ```py 
 # How to use 👽
 from EasyOutput.EasyOutput import *
 ```
-![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&color=55%2C%20117%2C%20169)
+![PyPI - Version](https://img.shields.io/pypi/v/EasyOutput?style=for-the-badge&logo=pypi&label=EasyOutput&color=55%2C%20117%2C%20169)\
+![PyPI - Downloads](https://img.shields.io/pypi/dm/EasyOutput?style=for-the-badge&logo=pypi&label=Monthly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dw/EasyOutput?style=for-the-badge&logo=pypi&label=Weekly%20Downloads&color=358)\
+![PyPI - Downloads](https://img.shields.io/pypi/dd/EasyOutput?style=for-the-badge&logo=pypi&label=Daily%20Downloads&color=358)\
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)\
+![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/FrankAustin808/EasyOutput?style=for-the-badge&logo=github)
+> [!IMPORTANT]
+> I am always updating this and sometimes those updates can go sideways. Please use the [issues](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) section on github to notify me of anything i have missed! If you would like me to add something, please use the [Feature Request](https://github.com/FrankAustin808/EasyOutput/issues/new/choose) option!
 
-![easyoutput](https://i.gyazo.com/e8c1bb4fe08ade9c2ce6856386f48e1f.png)
 
+## Information
+**EasyOutput** consists of easy colored print options without the extra work.
+
+```py
+# You can now highlight your message aswell! 
+Success_Message("New Highlight!", highlight=True)
+
+# Or keep it og 😄
+Success_Message("No Highlight!")
+# Same as
+Success_Message("No Highlight!", highlight=False)
+
+# As of v0.1.0 you can now change the color of your text.
+from EasyOutput.EasyOutput import Colors, Success_Message
+
+Success_Message("EasyOutput", color=Colors.Green)
+```
+
+In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing:
+```py
+from colorama import Fore, Style
+
+def Success(message):
+    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+
+print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
+# and calling it like so
+
+Success("Your Success Message")
+```
+
+If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal! 
+
+## Important Information 🥇
+[colorama](https://pypi.org/project/colorama/) and It's creator has done all heavy lifting here please show him some love!
+
+[Jonathan Hartley](https://github.com/tartley)\
+[colorama repo](https://github.com/tartley/colorama)
+
+## PYPI
+
+[EasyOutput](https://pypi.org/project/EasyOutput/)
+
+
+Badges from: [Shields.io](https://shields.io/badges)
 
 <details>
 <summary>Change-Log 📝</summary>
 
 [comment]: <> (v0.0.1)
 <details>
 <summary>v0.0.1</summary>
@@ -169,67 +219,7 @@
 <summary>v0.0.9.1</summary>
 
     FIXED
     - Info message oddly popping up after every function
 </details>
 
 </details>
-
-# Information
-**EasyOutput** consists of easy colored print options without the hassle of doing
-```py
-from colorama import Fore, Style
-
-def Success(message):
-    print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: {message}")
-
-# and calling it like so
-
-Success("Your Success Message")
-
-
-# You can now highlight your message aswell! 
-Success_Message("New Highlight!", highlight=True)
-
-# Or keep it og 😄
-Success_Message("No Highlight!")
-# Same as
-Success_Message("No Highlight!", highlight=False)
-```
-
-In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
-
-If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
-Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
-
-[Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
-[Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
-
-**Updating as much as I can!**
-# Functions
-
-### Success
-**Use:**
-```py
-Success_Message("EasyOutput")
-
-```
-**Shows:**
-
-Success: EasyOutput 
-
-### Error
-**Use:**
-```py
-Error_Message("EasyOutput")
-
-```
-**Shows:**
-
-Error: EasyOutput 
-
-## PYPI
-
-[EasyOutput](https://pypi.org/project/EasyOutput/)
-
-
-Badges from: [Shields.io](https://shields.io/badges)
```

