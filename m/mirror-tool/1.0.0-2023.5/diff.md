# Comparing `tmp/mirror-tool-1.0.0.tar.gz` & `tmp/mirror-tool-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirror-tool-1.0.0.tar", max compression
+gzip compressed data, was "mirror-tool-2023.5.tar", last modified: Sun May 21 23:43:52 2023, max compression
```

## Comparing `mirror-tool-1.0.0.tar` & `mirror-tool-2023.5.tar`

### file list

```diff
@@ -1,17 +1,28 @@
--rw-r--r--   0        0        0    35149 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/LICENSE
--rw-r--r--   0        0        0    10363 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/README.md
--rw-r--r--   0        0        0        0 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/__init__.py
--rwxr-xr-x   0        0        0     7648 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/cmd.py
--rw-r--r--   0        0        0    13822 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/conf.py
--rw-r--r--   0        0        0      473 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/git_config.py
--rw-r--r--   0        0        0     4581 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/git_info.py
--rw-r--r--   0        0        0      189 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/gitlab/__init__.py
--rw-r--r--   0        0        0     2230 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/gitlab/ci_template.py
--rw-r--r--   0        0        0    10098 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/gitlab/common.py
--rw-r--r--   0        0        0     2303 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/gitlab/promote.py
--rw-r--r--   0        0        0     3062 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/gitlab/update.py
--rw-r--r--   0        0        0      668 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/jinja.py
--rw-r--r--   0        0        0      113 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/mirror_tool/shared.py
--rw-r--r--   0        0        0      742 2022-09-05 23:13:23.802247 mirror-tool-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11545 1970-01-01 00:00:00.000000 mirror-tool-1.0.0/setup.py
--rw-r--r--   0        0        0    11104 1970-01-01 00:00:00.000000 mirror-tool-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 23:43:38.000000 mirror-tool-2023.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-05-21 23:43:52.277670 mirror-tool-2023.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-05-21 23:43:38.000000 mirror-tool-2023.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.273670 mirror-tool-2023.5/mirror_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8164 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/git_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/git_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/mirror_tool/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/ci_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/gitlab/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 23:43:38.000000 mirror-tool-2023.5/mirror_tool/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/mirror_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 23:43:52.000000 mirror-tool-2023.5/mirror_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-21 23:43:38.000000 mirror-tool-2023.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:43:52.277670 mirror-tool-2023.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:43:52.277670 mirror-tool-2023.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 23:43:38.000000 mirror-tool-2023.5/tests/test_import.py
```

### Comparing `mirror-tool-1.0.0/LICENSE` & `mirror-tool-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/README.md` & `mirror-tool-2023.5/README.md`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/cmd.py` & `mirror-tool-2023.5/mirror_tool/cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,14 +77,20 @@
                 action="store_true",
                 default=False,
                 help=(
                     "Create an empty update commit even if there are no "
                     "updates; primarily for testing purposes"
                 ),
             )
+            p.add_argument(
+                "--skip",
+                action="append",
+                default=[],
+                help="Skip update of these mirror dirs (comma-separated)",
+            )
 
         promote = subparsers.add_parser(
             "promote",
             help=("Promote formerly merged mirror-tool MRs to an additional branch"),
         )
         add_dryrun(promote)
         promote.set_defaults(func=self.promote)
@@ -101,14 +107,21 @@
 
     @property
     def config(self) -> Config:
         if not self._config:
             self._config = Config.from_file(self.args.conf)
         return self._config
 
+    @property
+    def skip(self) -> list[str]:
+        out: list[str] = []
+        for arg in getattr(self.args, "skip", []):
+            out.extend(arg.split(","))
+        return out
+
     def run_cmd(
         self, args, check=True, silent=False, env=None, capture_output=None
     ) -> subprocess.CompletedProcess:
         if not silent:
             LOG.info("+ %s" % " ".join(args))
         return subprocess.run(args, check=check, env=env, capture_output=capture_output)
 
@@ -171,14 +184,17 @@
 
     def update_local(self) -> list[UpdateInfo]:
         cfg = self.config
 
         updates = []
 
         for mirror in cfg.mirrors:
+            if mirror.dir in self.skip:
+                LOG.info("Skipping update of %s", mirror.dir)
+                continue
             updates.append(self.update_local_mirror(mirror))
 
         LOG.info("Mirror(s) locally updated.")
 
         return [u for u in updates if u.changed]
 
     def update(self):
```

### Comparing `mirror-tool-1.0.0/mirror_tool/conf.py` & `mirror-tool-2023.5/mirror_tool/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     title: str = "Update mirror"
 
     # This MUST be '$ENV_VAR_NAME'
     token: str = "$GITLAB_MIRROR_TOKEN"
 
     labels: List[str] = field(default_factory=list)
     description: str = "Automated update of dependencies."
-    comment: GitlabMergeComments = GitlabMergeComments()
+    comment: GitlabMergeComments = field(default_factory=GitlabMergeComments)
 
     # The defaults here assume that we are running from a gitlab CI pipeline.
     # Predefined vars are documented at:
     # https://docs.gitlab.com/ee/ci/variables/predefined_variables.html
     api_v4_url: str = field(default_factory=lambda: os.environ.get("CI_API_V4_URL"))
     project_id: int = field(
         default_factory=lambda: int(os.environ.get("CI_PROJECT_ID") or "0")
@@ -389,15 +389,15 @@
 
         append_gitlab_common(["gitlab_merge"], self.gitlab_merge, updates=updates)
 
         for i, elem in enumerate(self.gitlab_promote):
             base_path = ["gitlab_promote", i]
             append_gitlab_common(base_path, elem, src_mr=VALIDATE_MERGEREQUEST)
 
-        for (path, template, kwargs) in jinja_templates:
+        for path, template, kwargs in jinja_templates:
             self.jinja_validate(template, path, **kwargs)
 
     def jinja_validate(self, template, path, **kwargs):
         try:
             jinja_validate(template, **kwargs)
         except Exception as exc:
             raise jsonschema.ValidationError(
```

### Comparing `mirror-tool-1.0.0/mirror_tool/git_info.py` & `mirror-tool-2023.5/mirror_tool/git_info.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/gitlab/ci_template.py` & `mirror-tool-2023.5/mirror_tool/gitlab/ci_template.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/gitlab/common.py` & `mirror-tool-2023.5/mirror_tool/gitlab/common.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/gitlab/promote.py` & `mirror-tool-2023.5/mirror_tool/gitlab/promote.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/gitlab/update.py` & `mirror-tool-2023.5/mirror_tool/gitlab/update.py`

 * *Files identical despite different names*

### Comparing `mirror-tool-1.0.0/mirror_tool/jinja.py` & `mirror-tool-2023.5/mirror_tool/jinja.py`

 * *Files identical despite different names*

