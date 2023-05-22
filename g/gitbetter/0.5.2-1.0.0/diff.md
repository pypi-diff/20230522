# Comparing `tmp/gitbetter-0.5.2.tar.gz` & `tmp/gitbetter-1.0.0.tar.gz`

## Comparing `gitbetter-0.5.2.tar` & `gitbetter-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 gitbetter-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/index.html
--rw-r--r--   0        0        0    57989 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/search.js
--rw-r--r--   0        0        0   138514 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter/git.html
--rw-r--r--   0        0        0   248978 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/git.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.5.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 gitbetter-0.5.2/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 gitbetter-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 gitbetter-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/index.html
+-rw-r--r--   0        0        0    63165 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/search.js
+-rw-r--r--   0        0        0   224647 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 gitbetter-1.0.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 gitbetter-1.0.0/PKG-INFO
```

### Comparing `gitbetter-0.5.2/CHANGELOG.md` & `gitbetter-1.0.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
-## 0.5.1 (2023-05-13)
+## v0.5.2 (2023-05-15)
+
+#### Fixes
+
+* fix create_remote_from_cwd function to properly add remote and push
+
+
+## v0.5.1 (2023-05-13)
 
 #### Fixes
 
 * fix  create_remote_from_cwd() not setting remote to upstream
+#### Others
+
+* build v0.5.1
+* update changelog
 
 
 ## v0.5.0 (2023-05-11)
 
 #### New Features
 
 * add create_remote_from_cwd()
```

### Comparing `gitbetter-0.5.2/docs/gitbetter.html` & `gitbetter-1.0.0/docs/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 gitbetter    </h1>
 
                 
                         <input id="mod-gitbetter-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-gitbetter-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">git</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">gitbetter.git</span> <span class="kn">import</span> <span class="n">Git</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -5,9 +5,9 @@
 ***** Submodules *****
     * git
     * gitbetter
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter ******
 ⁰ View Source
-1from gitbetter import git
+1from gitbetter.git import Git
```

### Comparing `gitbetter-0.5.2/docs/search.js` & `gitbetter-1.0.0/docs/search.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -689,236 +689,256 @@
         "doc": "<p></p>\n"
     }, {
         "fullname": "gitbetter.git",
         "modulename": "gitbetter.git",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
-        "fullname": "gitbetter.git.execute",
+        "fullname": "gitbetter.git.Git",
         "modulename": "gitbetter.git",
-        "qualname": "execute",
+        "qualname": "Git",
+        "kind": "class",
+        "doc": "<p></p>\n"
+    }, {
+        "fullname": "gitbetter.git.Git.__init__",
+        "modulename": "gitbetter.git",
+        "qualname": "Git.__init__",
+        "kind": "function",
+        "doc": "<p>If <code>capture_stdout</code> is <code>True</code>, all functions will return their generated <code>stdout</code> as a string.\nOtherwise, the functions return the call's exit code.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">capture_stdout</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span>)</span>"
+    }, {
+        "fullname": "gitbetter.git.Git.capture_stdout",
+        "modulename": "gitbetter.git",
+        "qualname": "Git.capture_stdout",
+        "kind": "variable",
+        "doc": "<p>If <code>True</code>, member functions will return the generated <code>stdout</code> as a string,\notherwise they return the command's exit code.</p>\n",
+        "annotation": ": bool"
+    }, {
+        "fullname": "gitbetter.git.Git.execute",
+        "modulename": "gitbetter.git",
+        "qualname": "Git.execute",
         "kind": "function",
-        "doc": "<p>Execute git command.</p>\n\n<p>Equivalent to <code>os.system(f\"git {command}\")</code></p>\n\n<p>Returns the output of the <code>os.system</code> call.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">command</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
+        "doc": "<p>Execute git command.</p>\n\n<p>Equivalent to executing <code>git {command}</code> in the shell.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">command</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.new_repo",
+        "fullname": "gitbetter.git.Git.new_repo",
         "modulename": "gitbetter.git",
-        "qualname": "new_repo",
+        "qualname": "Git.new_repo",
         "kind": "function",
-        "doc": "<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">init</span> <span class=\"o\">-</span><span class=\"n\">b</span> <span class=\"n\">main</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Executes <code>git init -b main</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.loggy",
+        "fullname": "gitbetter.git.Git.loggy",
         "modulename": "gitbetter.git",
-        "qualname": "loggy",
+        "qualname": "Git.loggy",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git log --oneline --name-only --abbrev-commit --graph</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.status",
+        "fullname": "gitbetter.git.Git.status",
         "modulename": "gitbetter.git",
-        "qualname": "status",
+        "qualname": "Git.status",
         "kind": "function",
         "doc": "<p>Execute <code>git status</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.commit",
+        "fullname": "gitbetter.git.Git.commit",
         "modulename": "gitbetter.git",
-        "qualname": "commit",
+        "qualname": "Git.commit",
         "kind": "function",
         "doc": "<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">commit</span> <span class=\"p\">{</span><span class=\"n\">args</span><span class=\"p\">}</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.add",
+        "fullname": "gitbetter.git.Git.add",
         "modulename": "gitbetter.git",
-        "qualname": "add",
+        "qualname": "Git.add",
         "kind": "function",
         "doc": "<p>Stage a list of files.</p>\n\n<p>If no files are given (<code>files=None</code>), all files will be staged.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.commit_files",
+        "fullname": "gitbetter.git.Git.commit_files",
         "modulename": "gitbetter.git",
-        "qualname": "commit_files",
+        "qualname": "Git.commit_files",
         "kind": "function",
         "doc": "<p>Stage and commit a list of files with commit message <code>message</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>, </span><span class=\"param\"><span class=\"n\">message</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>, </span><span class=\"param\"><span class=\"n\">message</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.initcommit",
+        "fullname": "gitbetter.git.Git.initcommit",
         "modulename": "gitbetter.git",
-        "qualname": "initcommit",
+        "qualname": "Git.initcommit",
         "kind": "function",
         "doc": "<p>Equivalent to</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">add</span> <span class=\"o\">.</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">commit</span> <span class=\"o\">-</span><span class=\"n\">m</span> <span class=\"s2\">&quot;Initial commit&quot;</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.amend",
+        "fullname": "gitbetter.git.Git.amend",
         "modulename": "gitbetter.git",
-        "qualname": "amend",
+        "qualname": "Git.amend",
         "kind": "function",
         "doc": "<p>Stage and commit changes to the previous commit.</p>\n\n<p>If <code>files</code> is <code>None</code>, all files will be staged.</p>\n\n<p>Equivalent to:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">add</span> <span class=\"p\">{</span><span class=\"n\">files</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">commit</span> <span class=\"o\">--</span><span class=\"n\">amend</span> <span class=\"o\">--</span><span class=\"n\">no</span><span class=\"o\">-</span><span class=\"n\">edit</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.tag",
+        "fullname": "gitbetter.git.Git.tag",
         "modulename": "gitbetter.git",
-        "qualname": "tag",
+        "qualname": "Git.tag",
         "kind": "function",
         "doc": "<p>Tag the current commit with <code>id_</code>.</p>\n\n<p>Equivalent to <code>git tag {id_}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">id_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">id_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.add_remote_url",
+        "fullname": "gitbetter.git.Git.add_remote_url",
         "modulename": "gitbetter.git",
-        "qualname": "add_remote_url",
+        "qualname": "Git.add_remote_url",
         "kind": "function",
         "doc": "<p>Add remote url to repo.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">url</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;origin&#39;</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">url</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;origin&#39;</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.push",
+        "fullname": "gitbetter.git.Git.push",
         "modulename": "gitbetter.git",
-        "qualname": "push",
+        "qualname": "Git.push",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git push {args}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.pull",
+        "fullname": "gitbetter.git.Git.pull",
         "modulename": "gitbetter.git",
-        "qualname": "pull",
+        "qualname": "Git.pull",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git pull {args}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.push_new_branch",
+        "fullname": "gitbetter.git.Git.push_new_branch",
         "modulename": "gitbetter.git",
-        "qualname": "push_new_branch",
+        "qualname": "Git.push_new_branch",
         "kind": "function",
         "doc": "<p>Push a new branch to origin with tracking.</p>\n\n<p>Equivalent to <code>git push -u origin {branch}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.pull_branch",
+        "fullname": "gitbetter.git.Git.pull_branch",
         "modulename": "gitbetter.git",
-        "qualname": "pull_branch",
+        "qualname": "Git.pull_branch",
         "kind": "function",
         "doc": "<p>Pull <code>branch</code> from origin.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.branch",
+        "fullname": "gitbetter.git.Git.branch",
         "modulename": "gitbetter.git",
-        "qualname": "branch",
+        "qualname": "Git.branch",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git branch {args}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.list_branches",
+        "fullname": "gitbetter.git.Git.list_branches",
         "modulename": "gitbetter.git",
-        "qualname": "list_branches",
+        "qualname": "Git.list_branches",
         "kind": "function",
         "doc": "<p>Print a list of branches.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.checkout",
+        "fullname": "gitbetter.git.Git.checkout",
         "modulename": "gitbetter.git",
-        "qualname": "checkout",
+        "qualname": "Git.checkout",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git checkout {args}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.switch_branch",
+        "fullname": "gitbetter.git.Git.switch_branch",
         "modulename": "gitbetter.git",
-        "qualname": "switch_branch",
+        "qualname": "Git.switch_branch",
         "kind": "function",
         "doc": "<p>Switch to the branch specified by <code>branch_name</code>.</p>\n\n<p>Equivalent to <code>git checkout {branch_name}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.create_new_branch",
+        "fullname": "gitbetter.git.Git.create_new_branch",
         "modulename": "gitbetter.git",
-        "qualname": "create_new_branch",
+        "qualname": "Git.create_new_branch",
         "kind": "function",
         "doc": "<p>Create and switch to a new branch named with <code>branch_name</code>.</p>\n\n<p>Equivalent to <code>git checkout -b {branch_name} --track</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.delete_branch",
+        "fullname": "gitbetter.git.Git.delete_branch",
         "modulename": "gitbetter.git",
-        "qualname": "delete_branch",
+        "qualname": "Git.delete_branch",
         "kind": "function",
         "doc": "<p>Delete <code>branch_name</code> from repo.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>local_only</code>: Only delete the local copy of <code>branch</code>, otherwise also delete the remote branch on origin and remote-tracking branch.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">local_only</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">local_only</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.undo",
+        "fullname": "gitbetter.git.Git.undo",
         "modulename": "gitbetter.git",
-        "qualname": "undo",
+        "qualname": "Git.undo",
         "kind": "function",
         "doc": "<p>Undo uncommitted changes.</p>\n\n<p>Equivalent to <code>git checkout .</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.merge",
+        "fullname": "gitbetter.git.Git.merge",
         "modulename": "gitbetter.git",
-        "qualname": "merge",
+        "qualname": "Git.merge",
         "kind": "function",
         "doc": "<p>Merge branch <code>branch_name</code> with currently active branch.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.create_remote",
+        "fullname": "gitbetter.git.Git.create_remote",
         "modulename": "gitbetter.git",
-        "qualname": "create_remote",
+        "qualname": "Git.create_remote",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>name</code>: The name for the repo.</p>\n\n<p><code>public</code>: Set to <code>True</code> to create the repo as public, otherwise it'll be created as private.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.create_remote_from_cwd",
+        "fullname": "gitbetter.git.Git.create_remote_from_cwd",
         "modulename": "gitbetter.git",
-        "qualname": "create_remote_from_cwd",
+        "qualname": "Git.create_remote_from_cwd",
         "kind": "function",
         "doc": "<p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from\nthe current working directory repo and add its url as this repo's remote origin.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>public</code>: Create the GitHub repo as a public repo, default is to create it as private.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.make_private",
+        "fullname": "gitbetter.git.Git.make_private",
         "modulename": "gitbetter.git",
-        "qualname": "make_private",
+        "qualname": "Git.make_private",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>owner</code>: The repo owner.</p>\n\n<p><code>name</code>: The name of the repo to edit.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.make_public",
+        "fullname": "gitbetter.git.Git.make_public",
         "modulename": "gitbetter.git",
-        "qualname": "make_public",
+        "qualname": "Git.make_public",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>owner</code>: The repo owner.</p>\n\n<p><code>name</code>: The name of the repo to edit.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.git.delete_remote",
+        "fullname": "gitbetter.git.Git.delete_remote",
         "modulename": "gitbetter.git",
-        "qualname": "delete_remote",
+        "qualname": "Git.delete_remote",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>owner</code>: The repo owner.</p>\n\n<p><code>name</code>: The name of the remote repo to delete.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter",
         "modulename": "gitbetter.gitbetter",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
@@ -1065,16 +1085,16 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_commit",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_commit",
         "kind": "function",
-        "doc": "<p>Commit staged files with this message.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">message</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Commit staged files with provided <code>args</code> string.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_commitf",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_commitf",
         "kind": "function",
         "doc": "<p>Stage and commit a list of files.</p>\n",
```

### Comparing `gitbetter-0.5.2/docs/gitbetter/gitbetter.html` & `gitbetter-1.0.0/docs/gitbetter/gitbetter.html`

 * *Files 7% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                         <label class="view-source-button" for="mod-gitbetter-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">argshell</span> <span class="kn">import</span> <span class="n">ArgShell</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">,</span> <span class="n">with_parser</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">git</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">Git</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="k">def</span> <span class="nf">new_remote_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>        <span class="s2">&quot;--public&quot;</span><span class="p">,</span>
 </span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
@@ -271,206 +271,203 @@
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
 </span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
 </span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
 </span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
 </span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
 </span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="p">)</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="nd">@property</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="p">)</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                <span class="p">)</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="nd">@property</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="p">)</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
 </span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
 </span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
 </span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
 </span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
 </span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -664,198 +661,195 @@
     <a class="headerlink" href="#GitBetter"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter-100"><a href="#GitBetter-100"><span class="linenos">100</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
 </span><span id="GitBetter-101"><a href="#GitBetter-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
 </span><span id="GitBetter-102"><a href="#GitBetter-102"><span class="linenos">102</span></a>
 </span><span id="GitBetter-103"><a href="#GitBetter-103"><span class="linenos">103</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
 </span><span id="GitBetter-104"><a href="#GitBetter-104"><span class="linenos">104</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
 </span><span id="GitBetter-105"><a href="#GitBetter-105"><span class="linenos">105</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>
-</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>
-</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                <span class="p">)</span>
-</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
-</span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>
-</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>    <span class="nd">@property</span>
-</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>
-</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>        <span class="p">)</span>
-</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a>
-</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
-</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>
-</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>
-</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a>
-</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
-</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a>
-</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>
-</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>
-</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>
-</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>
-</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>
-</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>
-</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>
-</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>
-</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>
-</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>
-</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>
-</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>    <span class="n">git</span> <span class="o">=</span> <span class="n">Git</span><span class="p">()</span>
+</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>
+</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>
+</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>                <span class="p">)</span>
+</span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>
+</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>    <span class="nd">@property</span>
+</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>
+</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>        <span class="p">)</span>
+</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>
+</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>
+</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a>
+</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>
+</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>
+</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>
+</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a>
+</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>
+</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>
+</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>
+</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>
+</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>
+</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>
+</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>
+</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>
+</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>
+</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>
+</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
 </span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>
-</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>
-</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
 </span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>
-</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>
-</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>
-</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>
-</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>
-</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>
-</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>
-</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>
-</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>
-</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>
-</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>
-</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>
+</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>
+</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>
+</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>
+</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>
+</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>
+</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>
+</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>
+</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>
+</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
 </span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>
-</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>
-</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>
+</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a>
-</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
 </span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>
-</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>
-</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>
+</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a>
-</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
 </span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>
-</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>
-</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a>
-</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a>
-</span><span id="GitBetter-288"><a href="#GitBetter-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-289"><a href="#GitBetter-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>
+</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a>
+</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
@@ -866,19 +860,19 @@
         <span class="def">def</span>
         <span class="name">default</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">line</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.default-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.default"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.default-107"><a href="#GitBetter.default-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.default-108"><a href="#GitBetter.default-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter.default-109"><a href="#GitBetter.default-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="GitBetter.default-110"><a href="#GitBetter.default-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="GitBetter.default-111"><a href="#GitBetter.default-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.default-108"><a href="#GitBetter.default-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.default-109"><a href="#GitBetter.default-109"><span class="linenos">109</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.default-110"><a href="#GitBetter.default-110"><span class="linenos">110</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter.default-111"><a href="#GitBetter.default-111"><span class="linenos">111</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter.default-112"><a href="#GitBetter.default-112"><span class="linenos">112</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Called on an input line when the command prefix is not recognized.</p>
 
 <p>If this method is not overridden, it prints an error message and
 returns.</p>
@@ -893,24 +887,24 @@
         <span class="def">def</span>
         <span class="name">do_help</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_help-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_help"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_help-113"><a href="#GitBetter.do_help-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_help-114"><a href="#GitBetter.do_help-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_help-115"><a href="#GitBetter.do_help-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="GitBetter.do_help-116"><a href="#GitBetter.do_help-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="GitBetter.do_help-117"><a href="#GitBetter.do_help-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
-</span><span id="GitBetter.do_help-118"><a href="#GitBetter.do_help-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
-</span><span id="GitBetter.do_help-119"><a href="#GitBetter.do_help-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
-</span><span id="GitBetter.do_help-120"><a href="#GitBetter.do_help-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
-</span><span id="GitBetter.do_help-121"><a href="#GitBetter.do_help-121"><span class="linenos">121</span></a>                <span class="p">)</span>
-</span><span id="GitBetter.do_help-122"><a href="#GitBetter.do_help-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_help-114"><a href="#GitBetter.do_help-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_help-115"><a href="#GitBetter.do_help-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_help-116"><a href="#GitBetter.do_help-116"><span class="linenos">116</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-117"><a href="#GitBetter.do_help-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-118"><a href="#GitBetter.do_help-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-119"><a href="#GitBetter.do_help-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-120"><a href="#GitBetter.do_help-120"><span class="linenos">120</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter.do_help-121"><a href="#GitBetter.do_help-121"><span class="linenos">121</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter.do_help-122"><a href="#GitBetter.do_help-122"><span class="linenos">122</span></a>                <span class="p">)</span>
+</span><span id="GitBetter.do_help-123"><a href="#GitBetter.do_help-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>List available commands with "help" or detailed help with "help cmd".</p>
 </div>
 
 
@@ -922,22 +916,22 @@
         <span class="def">def</span>
         <span class="name">do_toggle_unrecognized_command_behavior</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_toggle_unrecognized_command_behavior-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_toggle_unrecognized_command_behavior"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_toggle_unrecognized_command_behavior-128"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-129"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-130"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-131"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-132"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-133"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-134"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-134"><span class="linenos">134</span></a>        <span class="p">)</span>
-</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-135"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_toggle_unrecognized_command_behavior-129"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-130"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-131"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-131"><span class="linenos">131</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-132"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-132"><span class="linenos">132</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-133"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-134"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-134"><span class="linenos">134</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-135"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-135"><span class="linenos">135</span></a>        <span class="p">)</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-136"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.
 When on (the default), <code><a href="#GitBetter">GitBetter</a></code> will treat unrecognized commands as if you added the <code>sys</code> command in front of the input, i.e. <code>os.system(your_input)</code>.
 When off, an <code>unknown syntax</code> message will be printed and no commands will be executed.</p>
 </div>
@@ -951,18 +945,18 @@
         <span class="def">def</span>
         <span class="name">do_cd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_cd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_cd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-137"><a href="#GitBetter.do_cd-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_cd-138"><a href="#GitBetter.do_cd-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_cd-139"><a href="#GitBetter.do_cd-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="GitBetter.do_cd-140"><a href="#GitBetter.do_cd-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-138"><a href="#GitBetter.do_cd-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_cd-139"><a href="#GitBetter.do_cd-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_cd-140"><a href="#GitBetter.do_cd-140"><span class="linenos">140</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter.do_cd-141"><a href="#GitBetter.do_cd-141"><span class="linenos">141</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Change current working directory to <code>path</code>.</p>
 </div>
 
 
@@ -974,19 +968,19 @@
         <span class="def">def</span>
         <span class="name">do_git</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_git-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_git"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-142"><a href="#GitBetter.do_git-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_git-143"><a href="#GitBetter.do_git-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter.do_git-144"><a href="#GitBetter.do_git-144"><span class="linenos">144</span></a>
-</span><span id="GitBetter.do_git-145"><a href="#GitBetter.do_git-145"><span class="linenos">145</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_git-146"><a href="#GitBetter.do_git-146"><span class="linenos">146</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-143"><a href="#GitBetter.do_git-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_git-144"><a href="#GitBetter.do_git-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter.do_git-145"><a href="#GitBetter.do_git-145"><span class="linenos">145</span></a>
+</span><span id="GitBetter.do_git-146"><a href="#GitBetter.do_git-146"><span class="linenos">146</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_git-147"><a href="#GitBetter.do_git-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Directly execute <code>git {arg}</code>.</p>
 
 <p>i.e. You can still do everything directly invoking git can do.</p>
 </div>
@@ -1000,17 +994,17 @@
         <span class="def">def</span>
         <span class="name">do_new_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-148"><a href="#GitBetter.do_new_repo-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_repo-149"><a href="#GitBetter.do_new_repo-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_repo-150"><a href="#GitBetter.do_new_repo-150"><span class="linenos">150</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-149"><a href="#GitBetter.do_new_repo-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_repo-150"><a href="#GitBetter.do_new_repo-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_repo-151"><a href="#GitBetter.do_new_repo-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a new git repo in this directory.</p>
 </div>
 
 
@@ -1022,17 +1016,17 @@
         <span class="def">def</span>
         <span class="name">do_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-152"><a href="#GitBetter.do_new_branch-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_branch-153"><a href="#GitBetter.do_new_branch-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_branch-154"><a href="#GitBetter.do_new_branch-154"><span class="linenos">154</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-153"><a href="#GitBetter.do_new_branch-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_branch-154"><a href="#GitBetter.do_new_branch-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_branch-155"><a href="#GitBetter.do_new_branch-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named after the supplied arg.</p>
 </div>
 
 
@@ -1045,20 +1039,20 @@
         <span class="def">def</span>
         <span class="name">do_new_gh_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_gh_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_gh_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-156"><a href="#GitBetter.do_new_gh_remote-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_new_gh_remote-157"><a href="#GitBetter.do_new_gh_remote-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_gh_remote-158"><a href="#GitBetter.do_new_gh_remote-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter.do_new_gh_remote-159"><a href="#GitBetter.do_new_gh_remote-159"><span class="linenos">159</span></a>
-</span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-157"><a href="#GitBetter.do_new_gh_remote-157"><span class="linenos">157</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_new_gh_remote-158"><a href="#GitBetter.do_new_gh_remote-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_gh_remote-159"><a href="#GitBetter.do_new_gh_remote-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a>
+</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_gh_remote-162"><a href="#GitBetter.do_new_gh_remote-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a remote GitHub repository for this repo.</p>
 
 <p>GitHub CLI must be installed and configured for this to work.</p>
 </div>
@@ -1072,17 +1066,17 @@
         <span class="def">def</span>
         <span class="name">do_initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-163"><a href="#GitBetter.do_initcommit-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_initcommit-164"><a href="#GitBetter.do_initcommit-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-164"><a href="#GitBetter.do_initcommit-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_initcommit-166"><a href="#GitBetter.do_initcommit-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with message "Initial Commit".</p>
 </div>
 
 
@@ -1094,17 +1088,17 @@
         <span class="def">def</span>
         <span class="name">do_undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-167"><a href="#GitBetter.do_undo-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_undo-168"><a href="#GitBetter.do_undo-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-168"><a href="#GitBetter.do_undo-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_undo-170"><a href="#GitBetter.do_undo-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo all uncommitted changes.</p>
 </div>
 
 
@@ -1117,50 +1111,46 @@
         <span class="def">def</span>
         <span class="name">do_add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-171"><a href="#GitBetter.do_add-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_add-172"><a href="#GitBetter.do_add-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-172"><a href="#GitBetter.do_add-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add-176"><a href="#GitBetter.do_add-176"><span class="linenos">176</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.
 If no files are given, all files will be added.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_commit" class="classattr">
                                         <input id="GitBetter.do_commit-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">do_commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+        <span class="name">do_commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-177"><a href="#GitBetter.do_commit-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-178"><a href="#GitBetter.do_commit-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commit-181"><a href="#GitBetter.do_commit-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-182"><a href="#GitBetter.do_commit-182"><span class="linenos">182</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commit-183"><a href="#GitBetter.do_commit-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-178"><a href="#GitBetter.do_commit-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with provided `args` string.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Commit staged files with this message.</p>
+            <div class="docstring"><p>Commit staged files with provided <code>args</code> string.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_commitf" class="classattr">
                                         <input id="GitBetter.do_commitf-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1169,18 +1159,18 @@
         <span class="def">def</span>
         <span class="name">do_commitf</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitf-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitf"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-185"><a href="#GitBetter.do_commitf-185"><span class="linenos">185</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_commitf-186"><a href="#GitBetter.do_commitf-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitf-187"><a href="#GitBetter.do_commitf-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitf-188"><a href="#GitBetter.do_commitf-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-182"><a href="#GitBetter.do_commitf-182"><span class="linenos">182</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_commitf-183"><a href="#GitBetter.do_commitf-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitf-184"><a href="#GitBetter.do_commitf-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitf-185"><a href="#GitBetter.do_commitf-185"><span class="linenos">185</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files.</p>
 </div>
 
 
@@ -1192,22 +1182,22 @@
         <span class="def">def</span>
         <span class="name">do_commitall</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitall-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitall"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-190"><a href="#GitBetter.do_commitall-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-195"><a href="#GitBetter.do_commitall-195"><span class="linenos">195</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commitall-196"><a href="#GitBetter.do_commitall-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter.do_commitall-197"><a href="#GitBetter.do_commitall-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-187"><a href="#GitBetter.do_commitall-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-188"><a href="#GitBetter.do_commitall-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitall-189"><a href="#GitBetter.do_commitall-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-190"><a href="#GitBetter.do_commitall-190"><span class="linenos">190</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with this message.</p>
 </div>
 
 
@@ -1219,17 +1209,17 @@
         <span class="def">def</span>
         <span class="name">do_switch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_switch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_switch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-199"><a href="#GitBetter.do_switch-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_switch-200"><a href="#GitBetter.do_switch-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_switch-201"><a href="#GitBetter.do_switch-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-196"><a href="#GitBetter.do_switch-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_switch-197"><a href="#GitBetter.do_switch-197"><span class="linenos">197</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_switch-198"><a href="#GitBetter.do_switch-198"><span class="linenos">198</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to this branch.</p>
 </div>
 
 
@@ -1241,18 +1231,18 @@
         <span class="def">def</span>
         <span class="name">do_add_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-203"><a href="#GitBetter.do_add_url-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_add_url-204"><a href="#GitBetter.do_add_url-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add_url-205"><a href="#GitBetter.do_add_url-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter.do_add_url-206"><a href="#GitBetter.do_add_url-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-200"><a href="#GitBetter.do_add_url-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_add_url-201"><a href="#GitBetter.do_add_url-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add_url-202"><a href="#GitBetter.do_add_url-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter.do_add_url-203"><a href="#GitBetter.do_add_url-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote origin url for repo and push repo.</p>
 </div>
 
 
@@ -1264,17 +1254,17 @@
         <span class="def">def</span>
         <span class="name">do_push_new</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push_new-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push_new"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-208"><a href="#GitBetter.do_push_new-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push_new-209"><a href="#GitBetter.do_push_new-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push_new-210"><a href="#GitBetter.do_push_new-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-205"><a href="#GitBetter.do_push_new-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push_new-206"><a href="#GitBetter.do_push_new-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push_new-207"><a href="#GitBetter.do_push_new-207"><span class="linenos">207</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push this new branch to origin with -u flag.</p>
 </div>
 
 
@@ -1286,19 +1276,19 @@
         <span class="def">def</span>
         <span class="name">do_push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-212"><a href="#GitBetter.do_push-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter.do_push-214"><a href="#GitBetter.do_push-214"><span class="linenos">214</span></a>
-</span><span id="GitBetter.do_push-215"><a href="#GitBetter.do_push-215"><span class="linenos">215</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push-216"><a href="#GitBetter.do_push-216"><span class="linenos">216</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-209"><a href="#GitBetter.do_push-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push-210"><a href="#GitBetter.do_push-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter.do_push-211"><a href="#GitBetter.do_push-211"><span class="linenos">211</span></a>
+</span><span id="GitBetter.do_push-212"><a href="#GitBetter.do_push-212"><span class="linenos">212</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git push</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git push</code> accepts.</p>
 </div>
@@ -1312,19 +1302,19 @@
         <span class="def">def</span>
         <span class="name">do_pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-218"><a href="#GitBetter.do_pull-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter.do_pull-220"><a href="#GitBetter.do_pull-220"><span class="linenos">220</span></a>
-</span><span id="GitBetter.do_pull-221"><a href="#GitBetter.do_pull-221"><span class="linenos">221</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull-222"><a href="#GitBetter.do_pull-222"><span class="linenos">222</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-215"><a href="#GitBetter.do_pull-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull-216"><a href="#GitBetter.do_pull-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter.do_pull-217"><a href="#GitBetter.do_pull-217"><span class="linenos">217</span></a>
+</span><span id="GitBetter.do_pull-218"><a href="#GitBetter.do_pull-218"><span class="linenos">218</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git pull</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git pull</code> accepts.</p>
 </div>
@@ -1338,17 +1328,17 @@
         <span class="def">def</span>
         <span class="name">do_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_branches-224"><a href="#GitBetter.do_branches-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_branches-225"><a href="#GitBetter.do_branches-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_branches-226"><a href="#GitBetter.do_branches-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_branches-221"><a href="#GitBetter.do_branches-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_branches-222"><a href="#GitBetter.do_branches-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_branches-223"><a href="#GitBetter.do_branches-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Show local and remote branches.</p>
 </div>
 
 
@@ -1360,17 +1350,17 @@
         <span class="def">def</span>
         <span class="name">do_loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-228"><a href="#GitBetter.do_loggy-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_loggy-229"><a href="#GitBetter.do_loggy-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_loggy-230"><a href="#GitBetter.do_loggy-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-225"><a href="#GitBetter.do_loggy-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_loggy-226"><a href="#GitBetter.do_loggy-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_loggy-227"><a href="#GitBetter.do_loggy-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -1382,17 +1372,17 @@
         <span class="def">def</span>
         <span class="name">do_status</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_status-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_status"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-232"><a href="#GitBetter.do_status-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_status-233"><a href="#GitBetter.do_status-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_status-234"><a href="#GitBetter.do_status-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-229"><a href="#GitBetter.do_status-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_status-230"><a href="#GitBetter.do_status-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_status-231"><a href="#GitBetter.do_status-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git status</code>.</p>
 </div>
 
 
@@ -1404,17 +1394,17 @@
         <span class="def">def</span>
         <span class="name">do_merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-236"><a href="#GitBetter.do_merge-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_merge-237"><a href="#GitBetter.do_merge-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_merge-238"><a href="#GitBetter.do_merge-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-233"><a href="#GitBetter.do_merge-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_merge-234"><a href="#GitBetter.do_merge-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_merge-235"><a href="#GitBetter.do_merge-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge supplied <code>branch_name</code> with the currently active branch.</p>
 </div>
 
 
@@ -1426,17 +1416,17 @@
         <span class="def">def</span>
         <span class="name">do_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-240"><a href="#GitBetter.do_tag-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_tag-241"><a href="#GitBetter.do_tag-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_tag-242"><a href="#GitBetter.do_tag-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-237"><a href="#GitBetter.do_tag-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_tag-238"><a href="#GitBetter.do_tag-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_tag-239"><a href="#GitBetter.do_tag-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag current commit with <code>tag_id</code>.</p>
 </div>
 
 
@@ -1449,18 +1439,18 @@
         <span class="def">def</span>
         <span class="name">do_amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_amend-246"><a href="#GitBetter.do_amend-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_amend-247"><a href="#GitBetter.do_amend-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-241"><a href="#GitBetter.do_amend-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_amend-242"><a href="#GitBetter.do_amend-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_amend-243"><a href="#GitBetter.do_amend-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage files and add to previous commit.</p>
 </div>
 
 
@@ -1473,18 +1463,18 @@
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-251"><a href="#GitBetter.do_delete_branch-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-252"><a href="#GitBetter.do_delete_branch-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-246"><a href="#GitBetter.do_delete_branch-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-247"><a href="#GitBetter.do_delete_branch-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-248"><a href="#GitBetter.do_delete_branch-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -1496,17 +1486,17 @@
         <span class="def">def</span>
         <span class="name">do_pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-254"><a href="#GitBetter.do_pull_branch-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull_branch-255"><a href="#GitBetter.do_pull_branch-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull_branch-256"><a href="#GitBetter.do_pull_branch-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-251"><a href="#GitBetter.do_pull_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull_branch-252"><a href="#GitBetter.do_pull_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull_branch-253"><a href="#GitBetter.do_pull_branch-253"><span class="linenos">253</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull this branch from the origin.</p>
 </div>
 
 
@@ -1518,20 +1508,20 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-262"><a href="#GitBetter.do_ignore-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-263"><a href="#GitBetter.do_ignore-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-255"><a href="#GitBetter.do_ignore-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-256"><a href="#GitBetter.do_ignore-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-257"><a href="#GitBetter.do_ignore-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns to <code>.gitignore</code>.</p>
 </div>
 
 
@@ -1543,21 +1533,21 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>
-</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a>
-</span><span id="GitBetter.do_make_private-270"><a href="#GitBetter.do_make_private-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-271"><a href="#GitBetter.do_make_private-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-262"><a href="#GitBetter.do_make_private-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-263"><a href="#GitBetter.do_make_private-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-264"><a href="#GitBetter.do_make_private-264"><span class="linenos">264</span></a>
+</span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>
+</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1573,21 +1563,21 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>
-</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a>
-</span><span id="GitBetter.do_make_public-278"><a href="#GitBetter.do_make_public-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-279"><a href="#GitBetter.do_make_public-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-270"><a href="#GitBetter.do_make_public-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-271"><a href="#GitBetter.do_make_public-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-272"><a href="#GitBetter.do_make_public-272"><span class="linenos">272</span></a>
+</span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>
+</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1603,23 +1593,23 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-288"><a href="#GitBetter.do_delete_gh_repo-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-289"><a href="#GitBetter.do_delete_gh_repo-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-278"><a href="#GitBetter.do_delete_gh_repo-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-279"><a href="#GitBetter.do_delete_gh_repo-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter.do_delete_gh_repo-280"><a href="#GitBetter.do_delete_gh_repo-280"><span class="linenos">280</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1667,16 +1657,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-292"><a href="#main-292"><span class="linenos">292</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-293"><a href="#main-293"><span class="linenos">293</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-289"><a href="#main-289"><span class="linenos">289</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-290"><a href="#main-290"><span class="linenos">290</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -47,15 +47,15 @@
 ****** gitbetter.gitbetter ******
 ⁰ View Source
 __1import os
 __2
 __3from argshell import ArgShell, ArgShellParser, Namespace, with_parser
 __4from pathier import Pathier
 __5
-__6from gitbetter import git
+__6from gitbetter import Git
 __7
 __8
 __9def new_remote_parser() -> ArgShellParser:
 _10    parser = ArgShellParser()
 _11    parser.add_argument(
 _12        "--public",
 _13        action="store_true",
@@ -156,220 +156,217 @@
 _98
 _99class GitBetter(ArgShell):
 100    """GitBetter Shell."""
 101
 102    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
 103    prompt = f"gitbetter::{Pathier.cwd()}>"
 104    execute_in_terminal_if_unrecognized = True
-105
-106    def default(self, line: str):
-107        if self.execute_in_terminal_if_unrecognized:
-108            os.system(line)
-109        else:
-110            super().default(line)
-111
-112    def do_help(self, arg: str):
-113        """List available commands with "help" or detailed help with "help
+105    git = Git()
+106
+107    def default(self, line: str):
+108        if self.execute_in_terminal_if_unrecognized:
+109            os.system(line)
+110        else:
+111            super().default(line)
+112
+113    def do_help(self, arg: str):
+114        """List available commands with "help" or detailed help with "help
 cmd"."""
-114        super().do_help(arg)
-115        if not arg:
-116            print(self.unrecognized_command_behavior_status)
-117            if self.execute_in_terminal_if_unrecognized:
-118                print(
-119                    "^Essentially makes this shell function as a super-shell
+115        super().do_help(arg)
+116        if not arg:
+117            print(self.unrecognized_command_behavior_status)
+118            if self.execute_in_terminal_if_unrecognized:
+119                print(
+120                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
-120                )
-121        print()
-122
-123    @property
-124    def unrecognized_command_behavior_status(self):
-125        return f"Unrecognized command behavior: {'Execute in shell with
+121                )
+122        print()
+123
+124    @property
+125    def unrecognized_command_behavior_status(self):
+126        return f"Unrecognized command behavior: {'Execute in shell with
 os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
 syntax error'}"
-126
-127    def do_toggle_unrecognized_command_behavior(self, arg: str):
-128        """Toggle whether the shell will attempt to execute unrecognized
+127
+128    def do_toggle_unrecognized_command_behavior(self, arg: str):
+129        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
-129        When on (the default), `GitBetter` will treat unrecognized commands
+130        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
-130        When off, an `unknown syntax` message will be printed and no
+131        When off, an `unknown syntax` message will be printed and no
 commands will be executed."""
-131        self.execute_in_terminal_if_unrecognized = (
-132            not self.execute_in_terminal_if_unrecognized
-133        )
-134        print(self.unrecognized_command_behavior_status)
-135
-136    def do_cd(self, path: str):
-137        """Change current working directory to `path`."""
-138        os.chdir(path)
-139        self.prompt = f"gitbetter::{Pathier.cwd()}>"
-140
-141    def do_git(self, arg: str):
-142        """Directly execute `git {arg}`.
-143
-144        i.e. You can still do everything directly invoking git can do."""
-145        git.execute(arg)
-146
-147    def do_new_repo(self, _: str):
-148        """Create a new git repo in this directory."""
-149        git.new_repo()
-150
-151    def do_new_branch(self, name: str):
-152        """Create and switch to a new branch named after the supplied
+132        self.execute_in_terminal_if_unrecognized = (
+133            not self.execute_in_terminal_if_unrecognized
+134        )
+135        print(self.unrecognized_command_behavior_status)
+136
+137    def do_cd(self, path: str):
+138        """Change current working directory to `path`."""
+139        os.chdir(path)
+140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+141
+142    def do_git(self, arg: str):
+143        """Directly execute `git {arg}`.
+144
+145        i.e. You can still do everything directly invoking git can do."""
+146        self.git.execute(arg)
+147
+148    def do_new_repo(self, _: str):
+149        """Create a new git repo in this directory."""
+150        self.git.new_repo()
+151
+152    def do_new_branch(self, name: str):
+153        """Create and switch to a new branch named after the supplied
 arg."""
-153        git.create_new_branch(name)
-154
-155    @with_parser(new_remote_parser)
-156    def do_new_gh_remote(self, args: Namespace):
-157        """Create a remote GitHub repository for this repo.
-158
-159        GitHub CLI must be installed and configured for this to work."""
-160        git.create_remote_from_cwd(args.public)
-161
-162    def do_initcommit(self, _: str):
-163        """Stage and commit all files with message "Initial Commit"."""
-164        git.initcommit()
-165
-166    def do_undo(self, _: str):
-167        """Undo all uncommitted changes."""
-168        git.undo()
-169
-170    @with_parser(amend_files_parser, [files_postparser])
-171    def do_add(self, args: Namespace):
-172        """Stage a list of files.
-173        If no files are given, all files will be added."""
-174        git.add(None if not args.files else args.files)
-175
-176    def do_commit(self, message: str):
-177        """Commit staged files with this message."""
-178        if not message.startswith('"'):
-179            message = '"' + message
-180        if not message.endswith('"'):
-181            message += '"'
-182        git.commit(f"-m {message}")
-183
-184    @with_parser(commit_files_parser, [files_postparser])
-185    def do_commitf(self, args: Namespace):
-186        """Stage and commit a list of files."""
-187        git.commit_files(args.files, args.message)
-188
-189    def do_commitall(self, message: str):
-190        """Stage and commit all files with this message."""
-191        if not message.startswith('"'):
-192            message = '"' + message
-193        if not message.endswith('"'):
-194            message += '"'
-195        git.add()
-196        git.commit(f"-m {message}")
-197
-198    def do_switch(self, branch_name: str):
-199        """Switch to this branch."""
-200        git.switch_branch(branch_name)
-201
-202    def do_add_url(self, url: str):
-203        """Add remote origin url for repo and push repo."""
-204        git.add_remote_url(url)
-205        git.push("-u origin main")
-206
-207    def do_push_new(self, branch_name: str):
-208        """Push this new branch to origin with -u flag."""
-209        git.push_new_branch(branch_name)
+154        self.git.create_new_branch(name)
+155
+156    @with_parser(new_remote_parser)
+157    def do_new_gh_remote(self, args: Namespace):
+158        """Create a remote GitHub repository for this repo.
+159
+160        GitHub CLI must be installed and configured for this to work."""
+161        self.git.create_remote_from_cwd(args.public)
+162
+163    def do_initcommit(self, _: str):
+164        """Stage and commit all files with message "Initial Commit"."""
+165        self.git.initcommit()
+166
+167    def do_undo(self, _: str):
+168        """Undo all uncommitted changes."""
+169        self.git.undo()
+170
+171    @with_parser(amend_files_parser, [files_postparser])
+172    def do_add(self, args: Namespace):
+173        """Stage a list of files.
+174        If no files are given, all files will be added."""
+175        self.git.add(None if not args.files else args.files)
+176
+177    def do_commit(self, args: str):
+178        """Commit staged files with provided `args` string."""
+179        self.git.commit(args)
+180
+181    @with_parser(commit_files_parser, [files_postparser])
+182    def do_commitf(self, args: Namespace):
+183        """Stage and commit a list of files."""
+184        self.git.commit_files(args.files, args.message)
+185
+186    def do_commitall(self, message: str):
+187        """Stage and commit all files with this message."""
+188        if not message.startswith('"'):
+189            message = '"' + message
+190        if not message.endswith('"'):
+191            message += '"'
+192        self.git.add()
+193        self.git.commit(f"-m {message}")
+194
+195    def do_switch(self, branch_name: str):
+196        """Switch to this branch."""
+197        self.git.switch_branch(branch_name)
+198
+199    def do_add_url(self, url: str):
+200        """Add remote origin url for repo and push repo."""
+201        self.git.add_remote_url(url)
+202        self.git.push("-u origin main")
+203
+204    def do_push_new(self, branch_name: str):
+205        """Push this new branch to origin with -u flag."""
+206        self.git.push_new_branch(branch_name)
+207
+208    def do_push(self, args: str):
+209        """Execute `git push`.
 210
-211    def do_push(self, args: str):
-212        """Execute `git push`.
+211        `args` can be any additional args that `git push` accepts."""
+212        self.git.push(args)
 213
-214        `args` can be any additional args that `git push` accepts."""
-215        git.push(args)
+214    def do_pull(self, args: str):
+215        """Execute `git pull`.
 216
-217    def do_pull(self, args: str):
-218        """Execute `git pull`.
+217        `args` can be any additional args that `git pull` accepts."""
+218        self.git.pull(args)
 219
-220        `args` can be any additional args that `git pull` accepts."""
-221        git.pull(args)
-222
-223    def do_branches(self, _: str):
-224        """Show local and remote branches."""
-225        git.list_branches()
-226
-227    def do_loggy(self, _: str):
-228        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-229        git.loggy()
-230
-231    def do_status(self, _: str):
-232        """Execute `git status`."""
-233        git.status()
-234
-235    def do_merge(self, branch_name: str):
-236        """Merge supplied `branch_name` with the currently active branch."""
-237        git.merge(branch_name)
-238
-239    def do_tag(self, tag_id: str):
-240        """Tag current commit with `tag_id`."""
-241        git.tag(tag_id)
-242
-243    @with_parser(amend_files_parser, [files_postparser])
-244    def do_amend(self, args: Namespace):
-245        """Stage files and add to previous commit."""
-246        git.amend(args.files)
-247
-248    @with_parser(delete_branch_parser)
-249    def do_delete_branch(self, args: Namespace):
-250        """Delete branch."""
-251        git.delete_branch(args.branch, not args.remote)
-252
-253    def do_pull_branch(self, branch: str):
-254        """Pull this branch from the origin."""
-255        git.pull_branch(branch)
-256
-257    def do_ignore(self, patterns: str):
-258        """Add the list of patterns to `.gitignore`."""
-259        patterns = "\n".join(patterns.split())
-260        path = Pathier(".gitignore")
-261        path.append("\n")
-262        path.append(patterns, False)
+220    def do_branches(self, _: str):
+221        """Show local and remote branches."""
+222        self.git.list_branches()
+223
+224    def do_loggy(self, _: str):
+225        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+226        self.git.loggy()
+227
+228    def do_status(self, _: str):
+229        """Execute `git status`."""
+230        self.git.status()
+231
+232    def do_merge(self, branch_name: str):
+233        """Merge supplied `branch_name` with the currently active branch."""
+234        self.git.merge(branch_name)
+235
+236    def do_tag(self, tag_id: str):
+237        """Tag current commit with `tag_id`."""
+238        self.git.tag(tag_id)
+239
+240    @with_parser(amend_files_parser, [files_postparser])
+241    def do_amend(self, args: Namespace):
+242        """Stage files and add to previous commit."""
+243        self.git.amend(args.files)
+244
+245    @with_parser(delete_branch_parser)
+246    def do_delete_branch(self, args: Namespace):
+247        """Delete branch."""
+248        self.git.delete_branch(args.branch, not args.remote)
+249
+250    def do_pull_branch(self, branch: str):
+251        """Pull this branch from the origin."""
+252        self.git.pull_branch(branch)
+253
+254    def do_ignore(self, patterns: str):
+255        """Add the list of patterns to `.gitignore`."""
+256        patterns = "\n".join(patterns.split())
+257        path = Pathier(".gitignore")
+258        path.append("\n")
+259        path.append(patterns, False)
+260
+261    def do_make_private(self, owner: str):
+262        """Make the GitHub remote for this repo private.
 263
-264    def do_make_private(self, owner: str):
-265        """Make the GitHub remote for this repo private.
-266
-267        Expects an argument for the repo owner, i.e. the `OWNER` in
+264        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-268
-269        This repo must exist and GitHub CLI must be installed and
+265
+266        This repo must exist and GitHub CLI must be installed and
 configured."""
-270        git.make_private(owner, Pathier.cwd().stem)
+267        self.git.make_private(owner, Pathier.cwd().stem)
+268
+269    def do_make_public(self, owner: str):
+270        """Make the GitHub remote for this repo public.
 271
-272    def do_make_public(self, owner: str):
-273        """Make the GitHub remote for this repo public.
-274
-275        Expects an argument for the repo owner, i.e. the `OWNER` in
+272        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-276
-277        This repo must exist and GitHub CLI must be installed and
+273
+274        This repo must exist and GitHub CLI must be installed and
 configured."""
-278        git.make_public(owner, Pathier.cwd().stem)
+275        self.git.make_public(owner, Pathier.cwd().stem)
+276
+277    def do_delete_gh_repo(self, owner: str):
+278        """Delete this repo from GitHub.
 279
-280    def do_delete_gh_repo(self, owner: str):
-281        """Delete this repo from GitHub.
-282
-283        Expects an argument for the repo owner, i.e. the `OWNER` in
+280        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-284
-285        GitHub CLI must be installed and configured.
+281
+282        GitHub CLI must be installed and configured.
+283
+284        May require you to reauthorize and rerun command."""
+285        self.git.delete_remote(owner, Pathier.cwd().stem)
 286
-287        May require you to reauthorize and rerun command."""
-288        git.delete_remote(owner, Pathier.cwd().stem)
-289
+287
+288def main():
+289    GitBetter().cmdloop()
 290
-291def main():
-292    GitBetter().cmdloop()
-293
-294
-295if __name__ == "__main__":
-296    main()
+291
+292if __name__ == "__main__":
+293    main()
   ⁰
 def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
 10def new_remote_parser() -> ArgShellParser:
 11    parser = ArgShellParser()
 12    parser.add_argument(
 13        "--public",
 14        action="store_true",
@@ -471,490 +468,483 @@
 class GitBetter(argshell.argshell.ArgShell): View Source
 100class GitBetter(ArgShell):
 101    """GitBetter Shell."""
 102
 103    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
 104    prompt = f"gitbetter::{Pathier.cwd()}>"
 105    execute_in_terminal_if_unrecognized = True
-106
-107    def default(self, line: str):
-108        if self.execute_in_terminal_if_unrecognized:
-109            os.system(line)
-110        else:
-111            super().default(line)
-112
-113    def do_help(self, arg: str):
-114        """List available commands with "help" or detailed help with "help
+106    git = Git()
+107
+108    def default(self, line: str):
+109        if self.execute_in_terminal_if_unrecognized:
+110            os.system(line)
+111        else:
+112            super().default(line)
+113
+114    def do_help(self, arg: str):
+115        """List available commands with "help" or detailed help with "help
 cmd"."""
-115        super().do_help(arg)
-116        if not arg:
-117            print(self.unrecognized_command_behavior_status)
-118            if self.execute_in_terminal_if_unrecognized:
-119                print(
-120                    "^Essentially makes this shell function as a super-shell
+116        super().do_help(arg)
+117        if not arg:
+118            print(self.unrecognized_command_behavior_status)
+119            if self.execute_in_terminal_if_unrecognized:
+120                print(
+121                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
-121                )
-122        print()
-123
-124    @property
-125    def unrecognized_command_behavior_status(self):
-126        return f"Unrecognized command behavior: {'Execute in shell with
+122                )
+123        print()
+124
+125    @property
+126    def unrecognized_command_behavior_status(self):
+127        return f"Unrecognized command behavior: {'Execute in shell with
 os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
 syntax error'}"
-127
-128    def do_toggle_unrecognized_command_behavior(self, arg: str):
-129        """Toggle whether the shell will attempt to execute unrecognized
+128
+129    def do_toggle_unrecognized_command_behavior(self, arg: str):
+130        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
-130        When on (the default), `GitBetter` will treat unrecognized commands
+131        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
-131        When off, an `unknown syntax` message will be printed and no
+132        When off, an `unknown syntax` message will be printed and no
 commands will be executed."""
-132        self.execute_in_terminal_if_unrecognized = (
-133            not self.execute_in_terminal_if_unrecognized
-134        )
-135        print(self.unrecognized_command_behavior_status)
-136
-137    def do_cd(self, path: str):
-138        """Change current working directory to `path`."""
-139        os.chdir(path)
-140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
-141
-142    def do_git(self, arg: str):
-143        """Directly execute `git {arg}`.
-144
-145        i.e. You can still do everything directly invoking git can do."""
-146        git.execute(arg)
-147
-148    def do_new_repo(self, _: str):
-149        """Create a new git repo in this directory."""
-150        git.new_repo()
-151
-152    def do_new_branch(self, name: str):
-153        """Create and switch to a new branch named after the supplied
+133        self.execute_in_terminal_if_unrecognized = (
+134            not self.execute_in_terminal_if_unrecognized
+135        )
+136        print(self.unrecognized_command_behavior_status)
+137
+138    def do_cd(self, path: str):
+139        """Change current working directory to `path`."""
+140        os.chdir(path)
+141        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+142
+143    def do_git(self, arg: str):
+144        """Directly execute `git {arg}`.
+145
+146        i.e. You can still do everything directly invoking git can do."""
+147        self.git.execute(arg)
+148
+149    def do_new_repo(self, _: str):
+150        """Create a new git repo in this directory."""
+151        self.git.new_repo()
+152
+153    def do_new_branch(self, name: str):
+154        """Create and switch to a new branch named after the supplied
 arg."""
-154        git.create_new_branch(name)
-155
-156    @with_parser(new_remote_parser)
-157    def do_new_gh_remote(self, args: Namespace):
-158        """Create a remote GitHub repository for this repo.
-159
-160        GitHub CLI must be installed and configured for this to work."""
-161        git.create_remote_from_cwd(args.public)
-162
-163    def do_initcommit(self, _: str):
-164        """Stage and commit all files with message "Initial Commit"."""
-165        git.initcommit()
-166
-167    def do_undo(self, _: str):
-168        """Undo all uncommitted changes."""
-169        git.undo()
-170
-171    @with_parser(amend_files_parser, [files_postparser])
-172    def do_add(self, args: Namespace):
-173        """Stage a list of files.
-174        If no files are given, all files will be added."""
-175        git.add(None if not args.files else args.files)
-176
-177    def do_commit(self, message: str):
-178        """Commit staged files with this message."""
-179        if not message.startswith('"'):
-180            message = '"' + message
-181        if not message.endswith('"'):
-182            message += '"'
-183        git.commit(f"-m {message}")
-184
-185    @with_parser(commit_files_parser, [files_postparser])
-186    def do_commitf(self, args: Namespace):
-187        """Stage and commit a list of files."""
-188        git.commit_files(args.files, args.message)
-189
-190    def do_commitall(self, message: str):
-191        """Stage and commit all files with this message."""
-192        if not message.startswith('"'):
-193            message = '"' + message
-194        if not message.endswith('"'):
-195            message += '"'
-196        git.add()
-197        git.commit(f"-m {message}")
-198
-199    def do_switch(self, branch_name: str):
-200        """Switch to this branch."""
-201        git.switch_branch(branch_name)
-202
-203    def do_add_url(self, url: str):
-204        """Add remote origin url for repo and push repo."""
-205        git.add_remote_url(url)
-206        git.push("-u origin main")
-207
-208    def do_push_new(self, branch_name: str):
-209        """Push this new branch to origin with -u flag."""
-210        git.push_new_branch(branch_name)
+155        self.git.create_new_branch(name)
+156
+157    @with_parser(new_remote_parser)
+158    def do_new_gh_remote(self, args: Namespace):
+159        """Create a remote GitHub repository for this repo.
+160
+161        GitHub CLI must be installed and configured for this to work."""
+162        self.git.create_remote_from_cwd(args.public)
+163
+164    def do_initcommit(self, _: str):
+165        """Stage and commit all files with message "Initial Commit"."""
+166        self.git.initcommit()
+167
+168    def do_undo(self, _: str):
+169        """Undo all uncommitted changes."""
+170        self.git.undo()
+171
+172    @with_parser(amend_files_parser, [files_postparser])
+173    def do_add(self, args: Namespace):
+174        """Stage a list of files.
+175        If no files are given, all files will be added."""
+176        self.git.add(None if not args.files else args.files)
+177
+178    def do_commit(self, args: str):
+179        """Commit staged files with provided `args` string."""
+180        self.git.commit(args)
+181
+182    @with_parser(commit_files_parser, [files_postparser])
+183    def do_commitf(self, args: Namespace):
+184        """Stage and commit a list of files."""
+185        self.git.commit_files(args.files, args.message)
+186
+187    def do_commitall(self, message: str):
+188        """Stage and commit all files with this message."""
+189        if not message.startswith('"'):
+190            message = '"' + message
+191        if not message.endswith('"'):
+192            message += '"'
+193        self.git.add()
+194        self.git.commit(f"-m {message}")
+195
+196    def do_switch(self, branch_name: str):
+197        """Switch to this branch."""
+198        self.git.switch_branch(branch_name)
+199
+200    def do_add_url(self, url: str):
+201        """Add remote origin url for repo and push repo."""
+202        self.git.add_remote_url(url)
+203        self.git.push("-u origin main")
+204
+205    def do_push_new(self, branch_name: str):
+206        """Push this new branch to origin with -u flag."""
+207        self.git.push_new_branch(branch_name)
+208
+209    def do_push(self, args: str):
+210        """Execute `git push`.
 211
-212    def do_push(self, args: str):
-213        """Execute `git push`.
+212        `args` can be any additional args that `git push` accepts."""
+213        self.git.push(args)
 214
-215        `args` can be any additional args that `git push` accepts."""
-216        git.push(args)
+215    def do_pull(self, args: str):
+216        """Execute `git pull`.
 217
-218    def do_pull(self, args: str):
-219        """Execute `git pull`.
+218        `args` can be any additional args that `git pull` accepts."""
+219        self.git.pull(args)
 220
-221        `args` can be any additional args that `git pull` accepts."""
-222        git.pull(args)
-223
-224    def do_branches(self, _: str):
-225        """Show local and remote branches."""
-226        git.list_branches()
-227
-228    def do_loggy(self, _: str):
-229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-230        git.loggy()
-231
-232    def do_status(self, _: str):
-233        """Execute `git status`."""
-234        git.status()
-235
-236    def do_merge(self, branch_name: str):
-237        """Merge supplied `branch_name` with the currently active branch."""
-238        git.merge(branch_name)
-239
-240    def do_tag(self, tag_id: str):
-241        """Tag current commit with `tag_id`."""
-242        git.tag(tag_id)
-243
-244    @with_parser(amend_files_parser, [files_postparser])
-245    def do_amend(self, args: Namespace):
-246        """Stage files and add to previous commit."""
-247        git.amend(args.files)
-248
-249    @with_parser(delete_branch_parser)
-250    def do_delete_branch(self, args: Namespace):
-251        """Delete branch."""
-252        git.delete_branch(args.branch, not args.remote)
-253
-254    def do_pull_branch(self, branch: str):
-255        """Pull this branch from the origin."""
-256        git.pull_branch(branch)
-257
-258    def do_ignore(self, patterns: str):
-259        """Add the list of patterns to `.gitignore`."""
-260        patterns = "\n".join(patterns.split())
-261        path = Pathier(".gitignore")
-262        path.append("\n")
-263        path.append(patterns, False)
+221    def do_branches(self, _: str):
+222        """Show local and remote branches."""
+223        self.git.list_branches()
+224
+225    def do_loggy(self, _: str):
+226        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+227        self.git.loggy()
+228
+229    def do_status(self, _: str):
+230        """Execute `git status`."""
+231        self.git.status()
+232
+233    def do_merge(self, branch_name: str):
+234        """Merge supplied `branch_name` with the currently active branch."""
+235        self.git.merge(branch_name)
+236
+237    def do_tag(self, tag_id: str):
+238        """Tag current commit with `tag_id`."""
+239        self.git.tag(tag_id)
+240
+241    @with_parser(amend_files_parser, [files_postparser])
+242    def do_amend(self, args: Namespace):
+243        """Stage files and add to previous commit."""
+244        self.git.amend(args.files)
+245
+246    @with_parser(delete_branch_parser)
+247    def do_delete_branch(self, args: Namespace):
+248        """Delete branch."""
+249        self.git.delete_branch(args.branch, not args.remote)
+250
+251    def do_pull_branch(self, branch: str):
+252        """Pull this branch from the origin."""
+253        self.git.pull_branch(branch)
+254
+255    def do_ignore(self, patterns: str):
+256        """Add the list of patterns to `.gitignore`."""
+257        patterns = "\n".join(patterns.split())
+258        path = Pathier(".gitignore")
+259        path.append("\n")
+260        path.append(patterns, False)
+261
+262    def do_make_private(self, owner: str):
+263        """Make the GitHub remote for this repo private.
 264
-265    def do_make_private(self, owner: str):
-266        """Make the GitHub remote for this repo private.
-267
-268        Expects an argument for the repo owner, i.e. the `OWNER` in
+265        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-269
-270        This repo must exist and GitHub CLI must be installed and
+266
+267        This repo must exist and GitHub CLI must be installed and
 configured."""
-271        git.make_private(owner, Pathier.cwd().stem)
+268        self.git.make_private(owner, Pathier.cwd().stem)
+269
+270    def do_make_public(self, owner: str):
+271        """Make the GitHub remote for this repo public.
 272
-273    def do_make_public(self, owner: str):
-274        """Make the GitHub remote for this repo public.
-275
-276        Expects an argument for the repo owner, i.e. the `OWNER` in
+273        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-277
-278        This repo must exist and GitHub CLI must be installed and
+274
+275        This repo must exist and GitHub CLI must be installed and
 configured."""
-279        git.make_public(owner, Pathier.cwd().stem)
+276        self.git.make_public(owner, Pathier.cwd().stem)
+277
+278    def do_delete_gh_repo(self, owner: str):
+279        """Delete this repo from GitHub.
 280
-281    def do_delete_gh_repo(self, owner: str):
-282        """Delete this repo from GitHub.
-283
-284        Expects an argument for the repo owner, i.e. the `OWNER` in
+281        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-285
-286        GitHub CLI must be installed and configured.
-287
-288        May require you to reauthorize and rerun command."""
-289        git.delete_remote(owner, Pathier.cwd().stem)
+282
+283        GitHub CLI must be installed and configured.
+284
+285        May require you to reauthorize and rerun command."""
+286        self.git.delete_remote(owner, Pathier.cwd().stem)
 GitBetter Shell.
 ⁰
 def default(self, line: str): View Source
-107    def default(self, line: str):
-108        if self.execute_in_terminal_if_unrecognized:
-109            os.system(line)
-110        else:
-111            super().default(line)
+108    def default(self, line: str):
+109        if self.execute_in_terminal_if_unrecognized:
+110            os.system(line)
+111        else:
+112            super().default(line)
 Called on an input line when the command prefix is not recognized.
 If this method is not overridden, it prints an error message and returns.
 ⁰
 def do_help(self, arg: str): View Source
-113    def do_help(self, arg: str):
-114        """List available commands with "help" or detailed help with "help
+114    def do_help(self, arg: str):
+115        """List available commands with "help" or detailed help with "help
 cmd"."""
-115        super().do_help(arg)
-116        if not arg:
-117            print(self.unrecognized_command_behavior_status)
-118            if self.execute_in_terminal_if_unrecognized:
-119                print(
-120                    "^Essentially makes this shell function as a super-shell
+116        super().do_help(arg)
+117        if not arg:
+118            print(self.unrecognized_command_behavior_status)
+119            if self.execute_in_terminal_if_unrecognized:
+120                print(
+121                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
-121                )
-122        print()
+122                )
+123        print()
 List available commands with "help" or detailed help with "help cmd".
 ⁰
 def do_toggle_unrecognized_command_behavior(self, arg: str): View Source
-128    def do_toggle_unrecognized_command_behavior(self, arg: str):
-129        """Toggle whether the shell will attempt to execute unrecognized
+129    def do_toggle_unrecognized_command_behavior(self, arg: str):
+130        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
-130        When on (the default), `GitBetter` will treat unrecognized commands
+131        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
-131        When off, an `unknown syntax` message will be printed and no
+132        When off, an `unknown syntax` message will be printed and no
 commands will be executed."""
-132        self.execute_in_terminal_if_unrecognized = (
-133            not self.execute_in_terminal_if_unrecognized
-134        )
-135        print(self.unrecognized_command_behavior_status)
+133        self.execute_in_terminal_if_unrecognized = (
+134            not self.execute_in_terminal_if_unrecognized
+135        )
+136        print(self.unrecognized_command_behavior_status)
 Toggle whether the shell will attempt to execute unrecognized commands as
 system commands in the terminal. When on (the default), GitBetter will treat
 unrecognized commands as if you added the sys command in front of the input,
 i.e. os.system(your_input). When off, an unknown syntax message will be printed
 and no commands will be executed.
 ⁰
 def do_cd(self, path: str): View Source
-137    def do_cd(self, path: str):
-138        """Change current working directory to `path`."""
-139        os.chdir(path)
-140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+138    def do_cd(self, path: str):
+139        """Change current working directory to `path`."""
+140        os.chdir(path)
+141        self.prompt = f"gitbetter::{Pathier.cwd()}>"
 Change current working directory to path.
 ⁰
 def do_git(self, arg: str): View Source
-142    def do_git(self, arg: str):
-143        """Directly execute `git {arg}`.
-144
-145        i.e. You can still do everything directly invoking git can do."""
-146        git.execute(arg)
+143    def do_git(self, arg: str):
+144        """Directly execute `git {arg}`.
+145
+146        i.e. You can still do everything directly invoking git can do."""
+147        self.git.execute(arg)
 Directly execute git {arg}.
 i.e. You can still do everything directly invoking git can do.
 ⁰
 def do_new_repo(self, _: str): View Source
-148    def do_new_repo(self, _: str):
-149        """Create a new git repo in this directory."""
-150        git.new_repo()
+149    def do_new_repo(self, _: str):
+150        """Create a new git repo in this directory."""
+151        self.git.new_repo()
 Create a new git repo in this directory.
 ⁰
 def do_new_branch(self, name: str): View Source
-152    def do_new_branch(self, name: str):
-153        """Create and switch to a new branch named after the supplied
+153    def do_new_branch(self, name: str):
+154        """Create and switch to a new branch named after the supplied
 arg."""
-154        git.create_new_branch(name)
+155        self.git.create_new_branch(name)
 Create and switch to a new branch named after the supplied arg.
 ⁰
 @with_parser(new_remote_parser)
 def do_new_gh_remote(self, args: argshell.argshell.Namespace): View Source
-156    @with_parser(new_remote_parser)
-157    def do_new_gh_remote(self, args: Namespace):
-158        """Create a remote GitHub repository for this repo.
-159
-160        GitHub CLI must be installed and configured for this to work."""
-161        git.create_remote_from_cwd(args.public)
+157    @with_parser(new_remote_parser)
+158    def do_new_gh_remote(self, args: Namespace):
+159        """Create a remote GitHub repository for this repo.
+160
+161        GitHub CLI must be installed and configured for this to work."""
+162        self.git.create_remote_from_cwd(args.public)
 Create a remote GitHub repository for this repo.
 GitHub CLI must be installed and configured for this to work.
 ⁰
 def do_initcommit(self, _: str): View Source
-163    def do_initcommit(self, _: str):
-164        """Stage and commit all files with message "Initial Commit"."""
-165        git.initcommit()
+164    def do_initcommit(self, _: str):
+165        """Stage and commit all files with message "Initial Commit"."""
+166        self.git.initcommit()
 Stage and commit all files with message "Initial Commit".
 ⁰
 def do_undo(self, _: str): View Source
-167    def do_undo(self, _: str):
-168        """Undo all uncommitted changes."""
-169        git.undo()
+168    def do_undo(self, _: str):
+169        """Undo all uncommitted changes."""
+170        self.git.undo()
 Undo all uncommitted changes.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_add(self, args: argshell.argshell.Namespace): View Source
-171    @with_parser(amend_files_parser, [files_postparser])
-172    def do_add(self, args: Namespace):
-173        """Stage a list of files.
-174        If no files are given, all files will be added."""
-175        git.add(None if not args.files else args.files)
+172    @with_parser(amend_files_parser, [files_postparser])
+173    def do_add(self, args: Namespace):
+174        """Stage a list of files.
+175        If no files are given, all files will be added."""
+176        self.git.add(None if not args.files else args.files)
 Stage a list of files. If no files are given, all files will be added.
 ⁰
-def do_commit(self, message: str): View Source
-177    def do_commit(self, message: str):
-178        """Commit staged files with this message."""
-179        if not message.startswith('"'):
-180            message = '"' + message
-181        if not message.endswith('"'):
-182            message += '"'
-183        git.commit(f"-m {message}")
-Commit staged files with this message.
+def do_commit(self, args: str): View Source
+178    def do_commit(self, args: str):
+179        """Commit staged files with provided `args` string."""
+180        self.git.commit(args)
+Commit staged files with provided args string.
 ⁰
 @with_parser(commit_files_parser, [files_postparser])
 def do_commitf(self, args: argshell.argshell.Namespace): View Source
-185    @with_parser(commit_files_parser, [files_postparser])
-186    def do_commitf(self, args: Namespace):
-187        """Stage and commit a list of files."""
-188        git.commit_files(args.files, args.message)
+182    @with_parser(commit_files_parser, [files_postparser])
+183    def do_commitf(self, args: Namespace):
+184        """Stage and commit a list of files."""
+185        self.git.commit_files(args.files, args.message)
 Stage and commit a list of files.
 ⁰
 def do_commitall(self, message: str): View Source
-190    def do_commitall(self, message: str):
-191        """Stage and commit all files with this message."""
-192        if not message.startswith('"'):
-193            message = '"' + message
-194        if not message.endswith('"'):
-195            message += '"'
-196        git.add()
-197        git.commit(f"-m {message}")
+187    def do_commitall(self, message: str):
+188        """Stage and commit all files with this message."""
+189        if not message.startswith('"'):
+190            message = '"' + message
+191        if not message.endswith('"'):
+192            message += '"'
+193        self.git.add()
+194        self.git.commit(f"-m {message}")
 Stage and commit all files with this message.
 ⁰
 def do_switch(self, branch_name: str): View Source
-199    def do_switch(self, branch_name: str):
-200        """Switch to this branch."""
-201        git.switch_branch(branch_name)
+196    def do_switch(self, branch_name: str):
+197        """Switch to this branch."""
+198        self.git.switch_branch(branch_name)
 Switch to this branch.
 ⁰
 def do_add_url(self, url: str): View Source
-203    def do_add_url(self, url: str):
-204        """Add remote origin url for repo and push repo."""
-205        git.add_remote_url(url)
-206        git.push("-u origin main")
+200    def do_add_url(self, url: str):
+201        """Add remote origin url for repo and push repo."""
+202        self.git.add_remote_url(url)
+203        self.git.push("-u origin main")
 Add remote origin url for repo and push repo.
 ⁰
 def do_push_new(self, branch_name: str): View Source
-208    def do_push_new(self, branch_name: str):
-209        """Push this new branch to origin with -u flag."""
-210        git.push_new_branch(branch_name)
+205    def do_push_new(self, branch_name: str):
+206        """Push this new branch to origin with -u flag."""
+207        self.git.push_new_branch(branch_name)
 Push this new branch to origin with -u flag.
 ⁰
 def do_push(self, args: str): View Source
-212    def do_push(self, args: str):
-213        """Execute `git push`.
-214
-215        `args` can be any additional args that `git push` accepts."""
-216        git.push(args)
+209    def do_push(self, args: str):
+210        """Execute `git push`.
+211
+212        `args` can be any additional args that `git push` accepts."""
+213        self.git.push(args)
 Execute git push.
 args can be any additional args that git push accepts.
 ⁰
 def do_pull(self, args: str): View Source
-218    def do_pull(self, args: str):
-219        """Execute `git pull`.
-220
-221        `args` can be any additional args that `git pull` accepts."""
-222        git.pull(args)
+215    def do_pull(self, args: str):
+216        """Execute `git pull`.
+217
+218        `args` can be any additional args that `git pull` accepts."""
+219        self.git.pull(args)
 Execute git pull.
 args can be any additional args that git pull accepts.
 ⁰
 def do_branches(self, _: str): View Source
-224    def do_branches(self, _: str):
-225        """Show local and remote branches."""
-226        git.list_branches()
+221    def do_branches(self, _: str):
+222        """Show local and remote branches."""
+223        self.git.list_branches()
 Show local and remote branches.
 ⁰
 def do_loggy(self, _: str): View Source
-228    def do_loggy(self, _: str):
-229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-230        git.loggy()
+225    def do_loggy(self, _: str):
+226        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+227        self.git.loggy()
 Execute git --oneline --name-only --abbrev-commit --graph.
 ⁰
 def do_status(self, _: str): View Source
-232    def do_status(self, _: str):
-233        """Execute `git status`."""
-234        git.status()
+229    def do_status(self, _: str):
+230        """Execute `git status`."""
+231        self.git.status()
 Execute git status.
 ⁰
 def do_merge(self, branch_name: str): View Source
-236    def do_merge(self, branch_name: str):
-237        """Merge supplied `branch_name` with the currently active branch."""
-238        git.merge(branch_name)
+233    def do_merge(self, branch_name: str):
+234        """Merge supplied `branch_name` with the currently active branch."""
+235        self.git.merge(branch_name)
 Merge supplied branch_name with the currently active branch.
 ⁰
 def do_tag(self, tag_id: str): View Source
-240    def do_tag(self, tag_id: str):
-241        """Tag current commit with `tag_id`."""
-242        git.tag(tag_id)
+237    def do_tag(self, tag_id: str):
+238        """Tag current commit with `tag_id`."""
+239        self.git.tag(tag_id)
 Tag current commit with tag_id.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_amend(self, args: argshell.argshell.Namespace): View Source
-244    @with_parser(amend_files_parser, [files_postparser])
-245    def do_amend(self, args: Namespace):
-246        """Stage files and add to previous commit."""
-247        git.amend(args.files)
+241    @with_parser(amend_files_parser, [files_postparser])
+242    def do_amend(self, args: Namespace):
+243        """Stage files and add to previous commit."""
+244        self.git.amend(args.files)
 Stage files and add to previous commit.
 ⁰
 @with_parser(delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-249    @with_parser(delete_branch_parser)
-250    def do_delete_branch(self, args: Namespace):
-251        """Delete branch."""
-252        git.delete_branch(args.branch, not args.remote)
+246    @with_parser(delete_branch_parser)
+247    def do_delete_branch(self, args: Namespace):
+248        """Delete branch."""
+249        self.git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_pull_branch(self, branch: str): View Source
-254    def do_pull_branch(self, branch: str):
-255        """Pull this branch from the origin."""
-256        git.pull_branch(branch)
+251    def do_pull_branch(self, branch: str):
+252        """Pull this branch from the origin."""
+253        self.git.pull_branch(branch)
 Pull this branch from the origin.
 ⁰
 def do_ignore(self, patterns: str): View Source
-258    def do_ignore(self, patterns: str):
-259        """Add the list of patterns to `.gitignore`."""
-260        patterns = "\n".join(patterns.split())
-261        path = Pathier(".gitignore")
-262        path.append("\n")
-263        path.append(patterns, False)
+255    def do_ignore(self, patterns: str):
+256        """Add the list of patterns to `.gitignore`."""
+257        patterns = "\n".join(patterns.split())
+258        path = Pathier(".gitignore")
+259        path.append("\n")
+260        path.append(patterns, False)
 Add the list of patterns to .gitignore.
 ⁰
 def do_make_private(self, owner: str): View Source
-265    def do_make_private(self, owner: str):
-266        """Make the GitHub remote for this repo private.
-267
-268        Expects an argument for the repo owner, i.e. the `OWNER` in
+262    def do_make_private(self, owner: str):
+263        """Make the GitHub remote for this repo private.
+264
+265        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-269
-270        This repo must exist and GitHub CLI must be installed and
+266
+267        This repo must exist and GitHub CLI must be installed and
 configured."""
-271        git.make_private(owner, Pathier.cwd().stem)
+268        self.git.make_private(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo private.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self, owner: str): View Source
-273    def do_make_public(self, owner: str):
-274        """Make the GitHub remote for this repo public.
-275
-276        Expects an argument for the repo owner, i.e. the `OWNER` in
+270    def do_make_public(self, owner: str):
+271        """Make the GitHub remote for this repo public.
+272
+273        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-277
-278        This repo must exist and GitHub CLI must be installed and
+274
+275        This repo must exist and GitHub CLI must be installed and
 configured."""
-279        git.make_public(owner, Pathier.cwd().stem)
+276        self.git.make_public(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo public.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_delete_gh_repo(self, owner: str): View Source
-281    def do_delete_gh_repo(self, owner: str):
-282        """Delete this repo from GitHub.
-283
-284        Expects an argument for the repo owner, i.e. the `OWNER` in
+278    def do_delete_gh_repo(self, owner: str):
+279        """Delete this repo from GitHub.
+280
+281        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-285
-286        GitHub CLI must be installed and configured.
-287
-288        May require you to reauthorize and rerun command."""
-289        git.delete_remote(owner, Pathier.cwd().stem)
+282
+283        GitHub CLI must be installed and configured.
+284
+285        May require you to reauthorize and rerun command."""
+286        self.git.delete_remote(owner, Pathier.cwd().stem)
 Delete this repo from GitHub.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ** Inherited Members **
   ⁰
 def main(): View Source
-292def main():
-293    GitBetter().cmdloop()
+289def main():
+290    GitBetter().cmdloop()
```

### Comparing `gitbetter-0.5.2/src/gitbetter/gitbetter.py` & `gitbetter-1.0.0/src/gitbetter/gitbetter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from argshell import ArgShell, ArgShellParser, Namespace, with_parser
 from pathier import Pathier
 
-from gitbetter import git
+from gitbetter import Git
 
 
 def new_remote_parser() -> ArgShellParser:
     parser = ArgShellParser()
     parser.add_argument(
         "--public",
         action="store_true",
@@ -98,14 +98,15 @@
 
 class GitBetter(ArgShell):
     """GitBetter Shell."""
 
     intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
     prompt = f"gitbetter::{Pathier.cwd()}>"
     execute_in_terminal_if_unrecognized = True
+    git = Git()
 
     def default(self, line: str):
         if self.execute_in_terminal_if_unrecognized:
             os.system(line)
         else:
             super().default(line)
 
@@ -138,158 +139,154 @@
         os.chdir(path)
         self.prompt = f"gitbetter::{Pathier.cwd()}>"
 
     def do_git(self, arg: str):
         """Directly execute `git {arg}`.
 
         i.e. You can still do everything directly invoking git can do."""
-        git.execute(arg)
+        self.git.execute(arg)
 
     def do_new_repo(self, _: str):
         """Create a new git repo in this directory."""
-        git.new_repo()
+        self.git.new_repo()
 
     def do_new_branch(self, name: str):
         """Create and switch to a new branch named after the supplied arg."""
-        git.create_new_branch(name)
+        self.git.create_new_branch(name)
 
     @with_parser(new_remote_parser)
     def do_new_gh_remote(self, args: Namespace):
         """Create a remote GitHub repository for this repo.
 
         GitHub CLI must be installed and configured for this to work."""
-        git.create_remote_from_cwd(args.public)
+        self.git.create_remote_from_cwd(args.public)
 
     def do_initcommit(self, _: str):
         """Stage and commit all files with message "Initial Commit"."""
-        git.initcommit()
+        self.git.initcommit()
 
     def do_undo(self, _: str):
         """Undo all uncommitted changes."""
-        git.undo()
+        self.git.undo()
 
     @with_parser(amend_files_parser, [files_postparser])
     def do_add(self, args: Namespace):
         """Stage a list of files.
         If no files are given, all files will be added."""
-        git.add(None if not args.files else args.files)
+        self.git.add(None if not args.files else args.files)
 
-    def do_commit(self, message: str):
-        """Commit staged files with this message."""
-        if not message.startswith('"'):
-            message = '"' + message
-        if not message.endswith('"'):
-            message += '"'
-        git.commit(f"-m {message}")
+    def do_commit(self, args: str):
+        """Commit staged files with provided `args` string."""
+        self.git.commit(args)
 
     @with_parser(commit_files_parser, [files_postparser])
     def do_commitf(self, args: Namespace):
         """Stage and commit a list of files."""
-        git.commit_files(args.files, args.message)
+        self.git.commit_files(args.files, args.message)
 
     def do_commitall(self, message: str):
         """Stage and commit all files with this message."""
         if not message.startswith('"'):
             message = '"' + message
         if not message.endswith('"'):
             message += '"'
-        git.add()
-        git.commit(f"-m {message}")
+        self.git.add()
+        self.git.commit(f"-m {message}")
 
     def do_switch(self, branch_name: str):
         """Switch to this branch."""
-        git.switch_branch(branch_name)
+        self.git.switch_branch(branch_name)
 
     def do_add_url(self, url: str):
         """Add remote origin url for repo and push repo."""
-        git.add_remote_url(url)
-        git.push("-u origin main")
+        self.git.add_remote_url(url)
+        self.git.push("-u origin main")
 
     def do_push_new(self, branch_name: str):
         """Push this new branch to origin with -u flag."""
-        git.push_new_branch(branch_name)
+        self.git.push_new_branch(branch_name)
 
     def do_push(self, args: str):
         """Execute `git push`.
 
         `args` can be any additional args that `git push` accepts."""
-        git.push(args)
+        self.git.push(args)
 
     def do_pull(self, args: str):
         """Execute `git pull`.
 
         `args` can be any additional args that `git pull` accepts."""
-        git.pull(args)
+        self.git.pull(args)
 
     def do_branches(self, _: str):
         """Show local and remote branches."""
-        git.list_branches()
+        self.git.list_branches()
 
     def do_loggy(self, _: str):
         """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-        git.loggy()
+        self.git.loggy()
 
     def do_status(self, _: str):
         """Execute `git status`."""
-        git.status()
+        self.git.status()
 
     def do_merge(self, branch_name: str):
         """Merge supplied `branch_name` with the currently active branch."""
-        git.merge(branch_name)
+        self.git.merge(branch_name)
 
     def do_tag(self, tag_id: str):
         """Tag current commit with `tag_id`."""
-        git.tag(tag_id)
+        self.git.tag(tag_id)
 
     @with_parser(amend_files_parser, [files_postparser])
     def do_amend(self, args: Namespace):
         """Stage files and add to previous commit."""
-        git.amend(args.files)
+        self.git.amend(args.files)
 
     @with_parser(delete_branch_parser)
     def do_delete_branch(self, args: Namespace):
         """Delete branch."""
-        git.delete_branch(args.branch, not args.remote)
+        self.git.delete_branch(args.branch, not args.remote)
 
     def do_pull_branch(self, branch: str):
         """Pull this branch from the origin."""
-        git.pull_branch(branch)
+        self.git.pull_branch(branch)
 
     def do_ignore(self, patterns: str):
         """Add the list of patterns to `.gitignore`."""
         patterns = "\n".join(patterns.split())
         path = Pathier(".gitignore")
         path.append("\n")
         path.append(patterns, False)
 
     def do_make_private(self, owner: str):
         """Make the GitHub remote for this repo private.
 
         Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`
 
         This repo must exist and GitHub CLI must be installed and configured."""
-        git.make_private(owner, Pathier.cwd().stem)
+        self.git.make_private(owner, Pathier.cwd().stem)
 
     def do_make_public(self, owner: str):
         """Make the GitHub remote for this repo public.
 
         Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`
 
         This repo must exist and GitHub CLI must be installed and configured."""
-        git.make_public(owner, Pathier.cwd().stem)
+        self.git.make_public(owner, Pathier.cwd().stem)
 
     def do_delete_gh_repo(self, owner: str):
         """Delete this repo from GitHub.
 
         Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`
 
         GitHub CLI must be installed and configured.
 
         May require you to reauthorize and rerun command."""
-        git.delete_remote(owner, Pathier.cwd().stem)
+        self.git.delete_remote(owner, Pathier.cwd().stem)
 
 
 def main():
     GitBetter().cmdloop()
 
 
 if __name__ == "__main__":
```

### Comparing `gitbetter-0.5.2/LICENSE.txt` & `gitbetter-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.2/README.md` & `gitbetter-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -83,17 +83,18 @@
   LICENSE.txt
   README.md
   gitbetter_test.py
   test.py
   test.txt
 </pre>
 
-Bindings can be accessed programmatically:
+Bindings can be accessed programmatically through the `Git` class.<br>
 <pre>
->>> from gitbetter import git
+>>> from gitbetter import Git
+>>> git = Git()
 >>> git.loggy()
 *   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
 |\
 | * b4478a3 feat: new print statement
 | | test.py
 * | eb89c2e docs: update readme
 |/
@@ -113,10 +114,42 @@
   gitbetter_test.py
   test.py
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
-
-### Future Features
-* Redirect the output of git commands so the bindings return the output instead of only being able to print.
+The `stdout` of `Git` functions can be returned as a string rather than being printed to the terminal
+by passing `True` to the `Git` constructor or setting the member variable `capture_stdout` to `True`.
+<pre>
+>>> from gitbetter import Git
+>>> git = Git(True)
+# or
+>>> git.capture_stdout = True
+>>> log = git.loggy()
+>>> print(log)
+*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
+|\
+| * b4478a3 feat: new print statement
+| | test.py
+* | eb89c2e docs: update readme
+|/
+|   README.md
+* fc6b7ac (origin/main) docs: update readme
+| README.md
+* 2a75c0c docs: added a comment
+| test.py
+* d22129a feat: new print statement
+| gitbetter_test.py
+* 1a002d7 chore: add items to ignore
+| .gitignore
+* 92cb7e7 Initial commit
+  .gitignore
+  LICENSE.txt
+  README.md
+  gitbetter_test.py
+  test.py
+  test.txt
+>>> git.list_branches()
+* main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
+  remotes/origin/main fc6b7ac docs: update readme
+</pre>
```

### Comparing `gitbetter-0.5.2/pyproject.toml` & `gitbetter-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e35 2e32 220d  rsion = "0.5.2".
+000000b0: 7273 696f 6e20 3d20 2231 2e30 2e30 220d  rsion = "1.0.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-0.5.2/PKG-INFO` & `gitbetter-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 0.5.2
+Version: 1.0.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
@@ -102,17 +102,18 @@
   LICENSE.txt
   README.md
   gitbetter_test.py
   test.py
   test.txt
 </pre>
 
-Bindings can be accessed programmatically:
+Bindings can be accessed programmatically through the `Git` class.<br>
 <pre>
->>> from gitbetter import git
+>>> from gitbetter import Git
+>>> git = Git()
 >>> git.loggy()
 *   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
 |\
 | * b4478a3 feat: new print statement
 | | test.py
 * | eb89c2e docs: update readme
 |/
@@ -132,10 +133,42 @@
   gitbetter_test.py
   test.py
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
-
-### Future Features
-* Redirect the output of git commands so the bindings return the output instead of only being able to print.
+The `stdout` of `Git` functions can be returned as a string rather than being printed to the terminal
+by passing `True` to the `Git` constructor or setting the member variable `capture_stdout` to `True`.
+<pre>
+>>> from gitbetter import Git
+>>> git = Git(True)
+# or
+>>> git.capture_stdout = True
+>>> log = git.loggy()
+>>> print(log)
+*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
+|\
+| * b4478a3 feat: new print statement
+| | test.py
+* | eb89c2e docs: update readme
+|/
+|   README.md
+* fc6b7ac (origin/main) docs: update readme
+| README.md
+* 2a75c0c docs: added a comment
+| test.py
+* d22129a feat: new print statement
+| gitbetter_test.py
+* 1a002d7 chore: add items to ignore
+| .gitignore
+* 92cb7e7 Initial commit
+  .gitignore
+  LICENSE.txt
+  README.md
+  gitbetter_test.py
+  test.py
+  test.txt
+>>> git.list_branches()
+* main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
+  remotes/origin/main fc6b7ac docs: update readme
+</pre>
```

