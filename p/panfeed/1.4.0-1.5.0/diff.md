# Comparing `tmp/panfeed-1.4.0.tar.gz` & `tmp/panfeed-1.5.0.tar.gz`

## Comparing `panfeed-1.4.0.tar` & `panfeed-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.4.0/environment.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-runner.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/__init__.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/get_kmers.py
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/panfeed.py
--rw-r--r--   0        0        0    16450 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.4.0/LICENSE
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.4.0/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.0/environment.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/__init__.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/panfeed.py
+-rw-r--r--   0        0        0    17064 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.5.0/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.5.0/PKG-INFO
```

### Comparing `panfeed-1.4.0/panfeed/__main__.py` & `panfeed-1.5.0/panfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/classes.py` & `panfeed-1.5.0/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/colorlog.py` & `panfeed-1.5.0/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/get_clusters.py` & `panfeed-1.5.0/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/get_kmers.py` & `panfeed-1.5.0/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/input.py` & `panfeed-1.5.0/panfeed/input.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/panfeed.py` & `panfeed-1.5.0/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/panfeed/plot.py` & `panfeed-1.5.0/panfeed/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
             if len(yindex) > 0:
                 yindex = yindex[0]
             else:
                 yindex = None
         else:
             logger.info("Phenotype is continuos")
         logger.info(f"sorting samples by their {args.phenotype_column} phenotype")
+        logger.info(f"ties will be broken by association p-value")
     else:
         logger.info(f"sorting samples by their lowest association p-value")
         if args.sample is not None:
             p = p.sample(frac=args.sample)
     strains = set(p.index)
     logger.info(f"plots will include {len(strains)} samples")
 
@@ -262,15 +263,19 @@
         if len(strains.difference(g.index)) > 0:
             g = g.reindex(sorted(g.index) + sorted(strains.difference(g.index)))
         if args.phenotype_column is None:
             # sort the table by p-values
             g = g.loc[g.fillna(0).T.max().sort_values(ascending=False).index]
         else:
             # sort by phenotype
-            g = g.loc[p.index]
+            df_sort = p.to_frame().join(g.fillna(0).T.max().to_frame(), how='outer')
+            df_sort.columns = ['pheno', 'pvalue']
+            df_sort = df_sort.fillna(0)
+            df_sort = df_sort.sort_values(['pheno', 'pvalue'], ascending=False)
+            g = g.loc[df_sort.index]
 
         # nucleotide matrix
         b = cl.pivot_table(index='strain', columns='gene_start',
                            values='scalar',
                            aggfunc=handle_paralogs)
         # add missing positions, if any
         b = b.reindex(columns=range(cl['gene_start'].min(), cl['gene_start'].max()+1))
@@ -295,15 +300,19 @@
                 t = t.reindex(sorted(t.index) + sorted(strains.difference(t.index)),
                               fill_value='-')
             if args.phenotype_column is None:
                 # sort the table by p-values
                 t = t.loc[g.index]
             else:
                 # sort by phenotype
-                t = t.loc[p.index]
+                df_sort = p.to_frame().join(g.fillna(0).T.max().to_frame(), how='outer')
+                df_sort.columns = ['pheno', 'pvalue']
+                df_sort = df_sort.fillna(0)
+                df_sort = df_sort.sort_values(['pheno', 'pvalue'], ascending=False)
+                t = t.loc[df_sort.index]
 
         # find the index for the gene start (if present)
         gene_start = [i for i, x in enumerate(g.columns)
                       if x == 0]
         if len(gene_start) > 0:
             gene_start = gene_start[0]
         else:
```

### Comparing `panfeed-1.4.0/LICENSE` & `panfeed-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/README.md` & `panfeed-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/pyproject.toml` & `panfeed-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.4.0/PKG-INFO` & `panfeed-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.4.0
+Version: 1.5.0
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

