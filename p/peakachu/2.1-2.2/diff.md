# Comparing `tmp/peakachu-2.1.tar.gz` & `tmp/peakachu-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/peakachu-2.1.tar", last modified: Sun Nov 27 08:37:27 2022, max compression
+gzip compressed data, was "peakachu-2.2.tar", last modified: Mon May 22 01:34:10 2023, max compression
```

## Comparing `peakachu-2.1.tar` & `peakachu-2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 xtwang     (501) staff       (20)        0 2022-11-27 08:37:27.000000 peakachu-2.1/
--rw-r--r--   0 xtwang     (501) staff       (20)    37809 2022-11-27 08:37:27.000000 peakachu-2.1/PKG-INFO
--rw-r--r--   0 xtwang     (501) staff       (20)    35220 2022-11-27 08:37:14.000000 peakachu-2.1/README.md
-drwxr-xr-x   0 xtwang     (501) staff       (20)        0 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu/
--rwxr-xr-x   0 xtwang     (501) staff       (20)      103 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/__init__.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     2316 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/calculate_depth.py
--rw-r--r--   0 xtwang     (501) staff       (20)      850 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/call_loops.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     6031 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/peakacluster.py
--rw-r--r--   0 xtwang     (501) staff       (20)     5522 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/scoreUtils.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     2755 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/score_chromosome.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     3250 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/score_genome.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     4843 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/trainUtils.py
--rwxr-xr-x   0 xtwang     (501) staff       (20)     3642 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/train_models.py
--rw-r--r--   0 xtwang     (501) staff       (20)     6417 2022-11-27 08:37:14.000000 peakachu-2.1/peakachu/utils.py
-drwxr-xr-x   0 xtwang     (501) staff       (20)        0 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu.egg-info/
--rw-r--r--   0 xtwang     (501) staff       (20)    37809 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu.egg-info/PKG-INFO
--rw-r--r--   0 xtwang     (501) staff       (20)      403 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu.egg-info/SOURCES.txt
--rw-r--r--   0 xtwang     (501) staff       (20)        1 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu.egg-info/dependency_links.txt
--rw-r--r--   0 xtwang     (501) staff       (20)        9 2022-11-27 08:37:27.000000 peakachu-2.1/peakachu.egg-info/top_level.txt
-drwxr-xr-x   0 xtwang     (501) staff       (20)        0 2022-11-27 08:37:27.000000 peakachu-2.1/scripts/
--rwxr-xr-x   0 xtwang     (501) staff       (20)     4945 2022-11-27 08:37:27.000000 peakachu-2.1/scripts/peakachu
--rw-r--r--   0 xtwang     (501) staff       (20)       38 2022-11-27 08:37:27.000000 peakachu-2.1/setup.cfg
--rw-r--r--   0 xtwang     (501) staff       (20)     1649 2022-11-27 08:37:14.000000 peakachu-2.1/setup.py
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342982 peakachu-2.2/
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     1063 2023-05-22 01:34:00.000000 peakachu-2.2/LICENSE
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    81407 2023-05-22 01:34:10.342850 peakachu-2.2/PKG-INFO
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    80675 2023-05-22 01:34:00.000000 peakachu-2.2/README.md
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342148 peakachu-2.2/peakachu/
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)      103 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/__init__.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2316 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/calculate_depth.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)      850 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/call_loops.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     5829 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/peakacluster.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     5166 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/scoreUtils.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2755 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/score_chromosome.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3250 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/score_genome.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4843 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/trainUtils.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3642 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/train_models.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     6417 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/utils.py
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342594 peakachu-2.2/peakachu.egg-info/
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    81407 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)      411 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)        1 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)        9 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/top_level.txt
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342699 peakachu-2.2/scripts/
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4945 2023-05-22 01:34:10.000000 peakachu-2.2/scripts/peakachu
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)       38 2023-05-22 01:34:10.343026 peakachu-2.2/setup.cfg
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     1649 2023-05-22 01:34:00.000000 peakachu-2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `peakachu-2.1/peakachu/calculate_depth.py` & `peakachu-2.2/peakachu/calculate_depth.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/call_loops.py` & `peakachu-2.2/peakachu/call_loops.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/peakacluster.py` & `peakachu-2.2/peakachu/peakacluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             c1, s1, s2, prob, v = p[0], int(p[1]), int(p[4]), float(p[6]), float(p[7])
             if prob >= thre:
                 D[c1][(s1//res, s2//res)] = v
                 score_pool[c1][(s1//res, s2//res)] = [prob, v]
     
     results = {}
     for c in D:
-        tmp = local_clustering(D[c], res, min_count=3, r=15000)
+        tmp = local_clustering(D[c], min_count=3, r=2)
         intermediate = []
         for i in tmp:
             if i[0] in D[c]:
                 intermediate.append([D[c][i[0]], i[0]])
         intermediate.sort(reverse=True)
         if len(intermediate) > 1:
             results[c] = second_run(intermediate)
@@ -49,21 +49,15 @@
             sub = pos[labels == c]
             final_list.append(p[1])
             for t in sub:
                 visited.add((int(t[0]), int(t[1])))
     
     return final_list
 
-def find_anchors(pos, min_count=3, min_dis=15000, wlen=40000, res=10000):
-
-    min_dis = max(min_dis//res, 2)
-    if res <= 10000:
-       wlen = min(wlen//res, 20)
-    else:
-        wlen = 4
+def find_anchors(pos, min_count=3, min_dis=2, wlen=4):
 
     count = Counter(pos)
     refidx = range(min(count), max(count)+1)
     signal = np.r_[[count[i] for i in refidx]]
     summits = find_peaks(signal, height=min_count, distance=min_dis)[0]
     sorted_summits = [(signal[i],i) for i in summits]
     sorted_summits.sort(reverse=True) # sort by peak count
@@ -133,25 +127,24 @@
                 sub = np.r_[out]
             for q in Local:
                 pool.add(q)
             final_list.append((p[1], cen, rad))
         
         visited.update(pool)
 
-def local_clustering(Donuts, res, min_count=3, r=15000):
+def local_clustering(Donuts, min_count=3, r=2):
 
     final_list = []
     x = np.r_[[i[0] for i in Donuts]]
     y = np.r_[[i[1] for i in Donuts]]
     if x.size == 0:
         return final_list
 
-    x_anchors = find_anchors(x, min_count=min_count, min_dis=r, res=res)
-    y_anchors = find_anchors(y, min_count=min_count, min_dis=r, res=res)
-    r = max(r//res, 2)
+    x_anchors = find_anchors(x, min_count=min_count, min_dis=r)
+    y_anchors = find_anchors(y, min_count=min_count, min_dis=r)
     visited = set()
     lookup = set(zip(x, y))
     for x_a in x_anchors:
         for y_a in y_anchors:
             sort_list = []
             for i in range(x_a[1], x_a[2]+1):
                 for j in range(y_a[1], y_a[2]+1):
```

### Comparing `peakachu-2.1/peakachu/scoreUtils.py` & `peakachu-2.2/peakachu/scoreUtils.py`

 * *Files 15% similar despite different names*

```diff
@@ -109,28 +109,22 @@
                 p = self.model.predict_proba(fea)[:, 1]
                 pfilter = p > thre
                 ri = np.r_[ri, clist[:, 0][pfilter]]
                 ci = np.r_[ci, clist[:, 1][pfilter]]
                 prob_pool = np.r_[prob_pool, p[pfilter]]
         ri = ri.astype(int)
         ci = ci.astype(int)
-        '''
-        # finely tune the probability score by combining the Fold-enrichment score
-        prob_tuned = []
-        for i in range(ri.size):
-            fc = fc_pool[i]
-            # change 0.1 and 0.9 if more weithts need to be given to FC
-            fc_factor = (1 / (1 + np.exp(-fc)) - 0.5) / 0.5 * 0.1 + 0.9
-            p = prob_pool[i] * fc_factor
-            prob_tuned.append(p)
-        prob_pool = np.r_[prob_tuned]
-        '''
+        
+        
         result = sparse.csr_matrix((prob_pool, (ri, ci)), shape=self.M.shape)
-        data = np.array(self.M[ri, ci]).ravel()
-        self.M = sparse.csr_matrix((data, (ri, ci)), shape=self.M.shape)
+        if ri.size > 0:
+            data = np.array(self.M[ri, ci]).ravel()
+            self.M = sparse.csr_matrix((data, (ri, ci)), shape=self.M.shape)
+        else:
+            self.M = result
 
         return result, self.M
 
     def writeBed(self, outfil, prob_csr, raw_csr):
         
         with open(outfil, 'a') as out:
             r, c = prob_csr.nonzero()
```

### Comparing `peakachu-2.1/peakachu/score_chromosome.py` & `peakachu-2.2/peakachu/score_chromosome.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/score_genome.py` & `peakachu-2.2/peakachu/score_genome.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/trainUtils.py` & `peakachu-2.2/peakachu/trainUtils.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/train_models.py` & `peakachu-2.2/peakachu/train_models.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/peakachu/utils.py` & `peakachu-2.2/peakachu/utils.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/scripts/peakachu` & `peakachu-2.2/scripts/peakachu`

 * *Files identical despite different names*

### Comparing `peakachu-2.1/setup.py` & `peakachu-2.2/setup.py`

 * *Files identical despite different names*

