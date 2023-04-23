# Comparing `tmp/bhv-0.2.3.tar.gz` & `tmp/bhv-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.3.tar", last modified: Thu Apr 20 22:30:47 2023, max compression
+gzip compressed data, was "bhv-0.2.4.tar", last modified: Sun Apr 23 18:45:46 2023, max compression
```

## Comparing `bhv-0.2.3.tar` & `bhv-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-20 22:30:47.164835 bhv-0.2.3/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3038 2023-04-18 21:57:32.000000 bhv-0.2.3/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.3/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12037 2023-04-18 17:15:37.000000 bhv-0.2.3/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.3/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.3/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.3/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-17 15:03:13.000000 bhv-0.2.3/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9164 2023-04-17 13:54:04.000000 bhv-0.2.3/bhv/symbolic.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-20 22:30:47.164835 bhv-0.2.3/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      256 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-20 22:30:47.000000 bhv-0.2.3/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-20 22:30:47.164835 bhv-0.2.3/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-20 22:29:22.000000 bhv-0.2.3/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.4/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-23 18:45:46.086419 bhv-0.2.4/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3142 2023-04-23 18:45:24.000000 bhv-0.2.4/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.4/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11929 2023-04-21 10:02:48.000000 bhv-0.2.4/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.4/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.4/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.4/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-17 15:03:13.000000 bhv-0.2.4/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13150 2023-04-23 16:54:25.000000 bhv-0.2.4/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      633 2023-04-23 18:40:01.000000 bhv-0.2.4/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      285 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-23 18:45:46.086419 bhv-0.2.4/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-23 18:17:55.000000 bhv-0.2.4/setup.py
```

### Comparing `bhv-0.2.3/PKG-INFO` & `bhv-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.3
+Version: 0.2.4
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,9 +18,10 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
+License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.2.3/README.md` & `bhv-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 - zscore and pvalue
 
 Additionally, provided are
 - A symbolic implementation with plotting and pretty printing
 - Efficient bit-packed representation
 - Three redundant implementations on NumPy for performance and correctness
 - A minimal abstraction for permutations with caching and composition
-- Very basic embeddings for other datatypes (more to come) 
+- Very basic embeddings for other datatypes (more to come)
+- Graph visualization of distances in hyperdimensional space ([see example](examples/viz_distances.py)).
 
 ## Installation
 `pip install bhv`
 
 If you only want to work with the symbolic implementation, you're good to go with `from bhv.symbolic import Var, SymbolicBHV`.
 
 Else you'll need
@@ -42,12 +43,12 @@
 - [Finite State Machine example](examples/state_machine.py)
 - [The base class AbstractBHV](bhv/abstract.py)
 - [The most idiomatic implementation NumPyBoolBHV](bhv/np.py)
 
 If you're comming at this from a Machine Learning angle, you may enjoy:
 - [A minimal implementation](examples/winnow_classification.py) of the [winnow algorithm](https://en.wikipedia.org/wiki/Winnow_(algorithm)) on a minimal problem
 - [A minimal implementation of classification based on the majority operator](examples/majority_classification.py) on a minimal problem
-- [A Google Colab hosted MNIST classification via plain majority notebook](https://colab.research.google.com/drive/1xYQAXxcdFw89RV5CsflcvFhx3zpmEUxk?usp=sharing)
+- [A Google Colab hosted digit classification via plain majority notebook](https://colab.research.google.com/drive/1xYQAXxcdFw89RV5CsflcvFhx3zpmEUxk?usp=sharing)
 
 ## Note
 This repository is highly active, and a work-in-progress.
 Do expect changes to the naming, and even features to be swapped for more elegant alternatives.
```

### Comparing `bhv-0.2.3/bhv/abstract.py` & `bhv-0.2.4/bhv/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,17 +147,14 @@
 
     def __invert__(self) -> Self:
         raise NotImplementedError()
 
     def select(self, when1: Self, when0: Self) -> Self:
         return when0 ^ (self & (when0 ^ when1))
 
-    def mix(self, other: Self, pick_l=0.5) -> Self:
-        return self.random(pick_l).select(self, other)
-
     def active(self) -> int:
         raise NotImplementedError()
 
     def bias_rel(self, other: Self, rel: Self) -> float:
         rel_l = rel.select(self, self.ZERO).active()
         rel_r = rel.select(other, self.ZERO).active()
         return rel_l / (rel_l + rel_r)
```

### Comparing `bhv-0.2.3/bhv/embedding.py` & `bhv-0.2.4/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.3/bhv/np.py` & `bhv-0.2.4/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.3/bhv/pytorch.py` & `bhv-0.2.4/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.3/bhv/shared.py` & `bhv-0.2.4/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.3/bhv/symbolic.py` & `bhv-0.2.4/bhv/symbolic.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def nodename(self, **kwargs):
         return f"{type(self).__name__.upper()}"
 
     def nodeid(self, structural=False, **kwargs):
         return f"{type(self).__name__}{stable_hashcode(self).replace('-', '') if structural else str(id(self))}"
 
     def children(self, **kwargs):
-        return [(getattr(self, f.name), f.name) for f in fields(self) if issubclass(f.type, Symbolic)]
+        return [(getattr(self, f.name), f.name) for f in fields(self) if type(f.type) is type and issubclass(f.type, Symbolic)]
 
     def graphviz(self, structural=False, done=None, **kwargs):
         noden = self.nodeid(structural, **kwargs)
         if done is None:
             done = set()
         if noden in done:
             return
@@ -32,14 +32,35 @@
         Shows the expression tree code-style.
         Only works on referentially transparent DAGs.
         :param kwargs: drawing options
         :return: str
         """
         raise NotImplementedError()
 
+    def instantiate(self, **kwargs):
+        raise NotImplementedError()
+
+    def execute(self, random: 'dict[int, AbstractBHV]' = None,
+                rand2: 'dict[int, AbstractBHV]' = None,
+                rand: 'dict[int, AbstractBHV]' = None,
+                randomperms: 'dict[int, MemoizedPermutation]' = None,
+                calculated = None, **kwargs):
+        if random is None: random = {}
+        if rand2 is None: rand2 = {}
+        if rand is None: rand = {}
+        if randomperms is None: randomperms = {}
+        if calculated is None: calculated = {}
+        kwargs |= dict(random=random, rand2=rand2, rand=rand, randomperms=randomperms, calculated=calculated)
+        if id(self) in calculated:
+            return calculated[id(self)]
+        else:
+            result = self.instantiate(**kwargs)
+            calculated[id(self)] = result
+            return result
+
 
 class SymbolicPermutation(Symbolic, MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
 
     @classmethod
     def random(cls) -> 'SymbolicPermutation':
         return PermRandom()
@@ -55,52 +76,68 @@
 
 @dataclass
 class PermVar(SymbolicPermutation):
     name: str
     def nodename(self, **kwargs):
         return self.name
 
-    def show(self, symbolic_var=False, **kwargs):
+    def show(self, **kwargs):
+        symbolic_var = kwargs.get("symbolic_var", False)
         return f"ParmVar(\"{self.name}\")" if symbolic_var else self.name
-@dataclass
-class PermUnit(SymbolicPermutation):
-    def show(self, impl="", **kwargs):
-        return impl + "UNIT"
-SymbolicPermutation.UNIT = PermUnit()
+
+    def instantiate(self, **kwargs):
+        permvars = kwargs.get("permvars")
+        if permvars is None:
+            raise RuntimeError(f"No Perm vars supplied but tried to instantiate `{self.name}`")
+        elif self.name not in permvars:
+            raise RuntimeError(f"Perm var `{self.name}` not in permvars ({set(permvars.keys())})")
+        else:
+            return permvars[self.name]
 randpermid = 0
 def next_perm_id():
     global randpermid
     randpermid += 1
     return randpermid
 @dataclass
 class PermRandom(SymbolicPermutation):
     id: int = field(default_factory=next_perm_id)
 
-    def show(self, impl="", random_id=False, **kwargs):
+    def show(self, **kwargs):
+        impl = kwargs.get("impl", "")
+        random_id = kwargs.get("random_id", False)
         return f"<{impl}random {self.id}>" if random_id else impl + "random()"
+
+    def instantiate(self, **kwargs):
+        randomperms = kwargs.get("randomperms")
+        if self.id in randomperms:
+            return randomperms[self.id]
+        else:
+            r = kwargs.get("perm").random()
+            randomperms[self.id] = r
+            return r
 @dataclass
 class PermCompose(SymbolicPermutation):
-    l: 'SymbolicPermutation'
-    r: 'SymbolicPermutation'
+    l: SymbolicPermutation
+    r: SymbolicPermutation
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} * {self.r.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs) * self.r.execute(**kwargs)
 @dataclass
 class PermInvert(SymbolicPermutation):
-    p: 'SymbolicPermutation'
+    p: SymbolicPermutation
 
     def show(self, **kwargs):
         return f"(~{self.p.show(**kwargs)})"
-@dataclass
-class PermApply(SymbolicPermutation):
-    p: 'SymbolicPermutation'
-    v: 'SymbolicBHV'
 
-    def show(self, **kwargs):
-        return f"{self.p.show(**kwargs)}({self.v.show(**kwargs)})"
+    def instantiate(self, **kwargs):
+        return ~self.p.execute(**kwargs)
+
 
 class SymbolicBHV(Symbolic, AbstractBHV):
     @classmethod
     def rand(cls) -> Self:
         return Rand()
 
     @classmethod
@@ -138,181 +175,258 @@
 
     def __invert__(self) -> Self:
         return Invert(self)
 
     def select(self, when1: Self, when0: Self) -> Self:
         return Select(self, when0, when1)
 
-    def mix(self, other: Self, pick_l=0.5) -> Self:
-        return Mix(pick_l, self, other)
-
     def active(self) -> int:
         return Active(self)
 
     def bias_rel(self, other: Self, rel: Self) -> float:
         return BiasRel(rel, self, other)
 
-    # def active_fraction(self) -> float:
-    #     return self.active()/DIMENSION
-    #
-    # def hamming(self, other: Self) -> int:
-    #     return (self ^ other).active()
-    #
-    # def bit_error_rate(self, other: Self) -> float:
-    #     return (self ^ other).active_fraction()
-    #
-    # def jaccard(self, other: Self) -> float:
-    #     return 1. - float((self & other).active()) / float((self | other).active() + 1E-7)
-    #
-    # def cosine(self, other: Self) -> float:
-    #     return 1 - float((self & other).active()) / float(self.active() * other.active() + 1E-7)**.5
-    #
-    # def zscore(self, other: Self) -> float:
-    #     p = 0.5
-    #     n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
-    #     return n.zscore(self.hamming(other))
-    #
-    # def pvalue(self, other: Self) -> float:
-    #     p = 0.5
-    #     n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
-    #     s = n.cdf(self.hamming(other))
-    #     return 2*min(s, 1 - s)
-    #
-    # def sixsigma(self, other: Self) -> bool:
-    #     return abs(self.zscore(other)) < 6
+    def unrelated(self, other: Self, stdvs=6) -> bool:
+        return Unrelated(self, other, stdvs)
 
+@dataclass
+class PermApply(SymbolicBHV):
+    p: SymbolicPermutation
+    v: SymbolicBHV
 
+    def show(self, **kwargs):
+        return f"{self.p.show(**kwargs)}({self.v.show(**kwargs)})"
 
+    def instantiate(self, **kwargs):
+        return self.p.execute(**kwargs)(self.v.execute(**kwargs))
 @dataclass
 class Var(SymbolicBHV):
     name: str
     def nodename(self, **kwards):
         return self.name
 
-    def show(self, symbolic_var=False, **kwargs):
+    def show(self, **kwargs):
+        symbolic_var = kwargs.get("symbolic_var", False)
         return f"Var(\"{self.name}\")" if symbolic_var else self.name
+
+    def instantiate(self, **kwargs):
+        vars = kwargs.get("vars")
+        if vars is None:
+            raise RuntimeError(f"No Perm vars supplied but tried to instantiate `{self.name}`")
+        elif self.name not in vars:
+            raise RuntimeError(f"Perm var `{self.name}` not in permvars ({set(vars.keys())})")
+        else:
+            return vars[self.name]
 @dataclass
 class Zero(SymbolicBHV):
-    def show(self, impl="", **kwargs):
-        return impl + "ZERO"
+    def show(self, **kwargs):
+        return kwargs.get("impl", "") + "ZERO"
+
+    def instantiate(self, bhv, **kwargs):
+        return kwargs.get("bhv").ZERO
 @dataclass
 class One(SymbolicBHV):
-    def show(self, impl="", **kwargs):
-        return impl + "ONE"
+    def show(self, **kwargs):
+        return kwargs.get("impl", "") + "ONE"
+
+    def instantiate(self, **kwargs):
+        return kwargs.get("bhv").ONE
 SymbolicBHV.ZERO = Zero()
 SymbolicBHV.ONE = One()
 randid = 0
 def next_id():
     global randid
     randid += 1
     return randid
 @dataclass
 class Rand(SymbolicBHV):
     id: int = field(default_factory=next_id)
 
-    def show(self, impl="", random_id=False, **kwargs):
+    def show(self, **kwargs):
+        impl = kwargs.get("impl", "")
+        random_id = kwargs.get("random_id", False)
         return f"<{impl}rand {self.id}>" if random_id else impl + "rand()"
+
+    def instantiate(self, **kwargs):
+        rand = kwargs.get("rand")
+        if self.id in rand:
+            return rand[self.id]
+        else:
+            r = kwargs.get("bhv").rand()
+            rand[self.id] = r
+            return r
 @dataclass
 class Rand2(SymbolicBHV):
     power: int
 
-    def show(self, impl="", **kwargs):
-        return impl + f"rand2({self.power})"
+    def show(self, **kwargs):
+        return kwargs.get("impl", "") + f"rand2({self.power})"
+
+    def instantiate(self, **kwargs):
+        rand2 = kwargs.get("rand2")
+        if self.id in rand2:
+            return rand2[self.id]
+        else:
+            r = kwargs.get("bhv").rand2()
+            rand2[self.id] = r
+            return r
 @dataclass
 class Random(SymbolicBHV):
     active: float
 
-    def show(self, impl="", **kwargs):
-        return impl + f"random({self.active})"
+    def show(self, **kwargs):
+        return kwargs.get("impl", "") + f"random({self.active})"
+
+    def instantiate(self, **kwargs):
+        random = kwargs.get("random")
+        if self.id in random:
+            return random[self.id]
+        else:
+            r = kwargs.get("bhv").random()
+            random[self.id] = r
+            return r
 @dataclass
 class Majority(SymbolicBHV):
     vs: list[SymbolicBHV]
 
-    def show(self, impl="", **kwargs):
-        return impl + f"majority({[v.show(**kwargs) for v in self.vs]})"
+    def children(self, **kwargs):
+        return list(zip(self.vs, map(str, range(len(self.vs)))))
+
+    def show(self, **kwargs):
+        return kwargs.get("impl", "") + f"majority({[v.show(**kwargs) for v in self.vs]})"
+
+    def instantiate(self, **kwargs):
+        return kwargs.get("bhv").majority([v.execute(**kwargs) for v in self.vs])
 @dataclass
 class Permute(SymbolicBHV):
     id: 'int | tuple[int, ...]'
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.permute({self.id})"
+
+    def instantiate(self, **kwargs):
+        return self.v.execute(**kwargs).permute(self.id)
 @dataclass
 class SwapHalves(SymbolicBHV):
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.swap_halves()"
+
+    def instantiate(self, **kwargs):
+        return self.v.execute(**kwargs).swap_halves()
 @dataclass
 class ReHash(SymbolicBHV):
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.rehash()"
+
+    def instantiate(self, **kwargs):
+        return self.v.execute(**kwargs).rehash()
 @dataclass
 class Eq:
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} == {self.r.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs) == self.r.execute(**kwargs)
 @dataclass
 class Xor(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} ^ {self.r.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs) ^ self.r.execute(**kwargs)
 @dataclass
 class And(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} & {self.r.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs) & self.r.execute(**kwargs)
 @dataclass
 class Or(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} | {self.r.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs) | self.r.execute(**kwargs)
 @dataclass
 class Invert(SymbolicBHV):
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"(~{self.v.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return ~self.v.execute(**kwargs)
 @dataclass
 class Select(SymbolicBHV):
     cond: SymbolicBHV
     when1: SymbolicBHV
     when0: SymbolicBHV
     def nodename(self, compact_select=True, **kwargs):
         return f"ON {self.cond.nodename()}" if compact_select else super().nodename(**kwargs)
     def children(self, compact_select=True, **kwargs):
-        return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().nodename(**kwargs)
+        return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().children(**kwargs)
 
     def show(self, **kwargs):
         return f"{self.cond.show(**kwargs)}.select({self.when1.show(**kwargs)}, {self.when0.show(**kwargs)})"
-@dataclass
-class Mix(SymbolicBHV):
-    frac: float
-    l: SymbolicBHV
-    r: SymbolicBHV
 
-    def show(self, **kwargs):
-        return f"{self.l.show(**kwargs)}.mix({self.r.show(**kwargs)}, {self.frac})"
+    def instantiate(self, **kwargs):
+        return self.cond.execute(**kwargs).select(self.when1.execute(**kwargs), self.when0.execute(**kwargs))
 @dataclass
-class Active(SymbolicBHV):
+class Active(Symbolic):
     v: SymbolicBHV
 
     def show(self, **kwargs):
         return f"{self.v.show(**kwargs)}.active()"
+
+    def instantiate(self, **kwargs):
+        return self.v.execute(**kwargs).active()
 @dataclass
 class BiasRel(SymbolicBHV):
     rel: SymbolicBHV
     l: SymbolicBHV
     r: SymbolicBHV
 
     def show(self, **kwargs):
-        return f"{self.l.show(**kwargs)}.mix({self.r.show(**kwargs)}, {self.rel.show(**kwargs)})"
+        return f"{self.l.show(**kwargs)}.bias_rel({self.r.show(**kwargs)}, {self.rel.show(**kwargs)})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs).bias_rel(self.r.execute(**kwargs), self.rel.execute(**kwargs))
+@dataclass
+class Related(Symbolic):
+    l: SymbolicBHV
+    r: SymbolicBHV
+    stdvs: float
+
+    def show(self, **kwargs):
+        return f"{self.l.show(**kwargs)}.related({self.r.show(**kwargs)}, {self.stdvs})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs).related(self.r.execute(**kwargs), self.stdvs)
+@dataclass
+class Unrelated(Symbolic):
+    l: SymbolicBHV
+    r: SymbolicBHV
+    stdvs: float
+
+    def show(self, **kwargs):
+        return f"{self.l.show(**kwargs)}.unrelated({self.r.show(**kwargs)}, {self.stdvs})"
+
+    def instantiate(self, **kwargs):
+        return self.l.execute(**kwargs).unrelated(self.r.execute(**kwargs), self.stdvs)
```

### Comparing `bhv-0.2.3/bhv.egg-info/PKG-INFO` & `bhv-0.2.4/bhv.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.3
+Version: 0.2.4
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,9 +18,10 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
+License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.2.3/setup.py` & `bhv-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

