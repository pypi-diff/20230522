# Comparing `tmp/databased-2.3.0.tar.gz` & `tmp/databased-2.4.0.tar.gz`

## Comparing `databased-2.3.0.tar` & `databased-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 databased-2.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.3.0/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.3.0/docs/index.html
--rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.3.0/docs/search.js
--rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.3.0/docs/databased/customshell.html
--rw-r--r--   0        0        0   428406 2020-02-02 00:00:00.000000 databased-2.3.0/docs/databased/databased.html
--rw-r--r--   0        0        0   127332 2020-02-02 00:00:00.000000 databased-2.3.0/docs/databased/dbparsers.html
--rw-r--r--   0        0        0   315998 2020-02-02 00:00:00.000000 databased-2.3.0/docs/databased/dbshell.html
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.3.0/src/databased/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.3.0/src/databased/customshell.py
--rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 databased-2.3.0/src/databased/databased.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 databased-2.3.0/src/databased/dbparsers.py
--rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 databased-2.3.0/src/databased/dbshell.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.3.0/LICENSE.txt
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.3.0/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 databased-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 databased-2.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.4.0/docs/index.html
+-rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.4.0/docs/search.js
+-rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/customshell.html
+-rw-r--r--   0        0        0   428406 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/databased.html
+-rw-r--r--   0        0        0   127332 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0   318210 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/dbshell.html
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/customshell.py
+-rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/databased.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/dbshell.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.4.0/README.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 databased-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.4.0/PKG-INFO
```

### Comparing `databased-2.3.0/CHANGELOG.md` & `databased-2.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 # Changelog
 
-## 2.2.1 (2023-05-08)
+## 2.3.0 (2023-05-13)
+
+#### Refactorings
+
+* use griddle.griddy in data_to_string()
+
+
+## v2.2.1 (2023-05-08)
 
 #### Fixes
 
-* do_vacuum actually calls vacuum function now
+* do_vacuum actually calls vacuum function now smh
+#### Others
+
+* build v2.2.1
+* update changelog
 
 
 ## v2.2.0 (2023-05-08)
 
 #### New Features
 
+* add backup parser
+#### Refactorings
+
 * add timestamp option to dbshell backup command
 #### Others
 
 * build v2.2.0
 * update changelog
```

### Comparing `databased-2.3.0/docs/databased.html` & `databased-2.4.0/docs/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/docs/search.js` & `databased-2.4.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/docs/databased/customshell.html` & `databased-2.4.0/docs/databased/customshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/docs/databased/databased.html` & `databased-2.4.0/docs/databased/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/docs/databased/dbparsers.html` & `databased-2.4.0/docs/databased/dbparsers.html`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/docs/databased/dbshell.html` & `databased-2.4.0/docs/databased/dbshell.html`

 * *Files 0% similar despite different names*

```diff
@@ -117,318 +117,322 @@
 
                 
                         <input id="mod-dbshell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-dbshell-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argshell</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">dbparsers</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">dbparsers</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="k">class</span> <span class="nc">DBShell</span><span class="p">(</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShell</span><span class="p">):</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting dbshell (enter help or ? for arg info)...&quot;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;based&gt;&quot;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="n">dbpath</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>                <span class="p">{</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>                <span class="p">}</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="p">]</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>                <span class="p">)</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                <span class="p">)</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                <span class="p">)</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>                    <span class="k">continue</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>                <span class="p">)</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="k">class</span> <span class="nc">DBShell</span><span class="p">(</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShell</span><span class="p">):</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting dbshell (enter help or ? for arg info)...&quot;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;based&gt;&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="n">dbpath</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="p">)</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>                <span class="p">{</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>                <span class="p">}</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="p">]</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>                <span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>                <span class="p">)</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                    <span class="k">continue</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                <span class="p">)</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DBShell">
                             <input id="DBShell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -436,309 +440,312 @@
     <span class="def">class</span>
     <span class="name">DBShell</span><wbr>(<span class="base">argshell.argshell.ArgShell</span>):
 
                 <label class="view-source-button" for="DBShell-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell-8"><a href="#DBShell-8"><span class="linenos">  8</span></a><span class="k">class</span> <span class="nc">DBShell</span><span class="p">(</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShell</span><span class="p">):</span>
-</span><span id="DBShell-9"><a href="#DBShell-9"><span class="linenos">  9</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting dbshell (enter help or ? for arg info)...&quot;</span>
-</span><span id="DBShell-10"><a href="#DBShell-10"><span class="linenos"> 10</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;based&gt;&quot;</span>
-</span><span id="DBShell-11"><a href="#DBShell-11"><span class="linenos"> 11</span></a>    <span class="n">dbpath</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-12"><a href="#DBShell-12"><span class="linenos"> 12</span></a>
-</span><span id="DBShell-13"><a href="#DBShell-13"><span class="linenos"> 13</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-14"><a href="#DBShell-14"><span class="linenos"> 14</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
-</span><span id="DBShell-15"><a href="#DBShell-15"><span class="linenos"> 15</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell-16"><a href="#DBShell-16"><span class="linenos"> 16</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-17"><a href="#DBShell-17"><span class="linenos"> 17</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-18"><a href="#DBShell-18"><span class="linenos"> 18</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-19"><a href="#DBShell-19"><span class="linenos"> 19</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell-20"><a href="#DBShell-20"><span class="linenos"> 20</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-21"><a href="#DBShell-21"><span class="linenos"> 21</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-22"><a href="#DBShell-22"><span class="linenos"> 22</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-23"><a href="#DBShell-23"><span class="linenos"> 23</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
-</span><span id="DBShell-24"><a href="#DBShell-24"><span class="linenos"> 24</span></a>
-</span><span id="DBShell-25"><a href="#DBShell-25"><span class="linenos"> 25</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-26"><a href="#DBShell-26"><span class="linenos"> 26</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
-</span><span id="DBShell-27"><a href="#DBShell-27"><span class="linenos"> 27</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell-28"><a href="#DBShell-28"><span class="linenos"> 28</span></a>
-</span><span id="DBShell-29"><a href="#DBShell-29"><span class="linenos"> 29</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
-</span><span id="DBShell-30"><a href="#DBShell-30"><span class="linenos"> 30</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-31"><a href="#DBShell-31"><span class="linenos"> 31</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell-32"><a href="#DBShell-32"><span class="linenos"> 32</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-33"><a href="#DBShell-33"><span class="linenos"> 33</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
-</span><span id="DBShell-34"><a href="#DBShell-34"><span class="linenos"> 34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-35"><a href="#DBShell-35"><span class="linenos"> 35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-36"><a href="#DBShell-36"><span class="linenos"> 36</span></a>
-</span><span id="DBShell-37"><a href="#DBShell-37"><span class="linenos"> 37</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-38"><a href="#DBShell-38"><span class="linenos"> 38</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell-39"><a href="#DBShell-39"><span class="linenos"> 39</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-40"><a href="#DBShell-40"><span class="linenos"> 40</span></a>
-</span><span id="DBShell-41"><a href="#DBShell-41"><span class="linenos"> 41</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
-</span><span id="DBShell-42"><a href="#DBShell-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-43"><a href="#DBShell-43"><span class="linenos"> 43</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
-</span><span id="DBShell-44"><a href="#DBShell-44"><span class="linenos"> 44</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-45"><a href="#DBShell-45"><span class="linenos"> 45</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
-</span><span id="DBShell-46"><a href="#DBShell-46"><span class="linenos"> 46</span></a>
-</span><span id="DBShell-47"><a href="#DBShell-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-48"><a href="#DBShell-48"><span class="linenos"> 48</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
-</span><span id="DBShell-49"><a href="#DBShell-49"><span class="linenos"> 49</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-50"><a href="#DBShell-50"><span class="linenos"> 50</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell-51"><a href="#DBShell-51"><span class="linenos"> 51</span></a>
-</span><span id="DBShell-52"><a href="#DBShell-52"><span class="linenos"> 52</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
-</span><span id="DBShell-53"><a href="#DBShell-53"><span class="linenos"> 53</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
-</span><span id="DBShell-54"><a href="#DBShell-54"><span class="linenos"> 54</span></a>    <span class="p">)</span>
-</span><span id="DBShell-55"><a href="#DBShell-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-56"><a href="#DBShell-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
-</span><span id="DBShell-57"><a href="#DBShell-57"><span class="linenos"> 57</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-58"><a href="#DBShell-58"><span class="linenos"> 58</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="DBShell-59"><a href="#DBShell-59"><span class="linenos"> 59</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-60"><a href="#DBShell-60"><span class="linenos"> 60</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-61"><a href="#DBShell-61"><span class="linenos"> 61</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-62"><a href="#DBShell-62"><span class="linenos"> 62</span></a>
-</span><span id="DBShell-63"><a href="#DBShell-63"><span class="linenos"> 63</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
-</span><span id="DBShell-64"><a href="#DBShell-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-65"><a href="#DBShell-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
-</span><span id="DBShell-66"><a href="#DBShell-66"><span class="linenos"> 66</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-67"><a href="#DBShell-67"><span class="linenos"> 67</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-68"><a href="#DBShell-68"><span class="linenos"> 68</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-69"><a href="#DBShell-69"><span class="linenos"> 69</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="DBShell-70"><a href="#DBShell-70"><span class="linenos"> 70</span></a>                <span class="p">{</span>
-</span><span id="DBShell-71"><a href="#DBShell-71"><span class="linenos"> 71</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell-72"><a href="#DBShell-72"><span class="linenos"> 72</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
-</span><span id="DBShell-73"><a href="#DBShell-73"><span class="linenos"> 73</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
-</span><span id="DBShell-74"><a href="#DBShell-74"><span class="linenos"> 74</span></a>                <span class="p">}</span>
-</span><span id="DBShell-75"><a href="#DBShell-75"><span class="linenos"> 75</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
-</span><span id="DBShell-76"><a href="#DBShell-76"><span class="linenos"> 76</span></a>            <span class="p">]</span>
-</span><span id="DBShell-77"><a href="#DBShell-77"><span class="linenos"> 77</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
-</span><span id="DBShell-78"><a href="#DBShell-78"><span class="linenos"> 78</span></a>
-</span><span id="DBShell-79"><a href="#DBShell-79"><span class="linenos"> 79</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-80"><a href="#DBShell-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-81"><a href="#DBShell-81"><span class="linenos"> 81</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
-</span><span id="DBShell-82"><a href="#DBShell-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
-</span><span id="DBShell-83"><a href="#DBShell-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
-</span><span id="DBShell-84"><a href="#DBShell-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
-</span><span id="DBShell-85"><a href="#DBShell-85"><span class="linenos"> 85</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
-</span><span id="DBShell-86"><a href="#DBShell-86"><span class="linenos"> 86</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell-87"><a href="#DBShell-87"><span class="linenos"> 87</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
-</span><span id="DBShell-88"><a href="#DBShell-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DBShell-89"><a href="#DBShell-89"><span class="linenos"> 89</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DBShell-90"><a href="#DBShell-90"><span class="linenos"> 90</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-91"><a href="#DBShell-91"><span class="linenos"> 91</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-92"><a href="#DBShell-92"><span class="linenos"> 92</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-93"><a href="#DBShell-93"><span class="linenos"> 93</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DBShell-94"><a href="#DBShell-94"><span class="linenos"> 94</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell-95"><a href="#DBShell-95"><span class="linenos"> 95</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell-96"><a href="#DBShell-96"><span class="linenos"> 96</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
-</span><span id="DBShell-97"><a href="#DBShell-97"><span class="linenos"> 97</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
-</span><span id="DBShell-98"><a href="#DBShell-98"><span class="linenos"> 98</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
-</span><span id="DBShell-99"><a href="#DBShell-99"><span class="linenos"> 99</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell-100"><a href="#DBShell-100"><span class="linenos">100</span></a>                <span class="p">)</span>
-</span><span id="DBShell-101"><a href="#DBShell-101"><span class="linenos">101</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DBShell-102"><a href="#DBShell-102"><span class="linenos">102</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
-</span><span id="DBShell-103"><a href="#DBShell-103"><span class="linenos">103</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-104"><a href="#DBShell-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-105"><a href="#DBShell-105"><span class="linenos">105</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-106"><a href="#DBShell-106"><span class="linenos">106</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-107"><a href="#DBShell-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-108"><a href="#DBShell-108"><span class="linenos">108</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="DBShell-109"><a href="#DBShell-109"><span class="linenos">109</span></a>
-</span><span id="DBShell-110"><a href="#DBShell-110"><span class="linenos">110</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="DBShell-111"><a href="#DBShell-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-112"><a href="#DBShell-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="DBShell-113"><a href="#DBShell-113"><span class="linenos">113</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="DBShell-114"><a href="#DBShell-114"><span class="linenos">114</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="DBShell-115"><a href="#DBShell-115"><span class="linenos">115</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-116"><a href="#DBShell-116"><span class="linenos">116</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-117"><a href="#DBShell-117"><span class="linenos">117</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-118"><a href="#DBShell-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-119"><a href="#DBShell-119"><span class="linenos">119</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DBShell-120"><a href="#DBShell-120"><span class="linenos">120</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DBShell-121"><a href="#DBShell-121"><span class="linenos">121</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="DBShell-122"><a href="#DBShell-122"><span class="linenos">122</span></a>                <span class="p">)</span>
-</span><span id="DBShell-123"><a href="#DBShell-123"><span class="linenos">123</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DBShell-124"><a href="#DBShell-124"><span class="linenos">124</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DBShell-125"><a href="#DBShell-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DBShell-126"><a href="#DBShell-126"><span class="linenos">126</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-127"><a href="#DBShell-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="DBShell-128"><a href="#DBShell-128"><span class="linenos">128</span></a>
-</span><span id="DBShell-129"><a href="#DBShell-129"><span class="linenos">129</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-130"><a href="#DBShell-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-131"><a href="#DBShell-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="DBShell-132"><a href="#DBShell-132"><span class="linenos">132</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="DBShell-133"><a href="#DBShell-133"><span class="linenos">133</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="DBShell-134"><a href="#DBShell-134"><span class="linenos">134</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-135"><a href="#DBShell-135"><span class="linenos">135</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell-136"><a href="#DBShell-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-137"><a href="#DBShell-137"><span class="linenos">137</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-138"><a href="#DBShell-138"><span class="linenos">138</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-139"><a href="#DBShell-139"><span class="linenos">139</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-140"><a href="#DBShell-140"><span class="linenos">140</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell-141"><a href="#DBShell-141"><span class="linenos">141</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-142"><a href="#DBShell-142"><span class="linenos">142</span></a>
-</span><span id="DBShell-143"><a href="#DBShell-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-144"><a href="#DBShell-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="DBShell-145"><a href="#DBShell-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-146"><a href="#DBShell-146"><span class="linenos">146</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-147"><a href="#DBShell-147"><span class="linenos">147</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell-148"><a href="#DBShell-148"><span class="linenos">148</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-149"><a href="#DBShell-149"><span class="linenos">149</span></a>            <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="DBShell-150"><a href="#DBShell-150"><span class="linenos">150</span></a>                <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="DBShell-151"><a href="#DBShell-151"><span class="linenos">151</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
-</span><span id="DBShell-152"><a href="#DBShell-152"><span class="linenos">152</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-153"><a href="#DBShell-153"><span class="linenos">153</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-154"><a href="#DBShell-154"><span class="linenos">154</span></a>
-</span><span id="DBShell-155"><a href="#DBShell-155"><span class="linenos">155</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-156"><a href="#DBShell-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-157"><a href="#DBShell-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="DBShell-158"><a href="#DBShell-158"><span class="linenos">158</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="DBShell-159"><a href="#DBShell-159"><span class="linenos">159</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="DBShell-160"><a href="#DBShell-160"><span class="linenos">160</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="DBShell-161"><a href="#DBShell-161"><span class="linenos">161</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-162"><a href="#DBShell-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="DBShell-163"><a href="#DBShell-163"><span class="linenos">163</span></a>
-</span><span id="DBShell-164"><a href="#DBShell-164"><span class="linenos">164</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell-165"><a href="#DBShell-165"><span class="linenos">165</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-166"><a href="#DBShell-166"><span class="linenos">166</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-167"><a href="#DBShell-167"><span class="linenos">167</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-168"><a href="#DBShell-168"><span class="linenos">168</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-169"><a href="#DBShell-169"><span class="linenos">169</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="DBShell-170"><a href="#DBShell-170"><span class="linenos">170</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell-171"><a href="#DBShell-171"><span class="linenos">171</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="DBShell-172"><a href="#DBShell-172"><span class="linenos">172</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="DBShell-173"><a href="#DBShell-173"><span class="linenos">173</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell-174"><a href="#DBShell-174"><span class="linenos">174</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell-175"><a href="#DBShell-175"><span class="linenos">175</span></a>                <span class="p">)</span>
-</span><span id="DBShell-176"><a href="#DBShell-176"><span class="linenos">176</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-177"><a href="#DBShell-177"><span class="linenos">177</span></a>
-</span><span id="DBShell-178"><a href="#DBShell-178"><span class="linenos">178</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-179"><a href="#DBShell-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-180"><a href="#DBShell-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="DBShell-181"><a href="#DBShell-181"><span class="linenos">181</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="DBShell-182"><a href="#DBShell-182"><span class="linenos">182</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="DBShell-183"><a href="#DBShell-183"><span class="linenos">183</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-184"><a href="#DBShell-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="DBShell-185"><a href="#DBShell-185"><span class="linenos">185</span></a>
-</span><span id="DBShell-186"><a href="#DBShell-186"><span class="linenos">186</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell-187"><a href="#DBShell-187"><span class="linenos">187</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-188"><a href="#DBShell-188"><span class="linenos">188</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-189"><a href="#DBShell-189"><span class="linenos">189</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-190"><a href="#DBShell-190"><span class="linenos">190</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-191"><a href="#DBShell-191"><span class="linenos">191</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell-192"><a href="#DBShell-192"><span class="linenos">192</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-193"><a href="#DBShell-193"><span class="linenos">193</span></a>
-</span><span id="DBShell-194"><a href="#DBShell-194"><span class="linenos">194</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="DBShell-195"><a href="#DBShell-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-196"><a href="#DBShell-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="DBShell-197"><a href="#DBShell-197"><span class="linenos">197</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-198"><a href="#DBShell-198"><span class="linenos">198</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-199"><a href="#DBShell-199"><span class="linenos">199</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-200"><a href="#DBShell-200"><span class="linenos">200</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
-</span><span id="DBShell-201"><a href="#DBShell-201"><span class="linenos">201</span></a>
-</span><span id="DBShell-202"><a href="#DBShell-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-203"><a href="#DBShell-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="DBShell-204"><a href="#DBShell-204"><span class="linenos">204</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="DBShell-205"><a href="#DBShell-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-206"><a href="#DBShell-206"><span class="linenos">206</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-207"><a href="#DBShell-207"><span class="linenos">207</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-208"><a href="#DBShell-208"><span class="linenos">208</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-209"><a href="#DBShell-209"><span class="linenos">209</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="DBShell-210"><a href="#DBShell-210"><span class="linenos">210</span></a>
-</span><span id="DBShell-211"><a href="#DBShell-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-212"><a href="#DBShell-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="DBShell-213"><a href="#DBShell-213"><span class="linenos">213</span></a>
-</span><span id="DBShell-214"><a href="#DBShell-214"><span class="linenos">214</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-215"><a href="#DBShell-215"><span class="linenos">215</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-216"><a href="#DBShell-216"><span class="linenos">216</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="DBShell-217"><a href="#DBShell-217"><span class="linenos">217</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell-218"><a href="#DBShell-218"><span class="linenos">218</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-219"><a href="#DBShell-219"><span class="linenos">219</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell-220"><a href="#DBShell-220"><span class="linenos">220</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-221"><a href="#DBShell-221"><span class="linenos">221</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
-</span><span id="DBShell-222"><a href="#DBShell-222"><span class="linenos">222</span></a>
-</span><span id="DBShell-223"><a href="#DBShell-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-224"><a href="#DBShell-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="DBShell-225"><a href="#DBShell-225"><span class="linenos">225</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="DBShell-226"><a href="#DBShell-226"><span class="linenos">226</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell-227"><a href="#DBShell-227"><span class="linenos">227</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell-228"><a href="#DBShell-228"><span class="linenos">228</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-229"><a href="#DBShell-229"><span class="linenos">229</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-230"><a href="#DBShell-230"><span class="linenos">230</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-231"><a href="#DBShell-231"><span class="linenos">231</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-232"><a href="#DBShell-232"><span class="linenos">232</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>
-</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>
-</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>            <span class="p">)</span>
-</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>                    <span class="k">continue</span>
-</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>
-</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>                <span class="p">)</span>
-</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell-9"><a href="#DBShell-9"><span class="linenos">  9</span></a><span class="k">class</span> <span class="nc">DBShell</span><span class="p">(</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShell</span><span class="p">):</span>
+</span><span id="DBShell-10"><a href="#DBShell-10"><span class="linenos"> 10</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting dbshell (enter help or ? for arg info)...&quot;</span>
+</span><span id="DBShell-11"><a href="#DBShell-11"><span class="linenos"> 11</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;based&gt;&quot;</span>
+</span><span id="DBShell-12"><a href="#DBShell-12"><span class="linenos"> 12</span></a>    <span class="n">dbpath</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell-13"><a href="#DBShell-13"><span class="linenos"> 13</span></a>
+</span><span id="DBShell-14"><a href="#DBShell-14"><span class="linenos"> 14</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-15"><a href="#DBShell-15"><span class="linenos"> 15</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
+</span><span id="DBShell-16"><a href="#DBShell-16"><span class="linenos"> 16</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell-17"><a href="#DBShell-17"><span class="linenos"> 17</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-18"><a href="#DBShell-18"><span class="linenos"> 18</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-19"><a href="#DBShell-19"><span class="linenos"> 19</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-20"><a href="#DBShell-20"><span class="linenos"> 20</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell-21"><a href="#DBShell-21"><span class="linenos"> 21</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-22"><a href="#DBShell-22"><span class="linenos"> 22</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-23"><a href="#DBShell-23"><span class="linenos"> 23</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-24"><a href="#DBShell-24"><span class="linenos"> 24</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
+</span><span id="DBShell-25"><a href="#DBShell-25"><span class="linenos"> 25</span></a>
+</span><span id="DBShell-26"><a href="#DBShell-26"><span class="linenos"> 26</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-27"><a href="#DBShell-27"><span class="linenos"> 27</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
+</span><span id="DBShell-28"><a href="#DBShell-28"><span class="linenos"> 28</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell-29"><a href="#DBShell-29"><span class="linenos"> 29</span></a>
+</span><span id="DBShell-30"><a href="#DBShell-30"><span class="linenos"> 30</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
+</span><span id="DBShell-31"><a href="#DBShell-31"><span class="linenos"> 31</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-32"><a href="#DBShell-32"><span class="linenos"> 32</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
+</span><span id="DBShell-33"><a href="#DBShell-33"><span class="linenos"> 33</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-34"><a href="#DBShell-34"><span class="linenos"> 34</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
+</span><span id="DBShell-35"><a href="#DBShell-35"><span class="linenos"> 35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-36"><a href="#DBShell-36"><span class="linenos"> 36</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-37"><a href="#DBShell-37"><span class="linenos"> 37</span></a>
+</span><span id="DBShell-38"><a href="#DBShell-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-39"><a href="#DBShell-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
+</span><span id="DBShell-40"><a href="#DBShell-40"><span class="linenos"> 40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-41"><a href="#DBShell-41"><span class="linenos"> 41</span></a>
+</span><span id="DBShell-42"><a href="#DBShell-42"><span class="linenos"> 42</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
+</span><span id="DBShell-43"><a href="#DBShell-43"><span class="linenos"> 43</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-44"><a href="#DBShell-44"><span class="linenos"> 44</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
+</span><span id="DBShell-45"><a href="#DBShell-45"><span class="linenos"> 45</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-46"><a href="#DBShell-46"><span class="linenos"> 46</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
+</span><span id="DBShell-47"><a href="#DBShell-47"><span class="linenos"> 47</span></a>
+</span><span id="DBShell-48"><a href="#DBShell-48"><span class="linenos"> 48</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-49"><a href="#DBShell-49"><span class="linenos"> 49</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
+</span><span id="DBShell-50"><a href="#DBShell-50"><span class="linenos"> 50</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-51"><a href="#DBShell-51"><span class="linenos"> 51</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell-52"><a href="#DBShell-52"><span class="linenos"> 52</span></a>
+</span><span id="DBShell-53"><a href="#DBShell-53"><span class="linenos"> 53</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
+</span><span id="DBShell-54"><a href="#DBShell-54"><span class="linenos"> 54</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
+</span><span id="DBShell-55"><a href="#DBShell-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
+</span><span id="DBShell-56"><a href="#DBShell-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-57"><a href="#DBShell-57"><span class="linenos"> 57</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
+</span><span id="DBShell-58"><a href="#DBShell-58"><span class="linenos"> 58</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-59"><a href="#DBShell-59"><span class="linenos"> 59</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="DBShell-60"><a href="#DBShell-60"><span class="linenos"> 60</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-61"><a href="#DBShell-61"><span class="linenos"> 61</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-62"><a href="#DBShell-62"><span class="linenos"> 62</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-63"><a href="#DBShell-63"><span class="linenos"> 63</span></a>
+</span><span id="DBShell-64"><a href="#DBShell-64"><span class="linenos"> 64</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
+</span><span id="DBShell-65"><a href="#DBShell-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-66"><a href="#DBShell-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
+</span><span id="DBShell-67"><a href="#DBShell-67"><span class="linenos"> 67</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-68"><a href="#DBShell-68"><span class="linenos"> 68</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-69"><a href="#DBShell-69"><span class="linenos"> 69</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-70"><a href="#DBShell-70"><span class="linenos"> 70</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="DBShell-71"><a href="#DBShell-71"><span class="linenos"> 71</span></a>                <span class="p">{</span>
+</span><span id="DBShell-72"><a href="#DBShell-72"><span class="linenos"> 72</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell-73"><a href="#DBShell-73"><span class="linenos"> 73</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
+</span><span id="DBShell-74"><a href="#DBShell-74"><span class="linenos"> 74</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
+</span><span id="DBShell-75"><a href="#DBShell-75"><span class="linenos"> 75</span></a>                <span class="p">}</span>
+</span><span id="DBShell-76"><a href="#DBShell-76"><span class="linenos"> 76</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
+</span><span id="DBShell-77"><a href="#DBShell-77"><span class="linenos"> 77</span></a>            <span class="p">]</span>
+</span><span id="DBShell-78"><a href="#DBShell-78"><span class="linenos"> 78</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
+</span><span id="DBShell-79"><a href="#DBShell-79"><span class="linenos"> 79</span></a>
+</span><span id="DBShell-80"><a href="#DBShell-80"><span class="linenos"> 80</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-81"><a href="#DBShell-81"><span class="linenos"> 81</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-82"><a href="#DBShell-82"><span class="linenos"> 82</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
+</span><span id="DBShell-83"><a href="#DBShell-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
+</span><span id="DBShell-84"><a href="#DBShell-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
+</span><span id="DBShell-85"><a href="#DBShell-85"><span class="linenos"> 85</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
+</span><span id="DBShell-86"><a href="#DBShell-86"><span class="linenos"> 86</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
+</span><span id="DBShell-87"><a href="#DBShell-87"><span class="linenos"> 87</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell-88"><a href="#DBShell-88"><span class="linenos"> 88</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
+</span><span id="DBShell-89"><a href="#DBShell-89"><span class="linenos"> 89</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DBShell-90"><a href="#DBShell-90"><span class="linenos"> 90</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DBShell-91"><a href="#DBShell-91"><span class="linenos"> 91</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-92"><a href="#DBShell-92"><span class="linenos"> 92</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-93"><a href="#DBShell-93"><span class="linenos"> 93</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-94"><a href="#DBShell-94"><span class="linenos"> 94</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DBShell-95"><a href="#DBShell-95"><span class="linenos"> 95</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell-96"><a href="#DBShell-96"><span class="linenos"> 96</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell-97"><a href="#DBShell-97"><span class="linenos"> 97</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
+</span><span id="DBShell-98"><a href="#DBShell-98"><span class="linenos"> 98</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
+</span><span id="DBShell-99"><a href="#DBShell-99"><span class="linenos"> 99</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
+</span><span id="DBShell-100"><a href="#DBShell-100"><span class="linenos">100</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell-101"><a href="#DBShell-101"><span class="linenos">101</span></a>                <span class="p">)</span>
+</span><span id="DBShell-102"><a href="#DBShell-102"><span class="linenos">102</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DBShell-103"><a href="#DBShell-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="DBShell-104"><a href="#DBShell-104"><span class="linenos">104</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-105"><a href="#DBShell-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell-106"><a href="#DBShell-106"><span class="linenos">106</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-107"><a href="#DBShell-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-108"><a href="#DBShell-108"><span class="linenos">108</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-109"><a href="#DBShell-109"><span class="linenos">109</span></a>                <span class="nb">print</span><span class="p">()</span>
+</span><span id="DBShell-110"><a href="#DBShell-110"><span class="linenos">110</span></a>
+</span><span id="DBShell-111"><a href="#DBShell-111"><span class="linenos">111</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="DBShell-112"><a href="#DBShell-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-113"><a href="#DBShell-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="DBShell-114"><a href="#DBShell-114"><span class="linenos">114</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="DBShell-115"><a href="#DBShell-115"><span class="linenos">115</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="DBShell-116"><a href="#DBShell-116"><span class="linenos">116</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-117"><a href="#DBShell-117"><span class="linenos">117</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-118"><a href="#DBShell-118"><span class="linenos">118</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-119"><a href="#DBShell-119"><span class="linenos">119</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-120"><a href="#DBShell-120"><span class="linenos">120</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DBShell-121"><a href="#DBShell-121"><span class="linenos">121</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DBShell-122"><a href="#DBShell-122"><span class="linenos">122</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="DBShell-123"><a href="#DBShell-123"><span class="linenos">123</span></a>                <span class="p">)</span>
+</span><span id="DBShell-124"><a href="#DBShell-124"><span class="linenos">124</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DBShell-125"><a href="#DBShell-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DBShell-126"><a href="#DBShell-126"><span class="linenos">126</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DBShell-127"><a href="#DBShell-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-128"><a href="#DBShell-128"><span class="linenos">128</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell-129"><a href="#DBShell-129"><span class="linenos">129</span></a>
+</span><span id="DBShell-130"><a href="#DBShell-130"><span class="linenos">130</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-131"><a href="#DBShell-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-132"><a href="#DBShell-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="DBShell-133"><a href="#DBShell-133"><span class="linenos">133</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="DBShell-134"><a href="#DBShell-134"><span class="linenos">134</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="DBShell-135"><a href="#DBShell-135"><span class="linenos">135</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-136"><a href="#DBShell-136"><span class="linenos">136</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell-137"><a href="#DBShell-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-138"><a href="#DBShell-138"><span class="linenos">138</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-139"><a href="#DBShell-139"><span class="linenos">139</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-140"><a href="#DBShell-140"><span class="linenos">140</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-141"><a href="#DBShell-141"><span class="linenos">141</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell-142"><a href="#DBShell-142"><span class="linenos">142</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-143"><a href="#DBShell-143"><span class="linenos">143</span></a>
+</span><span id="DBShell-144"><a href="#DBShell-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-145"><a href="#DBShell-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="DBShell-146"><a href="#DBShell-146"><span class="linenos">146</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-147"><a href="#DBShell-147"><span class="linenos">147</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-148"><a href="#DBShell-148"><span class="linenos">148</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell-149"><a href="#DBShell-149"><span class="linenos">149</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-150"><a href="#DBShell-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-151"><a href="#DBShell-151"><span class="linenos">151</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell-152"><a href="#DBShell-152"><span class="linenos">152</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-153"><a href="#DBShell-153"><span class="linenos">153</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell-154"><a href="#DBShell-154"><span class="linenos">154</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="DBShell-155"><a href="#DBShell-155"><span class="linenos">155</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-156"><a href="#DBShell-156"><span class="linenos">156</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-157"><a href="#DBShell-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
+</span><span id="DBShell-158"><a href="#DBShell-158"><span class="linenos">158</span></a>
+</span><span id="DBShell-159"><a href="#DBShell-159"><span class="linenos">159</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-160"><a href="#DBShell-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-161"><a href="#DBShell-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="DBShell-162"><a href="#DBShell-162"><span class="linenos">162</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="DBShell-163"><a href="#DBShell-163"><span class="linenos">163</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="DBShell-164"><a href="#DBShell-164"><span class="linenos">164</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="DBShell-165"><a href="#DBShell-165"><span class="linenos">165</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-166"><a href="#DBShell-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="DBShell-167"><a href="#DBShell-167"><span class="linenos">167</span></a>
+</span><span id="DBShell-168"><a href="#DBShell-168"><span class="linenos">168</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell-169"><a href="#DBShell-169"><span class="linenos">169</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-170"><a href="#DBShell-170"><span class="linenos">170</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-171"><a href="#DBShell-171"><span class="linenos">171</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-172"><a href="#DBShell-172"><span class="linenos">172</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-173"><a href="#DBShell-173"><span class="linenos">173</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="DBShell-174"><a href="#DBShell-174"><span class="linenos">174</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell-175"><a href="#DBShell-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="DBShell-176"><a href="#DBShell-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="DBShell-177"><a href="#DBShell-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell-178"><a href="#DBShell-178"><span class="linenos">178</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell-179"><a href="#DBShell-179"><span class="linenos">179</span></a>                <span class="p">)</span>
+</span><span id="DBShell-180"><a href="#DBShell-180"><span class="linenos">180</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-181"><a href="#DBShell-181"><span class="linenos">181</span></a>
+</span><span id="DBShell-182"><a href="#DBShell-182"><span class="linenos">182</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-183"><a href="#DBShell-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-184"><a href="#DBShell-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="DBShell-185"><a href="#DBShell-185"><span class="linenos">185</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="DBShell-186"><a href="#DBShell-186"><span class="linenos">186</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="DBShell-187"><a href="#DBShell-187"><span class="linenos">187</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-188"><a href="#DBShell-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="DBShell-189"><a href="#DBShell-189"><span class="linenos">189</span></a>
+</span><span id="DBShell-190"><a href="#DBShell-190"><span class="linenos">190</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell-191"><a href="#DBShell-191"><span class="linenos">191</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-192"><a href="#DBShell-192"><span class="linenos">192</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-193"><a href="#DBShell-193"><span class="linenos">193</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-194"><a href="#DBShell-194"><span class="linenos">194</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-195"><a href="#DBShell-195"><span class="linenos">195</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell-196"><a href="#DBShell-196"><span class="linenos">196</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-197"><a href="#DBShell-197"><span class="linenos">197</span></a>
+</span><span id="DBShell-198"><a href="#DBShell-198"><span class="linenos">198</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="DBShell-199"><a href="#DBShell-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-200"><a href="#DBShell-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="DBShell-201"><a href="#DBShell-201"><span class="linenos">201</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-202"><a href="#DBShell-202"><span class="linenos">202</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-203"><a href="#DBShell-203"><span class="linenos">203</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-204"><a href="#DBShell-204"><span class="linenos">204</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+</span><span id="DBShell-205"><a href="#DBShell-205"><span class="linenos">205</span></a>
+</span><span id="DBShell-206"><a href="#DBShell-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-207"><a href="#DBShell-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="DBShell-208"><a href="#DBShell-208"><span class="linenos">208</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="DBShell-209"><a href="#DBShell-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-210"><a href="#DBShell-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-211"><a href="#DBShell-211"><span class="linenos">211</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-212"><a href="#DBShell-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-213"><a href="#DBShell-213"><span class="linenos">213</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="DBShell-214"><a href="#DBShell-214"><span class="linenos">214</span></a>
+</span><span id="DBShell-215"><a href="#DBShell-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-216"><a href="#DBShell-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="DBShell-217"><a href="#DBShell-217"><span class="linenos">217</span></a>
+</span><span id="DBShell-218"><a href="#DBShell-218"><span class="linenos">218</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-219"><a href="#DBShell-219"><span class="linenos">219</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-220"><a href="#DBShell-220"><span class="linenos">220</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="DBShell-221"><a href="#DBShell-221"><span class="linenos">221</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell-222"><a href="#DBShell-222"><span class="linenos">222</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-223"><a href="#DBShell-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell-224"><a href="#DBShell-224"><span class="linenos">224</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-225"><a href="#DBShell-225"><span class="linenos">225</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+</span><span id="DBShell-226"><a href="#DBShell-226"><span class="linenos">226</span></a>
+</span><span id="DBShell-227"><a href="#DBShell-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-228"><a href="#DBShell-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="DBShell-229"><a href="#DBShell-229"><span class="linenos">229</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="DBShell-230"><a href="#DBShell-230"><span class="linenos">230</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="DBShell-231"><a href="#DBShell-231"><span class="linenos">231</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="DBShell-232"><a href="#DBShell-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>
+</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>
+</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>            <span class="p">)</span>
+</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>                    <span class="k">continue</span>
+</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>
+</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                <span class="p">)</span>
+</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell-303"><a href="#DBShell-303"><span class="linenos">303</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-304"><a href="#DBShell-304"><span class="linenos">304</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-305"><a href="#DBShell-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell-306"><a href="#DBShell-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -749,25 +756,25 @@
         <span class="def">def</span>
         <span class="name">do_use_db</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_use_db-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_use_db"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_use_db-13"><a href="#DBShell.do_use_db-13"><span class="linenos">13</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_use_db-14"><a href="#DBShell.do_use_db-14"><span class="linenos">14</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_use_db-15"><a href="#DBShell.do_use_db-15"><span class="linenos">15</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell.do_use_db-16"><a href="#DBShell.do_use_db-16"><span class="linenos">16</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_use_db-17"><a href="#DBShell.do_use_db-17"><span class="linenos">17</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_use_db-18"><a href="#DBShell.do_use_db-18"><span class="linenos">18</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_use_db-19"><a href="#DBShell.do_use_db-19"><span class="linenos">19</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell.do_use_db-20"><a href="#DBShell.do_use_db-20"><span class="linenos">20</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_use_db-21"><a href="#DBShell.do_use_db-21"><span class="linenos">21</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_use_db-22"><a href="#DBShell.do_use_db-22"><span class="linenos">22</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_use_db-23"><a href="#DBShell.do_use_db-23"><span class="linenos">23</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_use_db-14"><a href="#DBShell.do_use_db-14"><span class="linenos">14</span></a>    <span class="k">def</span> <span class="nf">do_use_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_use_db-15"><a href="#DBShell.do_use_db-15"><span class="linenos">15</span></a>        <span class="sd">&quot;&quot;&quot;Set which database file to use.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_use_db-16"><a href="#DBShell.do_use_db-16"><span class="linenos">16</span></a>        <span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell.do_use_db-17"><a href="#DBShell.do_use_db-17"><span class="linenos">17</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.do_use_db-18"><a href="#DBShell.do_use_db-18"><span class="linenos">18</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_use_db-19"><a href="#DBShell.do_use_db-19"><span class="linenos">19</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_use_db-20"><a href="#DBShell.do_use_db-20"><span class="linenos">20</span></a>        <span class="k">elif</span> <span class="ow">not</span> <span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell.do_use_db-21"><a href="#DBShell.do_use_db-21"><span class="linenos">21</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_use_db-22"><a href="#DBShell.do_use_db-22"><span class="linenos">22</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Still using </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_use_db-23"><a href="#DBShell.do_use_db-23"><span class="linenos">23</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_use_db-24"><a href="#DBShell.do_use_db-24"><span class="linenos">24</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbpath</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Set which database file to use.</p>
 </div>
 
 
@@ -779,17 +786,17 @@
         <span class="def">def</span>
         <span class="name">do_dbpath</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_dbpath-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_dbpath"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_dbpath-25"><a href="#DBShell.do_dbpath-25"><span class="linenos">25</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_dbpath-26"><a href="#DBShell.do_dbpath-26"><span class="linenos">26</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_dbpath-27"><a href="#DBShell.do_dbpath-27"><span class="linenos">27</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_dbpath-26"><a href="#DBShell.do_dbpath-26"><span class="linenos">26</span></a>    <span class="k">def</span> <span class="nf">do_dbpath</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_dbpath-27"><a href="#DBShell.do_dbpath-27"><span class="linenos">27</span></a>        <span class="sd">&quot;&quot;&quot;Print the .db file in use.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_dbpath-28"><a href="#DBShell.do_dbpath-28"><span class="linenos">28</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print the .db file in use.</p>
 </div>
 
 
@@ -802,21 +809,21 @@
         <span class="def">def</span>
         <span class="name">do_backup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_backup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_backup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_backup-29"><a href="#DBShell.do_backup-29"><span class="linenos">29</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_backup-30"><a href="#DBShell.do_backup-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_backup-31"><a href="#DBShell.do_backup-31"><span class="linenos">31</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_backup-32"><a href="#DBShell.do_backup-32"><span class="linenos">32</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_backup-33"><a href="#DBShell.do_backup-33"><span class="linenos">33</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
-</span><span id="DBShell.do_backup-34"><a href="#DBShell.do_backup-34"><span class="linenos">34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_backup-35"><a href="#DBShell.do_backup-35"><span class="linenos">35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_backup-30"><a href="#DBShell.do_backup-30"><span class="linenos">30</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_backup_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_backup-31"><a href="#DBShell.do_backup-31"><span class="linenos">31</span></a>    <span class="k">def</span> <span class="nf">do_backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_backup-32"><a href="#DBShell.do_backup-32"><span class="linenos">32</span></a>        <span class="sd">&quot;&quot;&quot;Create a backup of the current db file.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_backup-33"><a href="#DBShell.do_backup-33"><span class="linenos">33</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_backup-34"><a href="#DBShell.do_backup-34"><span class="linenos">34</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
+</span><span id="DBShell.do_backup-35"><a href="#DBShell.do_backup-35"><span class="linenos">35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_backup-36"><a href="#DBShell.do_backup-36"><span class="linenos">36</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a backup of the current db file.</p>
 </div>
 
 
@@ -828,17 +835,17 @@
         <span class="def">def</span>
         <span class="name">do_size</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_size-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_size"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_size-37"><a href="#DBShell.do_size-37"><span class="linenos">37</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_size-38"><a href="#DBShell.do_size-38"><span class="linenos">38</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_size-39"><a href="#DBShell.do_size-39"><span class="linenos">39</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_size-38"><a href="#DBShell.do_size-38"><span class="linenos">38</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_size-39"><a href="#DBShell.do_size-39"><span class="linenos">39</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_size-40"><a href="#DBShell.do_size-40"><span class="linenos">40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Display the size of the the current db file.</p>
 </div>
 
 
@@ -851,19 +858,19 @@
         <span class="def">def</span>
         <span class="name">do_add_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_add_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_add_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_table-41"><a href="#DBShell.do_add_table-41"><span class="linenos">41</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_add_table-42"><a href="#DBShell.do_add_table-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_add_table-43"><a href="#DBShell.do_add_table-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_add_table-44"><a href="#DBShell.do_add_table-44"><span class="linenos">44</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_add_table-45"><a href="#DBShell.do_add_table-45"><span class="linenos">45</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_table-42"><a href="#DBShell.do_add_table-42"><span class="linenos">42</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_add_table-43"><a href="#DBShell.do_add_table-43"><span class="linenos">43</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_add_table-44"><a href="#DBShell.do_add_table-44"><span class="linenos">44</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_add_table-45"><a href="#DBShell.do_add_table-45"><span class="linenos">45</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_add_table-46"><a href="#DBShell.do_add_table-46"><span class="linenos">46</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new table to the database.</p>
 </div>
 
 
@@ -875,18 +882,18 @@
         <span class="def">def</span>
         <span class="name">do_drop_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_drop_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_drop_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_drop_table-47"><a href="#DBShell.do_drop_table-47"><span class="linenos">47</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_drop_table-48"><a href="#DBShell.do_drop_table-48"><span class="linenos">48</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_drop_table-49"><a href="#DBShell.do_drop_table-49"><span class="linenos">49</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_drop_table-50"><a href="#DBShell.do_drop_table-50"><span class="linenos">50</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_drop_table-48"><a href="#DBShell.do_drop_table-48"><span class="linenos">48</span></a>    <span class="k">def</span> <span class="nf">do_drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_drop_table-49"><a href="#DBShell.do_drop_table-49"><span class="linenos">49</span></a>        <span class="sd">&quot;&quot;&quot;Drop the specified table.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_drop_table-50"><a href="#DBShell.do_drop_table-50"><span class="linenos">50</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_drop_table-51"><a href="#DBShell.do_drop_table-51"><span class="linenos">51</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">drop_table</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Drop the specified table.</p>
 </div>
 
 
@@ -899,24 +906,24 @@
         <span class="def">def</span>
         <span class="name">do_add_row</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_add_row-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_add_row"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_row-52"><a href="#DBShell.do_add_row-52"><span class="linenos">52</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
-</span><span id="DBShell.do_add_row-53"><a href="#DBShell.do_add_row-53"><span class="linenos">53</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
-</span><span id="DBShell.do_add_row-54"><a href="#DBShell.do_add_row-54"><span class="linenos">54</span></a>    <span class="p">)</span>
-</span><span id="DBShell.do_add_row-55"><a href="#DBShell.do_add_row-55"><span class="linenos">55</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_add_row-56"><a href="#DBShell.do_add_row-56"><span class="linenos">56</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_add_row-57"><a href="#DBShell.do_add_row-57"><span class="linenos">57</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_add_row-58"><a href="#DBShell.do_add_row-58"><span class="linenos">58</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="DBShell.do_add_row-59"><a href="#DBShell.do_add_row-59"><span class="linenos">59</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_add_row-60"><a href="#DBShell.do_add_row-60"><span class="linenos">60</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_add_row-61"><a href="#DBShell.do_add_row-61"><span class="linenos">61</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_row-53"><a href="#DBShell.do_add_row-53"><span class="linenos">53</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span>
+</span><span id="DBShell.do_add_row-54"><a href="#DBShell.do_add_row-54"><span class="linenos">54</span></a>        <span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_row_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">verify_matching_length</span><span class="p">]</span>
+</span><span id="DBShell.do_add_row-55"><a href="#DBShell.do_add_row-55"><span class="linenos">55</span></a>    <span class="p">)</span>
+</span><span id="DBShell.do_add_row-56"><a href="#DBShell.do_add_row-56"><span class="linenos">56</span></a>    <span class="k">def</span> <span class="nf">do_add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_add_row-57"><a href="#DBShell.do_add_row-57"><span class="linenos">57</span></a>        <span class="sd">&quot;&quot;&quot;Add a row to a table.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_add_row-58"><a href="#DBShell.do_add_row-58"><span class="linenos">58</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_add_row-59"><a href="#DBShell.do_add_row-59"><span class="linenos">59</span></a>            <span class="k">if</span> <span class="n">db</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">values</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="DBShell.do_add_row-60"><a href="#DBShell.do_add_row-60"><span class="linenos">60</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Added row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table successfully.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_add_row-61"><a href="#DBShell.do_add_row-61"><span class="linenos">61</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_add_row-62"><a href="#DBShell.do_add_row-62"><span class="linenos">62</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to add row to </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a row to a table.</p>
 </div>
 
 
@@ -929,29 +936,29 @@
         <span class="def">def</span>
         <span class="name">do_info</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_info-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_info"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_info-63"><a href="#DBShell.do_info-63"><span class="linenos">63</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_info-64"><a href="#DBShell.do_info-64"><span class="linenos">64</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_info-65"><a href="#DBShell.do_info-65"><span class="linenos">65</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_info-66"><a href="#DBShell.do_info-66"><span class="linenos">66</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_info-67"><a href="#DBShell.do_info-67"><span class="linenos">67</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_info-68"><a href="#DBShell.do_info-68"><span class="linenos">68</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_info-69"><a href="#DBShell.do_info-69"><span class="linenos">69</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="DBShell.do_info-70"><a href="#DBShell.do_info-70"><span class="linenos">70</span></a>                <span class="p">{</span>
-</span><span id="DBShell.do_info-71"><a href="#DBShell.do_info-71"><span class="linenos">71</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell.do_info-72"><a href="#DBShell.do_info-72"><span class="linenos">72</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
-</span><span id="DBShell.do_info-73"><a href="#DBShell.do_info-73"><span class="linenos">73</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
-</span><span id="DBShell.do_info-74"><a href="#DBShell.do_info-74"><span class="linenos">74</span></a>                <span class="p">}</span>
-</span><span id="DBShell.do_info-75"><a href="#DBShell.do_info-75"><span class="linenos">75</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
-</span><span id="DBShell.do_info-76"><a href="#DBShell.do_info-76"><span class="linenos">76</span></a>            <span class="p">]</span>
-</span><span id="DBShell.do_info-77"><a href="#DBShell.do_info-77"><span class="linenos">77</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_info-64"><a href="#DBShell.do_info-64"><span class="linenos">64</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_info_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_info-65"><a href="#DBShell.do_info-65"><span class="linenos">65</span></a>    <span class="k">def</span> <span class="nf">do_info</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_info-66"><a href="#DBShell.do_info-66"><span class="linenos">66</span></a>        <span class="sd">&quot;&quot;&quot;Print out the names of the database tables, their columns, and, optionally, the number of rows.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_info-67"><a href="#DBShell.do_info-67"><span class="linenos">67</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Getting database info...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_info-68"><a href="#DBShell.do_info-68"><span class="linenos">68</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_info-69"><a href="#DBShell.do_info-69"><span class="linenos">69</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_info-70"><a href="#DBShell.do_info-70"><span class="linenos">70</span></a>            <span class="n">info</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="DBShell.do_info-71"><a href="#DBShell.do_info-71"><span class="linenos">71</span></a>                <span class="p">{</span>
+</span><span id="DBShell.do_info-72"><a href="#DBShell.do_info-72"><span class="linenos">72</span></a>                    <span class="s2">&quot;Table Name&quot;</span><span class="p">:</span> <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell.do_info-73"><a href="#DBShell.do_info-73"><span class="linenos">73</span></a>                    <span class="s2">&quot;Columns&quot;</span><span class="p">:</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)),</span>
+</span><span id="DBShell.do_info-74"><a href="#DBShell.do_info-74"><span class="linenos">74</span></a>                    <span class="s2">&quot;Number of Rows&quot;</span><span class="p">:</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">rowcount</span> <span class="k">else</span> <span class="s2">&quot;n/a&quot;</span><span class="p">,</span>
+</span><span id="DBShell.do_info-75"><a href="#DBShell.do_info-75"><span class="linenos">75</span></a>                <span class="p">}</span>
+</span><span id="DBShell.do_info-76"><a href="#DBShell.do_info-76"><span class="linenos">76</span></a>                <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span>
+</span><span id="DBShell.do_info-77"><a href="#DBShell.do_info-77"><span class="linenos">77</span></a>            <span class="p">]</span>
+</span><span id="DBShell.do_info-78"><a href="#DBShell.do_info-78"><span class="linenos">78</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">info</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print out the names of the database tables, their columns, and, optionally, the number of rows.</p>
 </div>
 
 
@@ -964,44 +971,44 @@
         <span class="def">def</span>
         <span class="name">do_show</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_show-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_show"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_show-79"><a href="#DBShell.do_show-79"><span class="linenos"> 79</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_show-80"><a href="#DBShell.do_show-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_show-81"><a href="#DBShell.do_show-81"><span class="linenos"> 81</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
-</span><span id="DBShell.do_show-82"><a href="#DBShell.do_show-82"><span class="linenos"> 82</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
-</span><span id="DBShell.do_show-83"><a href="#DBShell.do_show-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
-</span><span id="DBShell.do_show-84"><a href="#DBShell.do_show-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
-</span><span id="DBShell.do_show-85"><a href="#DBShell.do_show-85"><span class="linenos"> 85</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
-</span><span id="DBShell.do_show-86"><a href="#DBShell.do_show-86"><span class="linenos"> 86</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_show-87"><a href="#DBShell.do_show-87"><span class="linenos"> 87</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_show-88"><a href="#DBShell.do_show-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DBShell.do_show-89"><a href="#DBShell.do_show-89"><span class="linenos"> 89</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DBShell.do_show-90"><a href="#DBShell.do_show-90"><span class="linenos"> 90</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_show-91"><a href="#DBShell.do_show-91"><span class="linenos"> 91</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_show-92"><a href="#DBShell.do_show-92"><span class="linenos"> 92</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_show-93"><a href="#DBShell.do_show-93"><span class="linenos"> 93</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DBShell.do_show-94"><a href="#DBShell.do_show-94"><span class="linenos"> 94</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell.do_show-95"><a href="#DBShell.do_show-95"><span class="linenos"> 95</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell.do_show-96"><a href="#DBShell.do_show-96"><span class="linenos"> 96</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
-</span><span id="DBShell.do_show-97"><a href="#DBShell.do_show-97"><span class="linenos"> 97</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
-</span><span id="DBShell.do_show-98"><a href="#DBShell.do_show-98"><span class="linenos"> 98</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
-</span><span id="DBShell.do_show-99"><a href="#DBShell.do_show-99"><span class="linenos"> 99</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell.do_show-100"><a href="#DBShell.do_show-100"><span class="linenos">100</span></a>                <span class="p">)</span>
-</span><span id="DBShell.do_show-101"><a href="#DBShell.do_show-101"><span class="linenos">101</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DBShell.do_show-102"><a href="#DBShell.do_show-102"><span class="linenos">102</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_show-103"><a href="#DBShell.do_show-103"><span class="linenos">103</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell.do_show-104"><a href="#DBShell.do_show-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell.do_show-105"><a href="#DBShell.do_show-105"><span class="linenos">105</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell.do_show-106"><a href="#DBShell.do_show-106"><span class="linenos">106</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_show-107"><a href="#DBShell.do_show-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_show-108"><a href="#DBShell.do_show-108"><span class="linenos">108</span></a>                <span class="nb">print</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_show-80"><a href="#DBShell.do_show-80"><span class="linenos"> 80</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_show-81"><a href="#DBShell.do_show-81"><span class="linenos"> 81</span></a>    <span class="k">def</span> <span class="nf">do_show</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_show-82"><a href="#DBShell.do_show-82"><span class="linenos"> 82</span></a>        <span class="sd">&quot;&quot;&quot;Find and print rows from the database.</span>
+</span><span id="DBShell.do_show-83"><a href="#DBShell.do_show-83"><span class="linenos"> 83</span></a><span class="sd">        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.</span>
+</span><span id="DBShell.do_show-84"><a href="#DBShell.do_show-84"><span class="linenos"> 84</span></a><span class="sd">        Use the -c/--columns flag to limit what columns are printed.</span>
+</span><span id="DBShell.do_show-85"><a href="#DBShell.do_show-85"><span class="linenos"> 85</span></a><span class="sd">        Use the -o/--order_by flag to order the results.</span>
+</span><span id="DBShell.do_show-86"><a href="#DBShell.do_show-86"><span class="linenos"> 86</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs</span>
+</span><span id="DBShell.do_show-87"><a href="#DBShell.do_show-87"><span class="linenos"> 87</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_show-88"><a href="#DBShell.do_show-88"><span class="linenos"> 88</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Finding records... &quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-89"><a href="#DBShell.do_show-89"><span class="linenos"> 89</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DBShell.do_show-90"><a href="#DBShell.do_show-90"><span class="linenos"> 90</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DBShell.do_show-91"><a href="#DBShell.do_show-91"><span class="linenos"> 91</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_show-92"><a href="#DBShell.do_show-92"><span class="linenos"> 92</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_show-93"><a href="#DBShell.do_show-93"><span class="linenos"> 93</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_show-94"><a href="#DBShell.do_show-94"><span class="linenos"> 94</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DBShell.do_show-95"><a href="#DBShell.do_show-95"><span class="linenos"> 95</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell.do_show-96"><a href="#DBShell.do_show-96"><span class="linenos"> 96</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell.do_show-97"><a href="#DBShell.do_show-97"><span class="linenos"> 97</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
+</span><span id="DBShell.do_show-98"><a href="#DBShell.do_show-98"><span class="linenos"> 98</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
+</span><span id="DBShell.do_show-99"><a href="#DBShell.do_show-99"><span class="linenos"> 99</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
+</span><span id="DBShell.do_show-100"><a href="#DBShell.do_show-100"><span class="linenos">100</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell.do_show-101"><a href="#DBShell.do_show-101"><span class="linenos">101</span></a>                <span class="p">)</span>
+</span><span id="DBShell.do_show-102"><a href="#DBShell.do_show-102"><span class="linenos">102</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DBShell.do_show-103"><a href="#DBShell.do_show-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-104"><a href="#DBShell.do_show-104"><span class="linenos">104</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_show-105"><a href="#DBShell.do_show-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell.do_show-106"><a href="#DBShell.do_show-106"><span class="linenos">106</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_show-107"><a href="#DBShell.do_show-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-108"><a href="#DBShell.do_show-108"><span class="linenos">108</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-109"><a href="#DBShell.do_show-109"><span class="linenos">109</span></a>                <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Find and print rows from the database.
 Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.
 Use the -c/--columns flag to limit what columns are printed.
 Use the -o/--order_by flag to order the results.
@@ -1019,32 +1026,32 @@
         <span class="def">def</span>
         <span class="name">do_search</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_search-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_search"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_search-110"><a href="#DBShell.do_search-110"><span class="linenos">110</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_search-111"><a href="#DBShell.do_search-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_search-112"><a href="#DBShell.do_search-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="DBShell.do_search-113"><a href="#DBShell.do_search-113"><span class="linenos">113</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="DBShell.do_search-114"><a href="#DBShell.do_search-114"><span class="linenos">114</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_search-115"><a href="#DBShell.do_search-115"><span class="linenos">115</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_search-116"><a href="#DBShell.do_search-116"><span class="linenos">116</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_search-117"><a href="#DBShell.do_search-117"><span class="linenos">117</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_search-118"><a href="#DBShell.do_search-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_search-119"><a href="#DBShell.do_search-119"><span class="linenos">119</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DBShell.do_search-120"><a href="#DBShell.do_search-120"><span class="linenos">120</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DBShell.do_search-121"><a href="#DBShell.do_search-121"><span class="linenos">121</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="DBShell.do_search-122"><a href="#DBShell.do_search-122"><span class="linenos">122</span></a>                <span class="p">)</span>
-</span><span id="DBShell.do_search-123"><a href="#DBShell.do_search-123"><span class="linenos">123</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DBShell.do_search-124"><a href="#DBShell.do_search-124"><span class="linenos">124</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DBShell.do_search-125"><a href="#DBShell.do_search-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DBShell.do_search-126"><a href="#DBShell.do_search-126"><span class="linenos">126</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_search-127"><a href="#DBShell.do_search-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_search-111"><a href="#DBShell.do_search-111"><span class="linenos">111</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_search-112"><a href="#DBShell.do_search-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_search-113"><a href="#DBShell.do_search-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="DBShell.do_search-114"><a href="#DBShell.do_search-114"><span class="linenos">114</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="DBShell.do_search-115"><a href="#DBShell.do_search-115"><span class="linenos">115</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_search-116"><a href="#DBShell.do_search-116"><span class="linenos">116</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_search-117"><a href="#DBShell.do_search-117"><span class="linenos">117</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_search-118"><a href="#DBShell.do_search-118"><span class="linenos">118</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_search-119"><a href="#DBShell.do_search-119"><span class="linenos">119</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_search-120"><a href="#DBShell.do_search-120"><span class="linenos">120</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DBShell.do_search-121"><a href="#DBShell.do_search-121"><span class="linenos">121</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DBShell.do_search-122"><a href="#DBShell.do_search-122"><span class="linenos">122</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="DBShell.do_search-123"><a href="#DBShell.do_search-123"><span class="linenos">123</span></a>                <span class="p">)</span>
+</span><span id="DBShell.do_search-124"><a href="#DBShell.do_search-124"><span class="linenos">124</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DBShell.do_search-125"><a href="#DBShell.do_search-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DBShell.do_search-126"><a href="#DBShell.do_search-126"><span class="linenos">126</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DBShell.do_search-127"><a href="#DBShell.do_search-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_search-128"><a href="#DBShell.do_search-128"><span class="linenos">128</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Search and return any rows containg the searched substring in any of its columns.
 Use the -t/--tables flag to limit the search to a specific table(s).
 Use the -c/--columns flag to limit the search to a specific column(s).</p>
 </div>
@@ -1059,27 +1066,27 @@
         <span class="def">def</span>
         <span class="name">do_count</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_count-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_count"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_count-129"><a href="#DBShell.do_count-129"><span class="linenos">129</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_count-130"><a href="#DBShell.do_count-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_count-131"><a href="#DBShell.do_count-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="DBShell.do_count-132"><a href="#DBShell.do_count-132"><span class="linenos">132</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="DBShell.do_count-133"><a href="#DBShell.do_count-133"><span class="linenos">133</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="DBShell.do_count-134"><a href="#DBShell.do_count-134"><span class="linenos">134</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_count-135"><a href="#DBShell.do_count-135"><span class="linenos">135</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_count-136"><a href="#DBShell.do_count-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_count-137"><a href="#DBShell.do_count-137"><span class="linenos">137</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_count-138"><a href="#DBShell.do_count-138"><span class="linenos">138</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_count-139"><a href="#DBShell.do_count-139"><span class="linenos">139</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_count-140"><a href="#DBShell.do_count-140"><span class="linenos">140</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell.do_count-141"><a href="#DBShell.do_count-141"><span class="linenos">141</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_count-130"><a href="#DBShell.do_count-130"><span class="linenos">130</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_count-131"><a href="#DBShell.do_count-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_count-132"><a href="#DBShell.do_count-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="DBShell.do_count-133"><a href="#DBShell.do_count-133"><span class="linenos">133</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="DBShell.do_count-134"><a href="#DBShell.do_count-134"><span class="linenos">134</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="DBShell.do_count-135"><a href="#DBShell.do_count-135"><span class="linenos">135</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_count-136"><a href="#DBShell.do_count-136"><span class="linenos">136</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_count-137"><a href="#DBShell.do_count-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_count-138"><a href="#DBShell.do_count-138"><span class="linenos">138</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_count-139"><a href="#DBShell.do_count-139"><span class="linenos">139</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_count-140"><a href="#DBShell.do_count-140"><span class="linenos">140</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_count-141"><a href="#DBShell.do_count-141"><span class="linenos">141</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell.do_count-142"><a href="#DBShell.do_count-142"><span class="linenos">142</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print the number of rows in the database.
 Use the -t/--tables flag to limit results to a specific table(s).
 Use the -m/--match_pairs flag to limit the results to rows matching these criteria.
 Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.
@@ -1095,25 +1102,28 @@
         <span class="def">def</span>
         <span class="name">do_query</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_query-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_query"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_query-143"><a href="#DBShell.do_query-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_query-144"><a href="#DBShell.do_query-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_query-145"><a href="#DBShell.do_query-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-146"><a href="#DBShell.do_query-146"><span class="linenos">146</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_query-147"><a href="#DBShell.do_query-147"><span class="linenos">147</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell.do_query-148"><a href="#DBShell.do_query-148"><span class="linenos">148</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell.do_query-149"><a href="#DBShell.do_query-149"><span class="linenos">149</span></a>            <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="DBShell.do_query-150"><a href="#DBShell.do_query-150"><span class="linenos">150</span></a>                <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-151"><a href="#DBShell.do_query-151"><span class="linenos">151</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-152"><a href="#DBShell.do_query-152"><span class="linenos">152</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell.do_query-153"><a href="#DBShell.do_query-153"><span class="linenos">153</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_query-144"><a href="#DBShell.do_query-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_query-145"><a href="#DBShell.do_query-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_query-146"><a href="#DBShell.do_query-146"><span class="linenos">146</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-147"><a href="#DBShell.do_query-147"><span class="linenos">147</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_query-148"><a href="#DBShell.do_query-148"><span class="linenos">148</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell.do_query-149"><a href="#DBShell.do_query-149"><span class="linenos">149</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_query-150"><a href="#DBShell.do_query-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_query-151"><a href="#DBShell.do_query-151"><span class="linenos">151</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell.do_query-152"><a href="#DBShell.do_query-152"><span class="linenos">152</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_query-153"><a href="#DBShell.do_query-153"><span class="linenos">153</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell.do_query-154"><a href="#DBShell.do_query-154"><span class="linenos">154</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-155"><a href="#DBShell.do_query-155"><span class="linenos">155</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_query-156"><a href="#DBShell.do_query-156"><span class="linenos">156</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-157"><a href="#DBShell.do_query-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute a query against the current database.</p>
 </div>
 
 
@@ -1126,36 +1136,36 @@
         <span class="def">def</span>
         <span class="name">do_update</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_update-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_update"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_update-155"><a href="#DBShell.do_update-155"><span class="linenos">155</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_update-156"><a href="#DBShell.do_update-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_update-157"><a href="#DBShell.do_update-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="DBShell.do_update-158"><a href="#DBShell.do_update-158"><span class="linenos">158</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="DBShell.do_update-159"><a href="#DBShell.do_update-159"><span class="linenos">159</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="DBShell.do_update-160"><a href="#DBShell.do_update-160"><span class="linenos">160</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="DBShell.do_update-161"><a href="#DBShell.do_update-161"><span class="linenos">161</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_update-162"><a href="#DBShell.do_update-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="DBShell.do_update-163"><a href="#DBShell.do_update-163"><span class="linenos">163</span></a>
-</span><span id="DBShell.do_update-164"><a href="#DBShell.do_update-164"><span class="linenos">164</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_update-165"><a href="#DBShell.do_update-165"><span class="linenos">165</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_update-166"><a href="#DBShell.do_update-166"><span class="linenos">166</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_update-167"><a href="#DBShell.do_update-167"><span class="linenos">167</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_update-168"><a href="#DBShell.do_update-168"><span class="linenos">168</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_update-169"><a href="#DBShell.do_update-169"><span class="linenos">169</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="DBShell.do_update-170"><a href="#DBShell.do_update-170"><span class="linenos">170</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell.do_update-171"><a href="#DBShell.do_update-171"><span class="linenos">171</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="DBShell.do_update-172"><a href="#DBShell.do_update-172"><span class="linenos">172</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="DBShell.do_update-173"><a href="#DBShell.do_update-173"><span class="linenos">173</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell.do_update-174"><a href="#DBShell.do_update-174"><span class="linenos">174</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell.do_update-175"><a href="#DBShell.do_update-175"><span class="linenos">175</span></a>                <span class="p">)</span>
-</span><span id="DBShell.do_update-176"><a href="#DBShell.do_update-176"><span class="linenos">176</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_update-159"><a href="#DBShell.do_update-159"><span class="linenos">159</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_update-160"><a href="#DBShell.do_update-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_update-161"><a href="#DBShell.do_update-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="DBShell.do_update-162"><a href="#DBShell.do_update-162"><span class="linenos">162</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="DBShell.do_update-163"><a href="#DBShell.do_update-163"><span class="linenos">163</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="DBShell.do_update-164"><a href="#DBShell.do_update-164"><span class="linenos">164</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="DBShell.do_update-165"><a href="#DBShell.do_update-165"><span class="linenos">165</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_update-166"><a href="#DBShell.do_update-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="DBShell.do_update-167"><a href="#DBShell.do_update-167"><span class="linenos">167</span></a>
+</span><span id="DBShell.do_update-168"><a href="#DBShell.do_update-168"><span class="linenos">168</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_update-169"><a href="#DBShell.do_update-169"><span class="linenos">169</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_update-170"><a href="#DBShell.do_update-170"><span class="linenos">170</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_update-171"><a href="#DBShell.do_update-171"><span class="linenos">171</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_update-172"><a href="#DBShell.do_update-172"><span class="linenos">172</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_update-173"><a href="#DBShell.do_update-173"><span class="linenos">173</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="DBShell.do_update-174"><a href="#DBShell.do_update-174"><span class="linenos">174</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell.do_update-175"><a href="#DBShell.do_update-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="DBShell.do_update-176"><a href="#DBShell.do_update-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="DBShell.do_update-177"><a href="#DBShell.do_update-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell.do_update-178"><a href="#DBShell.do_update-178"><span class="linenos">178</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell.do_update-179"><a href="#DBShell.do_update-179"><span class="linenos">179</span></a>                <span class="p">)</span>
+</span><span id="DBShell.do_update-180"><a href="#DBShell.do_update-180"><span class="linenos">180</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update a column to a new value.
 Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.
 Use the -t/--tables flag to limit what tables are updated.
 Use the -m/--match_pairs flag to specify which rows are updated.
@@ -1179,29 +1189,29 @@
         <span class="def">def</span>
         <span class="name">do_delete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_delete-178"><a href="#DBShell.do_delete-178"><span class="linenos">178</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_delete-179"><a href="#DBShell.do_delete-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_delete-180"><a href="#DBShell.do_delete-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="DBShell.do_delete-181"><a href="#DBShell.do_delete-181"><span class="linenos">181</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="DBShell.do_delete-182"><a href="#DBShell.do_delete-182"><span class="linenos">182</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="DBShell.do_delete-183"><a href="#DBShell.do_delete-183"><span class="linenos">183</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_delete-184"><a href="#DBShell.do_delete-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="DBShell.do_delete-185"><a href="#DBShell.do_delete-185"><span class="linenos">185</span></a>
-</span><span id="DBShell.do_delete-186"><a href="#DBShell.do_delete-186"><span class="linenos">186</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_delete-187"><a href="#DBShell.do_delete-187"><span class="linenos">187</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_delete-188"><a href="#DBShell.do_delete-188"><span class="linenos">188</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_delete-189"><a href="#DBShell.do_delete-189"><span class="linenos">189</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_delete-190"><a href="#DBShell.do_delete-190"><span class="linenos">190</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_delete-191"><a href="#DBShell.do_delete-191"><span class="linenos">191</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell.do_delete-192"><a href="#DBShell.do_delete-192"><span class="linenos">192</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_delete-182"><a href="#DBShell.do_delete-182"><span class="linenos">182</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_delete-183"><a href="#DBShell.do_delete-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_delete-184"><a href="#DBShell.do_delete-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="DBShell.do_delete-185"><a href="#DBShell.do_delete-185"><span class="linenos">185</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="DBShell.do_delete-186"><a href="#DBShell.do_delete-186"><span class="linenos">186</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="DBShell.do_delete-187"><a href="#DBShell.do_delete-187"><span class="linenos">187</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_delete-188"><a href="#DBShell.do_delete-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="DBShell.do_delete-189"><a href="#DBShell.do_delete-189"><span class="linenos">189</span></a>
+</span><span id="DBShell.do_delete-190"><a href="#DBShell.do_delete-190"><span class="linenos">190</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_delete-191"><a href="#DBShell.do_delete-191"><span class="linenos">191</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_delete-192"><a href="#DBShell.do_delete-192"><span class="linenos">192</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_delete-193"><a href="#DBShell.do_delete-193"><span class="linenos">193</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_delete-194"><a href="#DBShell.do_delete-194"><span class="linenos">194</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_delete-195"><a href="#DBShell.do_delete-195"><span class="linenos">195</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell.do_delete-196"><a href="#DBShell.do_delete-196"><span class="linenos">196</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete rows from the database.
 Use the -t/--tables flag to limit what tables rows are deleted from.
 Use the -m/--match_pairs flag to specify which rows are deleted.
 Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</p>
@@ -1224,21 +1234,21 @@
         <span class="def">def</span>
         <span class="name">do_add_column</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_add_column-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_add_column"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_column-194"><a href="#DBShell.do_add_column-194"><span class="linenos">194</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_add_column-195"><a href="#DBShell.do_add_column-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_add_column-196"><a href="#DBShell.do_add_column-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_add_column-197"><a href="#DBShell.do_add_column-197"><span class="linenos">197</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_add_column-198"><a href="#DBShell.do_add_column-198"><span class="linenos">198</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_add_column-199"><a href="#DBShell.do_add_column-199"><span class="linenos">199</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_add_column-200"><a href="#DBShell.do_add_column-200"><span class="linenos">200</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_column-198"><a href="#DBShell.do_add_column-198"><span class="linenos">198</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_add_column-199"><a href="#DBShell.do_add_column-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_add_column-200"><a href="#DBShell.do_add_column-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_add_column-201"><a href="#DBShell.do_add_column-201"><span class="linenos">201</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_add_column-202"><a href="#DBShell.do_add_column-202"><span class="linenos">202</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_add_column-203"><a href="#DBShell.do_add_column-203"><span class="linenos">203</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_add_column-204"><a href="#DBShell.do_add_column-204"><span class="linenos">204</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new column to the specified tables.</p>
 </div>
 
 
@@ -1250,22 +1260,22 @@
         <span class="def">def</span>
         <span class="name">do_flush_log</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_flush_log-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_flush_log"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_flush_log-202"><a href="#DBShell.do_flush_log-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_flush_log-203"><a href="#DBShell.do_flush_log-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_flush_log-204"><a href="#DBShell.do_flush_log-204"><span class="linenos">204</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-205"><a href="#DBShell.do_flush_log-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_flush_log-206"><a href="#DBShell.do_flush_log-206"><span class="linenos">206</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-207"><a href="#DBShell.do_flush_log-207"><span class="linenos">207</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_flush_log-208"><a href="#DBShell.do_flush_log-208"><span class="linenos">208</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-209"><a href="#DBShell.do_flush_log-209"><span class="linenos">209</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_flush_log-206"><a href="#DBShell.do_flush_log-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_flush_log-207"><a href="#DBShell.do_flush_log-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_flush_log-208"><a href="#DBShell.do_flush_log-208"><span class="linenos">208</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-209"><a href="#DBShell.do_flush_log-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.do_flush_log-210"><a href="#DBShell.do_flush_log-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-211"><a href="#DBShell.do_flush_log-211"><span class="linenos">211</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_flush_log-212"><a href="#DBShell.do_flush_log-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-213"><a href="#DBShell.do_flush_log-213"><span class="linenos">213</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Clear the log file for this database.</p>
 </div>
 
 
@@ -1277,25 +1287,25 @@
         <span class="def">def</span>
         <span class="name">do_scan_dbs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_scan_dbs-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_scan_dbs"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_scan_dbs-211"><a href="#DBShell.do_scan_dbs-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_scan_dbs-212"><a href="#DBShell.do_scan_dbs-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="DBShell.do_scan_dbs-213"><a href="#DBShell.do_scan_dbs-213"><span class="linenos">213</span></a>
-</span><span id="DBShell.do_scan_dbs-214"><a href="#DBShell.do_scan_dbs-214"><span class="linenos">214</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_scan_dbs-215"><a href="#DBShell.do_scan_dbs-215"><span class="linenos">215</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.do_scan_dbs-216"><a href="#DBShell.do_scan_dbs-216"><span class="linenos">216</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-217"><a href="#DBShell.do_scan_dbs-217"><span class="linenos">217</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_scan_dbs-218"><a href="#DBShell.do_scan_dbs-218"><span class="linenos">218</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-219"><a href="#DBShell.do_scan_dbs-219"><span class="linenos">219</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_scan_dbs-220"><a href="#DBShell.do_scan_dbs-220"><span class="linenos">220</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-221"><a href="#DBShell.do_scan_dbs-221"><span class="linenos">221</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_scan_dbs-215"><a href="#DBShell.do_scan_dbs-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_scan_dbs-216"><a href="#DBShell.do_scan_dbs-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="DBShell.do_scan_dbs-217"><a href="#DBShell.do_scan_dbs-217"><span class="linenos">217</span></a>
+</span><span id="DBShell.do_scan_dbs-218"><a href="#DBShell.do_scan_dbs-218"><span class="linenos">218</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_scan_dbs-219"><a href="#DBShell.do_scan_dbs-219"><span class="linenos">219</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.do_scan_dbs-220"><a href="#DBShell.do_scan_dbs-220"><span class="linenos">220</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-221"><a href="#DBShell.do_scan_dbs-221"><span class="linenos">221</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_scan_dbs-222"><a href="#DBShell.do_scan_dbs-222"><span class="linenos">222</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-223"><a href="#DBShell.do_scan_dbs-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_scan_dbs-224"><a href="#DBShell.do_scan_dbs-224"><span class="linenos">224</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-225"><a href="#DBShell.do_scan_dbs-225"><span class="linenos">225</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current working directory for <code>*.db</code> files and display them.</p>
 
 <p>If the command is entered as <code>based&gt;scan_dbs r</code>, the scan will be performed recursively.</p>
 </div>
@@ -1309,28 +1319,28 @@
         <span class="def">def</span>
         <span class="name">do_customize</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_customize-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_customize"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_customize-223"><a href="#DBShell.do_customize-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_customize-224"><a href="#DBShell.do_customize-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="DBShell.do_customize-225"><a href="#DBShell.do_customize-225"><span class="linenos">225</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="DBShell.do_customize-226"><a href="#DBShell.do_customize-226"><span class="linenos">226</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_customize-227"><a href="#DBShell.do_customize-227"><span class="linenos">227</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-228"><a href="#DBShell.do_customize-228"><span class="linenos">228</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_customize-229"><a href="#DBShell.do_customize-229"><span class="linenos">229</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-230"><a href="#DBShell.do_customize-230"><span class="linenos">230</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_customize-231"><a href="#DBShell.do_customize-231"><span class="linenos">231</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-232"><a href="#DBShell.do_customize-232"><span class="linenos">232</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_customize-227"><a href="#DBShell.do_customize-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_customize-228"><a href="#DBShell.do_customize-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="DBShell.do_customize-229"><a href="#DBShell.do_customize-229"><span class="linenos">229</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="DBShell.do_customize-230"><a href="#DBShell.do_customize-230"><span class="linenos">230</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_customize-231"><a href="#DBShell.do_customize-231"><span class="linenos">231</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-232"><a href="#DBShell.do_customize-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell.do_customize-237"><a href="#DBShell.do_customize-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="DBShell.do_customize-238"><a href="#DBShell.do_customize-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-239"><a href="#DBShell.do_customize-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-240"><a href="#DBShell.do_customize-240"><span class="linenos">240</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate a template file in the current working directory for creating a custom DBShell class.
 Expects one argument: the name of the custom dbshell.
 This will be used to name the generated file as well as several components in the file content.</p>
 </div>
@@ -1344,23 +1354,23 @@
         <span class="def">def</span>
         <span class="name">do_vacuum</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_vacuum-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_vacuum"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-238"><a href="#DBShell.do_vacuum-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_vacuum-239"><a href="#DBShell.do_vacuum-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_vacuum-240"><a href="#DBShell.do_vacuum-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-241"><a href="#DBShell.do_vacuum-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-242"><a href="#DBShell.do_vacuum-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-242"><a href="#DBShell.do_vacuum-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-247"><a href="#DBShell.do_vacuum-247"><span class="linenos">247</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_vacuum-248"><a href="#DBShell.do_vacuum-248"><span class="linenos">248</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-249"><a href="#DBShell.do_vacuum-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-250"><a href="#DBShell.do_vacuum-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce database disk memory.</p>
 </div>
 
 
@@ -1372,51 +1382,51 @@
         <span class="def">def</span>
         <span class="name">preloop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.preloop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.preloop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-266"><a href="#DBShell.preloop-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell.preloop-267"><a href="#DBShell.preloop-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell.preloop-268"><a href="#DBShell.preloop-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.preloop-269"><a href="#DBShell.preloop-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>                <span class="p">)</span>
-</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                <span class="p">)</span>
+</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-303"><a href="#DBShell.preloop-303"><span class="linenos">303</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.preloop-304"><a href="#DBShell.preloop-304"><span class="linenos">304</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-305"><a href="#DBShell.preloop-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell.preloop-306"><a href="#DBShell.preloop-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current directory for a .db file to use.
 If not found, prompt the user for one or to try again recursively.</p>
 </div>
 
@@ -1460,16 +1470,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-305"><a href="#main-305"><span class="linenos">305</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-306"><a href="#main-306"><span class="linenos">306</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-309"><a href="#main-309"><span class="linenos">309</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-310"><a href="#main-310"><span class="linenos">310</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -26,356 +26,20 @@
           o preloop
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** databased.dbshell ******
 ⁰ View Source
 __1import argshell
-__2from pathier import Pathier
-__3
-__4from databased import DataBased, dbparsers
-__5
+__2from griddle import griddy
+__3from pathier import Pathier
+__4
+__5from databased import DataBased, dbparsers
 __6
-__7class DBShell(argshell.ArgShell):
-__8    intro = "Starting dbshell (enter help or ? for arg info)..."
-__9    prompt = "based>"
-_10    dbpath: Pathier = None  # type: ignore
-_11
-_12    def do_use_db(self, arg: str):
-_13        """Set which database file to use."""
-_14        dbpath = Pathier(arg)
-_15        if not dbpath.exists():
-_16            print(f"{dbpath} does not exist.")
-_17            print(f"Still using {self.dbpath}")
-_18        elif not dbpath.is_file():
-_19            print(f"{dbpath} is not a file.")
-_20            print(f"Still using {self.dbpath}")
-_21        else:
-_22            self.dbpath = dbpath
-_23
-_24    def do_dbpath(self, arg: str):
-_25        """Print the .db file in use."""
-_26        print(self.dbpath)
-_27
-_28    @argshell.with_parser(dbparsers.get_backup_parser)
-_29    def do_backup(self, args: argshell.Namespace):
-_30        """Create a backup of the current db file."""
-_31        print(f"Creating a back up for {self.dbpath}...")
-_32        backup_path = self.dbpath.backup(args.timestamp)
-_33        print("Creating backup is complete.")
-_34        print(f"Backup path: {backup_path}")
-_35
-_36    def do_size(self, arg: str):
-_37        """Display the size of the the current db file."""
-_38        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
-_39
-_40    @argshell.with_parser(dbparsers.get_create_table_parser)
-_41    def do_add_table(self, args: argshell.Namespace):
-_42        """Add a new table to the database."""
-_43        with DataBased(self.dbpath) as db:
-_44            db.create_table(args.table_name, args.columns)
-_45
-_46    def do_drop_table(self, arg: str):
-_47        """Drop the specified table."""
-_48        with DataBased(self.dbpath) as db:
-_49            db.drop_table(arg)
-_50
-_51    @argshell.with_parser(
-_52        dbparsers.get_add_row_parser, [dbparsers.verify_matching_length]
-_53    )
-_54    def do_add_row(self, args: argshell.Namespace):
-_55        """Add a row to a table."""
-_56        with DataBased(self.dbpath) as db:
-_57            if db.add_row(args.table_name, args.values, args.columns or
-None):
-_58                print(f"Added row to {args.table_name} table successfully.")
-_59            else:
-_60                print(f"Failed to add row to {args.table_name} table.")
-_61
-_62    @argshell.with_parser(dbparsers.get_info_parser)
-_63    def do_info(self, args: argshell.Namespace):
-_64        """Print out the names of the database tables, their columns, and,
-optionally, the number of rows."""
-_65        print("Getting database info...")
-_66        with DataBased(self.dbpath) as db:
-_67            tables = args.tables or db.get_table_names()
-_68            info = [
-_69                {
-_70                    "Table Name": table,
-_71                    "Columns": ", ".join(db.get_column_names(table)),
-_72                    "Number of Rows": db.count(table) if args.rowcount else
-"n/a",
-_73                }
-_74                for table in tables
-_75            ]
-_76        print(DataBased.data_to_string(info))
-_77
-_78    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-_79    def do_show(self, args: argshell.Namespace):
-_80        """Find and print rows from the database.
-_81        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
-the search.
-_82        Use the -c/--columns flag to limit what columns are printed.
-_83        Use the -o/--order_by flag to order the results.
-_84        Use the -p/--partial_matching flag to enable substring matching on -
-m/--match_pairs
-_85        Pass -h/--help flag for parser help."""
-_86        print("Finding records... ")
-_87        if len(args.columns) == 0:
-_88            args.columns = None
-_89        with DataBased(self.dbpath) as db:
-_90            tables = args.tables or db.get_table_names()
-_91            for table in tables:
-_92                results = db.get_rows(
-_93                    table,
-_94                    args.match_pairs,
-_95                    columns_to_return=args.columns,
-_96                    order_by=args.order_by,
-_97                    limit=args.limit,
-_98                    exact_match=not args.partial_matching,
-_99                )
-100                db.close()
-101                print(f"{len(results)} matching rows in {table} table:")
-102                try:
-103                    print(DataBased.data_to_string(results))  # type: ignore
-104                except Exception as e:
-105                    print("Couldn't fit data into a grid.")
-106                    print(*results, sep="\n")
-107                print()
-108
-109    @argshell.with_parser(dbparsers.get_search_parser)
-110    def do_search(self, args: argshell.Namespace):
-111        """Search and return any rows containg the searched substring in any
-of its columns.
-112        Use the -t/--tables flag to limit the search to a specific table(s).
-113        Use the -c/--columns flag to limit the search to a specific column
-(s)."""
-114        print(f"Searching for {args.search_string}...")
-115        with DataBased(self.dbpath) as db:
-116            tables = args.tables or db.get_table_names()
-117            for table in tables:
-118                columns = args.columns or db.get_column_names(table)
-119                matcher = " OR ".join(
-120                    f'{column} LIKE "%{args.search_string}%"' for column in
-columns
-121                )
-122                query = f"SELECT * FROM {table} WHERE {matcher};"
-123                results = db.query(query)
-124                results = [db._get_dict(table, result) for result in
-results]
-125                print(f"Found {len(results)} results in {table} table.")
-126                print(DataBased.data_to_string(results))
-127
-128    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-129    def do_count(self, args: argshell.Namespace):
-130        """Print the number of rows in the database.
-131        Use the -t/--tables flag to limit results to a specific table(s).
-132        Use the -m/--match_pairs flag to limit the results to rows matching
-these criteria.
-133        Use the -p/--partial_matching flag to enable substring matching on -
-m/--match_pairs.
-134        Pass -h/--help flag for parser help."""
-135        print("Counting rows...")
-136        with DataBased(self.dbpath) as db:
-137            tables = args.tables or db.get_table_names()
-138            for table in tables:
-139                num_rows = db.count(table, args.match_pairs, not
-args.partial_matching)
-140                print(f"{num_rows} matching rows in {table} table.")
-141
-142    def do_query(self, arg: str):
-143        """Execute a query against the current database."""
-144        print(f"Executing {arg}")
-145        with DataBased(self.dbpath) as db:
-146            results = db.query(arg)
-147        try:
-148            for result in results:
-149                print(*result, sep="|-|")
-150            print(f"{db.cursor.rowcount} affected rows")
-151        except Exception as e:
-152            print(f"{type(e).__name__}: {e}")
-153
-154    @argshell.with_parser(dbparsers.get_update_parser,
-[dbparsers.convert_match_pairs])
-155    def do_update(self, args: argshell.Namespace):
-156        """Update a column to a new value.
-157        Two required args: the column (-c/--column) to update and the value
-(-v/--value) to update to.
-158        Use the -t/--tables flag to limit what tables are updated.
-159        Use the -m/--match_pairs flag to specify which rows are updated.
-160        Use the -p/--partial_matching flag to enable substring matching on -
-m/--match_pairs.
-161        >>> based>update -c username -v big_chungus -t users -m username
-lil_chungus
-162
-163        ^will update the username in the users 'table' to 'big_chungus'
-where the username is currently 'lil_chungus'^"""
-164        print("Updating rows...")
-165        with DataBased(self.dbpath) as db:
-166            tables = args.tables or db.get_table_names()
-167            for table in tables:
-168                num_updates = db.update(
-169                    table,
-170                    args.column,
-171                    args.new_value,
-172                    args.match_pairs,
-173                    not args.partial_matching,
-174                )
-175                print(f"Updated {num_updates} rows in {table} table.")
-176
-177    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-178    def do_delete(self, args: argshell.Namespace):
-179        """Delete rows from the database.
-180        Use the -t/--tables flag to limit what tables rows are deleted from.
-181        Use the -m/--match_pairs flag to specify which rows are deleted.
-182        Use the -p/--partial_matching flag to enable substring matching on -
-m/--match_pairs.
-183        >>> based>delete -t users -m username chungus -p
-184
-185        ^will delete all rows in the 'users' table whose username contains
-'chungus'^"""
-186        print("Deleting records...")
-187        with DataBased(self.dbpath) as db:
-188            tables = args.tables or db.get_table_names()
-189            for table in tables:
-190                num_rows = db.delete(table, args.match_pairs, not
-args.partial_matching)
-191                print(f"Deleted {num_rows} rows from {table} table.")
-192
-193    @argshell.with_parser(dbparsers.get_add_column_parser)
-194    def do_add_column(self, args: argshell.Namespace):
-195        """Add a new column to the specified tables."""
-196        with DataBased(self.dbpath) as db:
-197            tables = args.tables or db.get_table_names()
-198            for table in tables:
-199                db.add_column(table, args.column_name, args.type,
-args.default_value)
-200
-201    def do_flush_log(self, arg: str):
-202        """Clear the log file for this database."""
-203        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-204        if not log_path.exists():
-205            print(f"No log file at path {log_path}")
-206        else:
-207            print(f"Flushing log...")
-208            log_path.write_text("")
-209
-210    def do_scan_dbs(self, arg: str):
-211        """Scan the current working directory for `*.db` files and display
-them.
-212
-213        If the command is entered as `based>scan_dbs r`, the scan will be
-performed recursively."""
-214        cwd = Pathier.cwd()
-215        if arg.strip() == "r":
-216            dbs = cwd.rglob("*.db")
-217        else:
-218            dbs = cwd.glob("*.db")
-219        for db in dbs:
-220            print(db.separate(cwd.stem))
-221
-222    def do_customize(self, arg: str):
-223        """Generate a template file in the current working directory for
-creating a custom DBShell class.
-224        Expects one argument: the name of the custom dbshell.
-225        This will be used to name the generated file as well as several
-components in the file content."""
-226        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
-(".py")
-227        if custom_file.exists():
-228            print(f"Error: {custom_file.name} already exists in this
-location.")
-229        else:
-230            variable_name = "_".join(word for word in arg.lower().split())
-231            class_name = "".join(word.capitalize() for word in arg.split())
-232            content = (Pathier(__file__).parent /
-"customshell.py").read_text()
-233            content = content.replace("CustomShell", class_name)
-234            content = content.replace("customshell", variable_name)
-235            custom_file.write_text(content)
-236
-237    def do_vacuum(self, arg: str):
-238        """Reduce database disk memory."""
-239        starting_size = self.dbpath.size()
-240        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-241        print("Vacuuming database...")
-242        with DataBased(self.dbpath) as db:
-243            db.vacuum()
-244        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-245        print(f"Freed up {Pathier.format_size(starting_size -
-self.dbpath.size())} of disk space.")  # type: ignore
-246
-247    def _choose_db(self, options: list[Pathier]) -> Pathier:
-248        """Prompt the user to select from a list of files."""
-249        cwd = Pathier.cwd()
-250        paths = [path.separate(cwd.stem) for path in options]
-251        while True:
-252            print(
-253                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
-enumerate(paths,1)])}"
-254            )
-255            choice = input("Enter the number of the option to use: ")
-256            try:
-257                index = int(choice)
-258                if not 1 <= index <= len(options):
-259                    print("Choice out of range.")
-260                    continue
-261                return options[index - 1]
-262            except Exception as e:
-263                print(f"{choice} is not a valid option.")
-264
-265    def preloop(self):
-266        """Scan the current directory for a .db file to use.
-267        If not found, prompt the user for one or to try again
-recursively."""
-268        if self.dbpath:
-269            self.dbpath = Pathier(self.dbpath)
-270            print(f"Defaulting to database {self.dbpath}")
-271        else:
-272            print("Searching for database...")
-273            cwd = Pathier.cwd()
-274            dbs = list(cwd.glob("*.db"))
-275            if len(dbs) == 1:
-276                self.dbpath = dbs[0]
-277                print(f"Using database {self.dbpath}.")
-278            elif dbs:
-279                self.dbpath = self._choose_db(dbs)
-280            else:
-281                print(f"Could not find a .db file in {cwd}.")
-282                path = input(
-283                    "Enter path to .db file to use or press enter to search
-again recursively: "
-284                )
-285                if path:
-286                    self.dbpath = Pathier(path)
-287                elif not path:
-288                    print("Searching recursively...")
-289                    dbs = list(cwd.rglob("*.db"))
-290                    if len(dbs) == 1:
-291                        self.dbpath = dbs[0]
-292                        print(f"Using database {self.dbpath}.")
-293                    elif dbs:
-294                        self.dbpath = self._choose_db(dbs)
-295                    else:
-296                        print("Could not find a .db file.")
-297                        self.dbpath = Pathier(input("Enter path to a .db
-file: "))
-298        if not self.dbpath.exists():
-299            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-300        if not self.dbpath.is_file():
-301            raise ValueError(f"{self.dbpath} is not a file.")
-302
-303
-304def main():
-305    DBShell().cmdloop()
-  ⁰
-class DBShell(argshell.argshell.ArgShell): View Source
+__7
 __8class DBShell(argshell.ArgShell):
 __9    intro = "Starting dbshell (enter help or ? for arg info)..."
 _10    prompt = "based>"
 _11    dbpath: Pathier = None  # type: ignore
 _12
 _13    def do_use_db(self, arg: str):
 _14        """Set which database file to use."""
@@ -523,582 +187,928 @@
 142
 143    def do_query(self, arg: str):
 144        """Execute a query against the current database."""
 145        print(f"Executing {arg}")
 146        with DataBased(self.dbpath) as db:
 147            results = db.query(arg)
 148        try:
-149            for result in results:
-150                print(*result, sep="|-|")
-151            print(f"{db.cursor.rowcount} affected rows")
-152        except Exception as e:
-153            print(f"{type(e).__name__}: {e}")
-154
-155    @argshell.with_parser(dbparsers.get_update_parser,
+149            try:
+150                print(griddy(results))
+151            except Exception as e:
+152                for result in results:
+153                    print(*result, sep="|-|")
+154        except Exception as e:
+155            print(f"{type(e).__name__}: {e}")
+156        print(f"{db.cursor.rowcount} affected rows")
+157
+158    @argshell.with_parser(dbparsers.get_update_parser,
 [dbparsers.convert_match_pairs])
-156    def do_update(self, args: argshell.Namespace):
-157        """Update a column to a new value.
-158        Two required args: the column (-c/--column) to update and the value
+159    def do_update(self, args: argshell.Namespace):
+160        """Update a column to a new value.
+161        Two required args: the column (-c/--column) to update and the value
 (-v/--value) to update to.
-159        Use the -t/--tables flag to limit what tables are updated.
-160        Use the -m/--match_pairs flag to specify which rows are updated.
-161        Use the -p/--partial_matching flag to enable substring matching on -
+162        Use the -t/--tables flag to limit what tables are updated.
+163        Use the -m/--match_pairs flag to specify which rows are updated.
+164        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-162        >>> based>update -c username -v big_chungus -t users -m username
+165        >>> based>update -c username -v big_chungus -t users -m username
 lil_chungus
-163
-164        ^will update the username in the users 'table' to 'big_chungus'
+166
+167        ^will update the username in the users 'table' to 'big_chungus'
 where the username is currently 'lil_chungus'^"""
-165        print("Updating rows...")
-166        with DataBased(self.dbpath) as db:
-167            tables = args.tables or db.get_table_names()
-168            for table in tables:
-169                num_updates = db.update(
-170                    table,
-171                    args.column,
-172                    args.new_value,
-173                    args.match_pairs,
-174                    not args.partial_matching,
-175                )
-176                print(f"Updated {num_updates} rows in {table} table.")
-177
-178    @argshell.with_parser(dbparsers.get_lookup_parser,
+168        print("Updating rows...")
+169        with DataBased(self.dbpath) as db:
+170            tables = args.tables or db.get_table_names()
+171            for table in tables:
+172                num_updates = db.update(
+173                    table,
+174                    args.column,
+175                    args.new_value,
+176                    args.match_pairs,
+177                    not args.partial_matching,
+178                )
+179                print(f"Updated {num_updates} rows in {table} table.")
+180
+181    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-179    def do_delete(self, args: argshell.Namespace):
-180        """Delete rows from the database.
-181        Use the -t/--tables flag to limit what tables rows are deleted from.
-182        Use the -m/--match_pairs flag to specify which rows are deleted.
-183        Use the -p/--partial_matching flag to enable substring matching on -
+182    def do_delete(self, args: argshell.Namespace):
+183        """Delete rows from the database.
+184        Use the -t/--tables flag to limit what tables rows are deleted from.
+185        Use the -m/--match_pairs flag to specify which rows are deleted.
+186        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-184        >>> based>delete -t users -m username chungus -p
-185
-186        ^will delete all rows in the 'users' table whose username contains
+187        >>> based>delete -t users -m username chungus -p
+188
+189        ^will delete all rows in the 'users' table whose username contains
 'chungus'^"""
-187        print("Deleting records...")
-188        with DataBased(self.dbpath) as db:
-189            tables = args.tables or db.get_table_names()
-190            for table in tables:
-191                num_rows = db.delete(table, args.match_pairs, not
+190        print("Deleting records...")
+191        with DataBased(self.dbpath) as db:
+192            tables = args.tables or db.get_table_names()
+193            for table in tables:
+194                num_rows = db.delete(table, args.match_pairs, not
 args.partial_matching)
-192                print(f"Deleted {num_rows} rows from {table} table.")
-193
-194    @argshell.with_parser(dbparsers.get_add_column_parser)
-195    def do_add_column(self, args: argshell.Namespace):
-196        """Add a new column to the specified tables."""
-197        with DataBased(self.dbpath) as db:
-198            tables = args.tables or db.get_table_names()
-199            for table in tables:
-200                db.add_column(table, args.column_name, args.type,
+195                print(f"Deleted {num_rows} rows from {table} table.")
+196
+197    @argshell.with_parser(dbparsers.get_add_column_parser)
+198    def do_add_column(self, args: argshell.Namespace):
+199        """Add a new column to the specified tables."""
+200        with DataBased(self.dbpath) as db:
+201            tables = args.tables or db.get_table_names()
+202            for table in tables:
+203                db.add_column(table, args.column_name, args.type,
 args.default_value)
-201
-202    def do_flush_log(self, arg: str):
-203        """Clear the log file for this database."""
-204        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-205        if not log_path.exists():
-206            print(f"No log file at path {log_path}")
-207        else:
-208            print(f"Flushing log...")
-209            log_path.write_text("")
-210
-211    def do_scan_dbs(self, arg: str):
-212        """Scan the current working directory for `*.db` files and display
-them.
+204
+205    def do_flush_log(self, arg: str):
+206        """Clear the log file for this database."""
+207        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+208        if not log_path.exists():
+209            print(f"No log file at path {log_path}")
+210        else:
+211            print(f"Flushing log...")
+212            log_path.write_text("")
 213
-214        If the command is entered as `based>scan_dbs r`, the scan will be
+214    def do_scan_dbs(self, arg: str):
+215        """Scan the current working directory for `*.db` files and display
+them.
+216
+217        If the command is entered as `based>scan_dbs r`, the scan will be
+performed recursively."""
+218        cwd = Pathier.cwd()
+219        if arg.strip() == "r":
+220            dbs = cwd.rglob("*.db")
+221        else:
+222            dbs = cwd.glob("*.db")
+223        for db in dbs:
+224            print(db.separate(cwd.stem))
+225
+226    def do_customize(self, arg: str):
+227        """Generate a template file in the current working directory for
+creating a custom DBShell class.
+228        Expects one argument: the name of the custom dbshell.
+229        This will be used to name the generated file as well as several
+components in the file content."""
+230        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+(".py")
+231        if custom_file.exists():
+232            print(f"Error: {custom_file.name} already exists in this
+location.")
+233        else:
+234            variable_name = "_".join(word for word in arg.lower().split())
+235            class_name = "".join(word.capitalize() for word in arg.split())
+236            content = (Pathier(__file__).parent /
+"customshell.py").read_text()
+237            content = content.replace("CustomShell", class_name)
+238            content = content.replace("customshell", variable_name)
+239            custom_file.write_text(content)
+240
+241    def do_vacuum(self, arg: str):
+242        """Reduce database disk memory."""
+243        starting_size = self.dbpath.size()
+244        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+245        print("Vacuuming database...")
+246        with DataBased(self.dbpath) as db:
+247            db.vacuum()
+248        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+249        print(f"Freed up {Pathier.format_size(starting_size -
+self.dbpath.size())} of disk space.")  # type: ignore
+250
+251    def _choose_db(self, options: list[Pathier]) -> Pathier:
+252        """Prompt the user to select from a list of files."""
+253        cwd = Pathier.cwd()
+254        paths = [path.separate(cwd.stem) for path in options]
+255        while True:
+256            print(
+257                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+enumerate(paths,1)])}"
+258            )
+259            choice = input("Enter the number of the option to use: ")
+260            try:
+261                index = int(choice)
+262                if not 1 <= index <= len(options):
+263                    print("Choice out of range.")
+264                    continue
+265                return options[index - 1]
+266            except Exception as e:
+267                print(f"{choice} is not a valid option.")
+268
+269    def preloop(self):
+270        """Scan the current directory for a .db file to use.
+271        If not found, prompt the user for one or to try again
+recursively."""
+272        if self.dbpath:
+273            self.dbpath = Pathier(self.dbpath)
+274            print(f"Defaulting to database {self.dbpath}")
+275        else:
+276            print("Searching for database...")
+277            cwd = Pathier.cwd()
+278            dbs = list(cwd.glob("*.db"))
+279            if len(dbs) == 1:
+280                self.dbpath = dbs[0]
+281                print(f"Using database {self.dbpath}.")
+282            elif dbs:
+283                self.dbpath = self._choose_db(dbs)
+284            else:
+285                print(f"Could not find a .db file in {cwd}.")
+286                path = input(
+287                    "Enter path to .db file to use or press enter to search
+again recursively: "
+288                )
+289                if path:
+290                    self.dbpath = Pathier(path)
+291                elif not path:
+292                    print("Searching recursively...")
+293                    dbs = list(cwd.rglob("*.db"))
+294                    if len(dbs) == 1:
+295                        self.dbpath = dbs[0]
+296                        print(f"Using database {self.dbpath}.")
+297                    elif dbs:
+298                        self.dbpath = self._choose_db(dbs)
+299                    else:
+300                        print("Could not find a .db file.")
+301                        self.dbpath = Pathier(input("Enter path to a .db
+file: "))
+302        if not self.dbpath.exists():
+303            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+304        if not self.dbpath.is_file():
+305            raise ValueError(f"{self.dbpath} is not a file.")
+306
+307
+308def main():
+309    DBShell().cmdloop()
+  ⁰
+class DBShell(argshell.argshell.ArgShell): View Source
+__9class DBShell(argshell.ArgShell):
+_10    intro = "Starting dbshell (enter help or ? for arg info)..."
+_11    prompt = "based>"
+_12    dbpath: Pathier = None  # type: ignore
+_13
+_14    def do_use_db(self, arg: str):
+_15        """Set which database file to use."""
+_16        dbpath = Pathier(arg)
+_17        if not dbpath.exists():
+_18            print(f"{dbpath} does not exist.")
+_19            print(f"Still using {self.dbpath}")
+_20        elif not dbpath.is_file():
+_21            print(f"{dbpath} is not a file.")
+_22            print(f"Still using {self.dbpath}")
+_23        else:
+_24            self.dbpath = dbpath
+_25
+_26    def do_dbpath(self, arg: str):
+_27        """Print the .db file in use."""
+_28        print(self.dbpath)
+_29
+_30    @argshell.with_parser(dbparsers.get_backup_parser)
+_31    def do_backup(self, args: argshell.Namespace):
+_32        """Create a backup of the current db file."""
+_33        print(f"Creating a back up for {self.dbpath}...")
+_34        backup_path = self.dbpath.backup(args.timestamp)
+_35        print("Creating backup is complete.")
+_36        print(f"Backup path: {backup_path}")
+_37
+_38    def do_size(self, arg: str):
+_39        """Display the size of the the current db file."""
+_40        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+_41
+_42    @argshell.with_parser(dbparsers.get_create_table_parser)
+_43    def do_add_table(self, args: argshell.Namespace):
+_44        """Add a new table to the database."""
+_45        with DataBased(self.dbpath) as db:
+_46            db.create_table(args.table_name, args.columns)
+_47
+_48    def do_drop_table(self, arg: str):
+_49        """Drop the specified table."""
+_50        with DataBased(self.dbpath) as db:
+_51            db.drop_table(arg)
+_52
+_53    @argshell.with_parser(
+_54        dbparsers.get_add_row_parser, [dbparsers.verify_matching_length]
+_55    )
+_56    def do_add_row(self, args: argshell.Namespace):
+_57        """Add a row to a table."""
+_58        with DataBased(self.dbpath) as db:
+_59            if db.add_row(args.table_name, args.values, args.columns or
+None):
+_60                print(f"Added row to {args.table_name} table successfully.")
+_61            else:
+_62                print(f"Failed to add row to {args.table_name} table.")
+_63
+_64    @argshell.with_parser(dbparsers.get_info_parser)
+_65    def do_info(self, args: argshell.Namespace):
+_66        """Print out the names of the database tables, their columns, and,
+optionally, the number of rows."""
+_67        print("Getting database info...")
+_68        with DataBased(self.dbpath) as db:
+_69            tables = args.tables or db.get_table_names()
+_70            info = [
+_71                {
+_72                    "Table Name": table,
+_73                    "Columns": ", ".join(db.get_column_names(table)),
+_74                    "Number of Rows": db.count(table) if args.rowcount else
+"n/a",
+_75                }
+_76                for table in tables
+_77            ]
+_78        print(DataBased.data_to_string(info))
+_79
+_80    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+_81    def do_show(self, args: argshell.Namespace):
+_82        """Find and print rows from the database.
+_83        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
+the search.
+_84        Use the -c/--columns flag to limit what columns are printed.
+_85        Use the -o/--order_by flag to order the results.
+_86        Use the -p/--partial_matching flag to enable substring matching on -
+m/--match_pairs
+_87        Pass -h/--help flag for parser help."""
+_88        print("Finding records... ")
+_89        if len(args.columns) == 0:
+_90            args.columns = None
+_91        with DataBased(self.dbpath) as db:
+_92            tables = args.tables or db.get_table_names()
+_93            for table in tables:
+_94                results = db.get_rows(
+_95                    table,
+_96                    args.match_pairs,
+_97                    columns_to_return=args.columns,
+_98                    order_by=args.order_by,
+_99                    limit=args.limit,
+100                    exact_match=not args.partial_matching,
+101                )
+102                db.close()
+103                print(f"{len(results)} matching rows in {table} table:")
+104                try:
+105                    print(DataBased.data_to_string(results))  # type: ignore
+106                except Exception as e:
+107                    print("Couldn't fit data into a grid.")
+108                    print(*results, sep="\n")
+109                print()
+110
+111    @argshell.with_parser(dbparsers.get_search_parser)
+112    def do_search(self, args: argshell.Namespace):
+113        """Search and return any rows containg the searched substring in any
+of its columns.
+114        Use the -t/--tables flag to limit the search to a specific table(s).
+115        Use the -c/--columns flag to limit the search to a specific column
+(s)."""
+116        print(f"Searching for {args.search_string}...")
+117        with DataBased(self.dbpath) as db:
+118            tables = args.tables or db.get_table_names()
+119            for table in tables:
+120                columns = args.columns or db.get_column_names(table)
+121                matcher = " OR ".join(
+122                    f'{column} LIKE "%{args.search_string}%"' for column in
+columns
+123                )
+124                query = f"SELECT * FROM {table} WHERE {matcher};"
+125                results = db.query(query)
+126                results = [db._get_dict(table, result) for result in
+results]
+127                print(f"Found {len(results)} results in {table} table.")
+128                print(DataBased.data_to_string(results))
+129
+130    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+131    def do_count(self, args: argshell.Namespace):
+132        """Print the number of rows in the database.
+133        Use the -t/--tables flag to limit results to a specific table(s).
+134        Use the -m/--match_pairs flag to limit the results to rows matching
+these criteria.
+135        Use the -p/--partial_matching flag to enable substring matching on -
+m/--match_pairs.
+136        Pass -h/--help flag for parser help."""
+137        print("Counting rows...")
+138        with DataBased(self.dbpath) as db:
+139            tables = args.tables or db.get_table_names()
+140            for table in tables:
+141                num_rows = db.count(table, args.match_pairs, not
+args.partial_matching)
+142                print(f"{num_rows} matching rows in {table} table.")
+143
+144    def do_query(self, arg: str):
+145        """Execute a query against the current database."""
+146        print(f"Executing {arg}")
+147        with DataBased(self.dbpath) as db:
+148            results = db.query(arg)
+149        try:
+150            try:
+151                print(griddy(results))
+152            except Exception as e:
+153                for result in results:
+154                    print(*result, sep="|-|")
+155        except Exception as e:
+156            print(f"{type(e).__name__}: {e}")
+157        print(f"{db.cursor.rowcount} affected rows")
+158
+159    @argshell.with_parser(dbparsers.get_update_parser,
+[dbparsers.convert_match_pairs])
+160    def do_update(self, args: argshell.Namespace):
+161        """Update a column to a new value.
+162        Two required args: the column (-c/--column) to update and the value
+(-v/--value) to update to.
+163        Use the -t/--tables flag to limit what tables are updated.
+164        Use the -m/--match_pairs flag to specify which rows are updated.
+165        Use the -p/--partial_matching flag to enable substring matching on -
+m/--match_pairs.
+166        >>> based>update -c username -v big_chungus -t users -m username
+lil_chungus
+167
+168        ^will update the username in the users 'table' to 'big_chungus'
+where the username is currently 'lil_chungus'^"""
+169        print("Updating rows...")
+170        with DataBased(self.dbpath) as db:
+171            tables = args.tables or db.get_table_names()
+172            for table in tables:
+173                num_updates = db.update(
+174                    table,
+175                    args.column,
+176                    args.new_value,
+177                    args.match_pairs,
+178                    not args.partial_matching,
+179                )
+180                print(f"Updated {num_updates} rows in {table} table.")
+181
+182    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+183    def do_delete(self, args: argshell.Namespace):
+184        """Delete rows from the database.
+185        Use the -t/--tables flag to limit what tables rows are deleted from.
+186        Use the -m/--match_pairs flag to specify which rows are deleted.
+187        Use the -p/--partial_matching flag to enable substring matching on -
+m/--match_pairs.
+188        >>> based>delete -t users -m username chungus -p
+189
+190        ^will delete all rows in the 'users' table whose username contains
+'chungus'^"""
+191        print("Deleting records...")
+192        with DataBased(self.dbpath) as db:
+193            tables = args.tables or db.get_table_names()
+194            for table in tables:
+195                num_rows = db.delete(table, args.match_pairs, not
+args.partial_matching)
+196                print(f"Deleted {num_rows} rows from {table} table.")
+197
+198    @argshell.with_parser(dbparsers.get_add_column_parser)
+199    def do_add_column(self, args: argshell.Namespace):
+200        """Add a new column to the specified tables."""
+201        with DataBased(self.dbpath) as db:
+202            tables = args.tables or db.get_table_names()
+203            for table in tables:
+204                db.add_column(table, args.column_name, args.type,
+args.default_value)
+205
+206    def do_flush_log(self, arg: str):
+207        """Clear the log file for this database."""
+208        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+209        if not log_path.exists():
+210            print(f"No log file at path {log_path}")
+211        else:
+212            print(f"Flushing log...")
+213            log_path.write_text("")
+214
+215    def do_scan_dbs(self, arg: str):
+216        """Scan the current working directory for `*.db` files and display
+them.
+217
+218        If the command is entered as `based>scan_dbs r`, the scan will be
 performed recursively."""
-215        cwd = Pathier.cwd()
-216        if arg.strip() == "r":
-217            dbs = cwd.rglob("*.db")
-218        else:
-219            dbs = cwd.glob("*.db")
-220        for db in dbs:
-221            print(db.separate(cwd.stem))
-222
-223    def do_customize(self, arg: str):
-224        """Generate a template file in the current working directory for
+219        cwd = Pathier.cwd()
+220        if arg.strip() == "r":
+221            dbs = cwd.rglob("*.db")
+222        else:
+223            dbs = cwd.glob("*.db")
+224        for db in dbs:
+225            print(db.separate(cwd.stem))
+226
+227    def do_customize(self, arg: str):
+228        """Generate a template file in the current working directory for
 creating a custom DBShell class.
-225        Expects one argument: the name of the custom dbshell.
-226        This will be used to name the generated file as well as several
+229        Expects one argument: the name of the custom dbshell.
+230        This will be used to name the generated file as well as several
 components in the file content."""
-227        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+231        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
 (".py")
-228        if custom_file.exists():
-229            print(f"Error: {custom_file.name} already exists in this
+232        if custom_file.exists():
+233            print(f"Error: {custom_file.name} already exists in this
 location.")
-230        else:
-231            variable_name = "_".join(word for word in arg.lower().split())
-232            class_name = "".join(word.capitalize() for word in arg.split())
-233            content = (Pathier(__file__).parent /
+234        else:
+235            variable_name = "_".join(word for word in arg.lower().split())
+236            class_name = "".join(word.capitalize() for word in arg.split())
+237            content = (Pathier(__file__).parent /
 "customshell.py").read_text()
-234            content = content.replace("CustomShell", class_name)
-235            content = content.replace("customshell", variable_name)
-236            custom_file.write_text(content)
-237
-238    def do_vacuum(self, arg: str):
-239        """Reduce database disk memory."""
-240        starting_size = self.dbpath.size()
-241        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-242        print("Vacuuming database...")
-243        with DataBased(self.dbpath) as db:
-244            db.vacuum()
-245        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-246        print(f"Freed up {Pathier.format_size(starting_size -
+238            content = content.replace("CustomShell", class_name)
+239            content = content.replace("customshell", variable_name)
+240            custom_file.write_text(content)
+241
+242    def do_vacuum(self, arg: str):
+243        """Reduce database disk memory."""
+244        starting_size = self.dbpath.size()
+245        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+246        print("Vacuuming database...")
+247        with DataBased(self.dbpath) as db:
+248            db.vacuum()
+249        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+250        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
-247
-248    def _choose_db(self, options: list[Pathier]) -> Pathier:
-249        """Prompt the user to select from a list of files."""
-250        cwd = Pathier.cwd()
-251        paths = [path.separate(cwd.stem) for path in options]
-252        while True:
-253            print(
-254                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+251
+252    def _choose_db(self, options: list[Pathier]) -> Pathier:
+253        """Prompt the user to select from a list of files."""
+254        cwd = Pathier.cwd()
+255        paths = [path.separate(cwd.stem) for path in options]
+256        while True:
+257            print(
+258                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-255            )
-256            choice = input("Enter the number of the option to use: ")
-257            try:
-258                index = int(choice)
-259                if not 1 <= index <= len(options):
-260                    print("Choice out of range.")
-261                    continue
-262                return options[index - 1]
-263            except Exception as e:
-264                print(f"{choice} is not a valid option.")
-265
-266    def preloop(self):
-267        """Scan the current directory for a .db file to use.
-268        If not found, prompt the user for one or to try again
+259            )
+260            choice = input("Enter the number of the option to use: ")
+261            try:
+262                index = int(choice)
+263                if not 1 <= index <= len(options):
+264                    print("Choice out of range.")
+265                    continue
+266                return options[index - 1]
+267            except Exception as e:
+268                print(f"{choice} is not a valid option.")
+269
+270    def preloop(self):
+271        """Scan the current directory for a .db file to use.
+272        If not found, prompt the user for one or to try again
 recursively."""
-269        if self.dbpath:
-270            self.dbpath = Pathier(self.dbpath)
-271            print(f"Defaulting to database {self.dbpath}")
-272        else:
-273            print("Searching for database...")
-274            cwd = Pathier.cwd()
-275            dbs = list(cwd.glob("*.db"))
-276            if len(dbs) == 1:
-277                self.dbpath = dbs[0]
-278                print(f"Using database {self.dbpath}.")
-279            elif dbs:
-280                self.dbpath = self._choose_db(dbs)
-281            else:
-282                print(f"Could not find a .db file in {cwd}.")
-283                path = input(
-284                    "Enter path to .db file to use or press enter to search
+273        if self.dbpath:
+274            self.dbpath = Pathier(self.dbpath)
+275            print(f"Defaulting to database {self.dbpath}")
+276        else:
+277            print("Searching for database...")
+278            cwd = Pathier.cwd()
+279            dbs = list(cwd.glob("*.db"))
+280            if len(dbs) == 1:
+281                self.dbpath = dbs[0]
+282                print(f"Using database {self.dbpath}.")
+283            elif dbs:
+284                self.dbpath = self._choose_db(dbs)
+285            else:
+286                print(f"Could not find a .db file in {cwd}.")
+287                path = input(
+288                    "Enter path to .db file to use or press enter to search
 again recursively: "
-285                )
-286                if path:
-287                    self.dbpath = Pathier(path)
-288                elif not path:
-289                    print("Searching recursively...")
-290                    dbs = list(cwd.rglob("*.db"))
-291                    if len(dbs) == 1:
-292                        self.dbpath = dbs[0]
-293                        print(f"Using database {self.dbpath}.")
-294                    elif dbs:
-295                        self.dbpath = self._choose_db(dbs)
-296                    else:
-297                        print("Could not find a .db file.")
-298                        self.dbpath = Pathier(input("Enter path to a .db
+289                )
+290                if path:
+291                    self.dbpath = Pathier(path)
+292                elif not path:
+293                    print("Searching recursively...")
+294                    dbs = list(cwd.rglob("*.db"))
+295                    if len(dbs) == 1:
+296                        self.dbpath = dbs[0]
+297                        print(f"Using database {self.dbpath}.")
+298                    elif dbs:
+299                        self.dbpath = self._choose_db(dbs)
+300                    else:
+301                        print("Could not find a .db file.")
+302                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-299        if not self.dbpath.exists():
-300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-301        if not self.dbpath.is_file():
-302            raise ValueError(f"{self.dbpath} is not a file.")
+303        if not self.dbpath.exists():
+304            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+305        if not self.dbpath.is_file():
+306            raise ValueError(f"{self.dbpath} is not a file.")
 Subclass this to create custom ArgShells.
 ⁰
 def do_use_db(self, arg: str): View Source
-13    def do_use_db(self, arg: str):
-14        """Set which database file to use."""
-15        dbpath = Pathier(arg)
-16        if not dbpath.exists():
-17            print(f"{dbpath} does not exist.")
-18            print(f"Still using {self.dbpath}")
-19        elif not dbpath.is_file():
-20            print(f"{dbpath} is not a file.")
-21            print(f"Still using {self.dbpath}")
-22        else:
-23            self.dbpath = dbpath
+14    def do_use_db(self, arg: str):
+15        """Set which database file to use."""
+16        dbpath = Pathier(arg)
+17        if not dbpath.exists():
+18            print(f"{dbpath} does not exist.")
+19            print(f"Still using {self.dbpath}")
+20        elif not dbpath.is_file():
+21            print(f"{dbpath} is not a file.")
+22            print(f"Still using {self.dbpath}")
+23        else:
+24            self.dbpath = dbpath
 Set which database file to use.
 ⁰
 def do_dbpath(self, arg: str): View Source
-25    def do_dbpath(self, arg: str):
-26        """Print the .db file in use."""
-27        print(self.dbpath)
+26    def do_dbpath(self, arg: str):
+27        """Print the .db file in use."""
+28        print(self.dbpath)
 Print the .db file in use.
 ⁰
 @argshell.with_parser(dbparsers.get_backup_parser)
 def do_backup(self, args: argshell.argshell.Namespace): View Source
-29    @argshell.with_parser(dbparsers.get_backup_parser)
-30    def do_backup(self, args: argshell.Namespace):
-31        """Create a backup of the current db file."""
-32        print(f"Creating a back up for {self.dbpath}...")
-33        backup_path = self.dbpath.backup(args.timestamp)
-34        print("Creating backup is complete.")
-35        print(f"Backup path: {backup_path}")
+30    @argshell.with_parser(dbparsers.get_backup_parser)
+31    def do_backup(self, args: argshell.Namespace):
+32        """Create a backup of the current db file."""
+33        print(f"Creating a back up for {self.dbpath}...")
+34        backup_path = self.dbpath.backup(args.timestamp)
+35        print("Creating backup is complete.")
+36        print(f"Backup path: {backup_path}")
 Create a backup of the current db file.
 ⁰
 def do_size(self, arg: str): View Source
-37    def do_size(self, arg: str):
-38        """Display the size of the the current db file."""
-39        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+38    def do_size(self, arg: str):
+39        """Display the size of the the current db file."""
+40        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
 Display the size of the the current db file.
 ⁰
 @argshell.with_parser(dbparsers.get_create_table_parser)
 def do_add_table(self, args: argshell.argshell.Namespace): View Source
-41    @argshell.with_parser(dbparsers.get_create_table_parser)
-42    def do_add_table(self, args: argshell.Namespace):
-43        """Add a new table to the database."""
-44        with DataBased(self.dbpath) as db:
-45            db.create_table(args.table_name, args.columns)
+42    @argshell.with_parser(dbparsers.get_create_table_parser)
+43    def do_add_table(self, args: argshell.Namespace):
+44        """Add a new table to the database."""
+45        with DataBased(self.dbpath) as db:
+46            db.create_table(args.table_name, args.columns)
 Add a new table to the database.
 ⁰
 def do_drop_table(self, arg: str): View Source
-47    def do_drop_table(self, arg: str):
-48        """Drop the specified table."""
-49        with DataBased(self.dbpath) as db:
-50            db.drop_table(arg)
+48    def do_drop_table(self, arg: str):
+49        """Drop the specified table."""
+50        with DataBased(self.dbpath) as db:
+51            db.drop_table(arg)
 Drop the specified table.
 ⁰
 @argshell.with_parser(dbparsers.get_add_row_parser,
 [dbparsers.verify_matching_length])
 def do_add_row(self, args: argshell.argshell.Namespace): View Source
-52    @argshell.with_parser(
-53        dbparsers.get_add_row_parser, [dbparsers.verify_matching_length]
-54    )
-55    def do_add_row(self, args: argshell.Namespace):
-56        """Add a row to a table."""
-57        with DataBased(self.dbpath) as db:
-58            if db.add_row(args.table_name, args.values, args.columns or
+53    @argshell.with_parser(
+54        dbparsers.get_add_row_parser, [dbparsers.verify_matching_length]
+55    )
+56    def do_add_row(self, args: argshell.Namespace):
+57        """Add a row to a table."""
+58        with DataBased(self.dbpath) as db:
+59            if db.add_row(args.table_name, args.values, args.columns or
 None):
-59                print(f"Added row to {args.table_name} table successfully.")
-60            else:
-61                print(f"Failed to add row to {args.table_name} table.")
+60                print(f"Added row to {args.table_name} table successfully.")
+61            else:
+62                print(f"Failed to add row to {args.table_name} table.")
 Add a row to a table.
 ⁰
 @argshell.with_parser(dbparsers.get_info_parser)
 def do_info(self, args: argshell.argshell.Namespace): View Source
-63    @argshell.with_parser(dbparsers.get_info_parser)
-64    def do_info(self, args: argshell.Namespace):
-65        """Print out the names of the database tables, their columns, and,
+64    @argshell.with_parser(dbparsers.get_info_parser)
+65    def do_info(self, args: argshell.Namespace):
+66        """Print out the names of the database tables, their columns, and,
 optionally, the number of rows."""
-66        print("Getting database info...")
-67        with DataBased(self.dbpath) as db:
-68            tables = args.tables or db.get_table_names()
-69            info = [
-70                {
-71                    "Table Name": table,
-72                    "Columns": ", ".join(db.get_column_names(table)),
-73                    "Number of Rows": db.count(table) if args.rowcount else
+67        print("Getting database info...")
+68        with DataBased(self.dbpath) as db:
+69            tables = args.tables or db.get_table_names()
+70            info = [
+71                {
+72                    "Table Name": table,
+73                    "Columns": ", ".join(db.get_column_names(table)),
+74                    "Number of Rows": db.count(table) if args.rowcount else
 "n/a",
-74                }
-75                for table in tables
-76            ]
-77        print(DataBased.data_to_string(info))
+75                }
+76                for table in tables
+77            ]
+78        print(DataBased.data_to_string(info))
 Print out the names of the database tables, their columns, and, optionally, the
 number of rows.
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
 def do_show(self, args: argshell.argshell.Namespace): View Source
-_79    @argshell.with_parser(dbparsers.get_lookup_parser,
+_80    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-_80    def do_show(self, args: argshell.Namespace):
-_81        """Find and print rows from the database.
-_82        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
+_81    def do_show(self, args: argshell.Namespace):
+_82        """Find and print rows from the database.
+_83        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit
 the search.
-_83        Use the -c/--columns flag to limit what columns are printed.
-_84        Use the -o/--order_by flag to order the results.
-_85        Use the -p/--partial_matching flag to enable substring matching on -
+_84        Use the -c/--columns flag to limit what columns are printed.
+_85        Use the -o/--order_by flag to order the results.
+_86        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs
-_86        Pass -h/--help flag for parser help."""
-_87        print("Finding records... ")
-_88        if len(args.columns) == 0:
-_89            args.columns = None
-_90        with DataBased(self.dbpath) as db:
-_91            tables = args.tables or db.get_table_names()
-_92            for table in tables:
-_93                results = db.get_rows(
-_94                    table,
-_95                    args.match_pairs,
-_96                    columns_to_return=args.columns,
-_97                    order_by=args.order_by,
-_98                    limit=args.limit,
-_99                    exact_match=not args.partial_matching,
-100                )
-101                db.close()
-102                print(f"{len(results)} matching rows in {table} table:")
-103                try:
-104                    print(DataBased.data_to_string(results))  # type: ignore
-105                except Exception as e:
-106                    print("Couldn't fit data into a grid.")
-107                    print(*results, sep="\n")
-108                print()
+_87        Pass -h/--help flag for parser help."""
+_88        print("Finding records... ")
+_89        if len(args.columns) == 0:
+_90            args.columns = None
+_91        with DataBased(self.dbpath) as db:
+_92            tables = args.tables or db.get_table_names()
+_93            for table in tables:
+_94                results = db.get_rows(
+_95                    table,
+_96                    args.match_pairs,
+_97                    columns_to_return=args.columns,
+_98                    order_by=args.order_by,
+_99                    limit=args.limit,
+100                    exact_match=not args.partial_matching,
+101                )
+102                db.close()
+103                print(f"{len(results)} matching rows in {table} table:")
+104                try:
+105                    print(DataBased.data_to_string(results))  # type: ignore
+106                except Exception as e:
+107                    print("Couldn't fit data into a grid.")
+108                    print(*results, sep="\n")
+109                print()
 Find and print rows from the database. Use the -t/--tables, -m/--match_pairs,
 and -l/--limit flags to limit the search. Use the -c/--columns flag to limit
 what columns are printed. Use the -o/--order_by flag to order the results. Use
 the -p/--partial_matching flag to enable substring matching on -m/--match_pairs
 Pass -h/--help flag for parser help.
 ⁰
 @argshell.with_parser(dbparsers.get_search_parser)
 def do_search(self, args: argshell.argshell.Namespace): View Source
-110    @argshell.with_parser(dbparsers.get_search_parser)
-111    def do_search(self, args: argshell.Namespace):
-112        """Search and return any rows containg the searched substring in any
+111    @argshell.with_parser(dbparsers.get_search_parser)
+112    def do_search(self, args: argshell.Namespace):
+113        """Search and return any rows containg the searched substring in any
 of its columns.
-113        Use the -t/--tables flag to limit the search to a specific table(s).
-114        Use the -c/--columns flag to limit the search to a specific column
+114        Use the -t/--tables flag to limit the search to a specific table(s).
+115        Use the -c/--columns flag to limit the search to a specific column
 (s)."""
-115        print(f"Searching for {args.search_string}...")
-116        with DataBased(self.dbpath) as db:
-117            tables = args.tables or db.get_table_names()
-118            for table in tables:
-119                columns = args.columns or db.get_column_names(table)
-120                matcher = " OR ".join(
-121                    f'{column} LIKE "%{args.search_string}%"' for column in
+116        print(f"Searching for {args.search_string}...")
+117        with DataBased(self.dbpath) as db:
+118            tables = args.tables or db.get_table_names()
+119            for table in tables:
+120                columns = args.columns or db.get_column_names(table)
+121                matcher = " OR ".join(
+122                    f'{column} LIKE "%{args.search_string}%"' for column in
 columns
-122                )
-123                query = f"SELECT * FROM {table} WHERE {matcher};"
-124                results = db.query(query)
-125                results = [db._get_dict(table, result) for result in
+123                )
+124                query = f"SELECT * FROM {table} WHERE {matcher};"
+125                results = db.query(query)
+126                results = [db._get_dict(table, result) for result in
 results]
-126                print(f"Found {len(results)} results in {table} table.")
-127                print(DataBased.data_to_string(results))
+127                print(f"Found {len(results)} results in {table} table.")
+128                print(DataBased.data_to_string(results))
 Search and return any rows containg the searched substring in any of its
 columns. Use the -t/--tables flag to limit the search to a specific table(s).
 Use the -c/--columns flag to limit the search to a specific column(s).
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
 def do_count(self, args: argshell.argshell.Namespace): View Source
-129    @argshell.with_parser(dbparsers.get_lookup_parser,
+130    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-130    def do_count(self, args: argshell.Namespace):
-131        """Print the number of rows in the database.
-132        Use the -t/--tables flag to limit results to a specific table(s).
-133        Use the -m/--match_pairs flag to limit the results to rows matching
+131    def do_count(self, args: argshell.Namespace):
+132        """Print the number of rows in the database.
+133        Use the -t/--tables flag to limit results to a specific table(s).
+134        Use the -m/--match_pairs flag to limit the results to rows matching
 these criteria.
-134        Use the -p/--partial_matching flag to enable substring matching on -
+135        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-135        Pass -h/--help flag for parser help."""
-136        print("Counting rows...")
-137        with DataBased(self.dbpath) as db:
-138            tables = args.tables or db.get_table_names()
-139            for table in tables:
-140                num_rows = db.count(table, args.match_pairs, not
+136        Pass -h/--help flag for parser help."""
+137        print("Counting rows...")
+138        with DataBased(self.dbpath) as db:
+139            tables = args.tables or db.get_table_names()
+140            for table in tables:
+141                num_rows = db.count(table, args.match_pairs, not
 args.partial_matching)
-141                print(f"{num_rows} matching rows in {table} table.")
+142                print(f"{num_rows} matching rows in {table} table.")
 Print the number of rows in the database. Use the -t/--tables flag to limit
 results to a specific table(s). Use the -m/--match_pairs flag to limit the
 results to rows matching these criteria. Use the -p/--partial_matching flag to
 enable substring matching on -m/--match_pairs. Pass -h/--help flag for parser
 help.
 ⁰
 def do_query(self, arg: str): View Source
-143    def do_query(self, arg: str):
-144        """Execute a query against the current database."""
-145        print(f"Executing {arg}")
-146        with DataBased(self.dbpath) as db:
-147            results = db.query(arg)
-148        try:
-149            for result in results:
-150                print(*result, sep="|-|")
-151            print(f"{db.cursor.rowcount} affected rows")
-152        except Exception as e:
-153            print(f"{type(e).__name__}: {e}")
+144    def do_query(self, arg: str):
+145        """Execute a query against the current database."""
+146        print(f"Executing {arg}")
+147        with DataBased(self.dbpath) as db:
+148            results = db.query(arg)
+149        try:
+150            try:
+151                print(griddy(results))
+152            except Exception as e:
+153                for result in results:
+154                    print(*result, sep="|-|")
+155        except Exception as e:
+156            print(f"{type(e).__name__}: {e}")
+157        print(f"{db.cursor.rowcount} affected rows")
 Execute a query against the current database.
 ⁰
 @argshell.with_parser(dbparsers.get_update_parser,
 [dbparsers.convert_match_pairs])
 def do_update(self, args: argshell.argshell.Namespace): View Source
-155    @argshell.with_parser(dbparsers.get_update_parser,
+159    @argshell.with_parser(dbparsers.get_update_parser,
 [dbparsers.convert_match_pairs])
-156    def do_update(self, args: argshell.Namespace):
-157        """Update a column to a new value.
-158        Two required args: the column (-c/--column) to update and the value
+160    def do_update(self, args: argshell.Namespace):
+161        """Update a column to a new value.
+162        Two required args: the column (-c/--column) to update and the value
 (-v/--value) to update to.
-159        Use the -t/--tables flag to limit what tables are updated.
-160        Use the -m/--match_pairs flag to specify which rows are updated.
-161        Use the -p/--partial_matching flag to enable substring matching on -
+163        Use the -t/--tables flag to limit what tables are updated.
+164        Use the -m/--match_pairs flag to specify which rows are updated.
+165        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-162        >>> based>update -c username -v big_chungus -t users -m username
+166        >>> based>update -c username -v big_chungus -t users -m username
 lil_chungus
-163
-164        ^will update the username in the users 'table' to 'big_chungus'
+167
+168        ^will update the username in the users 'table' to 'big_chungus'
 where the username is currently 'lil_chungus'^"""
-165        print("Updating rows...")
-166        with DataBased(self.dbpath) as db:
-167            tables = args.tables or db.get_table_names()
-168            for table in tables:
-169                num_updates = db.update(
-170                    table,
-171                    args.column,
-172                    args.new_value,
-173                    args.match_pairs,
-174                    not args.partial_matching,
-175                )
-176                print(f"Updated {num_updates} rows in {table} table.")
+169        print("Updating rows...")
+170        with DataBased(self.dbpath) as db:
+171            tables = args.tables or db.get_table_names()
+172            for table in tables:
+173                num_updates = db.update(
+174                    table,
+175                    args.column,
+176                    args.new_value,
+177                    args.match_pairs,
+178                    not args.partial_matching,
+179                )
+180                print(f"Updated {num_updates} rows in {table} table.")
 Update a column to a new value. Two required args: the column (-c/--column) to
 update and the value (-v/--value) to update to. Use the -t/--tables flag to
 limit what tables are updated. Use the -m/--match_pairs flag to specify which
 rows are updated. Use the -p/--partial_matching flag to enable substring
 matching on -m/--match_pairs.
 >>> based>update -c username -v big_chungus -t users -m username lil_chungus
 ^will update the username in the users 'table' to 'big_chungus' where the
 username is currently 'lil_chungus'^
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
 def do_delete(self, args: argshell.argshell.Namespace): View Source
-178    @argshell.with_parser(dbparsers.get_lookup_parser,
+182    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-179    def do_delete(self, args: argshell.Namespace):
-180        """Delete rows from the database.
-181        Use the -t/--tables flag to limit what tables rows are deleted from.
-182        Use the -m/--match_pairs flag to specify which rows are deleted.
-183        Use the -p/--partial_matching flag to enable substring matching on -
+183    def do_delete(self, args: argshell.Namespace):
+184        """Delete rows from the database.
+185        Use the -t/--tables flag to limit what tables rows are deleted from.
+186        Use the -m/--match_pairs flag to specify which rows are deleted.
+187        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-184        >>> based>delete -t users -m username chungus -p
-185
-186        ^will delete all rows in the 'users' table whose username contains
+188        >>> based>delete -t users -m username chungus -p
+189
+190        ^will delete all rows in the 'users' table whose username contains
 'chungus'^"""
-187        print("Deleting records...")
-188        with DataBased(self.dbpath) as db:
-189            tables = args.tables or db.get_table_names()
-190            for table in tables:
-191                num_rows = db.delete(table, args.match_pairs, not
+191        print("Deleting records...")
+192        with DataBased(self.dbpath) as db:
+193            tables = args.tables or db.get_table_names()
+194            for table in tables:
+195                num_rows = db.delete(table, args.match_pairs, not
 args.partial_matching)
-192                print(f"Deleted {num_rows} rows from {table} table.")
+196                print(f"Deleted {num_rows} rows from {table} table.")
 Delete rows from the database. Use the -t/--tables flag to limit what tables
 rows are deleted from. Use the -m/--match_pairs flag to specify which rows are
 deleted. Use the -p/--partial_matching flag to enable substring matching on -m/
 --match_pairs.
 >>> based>delete -t users -m username chungus -p
 ^will delete all rows in the 'users' table whose username contains 'chungus'^
 ⁰
 @argshell.with_parser(dbparsers.get_add_column_parser)
 def do_add_column(self, args: argshell.argshell.Namespace): View Source
-194    @argshell.with_parser(dbparsers.get_add_column_parser)
-195    def do_add_column(self, args: argshell.Namespace):
-196        """Add a new column to the specified tables."""
-197        with DataBased(self.dbpath) as db:
-198            tables = args.tables or db.get_table_names()
-199            for table in tables:
-200                db.add_column(table, args.column_name, args.type,
+198    @argshell.with_parser(dbparsers.get_add_column_parser)
+199    def do_add_column(self, args: argshell.Namespace):
+200        """Add a new column to the specified tables."""
+201        with DataBased(self.dbpath) as db:
+202            tables = args.tables or db.get_table_names()
+203            for table in tables:
+204                db.add_column(table, args.column_name, args.type,
 args.default_value)
 Add a new column to the specified tables.
 ⁰
 def do_flush_log(self, arg: str): View Source
-202    def do_flush_log(self, arg: str):
-203        """Clear the log file for this database."""
-204        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-205        if not log_path.exists():
-206            print(f"No log file at path {log_path}")
-207        else:
-208            print(f"Flushing log...")
-209            log_path.write_text("")
+206    def do_flush_log(self, arg: str):
+207        """Clear the log file for this database."""
+208        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+209        if not log_path.exists():
+210            print(f"No log file at path {log_path}")
+211        else:
+212            print(f"Flushing log...")
+213            log_path.write_text("")
 Clear the log file for this database.
 ⁰
 def do_scan_dbs(self, arg: str): View Source
-211    def do_scan_dbs(self, arg: str):
-212        """Scan the current working directory for `*.db` files and display
+215    def do_scan_dbs(self, arg: str):
+216        """Scan the current working directory for `*.db` files and display
 them.
-213
-214        If the command is entered as `based>scan_dbs r`, the scan will be
+217
+218        If the command is entered as `based>scan_dbs r`, the scan will be
 performed recursively."""
-215        cwd = Pathier.cwd()
-216        if arg.strip() == "r":
-217            dbs = cwd.rglob("*.db")
-218        else:
-219            dbs = cwd.glob("*.db")
-220        for db in dbs:
-221            print(db.separate(cwd.stem))
+219        cwd = Pathier.cwd()
+220        if arg.strip() == "r":
+221            dbs = cwd.rglob("*.db")
+222        else:
+223            dbs = cwd.glob("*.db")
+224        for db in dbs:
+225            print(db.separate(cwd.stem))
 Scan the current working directory for *.db files and display them.
 If the command is entered as based>scan_dbs r, the scan will be performed
 recursively.
 ⁰
 def do_customize(self, arg: str): View Source
-223    def do_customize(self, arg: str):
-224        """Generate a template file in the current working directory for
+227    def do_customize(self, arg: str):
+228        """Generate a template file in the current working directory for
 creating a custom DBShell class.
-225        Expects one argument: the name of the custom dbshell.
-226        This will be used to name the generated file as well as several
+229        Expects one argument: the name of the custom dbshell.
+230        This will be used to name the generated file as well as several
 components in the file content."""
-227        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+231        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
 (".py")
-228        if custom_file.exists():
-229            print(f"Error: {custom_file.name} already exists in this
+232        if custom_file.exists():
+233            print(f"Error: {custom_file.name} already exists in this
 location.")
-230        else:
-231            variable_name = "_".join(word for word in arg.lower().split())
-232            class_name = "".join(word.capitalize() for word in arg.split())
-233            content = (Pathier(__file__).parent /
+234        else:
+235            variable_name = "_".join(word for word in arg.lower().split())
+236            class_name = "".join(word.capitalize() for word in arg.split())
+237            content = (Pathier(__file__).parent /
 "customshell.py").read_text()
-234            content = content.replace("CustomShell", class_name)
-235            content = content.replace("customshell", variable_name)
-236            custom_file.write_text(content)
+238            content = content.replace("CustomShell", class_name)
+239            content = content.replace("customshell", variable_name)
+240            custom_file.write_text(content)
 Generate a template file in the current working directory for creating a custom
 DBShell class. Expects one argument: the name of the custom dbshell. This will
 be used to name the generated file as well as several components in the file
 content.
 ⁰
 def do_vacuum(self, arg: str): View Source
-238    def do_vacuum(self, arg: str):
-239        """Reduce database disk memory."""
-240        starting_size = self.dbpath.size()
-241        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-242        print("Vacuuming database...")
-243        with DataBased(self.dbpath) as db:
-244            db.vacuum()
-245        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-246        print(f"Freed up {Pathier.format_size(starting_size -
+242    def do_vacuum(self, arg: str):
+243        """Reduce database disk memory."""
+244        starting_size = self.dbpath.size()
+245        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+246        print("Vacuuming database...")
+247        with DataBased(self.dbpath) as db:
+248            db.vacuum()
+249        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+250        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
 Reduce database disk memory.
 ⁰
 def preloop(self): View Source
-266    def preloop(self):
-267        """Scan the current directory for a .db file to use.
-268        If not found, prompt the user for one or to try again
+270    def preloop(self):
+271        """Scan the current directory for a .db file to use.
+272        If not found, prompt the user for one or to try again
 recursively."""
-269        if self.dbpath:
-270            self.dbpath = Pathier(self.dbpath)
-271            print(f"Defaulting to database {self.dbpath}")
-272        else:
-273            print("Searching for database...")
-274            cwd = Pathier.cwd()
-275            dbs = list(cwd.glob("*.db"))
-276            if len(dbs) == 1:
-277                self.dbpath = dbs[0]
-278                print(f"Using database {self.dbpath}.")
-279            elif dbs:
-280                self.dbpath = self._choose_db(dbs)
-281            else:
-282                print(f"Could not find a .db file in {cwd}.")
-283                path = input(
-284                    "Enter path to .db file to use or press enter to search
+273        if self.dbpath:
+274            self.dbpath = Pathier(self.dbpath)
+275            print(f"Defaulting to database {self.dbpath}")
+276        else:
+277            print("Searching for database...")
+278            cwd = Pathier.cwd()
+279            dbs = list(cwd.glob("*.db"))
+280            if len(dbs) == 1:
+281                self.dbpath = dbs[0]
+282                print(f"Using database {self.dbpath}.")
+283            elif dbs:
+284                self.dbpath = self._choose_db(dbs)
+285            else:
+286                print(f"Could not find a .db file in {cwd}.")
+287                path = input(
+288                    "Enter path to .db file to use or press enter to search
 again recursively: "
-285                )
-286                if path:
-287                    self.dbpath = Pathier(path)
-288                elif not path:
-289                    print("Searching recursively...")
-290                    dbs = list(cwd.rglob("*.db"))
-291                    if len(dbs) == 1:
-292                        self.dbpath = dbs[0]
-293                        print(f"Using database {self.dbpath}.")
-294                    elif dbs:
-295                        self.dbpath = self._choose_db(dbs)
-296                    else:
-297                        print("Could not find a .db file.")
-298                        self.dbpath = Pathier(input("Enter path to a .db
+289                )
+290                if path:
+291                    self.dbpath = Pathier(path)
+292                elif not path:
+293                    print("Searching recursively...")
+294                    dbs = list(cwd.rglob("*.db"))
+295                    if len(dbs) == 1:
+296                        self.dbpath = dbs[0]
+297                        print(f"Using database {self.dbpath}.")
+298                    elif dbs:
+299                        self.dbpath = self._choose_db(dbs)
+300                    else:
+301                        print("Could not find a .db file.")
+302                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-299        if not self.dbpath.exists():
-300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-301        if not self.dbpath.is_file():
-302            raise ValueError(f"{self.dbpath} is not a file.")
+303        if not self.dbpath.exists():
+304            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+305        if not self.dbpath.is_file():
+306            raise ValueError(f"{self.dbpath} is not a file.")
 Scan the current directory for a .db file to use. If not found, prompt the user
 for one or to try again recursively.
 ** Inherited Members **
   ⁰
 def main(): View Source
-305def main():
-306    DBShell().cmdloop()
+309def main():
+310    DBShell().cmdloop()
```

### Comparing `databased-2.3.0/src/databased/customshell.py` & `databased-2.4.0/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/src/databased/databased.py` & `databased-2.4.0/src/databased/databased.py`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/src/databased/dbparsers.py` & `databased-2.4.0/src/databased/dbparsers.py`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/src/databased/dbshell.py` & `databased-2.4.0/src/databased/dbshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argshell
+from griddle import griddy
 from pathier import Pathier
 
 from databased import DataBased, dbparsers
 
 
 class DBShell(argshell.ArgShell):
     intro = "Starting dbshell (enter help or ? for arg info)..."
@@ -141,19 +142,22 @@
 
     def do_query(self, arg: str):
         """Execute a query against the current database."""
         print(f"Executing {arg}")
         with DataBased(self.dbpath) as db:
             results = db.query(arg)
         try:
-            for result in results:
-                print(*result, sep="|-|")
-            print(f"{db.cursor.rowcount} affected rows")
+            try:
+                print(griddy(results))
+            except Exception as e:
+                for result in results:
+                    print(*result, sep="|-|")
         except Exception as e:
             print(f"{type(e).__name__}: {e}")
+        print(f"{db.cursor.rowcount} affected rows")
 
     @argshell.with_parser(dbparsers.get_update_parser, [dbparsers.convert_match_pairs])
     def do_update(self, args: argshell.Namespace):
         """Update a column to a new value.
         Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.
         Use the -t/--tables flag to limit what tables are updated.
         Use the -m/--match_pairs flag to specify which rows are updated.
```

### Comparing `databased-2.3.0/LICENSE.txt` & `databased-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/README.md` & `databased-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `databased-2.3.0/pyproject.toml` & `databased-2.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "2.3.0"
+version = "2.4.0"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier", "griddle"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
```

### Comparing `databased-2.3.0/PKG-INFO` & `databased-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 2.3.0
+Version: 2.4.0
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

