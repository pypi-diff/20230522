# Comparing `tmp/AutoCarver-4.2.1.tar.gz` & `tmp/AutoCarver-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.2.1.tar", last modified: Wed May 17 10:04:07 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.3.0.tar", last modified: Mon May 22 07:25:36 2023, max compression
```

## Comparing `AutoCarver-4.2.1.tar` & `AutoCarver-4.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:04:07.000000 AutoCarver-4.2.1/
-drwxrwxrwx   0        0        0        0 2023-05-17 10:04:07.000000 AutoCarver-4.2.1/AutoCarver/
--rw-rw-rw-   0        0        0    23091 2023-05-17 10:02:32.000000 AutoCarver-4.2.1/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0     4687 2023-05-17 07:51:12.000000 AutoCarver-4.2.1/AutoCarver/Converters.py
--rw-rw-rw-   0        0        0    50777 2023-05-17 09:48:49.000000 AutoCarver-4.2.1/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    23882 2023-05-17 09:47:05.000000 AutoCarver-4.2.1/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.2.1/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:04:07.000000 AutoCarver-4.2.1/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7119 2023-05-17 10:03:59.000000 AutoCarver-4.2.1/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-17 10:04:05.000000 AutoCarver-4.2.1/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:03:59.000000 AutoCarver-4.2.1/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 10:03:59.000000 AutoCarver-4.2.1/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.2.1/LICENSE
--rw-rw-rw-   0        0        0     7119 2023-05-17 10:04:07.000000 AutoCarver-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 10:04:07.000000 AutoCarver-4.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-17 10:02:46.000000 AutoCarver-4.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/
+drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/AutoCarver/
+-rw-rw-rw-   0        0        0    23961 2023-05-22 07:18:16.000000 AutoCarver-4.3.0/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0     8599 2023-05-22 07:18:35.000000 AutoCarver-4.3.0/AutoCarver/Converters.py
+-rw-rw-rw-   0        0        0    52539 2023-05-22 07:18:23.000000 AutoCarver-4.3.0/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    28038 2023-05-22 07:18:44.000000 AutoCarver-4.3.0/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-10 08:49:10.000000 AutoCarver-4.3.0/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     7119 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-22 07:25:34.000000 AutoCarver-4.3.0/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 07:25:27.000000 AutoCarver-4.3.0/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-01-05 13:13:13.000000 AutoCarver-4.3.0/LICENSE
+-rw-rw-rw-   0        0        0     7119 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-05-14 13:54:01.000000 AutoCarver-4.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:25:36.000000 AutoCarver-4.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-22 07:19:00.000000 AutoCarver-4.3.0/setup.py
```

### Comparing `AutoCarver-4.2.1/AutoCarver/AutoCarver.py` & `AutoCarver-4.3.0/AutoCarver/AutoCarver.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,69 +174,71 @@
 
         # discretizing features based on each feature's values_order
         super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
         super().fit(X, y)
 
         return self
 
+
     def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
+        """ Carves a feature"""
 
         # computing crosstabs
         # crosstab on TRAIN
         xtab = nan_crosstab(X[feature], y, self.str_nan)
-        notna_xtab = xtab[xtab.index != self.str_nan]  # filtering out nans
 
         # crosstab on TEST
-        xtab_test, notna_xtab_test = None, None
+        xtab_test = None
         if X_test is not None:
             xtab_test = nan_crosstab(X_test[feature], y_test, self.str_nan)
-            notna_xtab_test = xtab_test[xtab_test.index != self.str_nan]  # filtering out nans
 
         # printing the group statistics
         if self.verbose:
             self.display_xtabs(feature, 'Raw', xtab, xtab_test)
 
-        # getting all possible combinations for the feature without NaNS
-        combinations = get_all_combinations(self.values_orders.get(feature), self.max_n_mod)
-
         # measuring association with target for each combination and testing for stability on TEST
-        best_groups = best_combination(combinations, self.sort_by, notna_xtab, notna_xtab_test)
+        best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=True, str_nan=self.str_nan)
 
         # update of the values_orders grouped modalities in values_orders
         if best_groups:
             xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # testing adding NaNs to built groups
-        order = self.values_orders.get(feature)
         if (self.str_nan in xtab.index) & self.dropna:
 
-            # adding nans at the end of the order
-            order = order.append(self.str_nan)
-
-            # reordering order according to target rate
-            new_order = xtab[1].divide(xtab.sum(axis=1)).sort_values().index.tolist()
-            order = order.sort_by(new_order)
-            self.values_orders.update({feature: order})
-
-            # getting all possible combinations for the feature without NaNS
-            combinations = get_all_combinations(order, self.max_n_mod)
-
             # measuring association with target for each combination and testing for stability on TEST
-            best_groups = best_combination(combinations, self.sort_by, xtab, xtab_test)
+            best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=False, str_nan=self.str_nan)
+
+            # adding NaN to the order
+            self.insert_nan(feature, xtab)
 
             # update of the values_orders grouped modalities in values_orders
             if best_groups:
                 xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
 
         # printing the new group statistics
         if self.verbose and best_groups:
             self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
 
         return best_groups
 
+    def insert_nan(self, feature: str, xtab: DataFrame) -> GroupedList:
+        """ Inserts NaNs in the order"""
+
+        # accessing order for specified feature
+        order = self.values_orders.get(feature)
+
+        # adding nans at the end of the order
+        if self.str_nan not in order:
+            order = order.append(self.str_nan)
+
+            # updating values_orders
+            self.values_orders.update({feature: order})
+
+
     def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
         """ Updates the values_orders and xtabs according to the best_groups"""
 
         # updating values_orders with best_combination 
         self.values_orders.update({feature: best_groups})
 
         # update of the TRAIN crosstab
@@ -353,19 +355,42 @@
     association.update({'combi_xtab': combi_xtab})
 
     # measuring association with the target
     association.update(association_xtab(combi_xtab))
 
     return association
 
-def best_combination(combinations: List[GroupedList], sort_by: str, xtab: DataFrame, xtab_test: DataFrame=None):
+def best_combination(order: GroupedList, max_n_mod: int, sort_by: str, xtab_train: DataFrame, xtab_dev: DataFrame=None, dropna: bool=True, str_nan: str=None):
     """ Finds the best combination of groups of feature's values:
      - Most associated combination on train sample 
      - Stable target rate of combination on test sample.
     """
+    
+    # copying crosstabs
+    xtab = xtab_train
+    xtab_test = xtab_dev
+    
+    # removing nans if requested
+    if dropna:
+        
+        # crosstab on TRAIN
+        xtab = xtab_train[xtab_train.index != str_nan]  # filtering out nans
+
+        # crosstab on TEST
+        if xtab_test is not None:
+            xtab_test = xtab_dev[xtab_dev.index != str_nan]  # filtering out nans
+    
+        # getting all possible combinations for the feature without NaNS
+        combinations = get_all_combinations(order, max_n_mod, raw=False)
+    
+    # keeping nans as a modality
+    else:
+    
+        # getting all possible combinations for the feature with NaNS
+        combinations = get_all_nan_combinations(order, str_nan)
 
     # computing association measure per combination 
     associations = [apply_combination(xtab, combi) for combi in combinations]
 
     # sort according to association measure
     if len(combinations) > 0:
         associations = DataFrame(associations)
@@ -402,77 +427,84 @@
             if viability:
 
                 association.update({'combi_xtab_test': combi_xtab_test})
 
                 return association
 
 
-def get_all_combinations(values: GroupedList, max_n_mod: int=None):
+def get_all_combinations(values: GroupedList, max_n_mod: int=None, raw: bool=False) -> List[GroupedList]:
 
     # maximum number of classes
     q = len(values)
 
     # desired max number of classes
     if max_n_mod is None:
-    	max_n_mod = q
+        max_n_mod = q
 
     # all possible combinations
     combinations = list()
     for n_class in range(2, max_n_mod + 1):
         combinations += get_combinations(n_class, q)
 
-    combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]  # getting real feature values
-    combinations = [groupedlist_combination(combination, values) for combination in combinations]  # converting back to GroupedList
+    # getting real feature values
+    combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]
+    
+    # converting back to GroupedList
+    if not raw:
+        combinations = [groupedlist_combination(combination, values) for combination in combinations]
 
     return combinations
 
-def get_all_nan_combinations(order: List[Any]):
+def get_all_nan_combinations(order: GroupedList, str_nan: str) -> List[GroupedList]:
     """ all possible combinations of modalities with numpy.nan"""
 
     # computing all non-NaN combinations
     # case 0: several modalities -> several combinations
     if len(order) > 1:
-        combinations = get_all_combinations(order, len(order))
-    # case 1: unique modality -> two combinations
-    elif len(order) == 1:
-        combinations = [[order]]
-    # case 2: no modality (only nan) -> no combination
+        combinations = get_all_combinations(order, len(order), raw=True)
+    # case 1: unique or no modality -> two combinations
     else:
-        combinations = [[]]
+        combinations = []
 
     # iterating over each combinations of non-NaNs
     new_combinations = []
     for combi in combinations:
 
          # NaNs not attributed to a group (own modality)
-        new_combinations += [combi + [[nan]]] 
+        new_combinations += [combi + [[str_nan]]] 
 
         # NaNs attributed to a group of non NaNs
         for n in range(len(combi)):
 
             # grouping NaNs with an existing group
-            new_combination = [combi[n] + [nan]]
+            new_combination = [combi[n] + [str_nan]]
 
             # adding other groups unchanged
             pre = [o for o in combi[:n]]
             nex = [o for o in combi[n+1:]]
             new_combinations += [pre + new_combination + nex]
+            
+    # adding NaN to order
+    order = order.append(str_nan)
+    
+    # converting back to GroupedList
+    new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
 
     return new_combinations
 
 
 def consecutive_combinations(n_remaining: int, start: int, end: int, grp_for_this_step: list=None):
     """HELPER finds all consecutive combinations between start and end.    """
 
     # Import de la liste globale
     global __li_of_res__
 
     # initiating group
     if not grp_for_this_step:
-    	grp_for_this_step = []
+        grp_for_this_step = []
     
     # stopping when there are non more remaining classes
     if n_remaining == 0:
         
         ### On ajoute le dernier quantile restant au découpage ###
         grp_for_this_step += [(start, end)]
 
@@ -509,15 +541,17 @@
     n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
     min_n_mod = min(n_mod_x, n_mod_y)
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
 
     # Cramer's V
-    cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
+    cramerv = 0
+    if min_n_mod > 1:
+        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
 
     # Tschuprow's T
     dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
     tschuprowt = 0
     if dof_mods > 0:
         tschuprowt = sqrt(chi2 / n_obs / dof_mods)
```

### Comparing `AutoCarver-4.2.1/AutoCarver/Discretizers.py` & `AutoCarver-4.3.0/AutoCarver/Discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from IPython.display import display_html
-from numpy import sort, nan, inf, float16, where, isin, argsort, array, select, append, quantile, linspace, argmin
+from numpy import sort, nan, inf, float32, where, isin, argsort, array, select, append, quantile, linspace, argmin
 from pandas import DataFrame, Series, isna, qcut, notna, unique
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing import Any, Dict, List
 from warnings import warn
 
 def nan_unique(x: Series):
@@ -20,23 +20,28 @@
 class GroupedList(list):
     
     def __init__(self, iterable=()) -> None:
         """ An ordered list that historizes its elements' merges."""
 
         # case 0: iterable is the contained dict
         if isinstance(iterable, dict):
+            # TODO: check thaht keys are in list
             
             # récupération des valeurs de la liste (déjà ordonné)
             values = [key for key in iterable]
 
             # initialsiation de la liste
             super().__init__(values)
 
             # attribution des valeurs contenues
             self.contained = {k: v for k, v in iterable.items()}
+
+            # adding key to itself if that's not the case
+            for k in [k for k in values if k not in self.contained.get(k)]:
+                self.contained.update({k: self.contained.get(k) + [k]})
         
         # case 1: copying a GroupedList
         elif hasattr(iterable, 'contained'):
 
             # initialsiation de la liste
             super().__init__(iterable)
 
@@ -87,14 +92,26 @@
         """ Appends a new_value to the GroupedList"""
         
         self += [new_value]
         
         self.contained.update({new_value: [new_value]})
         
         return self
+        
+    def update(self, new_value: Dict[Any, List[Any]]) -> None:
+        """ Updates the GroupedList via a dict"""
+        
+        # adding keys to the order if they are new values
+        for k in [c for c in new_value if c not in self]:
+            self += new_value.keys()
+        
+        # updating contained accord to new_value
+        self.contained.update(new_value)
+        
+        return self
 
     def sort(self) -> None:
         """ Sorts the values of the list and dict (if any, NaNs are last). """
 
         # str values
         keys_str = [key for key in self if isinstance(key, str)]
 
@@ -148,15 +165,15 @@
         """ returns the group containing the specified value """
         
         found = [key for key, values in self.contained.items() if any(is_equal(value, elt) for elt in values)]
 
         if any(found):
             return found[0]
         else:
-        	return value
+            return value
 
     def values(self) -> List[Any]:
         """ returns all values contained in each group """
 
         known = [value for values in self.contained.values() for value in values]
 
         return known
@@ -194,16 +211,16 @@
                 
         return repr
 
 
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(self, values_orders: Dict[str, Any], *, 
-    	copy: bool=False, output: type= float,
-    	str_nan: str=None, verbose: bool=False) -> None:
+        copy: bool=False, output: type= float,
+        str_nan: str=None, verbose: bool=False) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.copy = copy
         self.output = output
         self.verbose = verbose
         self.str_nan = str_nan
@@ -242,26 +259,28 @@
 
             # grouping modalities
             else:
                 Xc[feature] = select(to_input, to_keep, default=Xc[feature])
 
         # converting to float
         if self.output == float:
-            Xc[self.features] = Xc[self.features].astype(float16)
+            Xc[self.features] = Xc[self.features].astype(float32)
 
         return Xc
 
 
 class QualitativeDiscretizer(BaseEstimator, TransformerMixin):
     """ Automatic discretizing of categorical and categorical ordinal features.
 
     Modalities/values of features are grouped according to there respective orders:
      - [Qualitative features] order based on modality target rate.
      - [Qualitative ordinal features] user-specified order.
 
+    TODO: pass ordinal_features/qualitati_features as parameters to be able to pass values_orders with other orders (ex: from chaineddiscretizer)
+
     Parameters
     ----------
     features: list
         Contains qualitative (categorical and categorical ordinal) features to be discretized.
 
     min_freq: int
         [Qualitative features] Minimal frequency of a modality.
@@ -583,45 +602,63 @@
 
         return Xc
 
 
 
 class ChainedDiscretizer(GroupedListDiscretizer):
     
-    def __init__(self, features: List[str], min_freq: float, chained_orders: List[List[Any]], *, copy: bool=False, verbose: bool=False) -> None:       
+    def __init__(self, features: List[str], min_freq: float, chained_orders: List[GroupedList], *, 
+                 remove_unknown: bool=False, str_nan: str='__NAN__', copy: bool=False, verbose: bool=False) -> None:       
         
         self.min_freq = min_freq
         self.features = features[:]
         self.chained_orders = [GroupedList(order) for order in chained_orders]
         self.copy = copy
         self.verbose = verbose
+
+        # parameters to handle missing/unknown values
+        self.remove_unknown = remove_unknown
+        self.str_nan = str_nan
         
         # initiating features' values orders to all possible values
         self.known_values = list(set([value for group in self.chained_orders for value in group.values()]))
-        self.values_orders = {f: GroupedList(self.known_values[:]) for f in self.features}
+        self.values_orders = {f: GroupedList(self.known_values[:] + [self.str_nan]) for f in self.features}
 
     def fit(self, X: DataFrame, y: Series=None) -> None:
         
-        # copying dataframe
-        Xc = X[self.features].copy()
+        # filling nans
+        Xc = X[self.features].fillna(self.str_nan)
         
         # iterating over each feature
         for n, feature in enumerate(self.features):
 
             # verbose if requested
             if self.verbose:
                 print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
 
             # computing frequencies of each modality
-            frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
+            frequencies = Xc[feature].value_counts(normalize=True)
             values, frequencies = frequencies.index, frequencies.values
 
             # checking for unknown values (values to present in an order of self.chained_orders)
             missing = [value for value in values if notna(value) and (value not in self.known_values)]
-            assert not any(missing), f"Order needs to be provided for values: {missing}"
+
+            # converting unknown values to NaN
+            if self.remove_unknown & (len(missing) > 0):
+
+            	# alerting user
+                print(f"Order for {feature} was not provided for values: {missing}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)")
+
+                # adding missing valyes to the order
+                order = self.values_orders.get(feature)
+                order.update({self.str_nan: missing + order.get(self.str_nan)})
+
+            # alerting user
+            else:
+                assert not len(missing) > 0, f"Order for {feature} needs to be provided for values: {missing}, otherwise set remove_unknown=True"
 
             # iterating over each specified orders
             for order in self.chained_orders:
                 
                 # identifying modalities which rarest values
                 to_keep = values[frequencies >= self.min_freq]
 
@@ -634,15 +671,15 @@
                 for discarded, kept in zip(to_discard, order):
                     self.values_orders.get(feature).group_list(discarded, kept)  # historisation dans l'order
                     
                 # updating frequencies of each modality for the next ordering
                 frequencies = Xc[feature].value_counts(dropna=False, normalize=True).drop(nan, errors='ignore')  # dropping nans to keep them anyways
                 values, frequencies = frequencies.index, frequencies.values
         
-        super().__init__(self.values_orders, copy=self.copy, output=str)
+        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=str)
         super().fit(X, y)
             
         return self
 
 class QuantileDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(self, features: List[str], q: int, *, 
@@ -833,37 +870,42 @@
 
 class DefaultDiscretizer(BaseEstimator, TransformerMixin):
     
     def __init__(
         self, features: List[str], min_freq: float, *, 
         values_orders: Dict[str, Any]={},
         default_value: str='__OTHER__',
+        str_nan: str='__NAN__',
         copy: bool=False, verbose: bool=False) -> None:
         """ Groups a qualitative features' values less frequent than min_freq into a default_value"""
         
         self.features = features[:]
         self.min_freq = min_freq
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.default_value = default_value[:]
+        self.str_nan = str_nan[:]
         self.copy = copy
         self.verbose = verbose
 
     def fit(self, X: DataFrame, y: Series) -> None:
 
+        # filling up NaNs
+        Xc = X[self.features].fillna(self.str_nan)
+
         # computing frequencies of each modality
-        frequencies = X[self.features].apply(value_counts, dropna=False, normalize=True, axis=0)
+        frequencies = Xc.apply(value_counts, normalize=True, axis=0)
 
         # computing ordered target rate per modality for ordering
-        target_rates = X[self.features].apply(target_rate, y=y, dropna=True, ascending=True, axis=0)
+        target_rates = Xc.apply(target_rate, y=y, ascending=True, axis=0)
 
         # attributing orders to each feature
         self.values_orders.update({f: GroupedList(list(target_rates[f])) for f in self.features})
         
-        #number of unique modality per feature
-        nuniques = X[self.features].apply(nunique, dropna=False, axis=0)
+        # number of unique modality per feature
+        nuniques = Xc.apply(nunique, axis=0)
             
         # identifying modalities which are the most common
         self.to_keep: Dict[str, Any] = {}  # dict of features and corresponding kept modalities
 
         # iterating over each feature
         for feature in self.features:
 
@@ -879,16 +921,15 @@
 
         # grouping rare modalities 
         for n, feature in enumerate(self.features):
 
         	# printing verbose
             if self.verbose:
                 print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
-            
-                
+
             # identifying values to discard (rare modalities)
             to_discard = [value for value in self.values_orders[feature] if value not in self.to_keep[feature]]
 
             # discarding rare modalities
             if len(to_discard) > 0:
 
                 # adding default_value to possible values
@@ -913,14 +954,17 @@
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataset if requested
         Xc = X
         if self.copy:
             Xc = X.copy()
 
+        # filling up NaNs
+        Xc[self.features] = Xc[self.features].fillna(self.str_nan)
+
         # grouping values inside groups of modalities
         for n, feature in enumerate(self.features):
 
         	# verbose if requested
             if self.verbose: 
                 print(f" - [DefaultDiscretizer] Transform {feature} ({n+1}/{len(self.features)})")
```

### Comparing `AutoCarver-4.2.1/AutoCarver/FeatureSelector.py` & `AutoCarver-4.3.0/AutoCarver/FeatureSelector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from IPython.display import display_html
 from math import sqrt
 from numpy import triu, ones, nan, inf
 from pandas import DataFrame, Series, notna, crosstab
+from random import shuffle
 from scipy.stats import kruskal, chi2_contingency
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 from typing import List, Dict, Any, Callable, Tuple
 
 
@@ -17,49 +18,75 @@
         
     Parameters
     ----------
     features: List[str]
         Features on which to compute association.
     n_best, int:
         Number of features to be selected
+    sample_size: float, default 1.
+        Should be set between ]0, 1]
+        Size of sampled list of features speeds up computation. 
+        By default, all features are used. For sample_size=0.5,
+        FeatureSelector will search for the best features in 
+        features[:len(features)//2] and then in features[len(features)//2:]
     measures, List[Callable]: default list().
         List of association measures to be used.
         Implemented measures are:
-            - For association evaluation: `kruskal_measure`, `R_measure`
-            - For outlier detection: `zscore_measure`, `iqr_measure`
+            [Quantitative Features] 
+             - For association evaluation: `kruskal_measure`, `R_measure`
+             - For outlier detection: `zscore_measure`, `iqr_measure`
+            [Qualitative Features] 
+             - For correlation: `chi2_measure`, `cramerv_measure`, `tschuprowt_measure`
         Ranks features based on last measure of the list.
     filters, List[Callable]: default list().
         List of filters to be used.
         Implemented filters are:
-          - For linear correlation: `spearman_filter`, `pearson_filter`
-          - For multicoloinearity: `vif_filter`
+            [Quantitative Features] 
+             - For linear correlation: `spearman_filter`, `pearson_filter`
+             - For multicoloinearity: `vif_filter`
+            [Qualitative Features] 
+             - For correlation: `cramerv_filter`, `tschuprowt_filter`
 
-    params examples
-    ---------------
+    Thresholds (to be passed as kwargs)
+    ----------
+    thresh_measure, float: default 0.
+        Minimum association between target and features
+        To be used with: `measure_filter`
+    name_measure, str
+        Measure to be used for minimum association filtering
+        To be used with: `measure_filter`
     thresh_nan, float: default 1.
         Maximum percentage of NaNs in a feature
+        To be used with: `nans_measure`
     thresh_mode, float: default 1.
         Maximum percentage of the mode of a feature
+        To be used with: `mode_measure`
     thresh_outlier, float: default 1.
         Maximum percentage of Outliers in a feature
+        To be used with: `iqr_measure`, `zscore_measure`
     thresh_corr, float: default 1.
         Maximum association between features
+        To be used with: `spearman_filter`, `pearson_filter`, `cramerv_filter`, `tschuprowt_filter`
     thresh_vif, float: default inf
         Maximum VIF between features
-    ascending, bool: default False
-        Ascending of Descending sort by sort_measure
+        To be used with: `vif_filter`
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
     """
     
     def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
-                 copy: bool=True, verbose: bool=True, **params) -> None:
+                 sample_size: float=1., copy: bool=True, verbose: bool=True, **params) -> None:
         
         self.features = features[:]
         self.n_best = n_best
         assert n_best <= len(features), "Must set n_best <= len(features)"
         self.best_features = features[:]
+        self.sample_size = sample_size
         
         self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
         self.filters = [thresh_filter] + filters[:]
         self.sort_measures = [measure.__name__ for measure in measures[::-1]]
 
         self.copy = copy
         self.verbose = verbose
@@ -73,25 +100,27 @@
 
         # iterating over each measure
         for measure in self.measures:
             passed, association = measure(passed, association, x, y, **self.params)
             
         return association
     
-    def measure_apply(self, X: DataFrame, y: Series) -> None:
+    def measure_apply(self, X: DataFrame, y: Series, features: List[str]) -> None:
         """ Measures association between columns of X and y
 
     Parameters
     ----------
-    ascending, bool: default False
-      Ascending of Descending sort by sort_measure
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
     """
         
         # applying association measure to each column
-        self.associations = X[self.features].apply(self.measure, y=y, result_type='expand', axis=0).T
+        self.associations = X[features].apply(self.measure, y=y, result_type='expand', axis=0).T
         
         # filtering non association measure (pct_zscore, pct_iqr...)
         asso_measures = [c for c in self.associations if '_measure' in c]
         self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
         
         # sorting statistics if an association measure was provided
         self.associations = self.associations.sort_values(
@@ -99,16 +128,18 @@
         )
     
     def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
         """ Filters out too correlated features (least relevant first)
 
     Parameters
     ----------
-    ascending, bool: default False
-      Ascending of Descending sort by sort_measure
+    ascending, bool default False
+        According to this measure:
+         - True: Lower values of the measure are to be considered as more associated to the target
+         - False: Higher values of the measure are to be considered as more associated to the target
     """
         
         # ordering features by sort_by
         self.filtered_associations = self.associations.sort_values(sort_measure, ascending=self.params.get('ascending', False))
 
         # applying successive filters
         for filtering in self.filters:
@@ -122,20 +153,19 @@
         # appllying style 
         subset = [c for c in association if 'pct_' in c or '_measure' in c or '_filter' in c]
         style = association.style.background_gradient(cmap='coolwarm', subset=subset)
         style = style.set_table_attributes("style='display:inline'")
         style = style.set_caption(caption)
         display_html(style._repr_html_(), raw=True)
         
-    
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """ Selects the n_best features"""
+    def fit_features(self, X: DataFrame, y: Series, features: List[str], n_best: int) -> List[str]:
+        """ Selects the n_best features amongst the specified ones"""
         
         # initial computation of all association measures
-        self.measure_apply(X, y)
+        self.measure_apply(X, y, features)
 
         # displaying association measure
         if self.verbose:
             self.display_stats(self.associations, 'Raw association')
         
         # iterating over each sort_measures 
         # useful when measures hints to specific associations
@@ -146,56 +176,95 @@
             self.filter_apply(X, sort_measure)
             ranks += [list(self.filtered_associations.index)]
 
             # displaying filtered out association measure
             if n == 0 and self.verbose and len(self.filters) > 1:
                 self.display_stats(self.filtered_associations, 'Filtered association')
 
-        # retrieving the n_best features per ranking
+        # retrieving the n_best features per each ranking
+        best_features = []
         if len(self.sort_measures) > 0:
-            self.best_features = [feature for rank in ranks for feature in rank[:self.n_best]]
-            self.best_features = list(set(self.best_features))  # deduplicating
+            best_features = [feature for rank in ranks for feature in rank[:n_best]]
+            best_features = list(set(best_features))  # deduplicating
+        
+        return best_features
+    
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """ Selects the n_best features"""
+        
+        # splitting features in chunks
+        if self.sample_size < 1:
+            
+            # shuffling features to get random samples of features
+            shuffle(self.features)
+
+            # number of features per sample
+            chunks = int(len(self.features) // (1 / self.sample_size))
+
+            # splitting feature list in samples
+            feature_samples = [self.features[chunks * i: chunks * (i + 1)] for i in range(int(1 / self.sample_size)-1)]
+
+            # adding last sample with all remaining features
+            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1):]]
+
+            # iterating over each feature samples
+            best_features = []
+            for features in feature_samples:
+
+                # fitting association on features
+                best_features += self.fit_features(X, y, features, int(self.n_best // 2))
+        
+        # splitting in chunks not requested
+        else:
+            best_features = self.features[:]
+        
+        # final selection with all best_features selected
+        self.best_features = self.fit_features(X, y, best_features, self.n_best)
+            
+        # dropped features
+        self.dropped_features = [c for c in self.features if c not in self.best_features]
 
         return self
 
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # copying dataset
         Xc = X
         if self.copy:
             Xc.copy()
 
         # filtering out unwanted features
-        Xc = X.drop([c for c in self.features if c not in self.best_features], axis=1)
+        Xc = Xc.drop(self.dropped_features, axis=1)
 
         return Xc
 
 
 # MEASURES
 def nans_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Measure of the percentage of NaNs
 
     Parameters
     ----------
     thresh_nan, float: default 1.
       Maximum percentage of NaNs in a feature
     """
     
-    passed = True  # whether or not tests where passed
+    # whether or not tests where passed
+    if active:
     
-    nans = x.isnull()  # ckecking for nans
-    pct_nan = nans.mean()   # Computing percentage of nans
+        nans = x.isnull()  # ckecking for nans
+        pct_nan = nans.mean()   # Computing percentage of nans
     
-    # updating association
-    association.update({'pct_nan': pct_nan})
+        # updating association
+        association.update({'pct_nan': pct_nan})
     
-    # Excluding feature that have to many NaNs
-    passed = pct_nan < params.get('thresh_nan', 1.)
+        # Excluding feature that have to many NaNs
+        active = pct_nan < params.get('thresh_nan', 1.)
     
-    return passed, association
+    return active, association
 
 def dtype_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Gets dtype"""
     
     # updating association
     association.update({'dtype': x.dtype})
         
@@ -206,26 +275,27 @@
 
     Parameters
     ----------
     thresh_mode, float: default 1.
       Maximum percentage of the mode of a feature
     """
     
-    passed = True  # whether or not tests where passed
+    # whether or not tests where passed
+    if active:
     
-    mode = x.mode(dropna=True).values[0]  # computing mode
-    pct_mode = (x == mode).mean()  # Computing percentage of the mode
+        mode = x.mode(dropna=True).values[0]  # computing mode
+        pct_mode = (x == mode).mean()  # Computing percentage of the mode
     
-    # updating association
-    association.update({'pct_mode': pct_mode, 'mode': mode})
+        # updating association
+        association.update({'pct_mode': pct_mode, 'mode': mode})
     
-    # Excluding feature with too frequent modes
-    passed = pct_mode < params.get('thresh_mode', 1.)
+        # Excluding feature with too frequent modes
+        active = pct_mode < params.get('thresh_mode', 1.)
     
-    return passed, association
+    return active, association
 
 def kruskal_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
     
     # check that previous steps where passed
     if active:
     
@@ -287,15 +357,15 @@
             'min': x.min(),
             'max': x.max(),
             'mean': mean,
             'std': std
         })
 
         # Excluding feature with too frequent modes
-        passed = pct_zscore < params.get('thresh_outlier', 1.)
+        active = pct_zscore < params.get('thresh_outlier', 1.)
         
     return active, association
 
 def iqr_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Computes outliers based on the inter-quartile range
 
     Parameters
@@ -321,15 +391,15 @@
             'pct_iqr': pct_iqr,
             'q1': q1,
             'median': x.median(),
             'q3': q3
         })
 
         # Excluding feature with too frequent modes
-        passed = pct_iqr < params.get('thresh_outlier', 1.)
+        active = pct_iqr < params.get('thresh_outlier', 1.)
         
     return active, association
 
 def chi2_measure(active: bool, association: Dict[str, Any], x: Series,
                  y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
     """ Chi2 Measure between two Series of qualitative features"""
         
@@ -410,32 +480,53 @@
 
         # updating association
         association.update({'tschuprowt_measure': tschuprowt})
     
     return active, association
 
     
-# FILTERS        
+# FILTERS 
 def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
     """ Filters out missing association measure (did not pass a threshold)"""
     
     # drops rows with nans
     associations = ranks.dropna(axis=0)
     
     return associations
 
+def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
+    """ Filters out specified measure's lower ranks than threshold
+
+    Parameters
+    ----------
+    thresh_measure, float: default 0.
+        Minimum association between target and features
+        To be used with: `association_filter`
+    name_measure, str
+        Measure to be used for minimum association filtering
+        To be used with: `association_filter`
+    """
+    
+    associations = ranks.copy()
+
+    # drops rows with nans
+    if 'name_measure' in params:
+        associations = ranks[ranks[params.get('name_measure')] > params.get('thresh_measure', 0.)]
+    
+    return associations
+
 def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
     """ Computes max association between X and X (quantitative) excluding features 
     that are correlated to a feature more associated with the target 
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
-      Maximum association between features
+        Maximum association between features
     """
     
     # accessing the prefered order
     prefered_order = ranks.index
 
     # computing correlation between features
     X_corr = X[prefered_order].corr(corr_measure).abs()
```

### Comparing `AutoCarver-4.2.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.3.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.2.1
+Version: 4.3.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.2.1/LICENSE` & `AutoCarver-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.2.1/PKG-INFO` & `AutoCarver-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.2.1
+Version: 4.3.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AutoCarver-4.2.1/README.md` & `AutoCarver-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.2.1/setup.py` & `AutoCarver-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.2.1',
+    version='4.3.0',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```

