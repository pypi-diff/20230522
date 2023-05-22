# Comparing `tmp/grewpy-0.3.0.tar.gz` & `tmp/grewpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grewpy-0.3.0.tar", last modified: Tue Apr 11 16:10:10 2023, max compression
+gzip compressed data, was "grewpy-0.4.0.tar", last modified: Mon May 22 13:57:03 2023, max compression
```

## Comparing `grewpy-0.3.0.tar` & `grewpy-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.744245 grewpy-0.3.0/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-04-11 16:10:10.744132 grewpy-0.3.0/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.3.0/README.md
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.741142 grewpy-0.3.0/examples/
--rw-r--r--   0 guillaum   (501) staff       (20)     2057 2023-04-11 16:02:43.000000 grewpy-0.3.0/examples/allemand.py
--rw-r--r--   0 guillaum   (501) staff       (20)     4786 2023-02-21 09:38:54.000000 grewpy-0.3.0/examples/classifier.py
--rw-r--r--   0 guillaum   (501) staff       (20)    17839 2023-02-21 09:38:54.000000 grewpy-0.3.0/examples/learner.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-02-07 12:49:09.000000 grewpy-0.3.0/examples/test_GRS.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2687 2023-04-11 16:00:39.000000 grewpy-0.3.0/examples/test_corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.3.0/examples/test_graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.3.0/examples/test_grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1405 2023-01-09 12:56:06.000000 grewpy-0.3.0/examples/test_search.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.743339 grewpy-0.3.0/grewpy/
--rw-r--r--   0 guillaum   (501) staff       (20)      340 2023-02-13 12:14:28.000000 grewpy-0.3.0/grewpy/__init__.py
--rw-r--r--   0 guillaum   (501) staff       (20)     8975 2023-04-11 16:02:47.000000 grewpy-0.3.0/grewpy/corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)     8497 2023-04-11 16:02:43.000000 grewpy-0.3.0/grewpy/graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.3.0/grewpy/grew.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2544 2023-04-11 16:02:43.000000 grewpy-0.3.0/grewpy/grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)    12874 2023-04-11 16:02:47.000000 grewpy-0.3.0/grewpy/grs.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.3.0/grewpy/matchings.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2980 2023-02-23 10:39:26.000000 grewpy-0.3.0/grewpy/network.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.3.0/grewpy/observation.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1259 2023-03-31 09:13:11.000000 grewpy-0.3.0/grewpy/sketch.py
--rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.3.0/grewpy/utils.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.743975 grewpy-0.3.0/grewpy.egg-info/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      513 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/SOURCES.txt
--rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/dependency_links.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/top_level.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-04-11 16:10:10.744284 grewpy-0.3.0/setup.cfg
--rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-04-11 16:10:02.000000 grewpy-0.3.0/setup.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-05-22 13:57:03.853682 grewpy-0.4.0/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-05-22 13:57:03.853572 grewpy-0.4.0/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.4.0/README.md
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-05-22 13:57:03.850995 grewpy-0.4.0/examples/
+-rw-r--r--   0 guillaum   (501) staff       (20)     2057 2023-04-11 16:02:43.000000 grewpy-0.4.0/examples/allemand.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     4741 2023-05-22 13:43:57.000000 grewpy-0.4.0/examples/classifier.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     6822 2023-05-22 13:43:57.000000 grewpy-0.4.0/examples/learner.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9359 2023-05-22 13:43:57.000000 grewpy-0.4.0/examples/rule_forgery.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-05-02 13:38:29.000000 grewpy-0.4.0/examples/test_GRS.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2687 2023-04-11 16:00:39.000000 grewpy-0.4.0/examples/test_corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.4.0/examples/test_graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.4.0/examples/test_grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1405 2023-01-09 12:56:06.000000 grewpy-0.4.0/examples/test_search.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-05-22 13:57:03.852879 grewpy-0.4.0/grewpy/
+-rw-r--r--   0 guillaum   (501) staff       (20)      365 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/__init__.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9099 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9316 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.4.0/grewpy/grew.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2737 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)    13053 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/grs.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.4.0/grewpy/matchings.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2938 2023-05-22 13:43:46.000000 grewpy-0.4.0/grewpy/network.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.4.0/grewpy/observation.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1099 2023-05-22 13:43:57.000000 grewpy-0.4.0/grewpy/sketch.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.4.0/grewpy/utils.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-05-22 13:57:03.853427 grewpy-0.4.0/grewpy.egg-info/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-05-22 13:57:03.000000 grewpy-0.4.0/grewpy.egg-info/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      538 2023-05-22 13:57:03.000000 grewpy-0.4.0/grewpy.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-05-22 13:57:03.000000 grewpy-0.4.0/grewpy.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-05-22 13:57:03.000000 grewpy-0.4.0/grewpy.egg-info/top_level.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-05-22 13:57:03.853716 grewpy-0.4.0/setup.cfg
+-rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-05-22 13:45:25.000000 grewpy-0.4.0/setup.py
```

### Comparing `grewpy-0.3.0/examples/allemand.py` & `grewpy-0.4.0/examples/allemand.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/examples/classifier.py` & `grewpy-0.4.0/examples/classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,15 @@
             nodes = m['matching']['nodes']
             obs = [0]*len(self.pos)
             for n in nodes:
                 feat = graph[nodes[n]]
                 for k, v in feat.items():
                     if (n, k, v) in self.pos:
                         obs[self.pos[(n, k, v)]] = 1
-            es = {e for e in graph.edges(
-                nodes['X'], nodes['Y']) if "rank" in e}
+            es = graph.edges(nodes['X'], nodes['Y'])
             if len(es) > 1:
                 print("mmmmhh that should not happen")
             elif len(es) <= 1:
                 e = es.pop() if es else None
                 if e not in y1:
                     y1[e] = len(y1)
                 y.append(y1[e])
```

### Comparing `grewpy-0.3.0/examples/test_GRS.py` & `grewpy-0.4.0/examples/test_GRS.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/examples/test_corpus.py` & `grewpy-0.4.0/examples/test_corpus.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/examples/test_graph.py` & `grewpy-0.4.0/examples/test_graph.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/examples/test_grew_web.py` & `grewpy-0.4.0/examples/test_grew_web.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/examples/test_search.py` & `grewpy-0.4.0/examples/test_search.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/grewpy/corpus.py` & `grewpy-0.4.0/grewpy/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 
     def apply(self, fun):
         """
         Apply fun to all graphs, return the new Corpus
         """
         return CorpusDraft({sid : fun(self[sid]) for sid in self})
 
+    def to_conll(self):
+        return Corpus(self).to_conll()
 
 class Corpus(AbstractCorpus):
     def __init__(self, data):
         """An abstract corpus
         :param data: a file, a list of files or a CoNLL string representation of a corpus
         :return: an integer index for latter reference to the corpus
         :raise an error if the files was not correctly loaded
@@ -116,15 +118,15 @@
             reply = network.send_and_receive(req)
         elif isinstance(data, dict):
             req = {"command": "corpus_from_dict", "graphs": {
                 sent_id: graph.json_data() for (sent_id, graph) in data.items()}}
             reply = network.send_and_receive(req)
         elif os.path.isdir(data):
             # load of connlu files of the directory
-            file_list = glob.glob(f"{data}/*.conllu")
+            file_list = glob.glob(f"{data}/*.conllu") + glob.glob(f"{data}/*.conll") + glob.glob(f"{data}/*.cupt")
             req = {"command": "corpus_load", "files": file_list}
             reply = network.send_and_receive(req)
         elif os.path.isfile(data):
             req = {"command": "corpus_load", "files": [data]}
             reply = network.send_and_receive(req)
         else:
             with tempfile.NamedTemporaryFile(mode="w", delete=True, suffix=".conll") as f:
```

### Comparing `grewpy-0.3.0/grewpy/graph.py` & `grewpy-0.4.0/grewpy/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,55 @@
     def __init__(self,data):
         if isinstance(data,str):
             #try to split a dict
             if "=" in data and "," in data:
                 #suppose it is a dictionary
                 super().__init__(Fs_edge.decompose_edge(data))
             else:
-                super().__init__({"1": data})
+                super().__init__(Fs_edge.decompose_edge(data))
         elif isinstance(data, dict):
-            super().__init__(data)
+            clauses = dict()
+            for k in data:
+                Fs_edge.extract(data[k],clauses, k)
+            super().__init__(clauses)
         else:
             raise ValueError(f"data is not a feature structure {data}")
 
+    def __eq__(self, other):
+        for k,v in self.items():
+            if k not in other or v != other[k]:
+                return False
+        return len(self) == len(other)
+
+    def __neq__(self, other):
+        return not self.__eq__(other)
+
     def __hash__(self):
-        return (hash (str(self)))
+        return hash(tuple((sorted(self.items()))))
     
     @staticmethod
+    def extract(u, clauses, key='1'):
+            if '@' in u:
+                u, t = u.split('@')
+                clauses['deep'] = t
+            if ':' in u:
+                u,t = u.split(':')
+                clauses['1'] = u
+                clauses['2'] = t
+            else:
+                clauses[key] = u
+    @staticmethod
     def decompose_edge(s):
         clauses = dict()
         for it in s.split(","):
-            a, b = it.split("=")
-            clauses[a] = b
+            if '=' in s:
+                a,b = it.split("=")
+                clauses[a] = b
+            else:
+                Fs_edge.extract(s,clauses)
         return clauses
 
 class Graph():
     """
     a dict mapping node keys to feature structure
 
     with extra data:
@@ -64,18 +90,19 @@
             self.order = list(data.order)  
         elif data is None:
             self.features = kwargs.get("features", dict())
             self.order = kwargs.get("order", [])
             self.meta = kwargs.get("meta", dict())
             self._sucs = kwargs.get("sucs", dict())
         elif isinstance(data, dict):
-            self.features = data.get("features", dict())
-            self.order = data.get("order", [])
-            self.meta = data.get("meta", dict())
-            self._sucs = data.get("sucs", dict())
+            (features, sucs, meta, order) = Graph._from_json(data)
+            self.features = features
+            self.order = order
+            self.meta = meta            
+            self._sucs = sucs
         elif isinstance(data,str):
             #either filename, json or conll
             if os.path.isfile(data):
                 req = {"command": "graph_load", "file": data}
                 data_json = network.send_and_receive(req)
             else:
                 try:
```

### Comparing `grewpy-0.3.0/grewpy/grew.py` & `grewpy-0.4.0/grewpy/grew.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/grewpy/grew_web.py` & `grewpy-0.4.0/grewpy/grew_web.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # used for launching grew web on a given corpus
 import tempfile
 import requests
 import webbrowser
 import http
 import json
 from .grew import GrewError
+from grewpy import GRSDraft
 
 
 local = False
 if local:
     grew_web_back = "http://localhost:8080"
     grew_web_front = "http://localhost:8888/grew_web"
 else:
@@ -48,15 +49,20 @@
         with tempfile.NamedTemporaryFile(mode="a+", delete=True, suffix=".grs") as f:
             f.write(json.dumps(json_grs))
             f.seek(0)  # ready to be read
             r = requests.post(f"{grew_web_back}/upload_grs",
                           data={"session_id": self.session_id},
                           files={"json_file": f}
                           )
-            _post_request("upload_grs", r)
+            try:
+                _post_request("upload_grs", r)
+            except GrewError:
+                with open("error.grs","w") as g:
+                    g.write(str(GRSDraft(grs)))
+                
 
 
     def load_corpus(self,   corpus):
         conll = corpus.to_conll()
         if self.session_id == "":
             raise GrewError({"grew_web": "not connected"})
         with tempfile.NamedTemporaryFile(mode="a+", delete=True, suffix=".conllu") as f:
```

### Comparing `grewpy-0.3.0/grewpy/grs.py` & `grewpy-0.4.0/grewpy/grs.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,20 @@
 class Delete_edge(Command):
     def __init__(self, X, e, Y):
         super().__init__(f"del_edge {X}-[{e}]->{Y}")
         self.X, self.e, self.Y = X, e, Y
 
     def safe(self):           
         return RequestItem("pattern", self.item.replace("add_edge", ""))
+    
+class Delete_feature(Command):
+    def __init__(self, X, f):
+        super().__init__(f"del_feat {X}.{f}")
+        self.X = X
+        self.f = f
 
 
 class Commands(list):
     def __init__(self, *L):
         super().__init__()
         for elt in L:
             if isinstance(elt,str):
@@ -290,14 +296,18 @@
             safe_rule = Rule(safe_request, rule.commands, rule.lexicons)
             grs[rule_name] = safe_rule
         return grs
 
     def onf(self, strat_name="main"):
         self[strat_name] = f'Onf(Alt({",".join(self.rules())}))'
         return self
+    
+    def save(self, filename):
+        with open(filename, "w") as f:
+            f.write(str(self))
       
 class GRS:
     """
     An abstract GRS. Offers the possibility to apply rewriting.
     The object is abstract and cannot be changed. 
     For that, use a GRSDraft
     """
@@ -337,18 +347,17 @@
 
     def __str__(self):
         return f"GRS({self.id})"
 
     def run(self, data, strat="main"):
         """
         run a Grs on a graph
-        :param grs_data: a graph rewriting system or a Grew string representation of a grs
-        :param G: the graph, either a str (in grew format) or a dict
+        :param data: a graph or an AbstractCorpus
         :param strat: the strategy (by default "main")
-        :return: the list of rewritten graphs
+        :return: a dictionary mapping sid to the list of rewritten graphs
         """
         if isinstance(data, Graph):
             req = {
                 "command": "grs_run_graph",
                 "graph": json.dumps(data.json_data()),
                 "grs_index": self.id,
                 "strat": strat
@@ -392,7 +401,9 @@
                 "strat": strat
             } # return None because inplace
             network.send_and_receive(req)
             return data if abstract else CorpusDraft (data)
         elif isinstance(data, CorpusDraft):
             acorpus = Corpus(data)
             self.apply(acorpus, strat, abstract)
+
+
```

### Comparing `grewpy-0.3.0/grewpy/matchings.py` & `grewpy-0.4.0/grewpy/matchings.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/grewpy/network.py` & `grewpy-0.4.0/grewpy/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ''' Utility tools to connect to ocaml GREW'''
 
-import subprocess
+from subprocess import Popen, PIPE
 import time
 import socket
 import os.path
 import json
 import os
 import sys
 
@@ -29,30 +29,30 @@
         return 0
 
 def init():
     global port, remote_ip, caml_pid
     grewpy = "grewpy_backend"
     if not pid_exist(caml_pid):
         python_pid = os.getpid()
-        while (port<8898):
-            caml = subprocess.Popen(
-                [grewpy, "--caller", str(python_pid), "--port", str(port)],
-                preexec_fn=preexec_function
-            )
-            caml_pid = caml.pid
-            #wait for grew's lib answer
-            time.sleep(0.1)
-            if caml.poll() == None:
-                print ("connected to port: " + str(port), file=sys.stderr)
-                remote_ip = socket.gethostbyname(host)
-                return (caml)
-            else:
-                port += 1
-        print ("Failed to connect 10 times!", file=sys.stderr)
-        exit (1)
+        caml = Popen(
+            [grewpy, "--caller", str(python_pid)],
+            preexec_fn=preexec_function,
+            stdout=PIPE
+        )
+        port = int(caml.stdout.readline().strip())
+        caml_pid = caml.pid
+        #wait for grew's lib answer
+        time.sleep(0.1)
+        if caml.poll() == None:
+            print ("connected to port: " + str(port), file=sys.stderr)
+            remote_ip = socket.gethostbyname(host)
+            return (caml)
+        else:
+            print ("Failed to connect", file=sys.stderr)
+            exit (1)
 
 def connect():
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.connect((remote_ip, port))
         return s
     except socket.error:
```

### Comparing `grewpy-0.3.0/grewpy/observation.py` & `grewpy-0.4.0/grewpy/observation.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.3.0/grewpy/sketch.py` & `grewpy-0.4.0/grewpy/sketch.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,21 +12,17 @@
         self.P = P
         self.cluster_criterion = cluster_criterion
         self.avec = avec
         self.without = without
         self.target = target
 
     def cluster(self, corpus):
-        """
-        search for a link X -> Y with respect to the sketch in the corpus
-        we build a cluster depending on cluster criterion (e.g. X.upos, Y.upos)
-        """
-        P1 = self.avec(self.P)
-        obs = corpus.count(P1, self.cluster_criterion, [self.target], True)
-        if not obs:
-            return obs
-        W1 = self.without(Request(self.P))
-        clus = corpus.count(W1, self.cluster_criterion, [], True)
-        for L in obs:
-            if L in clus:
-                obs[L][''] = clus[L][tuple()]
-        return obs
+        def _none_(n):
+            return '' if '__none__' in n else n[0]
+        obs2 = corpus.count(self.P, self.cluster_criterion, ["X->Y"], True)
+        obs3 = dict()
+        for k1, o1 in obs2.obs.items():
+            if len(o1) == 1 and ('__none__',) in o1:
+                ...
+            else:
+                obs3[k1] = {_none_(k2) : v for k2,v in o1.items()}
+        return obs3
```

