# Comparing `tmp/automathon-0.0.8.tar.gz` & `tmp/automathon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automathon-0.0.8.tar", last modified: Thu Mar 31 15:48:46 2022, max compression
+gzip compressed data, was "automathon-0.0.9.tar", last modified: Fri Apr  1 02:27:10 2022, max compression
```

## Comparing `automathon-0.0.8.tar` & `automathon-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-03-31 15:48:46.753250 automathon-0.0.8/
--rw-rw-rw-   0        0        0    18432 2021-07-16 07:33:30.000000 automathon-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    11699 2022-03-31 15:48:46.754241 automathon-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10896 2021-07-20 15:56:03.000000 automathon-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-03-31 15:48:46.696242 automathon-0.0.8/automathon/
--rw-rw-rw-   0        0        0       74 2021-07-17 02:19:02.000000 automathon-0.0.8/automathon/__init__.py
--rw-rw-rw-   0        0        0      311 2022-03-31 15:43:05.000000 automathon-0.0.8/automathon/__version__.py
-drwxrwxrwx   0        0        0        0 2022-03-31 15:48:46.745245 automathon-0.0.8/automathon/errors/
--rw-rw-rw-   0        0        0       49 2021-07-16 07:33:30.000000 automathon-0.0.8/automathon/errors/__init__.py
--rw-rw-rw-   0        0        0      847 2021-07-16 07:33:30.000000 automathon-0.0.8/automathon/errors/errors.py
-drwxrwxrwx   0        0        0        0 2022-03-31 15:48:46.752243 automathon-0.0.8/automathon/finiteAutomata/
--rw-rw-rw-   0        0        0       42 2021-07-16 07:33:30.000000 automathon-0.0.8/automathon/finiteAutomata/__init__.py
--rw-rw-rw-   0        0        0     7171 2021-07-20 15:45:31.000000 automathon-0.0.8/automathon/finiteAutomata/dfa.py
--rw-rw-rw-   0        0        0    11520 2022-03-31 15:48:02.000000 automathon-0.0.8/automathon/finiteAutomata/nfa.py
-drwxrwxrwx   0        0        0        0 2022-03-31 15:48:46.724245 automathon-0.0.8/automathon.egg-info/
--rw-rw-rw-   0        0        0    11699 2022-03-31 15:48:46.000000 automathon-0.0.8/automathon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2022-03-31 15:48:46.000000 automathon-0.0.8/automathon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-31 15:48:46.000000 automathon-0.0.8/automathon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-03-31 15:48:46.000000 automathon-0.0.8/automathon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-31 15:48:46.000000 automathon-0.0.8/automathon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-03-31 15:48:46.758246 automathon-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1440 2022-03-31 15:43:49.000000 automathon-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-01 02:27:10.873890 automathon-0.0.9/
+-rw-rw-rw-   0        0        0    18432 2021-07-16 07:33:30.000000 automathon-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    11699 2022-04-01 02:27:10.873890 automathon-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10896 2021-07-20 15:56:03.000000 automathon-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-04-01 02:27:10.792892 automathon-0.0.9/automathon/
+-rw-rw-rw-   0        0        0       74 2021-07-17 02:19:02.000000 automathon-0.0.9/automathon/__init__.py
+-rw-rw-rw-   0        0        0      311 2022-04-01 02:25:45.000000 automathon-0.0.9/automathon/__version__.py
+drwxrwxrwx   0        0        0        0 2022-04-01 02:27:10.865890 automathon-0.0.9/automathon/errors/
+-rw-rw-rw-   0        0        0       49 2021-07-16 07:33:30.000000 automathon-0.0.9/automathon/errors/__init__.py
+-rw-rw-rw-   0        0        0      847 2021-07-16 07:33:30.000000 automathon-0.0.9/automathon/errors/errors.py
+drwxrwxrwx   0        0        0        0 2022-04-01 02:27:10.872887 automathon-0.0.9/automathon/finiteAutomata/
+-rw-rw-rw-   0        0        0       42 2021-07-16 07:33:30.000000 automathon-0.0.9/automathon/finiteAutomata/__init__.py
+-rw-rw-rw-   0        0        0     7171 2022-04-01 02:16:24.000000 automathon-0.0.9/automathon/finiteAutomata/dfa.py
+-rw-rw-rw-   0        0        0    11458 2022-04-01 02:20:55.000000 automathon-0.0.9/automathon/finiteAutomata/nfa.py
+drwxrwxrwx   0        0        0        0 2022-04-01 02:27:10.845886 automathon-0.0.9/automathon.egg-info/
+-rw-rw-rw-   0        0        0    11699 2022-04-01 02:27:10.000000 automathon-0.0.9/automathon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2022-04-01 02:27:10.000000 automathon-0.0.9/automathon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-01 02:27:10.000000 automathon-0.0.9/automathon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2022-04-01 02:27:10.000000 automathon-0.0.9/automathon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-04-01 02:27:10.000000 automathon-0.0.9/automathon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-04-01 02:27:10.877891 automathon-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1440 2022-04-01 02:26:10.000000 automathon-0.0.9/setup.py
```

### Comparing `automathon-0.0.8/LICENSE` & `automathon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automathon-0.0.8/PKG-INFO` & `automathon-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: automathon
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for simulating and visualizing finite automata
 Home-page: https://github.com/rohaquinlop/automathon
 Author: Robin Hafid Quintero Lopez
 Author-email: rohaquinlop301@gmail.com
 License: GNU General Public License v2.0
-Download-URL: https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.8.tar.gz
+Download-URL: https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.9.tar.gz
 Keywords: python,automata,automata,automathon
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automathon-0.0.8/README.md` & `automathon-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `automathon-0.0.8/automathon/errors/errors.py` & `automathon-0.0.9/automathon/errors/errors.py`

 * *Files identical despite different names*

### Comparing `automathon-0.0.8/automathon/finiteAutomata/dfa.py` & `automathon-0.0.9/automathon/finiteAutomata/dfa.py`

 * *Files identical despite different names*

### Comparing `automathon-0.0.8/automathon/finiteAutomata/nfa.py` & `automathon-0.0.9/automathon/finiteAutomata/nfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,26 +226,18 @@
           
           if sigma != '':
             deltaPrime[q][sigma] = newTransitions
     
     return NFA(Qprime, self.sigma, deltaPrime, deltaInitState, deltaF)
   
   def getDFA(self) -> DFA:
-    """Convert the actual NFA to DFA and return it's conversion"""
+    """Convert the actual NFA to DFA and return its conversion"""
     
     localNFA = NFA(self.Q, self.sigma, self.delta, self.initialState, self.F)
-    flag = False
-    
-    ##verify if have epsilon transitions
-    for q in self.Q:
-      if q in self.delta and not flag:
-        for transitionValue in self.delta[q]:
-          if transitionValue == '' and not flag:
-            localNFA = self.removeEpsilonTransitions()
-            flag = True
+    localNFA = localNFA.removeEpsilonTransitions()
     
     Qprime = []
     deltaPrime = dict()
     
     queue = deque()
     visited = [[localNFA.initialState]]
     queue.append([localNFA.initialState])
@@ -255,19 +247,20 @@
       
       T = dict()  ## {str : list}
       
       for q in qs:
         if q in localNFA.delta:
           for s in localNFA.delta[q]:
             tmp = localNFA.delta[q][s].copy()
-            if s in T:
-              ## avoid add repeated values
-              T[s].extend([k for k in tmp if k not in T[s]])
-            else:
-              T[s] = tmp
+            if tmp:
+              if s in T:
+                ## avoid add repeated values
+                T[s].extend([k for k in tmp if k not in T[s]])
+              else:
+                T[s] = tmp
       
       for t in T:
         T[t].sort()
         tmp = T[t].copy()
         if tmp not in visited:
           queue.append(tmp)
           visited.append(tmp)
@@ -289,14 +282,19 @@
     for qs in Qprime:
       aux.add(str(qs))
     
     Qprime = aux
     
     return DFA(Qprime, localNFA.sigma, deltaPrime, str([localNFA.initialState]), Fprime)
   
+  def minimize(self):
+    """Minimize the automata and return the result of the minimization"""
+    localDFA = self.getDFA()
+    return localDFA.getNFA()
+  
   def union(self, M: 'NFA') -> 'NFA':
     """Given a NFA M returns the union automaton"""
     sigma = self.sigma.union(M.sigma)
     Q = set()
     F = set()
     initialState = "q0"
     Q.add(initialState)
```

### Comparing `automathon-0.0.8/automathon.egg-info/PKG-INFO` & `automathon-0.0.9/automathon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: automathon
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for simulating and visualizing finite automata
 Home-page: https://github.com/rohaquinlop/automathon
 Author: Robin Hafid Quintero Lopez
 Author-email: rohaquinlop301@gmail.com
 License: GNU General Public License v2.0
-Download-URL: https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.8.tar.gz
+Download-URL: https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.9.tar.gz
 Keywords: python,automata,automata,automathon
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automathon-0.0.8/setup.py` & `automathon-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 with open(path.join(thisDirectory, 'README.md'), encoding='utf-8') as f:
   longDescription = f.read()
 
 setup(
     name="automathon",
     packages=find_packages(include=['automathon', 'automathon.finiteAutomata', 'automathon.errors']),
     include_package_data=True,
-    version='0.0.8',
+    version='0.0.9',
     description="A Python library for simulating and visualizing finite automata",
     long_description=longDescription,
     long_description_content_type="text/markdown",
     author="Robin Hafid Quintero Lopez",
     license="GNU General Public License v2.0",
     install_requires=['graphviz==0.16'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==4.4.1', 'graphviz==0.16'],
     test_suite='tests',
     author_email='rohaquinlop301@gmail.com',
     url='https://github.com/rohaquinlop/automathon',
-    download_url="https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.8.tar.gz",
+    download_url="https://github.com/rohaquinlop/automathon/archive/refs/tags/v0.0.9.tar.gz",
     keywords=["python", "automata", "automata", "automathon"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3'
```

