# Comparing `tmp/ipywardley-0.0.5.tar.gz` & `tmp/ipywardley-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywardley-0.0.5.tar", last modified: Thu May 18 15:05:26 2023, max compression
+gzip compressed data, was "ipywardley-0.0.6.tar", last modified: Sun May 21 22:43:08 2023, max compression
```

## Comparing `ipywardley-0.0.5.tar` & `ipywardley-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1810 2023-05-18 15:04:58.849881 ipywardley-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2023-04-11 11:12:17.266035 ipywardley-0.0.5/LICENSE
--rw-r--r--   0        0        0     2738 2023-04-11 11:12:17.266191 ipywardley-0.0.5/README.md
--rw-r--r--   0        0        0   241725 2023-04-11 11:12:17.268171 ipywardley-0.0.5/doc/example.png
--rw-r--r--   0        0        0      194 2023-05-18 15:04:15.582056 ipywardley-0.0.5/ipywardley/__init__.py
--rw-r--r--   0        0        0     9917 2023-05-18 15:01:40.028249 ipywardley-0.0.5/ipywardley/wardley.py
--rw-r--r--   0        0        0      466 2023-05-18 15:02:47.122315 ipywardley-0.0.5/pyproject.toml
--rw-r--r--   0        0        0  1313519 2023-04-11 11:12:17.274398 ipywardley-0.0.5/test/wardley-maps.ipynb
--rw-r--r--   0        0        0      772 2023-04-11 11:12:17.274563 ipywardley-0.0.5/test/wardley-test.owm
--rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 ipywardley-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1810 2023-05-18 15:04:58.849881 ipywardley-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2023-04-11 11:12:17.266035 ipywardley-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3072 2023-05-21 22:41:36.238757 ipywardley-0.0.6/README.md
+-rw-r--r--   0        0        0   241725 2023-04-11 11:12:17.268171 ipywardley-0.0.6/doc/example.png
+-rw-r--r--   0        0        0      194 2023-05-21 22:38:50.654086 ipywardley-0.0.6/ipywardley/__init__.py
+-rw-r--r--   0        0        0    10991 2023-05-21 22:35:53.157331 ipywardley-0.0.6/ipywardley/wardley.py
+-rw-r--r--   0        0        0      466 2023-05-18 15:02:47.122315 ipywardley-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0  1313519 2023-04-11 11:12:17.274398 ipywardley-0.0.6/test/wardley-maps.ipynb
+-rw-r--r--   0        0        0      772 2023-04-11 11:12:17.274563 ipywardley-0.0.6/test/wardley-test.owm
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 ipywardley-0.0.6/PKG-INFO
```

### Comparing `ipywardley-0.0.5/.gitignore` & `ipywardley-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.5/LICENSE` & `ipywardley-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.5/README.md` & `ipywardley-0.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,17 @@
   - [ ] `y-axis Value Chain->Invisible->Visible` or `y-axis none` to make 'Visibility' axis optional.
   - [ ] `evolve`
   - [ ] `annotation` & `annotations`?
   - [x] `note`?
   - [ ] `market` nodes?
   - [ ] `pipeline` nodes?
   - [ ] node `inertia`?
-  - [ ] `+<>`, `+>`, `+<` links to indicate flow?
+  - [x] `+<>` links to indicate flow.
+  - [ ] `+>` links to indicate flow.
+  - [ ] `+<` links to indicate flow.
   - [ ] `Hot Water+'$0.10'>Kettle` flow labels?
   - [ ] `build`, `buy`, `outsource` node augmentation?
   - [ ] `submap` and related syntax?
   - [ ] `pioneer`, `settler`, `townplanner` areas/boxes?
 - [ ] Add 'Uncharted' and 'Industrialised' labels
 - [ ] Support rendering from a file, via e.g. `%wardley file=example.owm style=plain`
 - [ ] Make it easier to download the SVG/rendered version?
@@ -60,7 +62,16 @@
 1. Clone this directory.
 2. Set up a `virtualenv` and activate it.
 3. Modify the code.
 4. Run `flit install`
 5. Run `jupyter-lab` and test your changes.
 6. Repeat 3-5 _ad infinitum_.
 7. Turn your changes into a pull request.
+
+
+## Change Log
+
+- 0.0.6:
+  - [Added support for the bluelines +<> within Wardley Maps code.](https://github.com/anjackson/ipywardley/pull/7)
+- 0.0.5:
+  - [Updated the 'b' parameter to 'visibility' as 'b' now depreciated.](https://github.com/anjackson/ipywardley/pull/6)
+
```

### Comparing `ipywardley-0.0.5/doc/example.png` & `ipywardley-0.0.6/doc/example.png`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.5/ipywardley/wardley.py` & `ipywardley-0.0.6/ipywardley/wardley.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     _note_regex = re.compile(r"^(\w+) ([\S ]+)\s+{COORDS}\s*".format(COORDS=_coords_regexs))
 
     def __init__(self, owm):
         # Defaults:
         self.title = None
         self.nodes = {}
         self.edges = []
+        self.bluelines = []
         self.evolutions = {}
         self.annotations = []
         self.annotation = {}
         self.notes = []
         self.style = None
         self.warnings = []
 
@@ -60,14 +61,22 @@
                     # And store it:
                     self.nodes[node['title']] = node
                 else:
                     self.warnings.append("Could not parse component line: %s" % cl)
             elif "->" in cl:
                 n_from, n_to = cl.split('->')
                 self.edges.append([n_from.strip(), n_to.strip()])
+            elif "+<>" in cl:
+                edge_parts = cl.split('+<>')
+                if len(edge_parts) != 2:
+                    self.warnings.append(f"Unexpected format for blueline definition: {cl}. Skipping this edge.")
+                    continue
+                n_from, n_to = edge_parts
+                self.bluelines.append([n_from.strip(), n_to.strip()])
+                continue
             elif cl.startswith('evolve '):
                 match = self._evolve_regex.search(cl)
                 if match != None:
                     matches = match.groups()
                     evol = {
                         'title' : matches[0],
                         'mat' : float(matches[1])
@@ -204,15 +213,30 @@
                 for n in edge:
                     if n not in wm.nodes:
                         self.show_warning("Could not find a component called '%s'!" % n)
         if len(l) > 0:
             lc = LineCollection(l, color=matplotlib.rcParams['axes.edgecolor'], lw=1)
             #lc = LineCollection(l, color="k", lw=1, linestyle=['-'])
             ax.add_collection(lc)
-
+            
+        # Plot bluelines :
+        b = []
+        for blueline in wm.bluelines:
+            if blueline[0] in wm.nodes and blueline[1] in wm.nodes:
+                n_from = wm.nodes[blueline[0]]
+                n_to = wm.nodes[blueline[1]]
+                b.append([ (n_from['mat'],n_from['vis']), (n_to['mat'],n_to['vis']) ])
+            else:
+                for n in blueline:
+                    if n not in wm.nodes:
+                        show_warning("Could not find a component called '%s'!" % n)
+        if len(b) > 0:
+            lc = LineCollection(b, color='blue', lw=2)
+            ax.add_collection(lc)       
+            
         # Add the nodes:
         for node_title in wm.nodes:
             n = wm.nodes[node_title]
             if n['type'] == 'component':
                 #plt.plot(n['mat'], n['vis'], marker='o', color='w', markeredgecolor='k', markeredgewidth=1.0)
                 plt.plot(n['mat'], n['vis'], marker='o', color=matplotlib.rcParams['axes.facecolor'], 
                     markeredgecolor=matplotlib.rcParams['axes.edgecolor'])
```

### Comparing `ipywardley-0.0.5/test/wardley-maps.ipynb` & `ipywardley-0.0.6/test/wardley-maps.ipynb`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.5/test/wardley-test.owm` & `ipywardley-0.0.6/test/wardley-test.owm`

 * *Files identical despite different names*

### Comparing `ipywardley-0.0.5/PKG-INFO` & `ipywardley-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywardley
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bringing Wardley Map magic to Jupyter notebooks.
 Home-page: https://github.com/anjackson/ipywardley
 Author: Andrew N. Jackson
 Author-email: anj@anjackson.net
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: ipython
@@ -56,15 +56,17 @@
   - [ ] `y-axis Value Chain->Invisible->Visible` or `y-axis none` to make 'Visibility' axis optional.
   - [ ] `evolve`
   - [ ] `annotation` & `annotations`?
   - [x] `note`?
   - [ ] `market` nodes?
   - [ ] `pipeline` nodes?
   - [ ] node `inertia`?
-  - [ ] `+<>`, `+>`, `+<` links to indicate flow?
+  - [x] `+<>` links to indicate flow.
+  - [ ] `+>` links to indicate flow.
+  - [ ] `+<` links to indicate flow.
   - [ ] `Hot Water+'$0.10'>Kettle` flow labels?
   - [ ] `build`, `buy`, `outsource` node augmentation?
   - [ ] `submap` and related syntax?
   - [ ] `pioneer`, `settler`, `townplanner` areas/boxes?
 - [ ] Add 'Uncharted' and 'Industrialised' labels
 - [ ] Support rendering from a file, via e.g. `%wardley file=example.owm style=plain`
 - [ ] Make it easier to download the SVG/rendered version?
@@ -75,7 +77,16 @@
 2. Set up a `virtualenv` and activate it.
 3. Modify the code.
 4. Run `flit install`
 5. Run `jupyter-lab` and test your changes.
 6. Repeat 3-5 _ad infinitum_.
 7. Turn your changes into a pull request.
 
+
+## Change Log
+
+- 0.0.6:
+  - [Added support for the bluelines +<> within Wardley Maps code.](https://github.com/anjackson/ipywardley/pull/7)
+- 0.0.5:
+  - [Updated the 'b' parameter to 'visibility' as 'b' now depreciated.](https://github.com/anjackson/ipywardley/pull/6)
+
+
```

