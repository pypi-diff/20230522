# Comparing `tmp/FastCG-0.0.2.tar.gz` & `tmp/FastCG-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastCG-0.0.2.tar", last modified: Sun Apr 30 18:29:21 2023, max compression
+gzip compressed data, was "FastCG-0.0.3.tar", last modified: Mon May 22 16:26:47 2023, max compression
```

## Comparing `FastCG-0.0.2.tar` & `FastCG-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 18:29:21.605152 FastCG-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-30 18:29:21.591191 FastCG-0.0.2/FastCG/
--rw-rw-rw-   0        0        0       40 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 18:29:21.601162 FastCG-0.0.2/FastCG/generators/
--rw-rw-rw-   0        0        0    21683 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/generators/GeneratorBase.py
--rw-rw-rw-   0        0        0     9042 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/generators/ProbKnnGenerator.py
--rw-rw-rw-   0        0        0      162 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 18:29:21.603157 FastCG-0.0.2/FastCG/utils/
--rw-rw-rw-   0        0        0     1524 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/utils/SmartCondition.py
--rw-rw-rw-   0        0        0      148 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/utils/logger.py
--rw-rw-rw-   0        0        0     6319 2023-04-30 18:15:03.000000 FastCG-0.0.2/FastCG/utils/util_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-30 18:29:21.599167 FastCG-0.0.2/FastCG.egg-info/
--rw-rw-rw-   0        0        0      452 2023-04-30 18:29:21.000000 FastCG-0.0.2/FastCG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-04-30 18:29:21.000000 FastCG-0.0.2/FastCG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 18:29:21.000000 FastCG-0.0.2/FastCG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-04-30 18:29:21.000000 FastCG-0.0.2/FastCG.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-30 18:29:21.000000 FastCG-0.0.2/FastCG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      452 2023-04-30 18:29:21.604154 FastCG-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8491 2023-04-30 18:15:03.000000 FastCG-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 18:29:21.605152 FastCG-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-04-30 18:29:17.000000 FastCG-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.542010 FastCG-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.506594 FastCG-0.0.3/FastCG/
+-rw-rw-rw-   0        0        0       40 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.532526 FastCG-0.0.3/FastCG/generators/
+-rw-rw-rw-   0        0        0    21815 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/generators/GeneratorBase.py
+-rw-rw-rw-   0        0        0     8419 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/generators/ProbKnnGenerator.py
+-rw-rw-rw-   0        0        0      162 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.541012 FastCG-0.0.3/FastCG/utils/
+-rw-rw-rw-   0        0        0     1524 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/SmartCondition.py
+-rw-rw-rw-   0        0        0      148 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/logger.py
+-rw-rw-rw-   0        0        0     6320 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/utils/util_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.518561 FastCG-0.0.3/FastCG.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      452 2023-05-22 16:26:47.542010 FastCG-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8491 2023-04-30 18:15:03.000000 FastCG-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:26:47.542010 FastCG-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-05-22 16:26:06.000000 FastCG-0.0.3/setup.py
```

### Comparing `FastCG-0.0.2/FastCG/generators/GeneratorBase.py` & `FastCG-0.0.3/FastCG/generators/GeneratorBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 
 
 class GeneratorBase():
 
     configuration_schema = {'features_to_change': {'type': list, 'schema': {'type': str}, 'required': True, 'minlength': 1},
                             'increase_only': {'type': list, 'schema': {'type': str}, 'required': False},
+                            'decrease_only': {'type': list, 'schema': {'type': str}, 'required': False},
                             'max_features_to_change' : {'type': int, 'required': True, 'min': 1, 'default': 2},
                             'target': {'type': str, 'required': True},
-                            'ID': {'type': str, 'required': True}}
+                            'ID': {'type': str, 'required': False}}
     
     def __init__(self, all_data, model, config, target, condition, verbose=0):
         """
         Base class for all generators
 
         Parameters
         ----------
@@ -31,15 +32,15 @@
         model : ModelBase
             Model to be used to generate data
         config : dict
             Configuration for the generator
         verbose : int
             Verbosity level, 0 means only show warning, 1 means show info, 2 means show debug
         """
-        self.all_data = all_data
+        self.all_data = all_data.copy()
         if not self._is_valid_config(config):
             raise ValueError("Invalid config")
         self.config = config
         self.verbose = verbose
         self.model = model
 
         Logger.set_verbosity(verbose)
@@ -165,18 +166,17 @@
             List of data to be checked
             
         Returns
         -------
         chunk : list
             List of data that contains counterfactual targets
             """
-        id = self.config['ID']
         data_to_generate = []
         for index, obs in chunk.iterrows():
-            pred_result = self.model.predict(obs.to_frame().T)
+            pred_result = self.model.predict(obs.to_frame().T.drop(self.id, axis=1))
             if not self.smart_condition(pred_result):
                 preprocessed_obs = self._preprocess_counterfactual_targets(obs)
                 data_to_generate.append((obs,preprocessed_obs))
         return data_to_generate
 
     
     def generate(self, data, n_jobs=-1, chunk_size=1000) -> tuple:
@@ -255,17 +255,17 @@
 
         valid_data = []
         invalid_data = []
 
         for obs in tqdm(generated_data, desc="Sanity check on generated data"):
             #if obs is df 
             if isinstance(obs, pd.DataFrame):
-                res = self.model.predict(obs)
+                res = self.model.predict(obs.drop(self.id, axis=1))
             else:
-                obs = obs.to_frame().T
+                obs = obs.to_frame().T.drop(self.id, axis=1)
                 res = self.model.predict(obs)
             if not self.smart_condition.check(res):
                 invalid_data.append(obs)
                 continue
             valid_data.append(obs)
 
         initial_valid_data_len = len(valid_data)
@@ -284,15 +284,15 @@
             valid_data = Parallel(n_jobs=n_jobs)(tqdm([delayed(self._postprocess_valid_data)(chunk) for chunk in chunks], desc="Postprocessing valid data in parallel"))
 
             # merge list of dicts into a single dict containing all keys and values
             valid_data = {k: v for d in valid_data for k, v in d.items()}
         else:
             valid_data = []
             for chunk in tqdm(chunks, desc="Postprocessing valid data in sequencial"):
-                valid_data += self._postprocess_valid_data(chunk)
+                valid_data.append(self._postprocess_valid_data(chunk))
             valid_data = {k: v for d in valid_data for k, v in d.items()}
 
         # valid_data = self._postprocess_valid_data(valid_data)
         Logger.debug(f"Total valid data after postprocessing: {len(valid_data)}")
         if len(valid_data) != initial_valid_data_len:
             Logger.warning(f"Postprocessing valid data removed {initial_valid_data_len - len(valid_data)} data points")
             
@@ -372,27 +372,25 @@
         chunks = [data[i:i + chunk_size]
                   for i in range(0, len(data), chunk_size)]
 
         # generate data for each chunk
         Logger.debug(
             f"Generating data for each chunk, total chunks: {len(chunks)}")
         generated_data = Parallel(n_jobs=n_jobs, require='sharedmem')(
-            delayed(self._generate_chunk)(chunk) for chunk in tqdm(chunks, desc="Generating Counterfactuals in chunks in parallel"))
+            delayed(self._generate_chunk)(chunk) for chunk in tqdm(chunks, desc="Generating Counterfactual in chunks in parallel"))
 
         if not generated_data:
             Logger.critical("No data generated")
             raise ValueError("No data generated")
 
         # flatten the generated data in case of list of lists
         if isinstance(generated_data[0], list):
             generated_data = [
                 item for sublist in generated_data for item in sublist]
 
-        # TODO: Check with linoy what to do here
-
         return generated_data
 
     def _generate_chunk(self, chunk):
         # logging.debug(f"Generating data for chunk of size {len(chunk)}")
         all_generated_data = []
         for obs,processed_obs in chunk:
             generated_data = self._generate_single(obs,processed_obs)
@@ -401,52 +399,52 @@
         return all_generated_data
 
     def _generate_single(self, obs,processed_obs):
         raise NotImplementedError
     
     def show_counterfactual(self, key, counterfactual_list, show_plot=False):
         """
-        Show the counterfactual for a given loan ID.
+        Show the counterfactual for a given ID.
 
         Parameters
         ----------
         key : int
-            The loan ID.
+            The ID.
         
         counterfactual_list : list
             A list of counterfactuals.
 
         show_plot : bool
             Whether to show the plot or not. Default is False.
 
         Returns
         -------
         None
     
         """
         results = pd.DataFrame()
         counterfactual = counterfactual_list.get(key)
-        self.obs = self.all_data[self.all_data[self.config["ID"]] == key].copy().drop(self.config["target"], axis=1)
+        self.obs = self.all_data[self.all_data[self.id] == key].copy().drop(self.config["target"], axis=1)
         for col in self.all_data.columns:
             if col != self.config["target"]:
                 results.loc[0, col] = self.obs[col].values[0].astype(int)
                 results.loc[1, col] = counterfactual[col].values[0].astype(int)
         results = results.T
         results.columns = ["Original", "Counterfactual"]
         self.counterfactual = results["Counterfactual"].to_frame().T
         results["Difference"] = results["Counterfactual"] - results["Original"]
         results["% Difference"] = results["Difference"] / results["Original"] * 100 
         results["% Difference"] = results["% Difference"].fillna(0)
         results["% Difference"] = results["% Difference"].replace([np.inf, -np.inf], 0)
-        print("In order for the loan to be approved, the following changes need to be made:")
+        # print("In order to change the prediction from ", self.obs[self.config["target"]].values[0], " to ", counterfactual[self.config["target"]].values[0], " do the following:")
         print("-------------------------------------------------------------------")
         print("ID: ", key)
         print("-------------------------------------------------------------------")
         for row in results.iterrows():
-            if row[0] == self.config["ID"]:
+            if row[0] == self.id:
                     continue
             if results["Difference"][row[0]] > 0:
                 print("Increase ", row[0], " by ", row[1]["% Difference"], "%") 
                 print("Increase ", row[0], " by ", row[1]["Difference"], " units")
             elif results["Difference"][row[0]] < 0:
                 print("Decrease ", row[0], " by ", row[1]["% Difference"], "%")
                 print("Decrease ", row[0], " by ", row[1]["Difference"], " units")
@@ -455,20 +453,20 @@
             self.plot_the_counterfactual(self.obs, self.counterfactual)
 
         display(results)
         return self.obs, self.counterfactual
 
     def get_counterfactual(self, key, counterfactual_list):
         """
-        Get the counterfactual for a given loan ID. 
+        Get the counterfactual for a given ID. 
 
         Parameters
         ----------
         key : int
-            The loan ID.
+            The ID.
         
         counterfactual_list : list
             A list of counterfactuals.
 
         Returns
         -------
         obs : pd.DataFrame
@@ -477,28 +475,28 @@
         counterfactual : pd.DataFrame
             The counterfactual.
         
         """
 
         results = pd.DataFrame()
         counterfactual = counterfactual_list.get(key)
-        obs = self.all_data[self.all_data[self.config["ID"]] == key].copy().drop(self.config['target'], axis=1)
+        obs = self.all_data[self.all_data[self.id] == key].copy().drop(self.config['target'], axis=1)
         for col in self.all_data.columns:
             if col != self.config["target"]:
                 results.loc[0, col] = self.obs[col].values[0]
                 results.loc[1, col] = counterfactual[col].values[0]
         results = results.T
         results.columns = ["Original", "Counterfactual"]
         counterfactual = results["Counterfactual"].to_frame().T
         return obs, counterfactual
     
 
     def plot_the_counterfactual(self, obs, counterfactual):
         """
-        Plot the counterfactual for a given loan ID.
+        Plot the counterfactual for a given ID.
 
         Parameters
         ----------
         obs : pd.DataFrame
             The original observation.
 
         counterfactual : pd.DataFrame
```

### Comparing `FastCG-0.0.2/FastCG/generators/ProbKnnGenerator.py` & `FastCG-0.0.3/FastCG/generators/ProbKnnGenerator.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,71 +17,66 @@
 #     datefmt='%Y-%m-%d:%H:%M:%S')
 
 class ProbKnnGenerator(GeneratorBase):
 
     def _preprocess_all_data(self):
         self.data_matching_condition = \
                 self.all_data[
-                    self.smart_condition.check(
-                        self.model.predict(self.all_data.drop(self.config["target"], axis=1)))
+                    self.smart_condition.check(self.model.predict(self.all_data.drop([self.config["target"]], axis=1)))
                     ]
         self.features_to_use = \
             find_feature_improtance_Anova(
                 self.data_matching_condition, 
                 self.config["max_features_to_change"],
                 self.config["features_to_change"], 
                 self.config["target"]
                 )
-        
-        if "increase_only" in self.config and "decrease_only" in self.config:
-            self.features_increase_only = self.config["increase_only"]
-            self.features_decrease_only = self.config["decrease_only"]
-        elif "increase_only" in self.config and "decrease_only" not in self.config:
+        if "increase_only" in self.config and self.config["increase_only"] is not None:
             self.features_increase_only = self.config["increase_only"]
-            _, self.features_decrease_only = find_feature_direction(self.data_matching_condition, self.features_to_use, self.config["target"])
-        elif "increase_only" not in self.config and "decrease_only" in self.config:
-            _, self.features_increase_only = find_feature_direction(self.data_matching_condition, self.features_to_use, self.config["target"])
+        else: 
+            self.features_increase_only = []
+        if "decrease_only" in self.config and self.config["decrease_only"] is not None:
             self.features_decrease_only = self.config["decrease_only"]
-        else:
-            Logger.debug("Finding features to increase and decrease by using feature direction")
-            self.features_increase_only, self.features_decrease_only = find_feature_direction(self.data_matching_condition, self.features_to_use, self.config["target"])
-
+        else: 
+            self.features_decrease_only = []
         Logger.info("Features to use: " + str(self.features_to_use))
         Logger.info("Features to increase: " + str(self.features_increase_only))
         Logger.info("Features to decrease: " + str(self.features_decrease_only))
 
         self.all_data_features_to_use = self.all_data[self.features_to_use]
-        
+        self.all_data["ID"] = self.all_data.index
+        self.id = "ID"
         self.normalizer = StandardScaler().fit(self.all_data_features_to_use)
         self.data_normalized_features_to_use = self.normalizer.transform(self.all_data_features_to_use)
         
         self.n_components = choose_pca_components(self.data_normalized_features_to_use, 0.75)
         self.pca = PCA(n_components=self.n_components).fit(self.data_normalized_features_to_use)
         self.features_pca = ['principal component ' + str(i) for i in range(1, self.n_components+1)]
         self.data_pca = convert_to_pca(self.data_matching_condition, self.pca, self.normalizer, self.features_to_use, self.features_pca)
         self.data_centroid, self.kmean_lables = find_centroid(self.data_pca.drop(self.config["target"], axis=1).copy()[self.features_pca],features_pca=self.features_pca)
 
         Logger.debug(f"training on centroids with the following features: {self.features_pca}")
         self.nbrs = NearestNeighbors(n_neighbors=2).fit(self.data_centroid) #TODO: move n_neighbors to config
 
     def _preprocess_generate(self, data) -> None:
         self.current_data = data
+        self.current_data["ID"] = self.current_data.index
     
     def _preprocess_counterfactual_targets(self, obs) -> pd.DataFrame:
         data_to_genrate = convert_to_pca(obs.to_frame().T, self.pca, self.normalizer, self.features_to_use, self.features_pca)
         data_to_genrate = data_to_genrate.fillna(0)
         return data_to_genrate
 
     def __init__(self, all_data, model, config, target, condition,verbose=0):
         super().__init__(all_data, model, config, target, condition,verbose)
 
     def _generate_single(self, original_obs, processed_obs):
         # Logger.info("Generating counterfactual for observation: " + str(processed_obs))
         indices = self.knn_on_cluster(processed_obs)
-        base_obs = self.current_data[self.current_data[self.config["ID"]] == processed_obs[self.config["ID"]].values[0]].copy()
+        base_obs = self.current_data[self.current_data[self.id] == processed_obs[self.id].values[0]]
         cf = {}
         for idx in indices:
             counterfactual = processed_obs.copy()
             for feature in self.features_pca: 
                 counterfactual[feature] = self.data_pca[feature].iloc[idx]
             
             counterfactual = convert_from_pca(counterfactual,base_obs, self.pca, self.normalizer, self.features_to_use, self.features_pca)
@@ -92,17 +87,17 @@
             for feature in self.features_decrease_only:
                 if counterfactual[feature].values[0] > original_obs[feature]:
                     counterfactual[feature].values[0] = original_obs[feature]/2            
             tmp_counterfactual = counterfactual.copy()
             if self.config["target"] in tmp_counterfactual:
                     tmp_counterfactual = counterfactual.drop(self.config["target"], axis=1)
 
-            if self.smart_condition.check(self.model.predict(tmp_counterfactual)[0]):
+            if self.smart_condition.check(self.model.predict(tmp_counterfactual.drop(self.id, axis=1)))[0]:
                 # return counterfactual
-                distance = obs_distance(counterfactual.copy(), processed_obs.copy(), self.config["target"])
+                distance = obs_distance(counterfactual.copy(), base_obs.copy(), self.config["target"])
                 if distance not in cf:
                     cf[distance] = counterfactual.copy()
         if cf:
             return cf[min(cf.keys())]
         else:
             return original_obs
     
@@ -139,28 +134,28 @@
                 idx = self.data_pca.iloc[member].name
                 if idx not in index:
                     index.append(idx)
         
         weights = []
         data_cluster = self.data_pca.loc[index] 
         for feature in data_cluster.drop(self.config["target"], axis=1).columns: 
-            if feature == self.config["ID"]:
+            if feature == self.id:
                 weights.append(0)  
             elif feature not in self.features_pca: 
                 weights.append(1)
             else:
                 weights.append(0)
         w_minkowski = partial(minkowski, p=2, w=weights)
         n_neigh = min(5, len(data_cluster))
         nbrs = NearestNeighbors(n_neighbors=n_neigh, metric=w_minkowski).fit(data_cluster.drop(self.config["target"], axis=1))
         indices = nbrs.kneighbors(obs_original, return_distance=False)
         return indices[0]
     
     def _postprocess_valid_data(self, data) -> list:        
         improve_cf = {}
-        for couterfactual in tqdm(data, desc="Improving counterfactualswith binary search"):
-            id_key = couterfactual[self.config["ID"]].values[0]
-            original_obs = self.all_data[self.all_data[self.config["ID"]] == couterfactual[self.config["ID"]].values[0]].drop(self.config["target"], axis=1).copy()
+        for couterfactual in tqdm(data, desc="Improving counterfactuals with binary search"):
+            id_key = couterfactual[self.id].values[0]
+            original_obs = self.all_data[self.all_data[self.id] == couterfactual[self.id].values[0]].drop(self.config["target"], axis=1).copy()
             cf = couterfactual.copy()
             imrpoved = improve_with_binary_search_by_vectors(original_obs, cf, self.model, self.features_to_use, self.smart_condition)
             improve_cf[id_key] = imrpoved
         return improve_cf
```

### Comparing `FastCG-0.0.2/FastCG/utils/SmartCondition.py` & `FastCG-0.0.3/FastCG/utils/SmartCondition.py`

 * *Files identical despite different names*

### Comparing `FastCG-0.0.2/FastCG/utils/logger.py` & `FastCG-0.0.3/FastCG/utils/logger.py`

 * *Files identical despite different names*

### Comparing `FastCG-0.0.2/FastCG/utils/util_functions.py` & `FastCG-0.0.3/FastCG/utils/util_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,18 @@
     start_distance = -distance
     end_distance = distance
     try:
         while (end_distance-start_distance).sum() > distance*0.001: 
             mid_point = calculate_point(original_obs,direction,(start_distance+end_distance)/2)
             mid_point = mid_point[cols]
             mid_point[features_to_use] = mid_point[features_to_use].astype(int)
-            if smart_condition.check(model.predict(mid_point)[0]): # TODO: Check why predict gave back an array instead of int / float
+            if smart_condition.check(model.predict(mid_point.drop("ID", axis=1))[0]):
                 end_distance = (start_distance+end_distance)/2
             else:
                 start_distance = (start_distance+end_distance)/2
     except Exception as e:
-        Logger.info("Error in binary search: {}".format(e))
-        Logger.info(mid_point)
+        Logger.exception("Error in binary search: {}".format(e))
+        Logger.exception(mid_point)
         return None
     end_distance += distance*0.01
-    return calculate_point(original_obs,direction,(start_distance+end_distance)/2)
+    final_point = calculate_point(original_obs,direction,end_distance)
+    return pd.DataFrame(final_point, columns=cols)
```

### Comparing `FastCG-0.0.2/README.md` & `FastCG-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `FastCG-0.0.2/setup.py` & `FastCG-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Counterfactual Generation Package'
 LONG_DESCRIPTION = 'A package that makes it easy generate counterfactuals in a fast manner'
 
 setup(
     name="FastCG",
     version=VERSION,
     description=DESCRIPTION,
```

