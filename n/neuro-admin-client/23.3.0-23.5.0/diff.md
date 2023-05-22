# Comparing `tmp/neuro-admin-client-23.3.0.tar.gz` & `tmp/neuro-admin-client-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-admin-client-23.3.0.tar", last modified: Thu Mar 30 08:19:52 2023, max compression
+gzip compressed data, was "neuro-admin-client-23.5.0.tar", last modified: Mon May 22 08:57:31 2023, max compression
```

## Comparing `neuro-admin-client-23.3.0.tar` & `neuro-admin-client-23.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.github/actionlint-matcher.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.github/workflows/remove-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.github/workflows/setup-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/neuro_admin_client/
--rw-r--r--   0 runner    (1001) docker     (123)    95599 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/neuro_admin_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/neuro_admin_client/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/neuro_admin_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-30 08:19:52.000000 neuro-admin-client-23.3.0/neuro_admin_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-30 08:19:52.705326 neuro-admin-client-23.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:52.701326 neuro-admin-client-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56290 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    64626 2023-03-30 08:19:30.000000 neuro-admin-client-23.3.0/tests/test_admin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.738733 neuro-admin-client-23.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.github/actionlint-matcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.github/workflows/remove-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.github/workflows/setup-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/neuro_admin_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    95683 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/neuro_admin_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/neuro_admin_client/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/neuro_admin_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 08:57:31.000000 neuro-admin-client-23.5.0/neuro_admin_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:31.742733 neuro-admin-client-23.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56556 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66572 2023-05-22 08:57:12.000000 neuro-admin-client-23.5.0/tests/test_admin_client.py
```

### Comparing `neuro-admin-client-23.3.0/.github/workflows/ci.yaml` & `neuro-admin-client-23.5.0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     name: Run tests
     runs-on: ubuntu-latest
     if: |
       (github.event_name != 'pull_request_target' && github.actor != 'dependabot[bot]') ||
       (github.event_name == 'pull_request_target' && github.actor == 'dependabot[bot]')
     strategy:
       matrix:
-        py_version: ['3.7', '3.8', '3.9', '3.10']
+        py_version: ['3.8', '3.9', '3.10', '3.11']
     steps:
     - name: Checkout commit
       uses: actions/checkout@v3
       with:
         ref: ${{ github.event.pull_request.head.sha }}
     - name: Install python
       uses: actions/setup-python@v4
```

### Comparing `neuro-admin-client-23.3.0/.github/workflows/remove-automerge.yml` & `neuro-admin-client-23.5.0/.github/workflows/remove-automerge.yml`

 * *Files identical despite different names*

### Comparing `neuro-admin-client-23.3.0/.github/workflows/setup-automerge.yml` & `neuro-admin-client-23.5.0/.github/workflows/setup-automerge.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - id: generate_token
       uses: tibdex/github-app-token@v1
       with:
         app_id: ${{ secrets.BOT_APP_ID }}
         private_key: ${{ secrets.BOT_PRIVATE_KEY }}
     - name: metadata
       id: metadata
-      uses: dependabot/fetch-metadata@v1.3.6
+      uses: dependabot/fetch-metadata@v1.4.0
       with:
         github-token: ${{ steps.generate_token.outputs.token }}
     - name: Enable auto-merge for bot PRs
       run: gh pr merge --auto --squash --delete-branch "$PR_URL"
       env:
         PR_URL: ${{ github.event.pull_request.html_url }}
         GH_TOKEN: ${{ steps.generate_token.outputs.token }}
```

### Comparing `neuro-admin-client-23.3.0/.gitignore` & `neuro-admin-client-23.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `neuro-admin-client-23.3.0/.pre-commit-config.yaml` & `neuro-admin-client-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `neuro-admin-client-23.3.0/LICENSE` & `neuro-admin-client-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-admin-client-23.3.0/neuro_admin_client/__init__.py` & `neuro-admin-client-23.5.0/neuro_admin_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1145,17 +1145,18 @@
             spent_credits=Decimal(payload["spent_credits"]),
             credits=Decimal(payload["credits"]) if payload.get("credits") else None,
         )
 
     def _parse_cluster_user(
         self, cluster_name: str, payload: dict[str, Any]
     ) -> ClusterUser | ClusterUserWithInfo:
+        role = ClusterUserRoleType(payload["role"]) if "role" in payload else None
         cluster_user = ClusterUser(
             user_name=payload["user_name"],
-            role=ClusterUserRoleType(payload["role"]),
+            role=role,
             quota=self._parse_quota(payload.get("quota")),
             balance=self._parse_balance(payload.get("balance")),
             org_name=payload.get("org_name"),
             cluster_name=cluster_name,
         )
         if "user_info" in payload:
             user_info = self._parse_user_info_payload(payload["user_info"])
@@ -1325,14 +1326,15 @@
         self, cluster_user: ClusterUser, with_user_info: Literal[False] = ...
     ) -> ClusterUser:
         ...
 
     async def update_cluster_user(
         self, cluster_user: ClusterUser, with_user_info: bool = False
     ) -> ClusterUser | ClusterUserWithInfo:
+        assert cluster_user.role
         payload: dict[str, Any] = {
             "user_name": cluster_user.user_name,
             "role": cluster_user.role.value,
             "quota": {},
             "balance": {},
         }
         if cluster_user.org_name:
```

### Comparing `neuro-admin-client-23.3.0/neuro_admin_client/entities.py` & `neuro-admin-client-23.5.0/neuro_admin_client/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     maintenance: bool = False
 
 
 @dataclass(frozen=True)
 class ClusterUser:
     cluster_name: str
     user_name: str
-    role: ClusterUserRoleType
+    role: Optional[ClusterUserRoleType]
     quota: Quota
     balance: Balance
     org_name: Optional[str]
 
     def add_info(self, user_info: UserInfo) -> "ClusterUserWithInfo":
         return ClusterUserWithInfo(
             cluster_name=self.cluster_name,
```

### Comparing `neuro-admin-client-23.3.0/neuro_admin_client.egg-info/SOURCES.txt` & `neuro-admin-client-23.5.0/neuro_admin_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-admin-client-23.3.0/setup.cfg` & `neuro-admin-client-23.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 license = Apache 2
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = False
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 packages = find:
 install_requires = 
 	aiohttp>=3.8.1
 
 [tool:pytest]
 addopts =
```

### Comparing `neuro-admin-client-23.3.0/tests/conftest.py` & `neuro-admin-client-23.5.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,25 +285,31 @@
         for idx, cluster in enumerate(self.clusters):
             if cluster.name == cluster_name:
                 del self.clusters[idx]
                 return aiohttp.web.json_response(self._serialize_cluster(cluster))
         raise aiohttp.web.HTTPNotFound
 
     def _serialize_cluster_user(
-        self, cluster_user: ClusterUser, with_info: bool
+        self,
+        cluster_user: ClusterUser,
+        with_info: bool,
+        only_usernames: bool = False,
     ) -> dict[str, Any]:
+        if only_usernames:
+            return {"user_name": cluster_user.user_name}
         res: dict[str, Any] = {
             "user_name": cluster_user.user_name,
-            "role": cluster_user.role.value,
             "org_name": cluster_user.org_name,
             "quota": {},
             "balance": {
                 "spent_credits": str(cluster_user.balance.spent_credits),
             },
         }
+        if cluster_user.role:
+            res["role"] = cluster_user.role.value
         if cluster_user.quota.total_running_jobs is not None:
             res["quota"]["total_running_jobs"] = cluster_user.quota.total_running_jobs
         if cluster_user.balance.credits is not None:
             res["balance"]["credits"] = str(cluster_user.balance.credits)
         if with_info:
             user = next(
                 user for user in self.users if user.name == cluster_user.user_name
@@ -540,15 +546,17 @@
     async def handle_cluster_user_list(
         self, request: aiohttp.web.Request
     ) -> aiohttp.web.Response:
         cluster_name = request.match_info["cname"]
         org_name = request.match_info.get("oname")
         resp = [
             self._serialize_cluster_user(
-                cluster_user, _parse_bool(request.query.get("with_user_info", "false"))
+                cluster_user,
+                _parse_bool(request.query.get("with_user_info", "false")),
+                _parse_bool(request.query.get("only_usernames", "false")),
             )
             for cluster_user in self.cluster_users
             if cluster_user.cluster_name == cluster_name
             and (org_name is None or cluster_user.org_name == org_name)
         ]
         return aiohttp.web.json_response(resp)
```

### Comparing `neuro-admin-client-23.3.0/tests/test_admin_client.py` & `neuro-admin-client-23.5.0/tests/test_admin_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
+import typing as t
 from dataclasses import replace
 from decimal import Decimal
+from contextlib import AbstractAsyncContextManager, asynccontextmanager
 
 import pytest
-from aiohttp import ClientResponseError
+from aiohttp import ClientResponseError, ClientResponse
 
 from neuro_admin_client import (
     AdminClient,
     Balance,
     GetUserResponse,
     Cluster,
     ClusterUser,
@@ -601,14 +603,68 @@
 
         async with AdminClient(base_url=mock_admin_server.url) as client:
             cluster_users = await client.list_cluster_users("cluster")
 
         assert len(cluster_users) == 2
         assert set(cluster_users) == set(mock_admin_server.cluster_users)
 
+    async def test_list_clusters_user_can_only_get_usernames(
+        self, mock_admin_server: AdminServer
+    ) -> None:
+        mock_admin_server.users = [
+            User(
+                name="test1",
+                email="email",
+            ),
+            User(
+                name="test2",
+                email="email",
+            ),
+        ]
+        mock_admin_server.clusters = [
+            Cluster(
+                name="cluster",
+                default_credits=None,
+                default_quota=Quota(),
+                default_role=ClusterUserRoleType.USER,
+            ),
+        ]
+        mock_admin_server.cluster_users = [
+            ClusterUser(
+                user_name="test1",
+                cluster_name="cluster",
+                org_name=None,
+                balance=Balance(),
+                quota=Quota(),
+                role=ClusterUserRoleType.USER,
+            ),
+            ClusterUser(
+                user_name="test2",
+                cluster_name="cluster",
+                org_name=None,
+                balance=Balance(),
+                quota=Quota(),
+                role=ClusterUserRoleType.ADMIN,
+            ),
+        ]
+
+        class PatchedAdminClient(AdminClient):
+            @asynccontextmanager
+            async def _request(self, *args, **kwargs) -> t.Any:  # type: ignore
+                kwargs["params"]["only_usernames"] = "true"
+                async with AdminClient._request(self, *args, **kwargs) as resp:
+                    yield resp
+
+        async with PatchedAdminClient(base_url=mock_admin_server.url) as client:
+            cluster_users = await client.list_cluster_users("cluster")
+
+        expected = [replace(u, role=None) for u in mock_admin_server.cluster_users]
+        assert len(cluster_users) == 2
+        assert set(cluster_users) == set(expected)
+
     async def test_list_clusters_user_with_org(
         self, mock_admin_server: AdminServer
     ) -> None:
         mock_admin_server.users = [
             User(
                 name="test1",
                 email="email",
```

