# Comparing `tmp/porgo-1.0.0-py3-none-any.whl.zip` & `tmp/porgo-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5467 bytes, number of entries: 9
+Zip file size: 5512 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      225 b- defN 24-Mar-23 13:55 porgo/__init__.py
 -rw-rw-rw-  2.0 fat      157 b- defN 24-Mar-21 07:37 porgo/_typing.py
--rw-rw-rw-  2.0 fat       57 b- defN 24-Mar-21 07:04 porgo/_version.py
--rw-rw-rw-  2.0 fat     4060 b- defN 24-Mar-24 11:30 porgo/runtime.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-Mar-24 11:34 porgo-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3294 b- defN 24-Mar-24 11:34 porgo-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-24 11:34 porgo-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Mar-24 11:34 porgo-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      665 b- defN 24-Mar-24 11:34 porgo-1.0.0.dist-info/RECORD
-9 files, 9645 bytes uncompressed, 4331 bytes compressed:  55.1%
+-rw-rw-rw-  2.0 fat       57 b- defN 24-Apr-09 10:19 porgo/_version.py
+-rw-rw-rw-  2.0 fat     4193 b- defN 24-Apr-09 10:35 porgo/runtime.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3285 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      665 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/RECORD
+9 files, 9769 bytes uncompressed, 4376 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: porgo/_version.py
 Comment: 
 
 Filename: porgo/runtime.py
 Comment: 
 
-Filename: porgo-1.0.0.dist-info/LICENSE
+Filename: porgo-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: porgo-1.0.0.dist-info/METADATA
+Filename: porgo-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: porgo-1.0.0.dist-info/WHEEL
+Filename: porgo-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: porgo-1.0.0.dist-info/top_level.txt
+Filename: porgo-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: porgo-1.0.0.dist-info/RECORD
+Filename: porgo-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porgo/_version.py

```diff
@@ -1,3 +1,3 @@
 # Copyright (c) 2024 linjing-lab
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

## porgo/runtime.py

```diff
@@ -19,14 +19,15 @@
         assert recombination > 0 and recombination < 1
         self.obj = objective_function
         self.scale = len(bounds) # the dimension of objective_function
         assert self.scale > 0
         assert all(map(lambda x: isinstance(x, (List, Tuple)), bounds))
         if not isinstance(bounds, NUMPY_NDARRAY):
             self.bounds = numpy.array(bounds)
+        assert numpy.all(self.bounds[:,0] < self.bounds[:,1]), 'Search bounds use the form as [[-10, 10]] * 3 or [(-10, 10)] * 3.'
         self.F = mutation
         self.CR = recombination
 
     def _tri_cr(self, pop_ind: int) -> None:
         '''
         Update target population by `self.CR`.
         :param pop_ind: int. the sequential population number.
@@ -58,15 +59,15 @@
         '''
         Use `random` module to generate the range distribution of population.
         :param population_size: int. the size of population. default: 50.
         :param verbose: bool. whether to output initial population. default: False.
         '''
         assert population_size > 0
         self.population_size: int = population_size
-        self.uniform = numpy.random.uniform(self.bounds[:,0], self.bounds[:,1], (self.population_size, self.scale)) # relace with another initial pattern
+        self.uniform = numpy.random.uniform(self.bounds[:,0], self.bounds[:,1], (self.population_size, self.scale)) # replace with another initial pattern
         if verbose:
             print(self.uniform)
 
     def train_gen(self, cycles: int=1000):
         '''
         Configure the numbers of generations to accelerate convergence.
         :param cycles: int. set the times of train_gen. default: 1000.
```

## Comparing `porgo-1.0.0.dist-info/LICENSE` & `porgo-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porgo-1.0.0.dist-info/METADATA` & `porgo-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porgo
-Version: 1.0.0
+Version: 1.0.1
 Summary: The portable universal library in global optimization.
 Home-page: https://github.com/linjing-lab/porgo
 Download-URL: https://github.com/linjing-lab/porgo/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/porgo/tree/master/porgo/
@@ -33,24 +33,24 @@
 
 When I was researching a function without given all local minima, like the underlined function:
 
 $$
 f(x)=\sum_{i=1}^{n/2}(-13+x_{2i-1}+((5-x_{2i})x_{2i}-2)x_{2i})^2+(-29+x_{2i-1}+((x_{2i}+1)x_{2i}-14)x_{2i})^2.
 $$
 
-I used `optimtool.unconstrain` to search local minma, got an efficient experience about searching the nearest minimum point. Add a mechanism to jump out of the local area would increase the runtime of the whole script, so `porgo` is a new progam to accelerate to search global minma.
+I used `optimtool.unconstrain` to search local minima, got an efficient experience about searching the nearest minimum point. Add a mechanism to jump out of the local area would increase the runtime of the whole script, so `porgo` is a new progam to accelerate to search global minima.
 
-refer to [test.py](./test.py) and the global minma of 4-dimensional $f(x)$ is (5, 4, 5, 4).
+refer to test.py and the global minima of 4-dimensional $f(x)$ is (5, 4, 5, 4).
 
 ## glos
 
 glos is the main runtime to serve as a global search class, users can run train_gen module with given cycles at any times until the function searching process converged.
 
 init:
-- objective_function: *Callable*, a high-dimensional function with convex, non-convex, and many local minma.
+- objective_function: *Callable*, a high-dimensional function with convex, non-convex, and many local minima.
 - bounds: *List[List[float]] | List[Tuple[float]]*, changes this value makes a significant influence of best and best_fit.
 - mutation: *float=0.5*, increase this value makes the search radius larger.
 - recombination: *float=0.9*, increase this value allows larger number of mutation.
 
 rand_pop:
 - population_size: *int=50*, randomly init the population (or called initial points) with shape at (population, dimension).
 - verbose: *bool=False*, whether to output initial population when manually replace the random generated rule.
```

## Comparing `porgo-1.0.0.dist-info/RECORD` & `porgo-1.0.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 porgo/__init__.py,sha256=38xCrK8ms2668EMOzga_pryhdruIgnMdKXzskCKP3mg,225
 porgo/_typing.py,sha256=mGwg2-1CTe39GGslsJr4VTHcK0FQbECOh5Bx2JBwWgA,157
-porgo/_version.py,sha256=mkm9pnUO65paBFSUplsO7A2Ek3rE1eOoa_hbeKLrweg,57
-porgo/runtime.py,sha256=x2_h12EbT9paAQEK3euDdqwDW-_emLin5qQPmcplLm8,4060
-porgo-1.0.0.dist-info/LICENSE,sha256=6tZMvmRANwvfuPHCTWM4gS9MHtQFReXNH_yqQFVRqlw,1089
-porgo-1.0.0.dist-info/METADATA,sha256=ih98d3-FM2FdrKY6uOp6QDIRFyPk4YbJJc-KlTsfTEI,3294
-porgo-1.0.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-porgo-1.0.0.dist-info/top_level.txt,sha256=rE9a1sFwUTPF1rtbHkyRSdCEK2q_yytJfKybWP8tMRo,6
-porgo-1.0.0.dist-info/RECORD,,
+porgo/_version.py,sha256=TJ5JaRCRguW7179mPLN9aTCOeZZJ6_tzBhnYU6SVlbY,57
+porgo/runtime.py,sha256=ZH2Yb365ikIkPO0uxhe4rgEjVZecj5naMa6bEkwDz84,4193
+porgo-1.0.1.dist-info/LICENSE,sha256=6tZMvmRANwvfuPHCTWM4gS9MHtQFReXNH_yqQFVRqlw,1089
+porgo-1.0.1.dist-info/METADATA,sha256=zj5EieBZ6jhjqNnS68IbIjnd6P7Ob0D26-RAbvOyja8,3285
+porgo-1.0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+porgo-1.0.1.dist-info/top_level.txt,sha256=rE9a1sFwUTPF1rtbHkyRSdCEK2q_yytJfKybWP8tMRo,6
+porgo-1.0.1.dist-info/RECORD,,
```

