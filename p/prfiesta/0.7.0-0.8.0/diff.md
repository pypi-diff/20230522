# Comparing `tmp/prfiesta-0.7.0.tar.gz` & `tmp/prfiesta-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.7.0.tar", max compression
+gzip compressed data, was "prfiesta-0.8.0.tar", max compression
```

## Comparing `prfiesta-0.7.0.tar` & `prfiesta-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-22 04:20:37.086772 prfiesta-0.7.0/LICENSE
--rw-r--r--   0        0        0     5494 2023-05-22 04:20:37.086772 prfiesta-0.7.0/README.md
--rw-r--r--   0        0        0      487 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/__init__.py
--rw-r--r--   0        0        0     2542 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4661 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-22 04:20:37.094771 prfiesta-0.7.0/prfiesta/spinner.py
--rw-r--r--   0        0        0     2949 2023-05-22 04:20:47.578742 prfiesta-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 prfiesta-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-22 18:59:38.045992 prfiesta-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6272 2023-05-22 18:59:38.045992 prfiesta-0.8.0/README.md
+-rw-r--r--   0        0        0      487 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     4981 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3183 2023-05-22 18:59:50.026659 prfiesta-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 prfiesta-0.8.0/PKG-INFO
```

### Comparing `prfiesta-0.7.0/LICENSE` & `prfiesta-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.7.0/README.md` & `prfiesta-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # prfiesta 🦜🥳
 
-[![main](https://github.com/kiran94/prfiesta/actions/workflows/main.yml/badge.svg)](https://github.com/kiran94/prfiesta/actions/workflows/main.yml) ![GitHub](https://img.shields.io/github/license/kiran94/prfiesta)
+[![main](https://github.com/kiran94/prfiesta/actions/workflows/main.yml/badge.svg)](https://github.com/kiran94/prfiesta/actions/workflows/main.yml) ![GitHub](https://img.shields.io/github/license/kiran94/prfiesta) [![PyPI](https://img.shields.io/pypi/v/prfiesta)](https://pypi.org/project/prfiesta/)
 
 > Collect and Analyze Individual Contributor Pull Requests
 
 `prfiesta` allows you to collect, analyze and celebrate pull requests made by an individual 🎉.
 
 It can be used by engineers or managers to gain insights into all the great work the contributor has made over a specified period of time. A great use case of this tool is during a performance review process when you want to perform analysis on all the contributions made over the year.
 
 ## Install
 
-```
-TODO
+```bash
+python -m pip install prfiesta
 ```
 
 Dependencies:
 
 - Python 3.8+
 
 ## Usage
@@ -23,20 +23,23 @@
 ```bash
 # Authenticate yourself
 export GITHUB_TOKEN=... # or GITHUB_ENTERPRISE_TOKEN
 
 # Get all pull requests for a user
 prfiesta -u kiran94
 
-# Get all pull requests for a user a date
+# Get all pull requests for a user created after a date
 prfiesta -u kiran94 --after 2023-01-01
 
-# Get all pull requests for a user between two dates
+# Get all pull requests for a user created between two dates
 prfiesta -u kiran94 --after 2023-01-01 --before 2023-06-01
 
+# Get all pull requests for a user updated after a date
+prfiesta -u kiran94 --after 2023-01-01 --use_updated
+
 # Get all pull requests with a custom output file name
 prfiesta -u kiran94 --output my_pull_requests.csv
 
 # Get all pull requests in parquet format with a custom file name
 prfiesta -u kiran94 --output_type parquet --output my_pull_requests.parquet
 
 # Get all pull requests for more then one user
@@ -48,18 +51,17 @@
 # Get help
 prfiesta --help
 ```
 
 You can also leverage `prfiesta` directly in your own application:
 
 ```python
-from datetime import datetime
-
 import pandas as pd
 
+from datetime import datetime
 from prfiesta.collectors.github import GitHubCollector
 
 github = GitHubCollector()
 frame: pd.DataFrame = github.collect('kiran94', 'user2', after=datetime(2023, 1, 1))
 
 print(frame)
 ```
@@ -69,14 +71,20 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
+### Time Filter
+
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` time dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+
+See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
+
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](./docs/analysis.md).
 
 ## Using GitHub Enterprise
 
 If you trying to fetch data from a [GitHub Enterprise](https://docs.github.com/en/enterprise-cloud@latest/rest/enterprise-admin?apiVersion=2022-11-28) server, then much of the same functionality should work the same. You just need to make sure that:
```

### Comparing `prfiesta-0.7.0/prfiesta/__main__.py` & `prfiesta-0.8.0/prfiesta/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,38 +17,40 @@
 
 
 @click.command()
 @click.option('-u', '--users', required=True, multiple=True, help='The GitHub Users to search for. Can be multiple (space delimited)')
 @click.option('-t', '--token', help='The Authentication token to use')
 @click.option('-x', '--url', help='The URL of the Git provider to use')
 @click.option('-o', '--output', default=None, help='The output location')
-@click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', help='The output format')
+@click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, help='The output format')
 @click.option('-dc', '--drop_columns', multiple=True, help='Drop columns from the output dataframe')
 @click.option('--after', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests after this date e.g 2023-01-01')
 @click.option('--before', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests before this date e.g 2023-04-30')
+@click.option('--use_updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
 @click.version_option(__version__)
 def main(**kwargs) -> None:
 
     users: tuple[str] = kwargs.get('users')
     token: str = kwargs.get('token') or github_environment.get_token()
     url: str = kwargs.get('url') or github_environment.get_url()
     output: str = kwargs.get('output')
     output_type: str = kwargs.get('output_type')
     before: datetime = kwargs.get('before')
     after: datetime = kwargs.get('after')
     drop_columns: list[str] = list(kwargs.get('drop_columns'))
+    use_updated: bool = kwargs.get('use_updated')
 
     logger.info('[bold green]PR Fiesta 🦜🥳')
 
     spinner = Spinner('dots', text=Text('Loading', style=SPINNER_STYLE))
 
     with Live(spinner, refresh_per_second=20, transient=True):
 
         collector = GitHubCollector(token=token, url=url, spinner=spinner, drop_columns=drop_columns)
-        pr_frame = collector.collect(*users, after=after, before=before)
+        pr_frame = collector.collect(*users, after=after, before=before, use_updated=use_updated)
 
         if not pr_frame.empty:
             logger.info('Found [bold green]%s[/bold green] pull requests!', pr_frame.shape[0])
 
             output_frame(pr_frame, output_type, spinner=spinner, output_name=output)
             logger.info('Time to analyze 🔎 See https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md for some inspiration!')
```

### Comparing `prfiesta-0.7.0/prfiesta/analysis/plot.py` & `prfiesta-0.8.0/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.7.0/prfiesta/analysis/view.py` & `prfiesta-0.8.0/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.7.0/prfiesta/collectors/github.py` & `prfiesta-0.8.0/prfiesta/collectors/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,23 @@
         self._datetime_columns = [
             'created_at',
             'updated_at',
             'closed_at',
         ]
 
 
-    def collect(self, *users: Tuple[str], after: Optional[datetime] = None, before: Optional[datetime] = None) -> pd.DataFrame:
+    def collect(
+            self,
+            *users: Tuple[str],
+            after: Optional[datetime] = None,
+            before: Optional[datetime] = None,
+            use_updated: bool = False,
+        ) -> pd.DataFrame:
 
-        query = self._construct_query(users, after, before)
+        query = self._construct_query(users, after, before, use_updated)
 
         update_spinner(f'Searching {self._url} with[bold blue] {query}', self._spinner,  logger)
 
         pull_request_data = None
         try:
             pulls = self._github.search_issues(query=query)
 
@@ -75,41 +81,46 @@
         pr_frame['repository_name'] = pr_frame['repository_url'].str.extract(r'(.*)\/repos\/(?P<repository_name>(.*))')['repository_name']
         pr_frame = self._move_column_to_end(pr_frame)
 
         return pr_frame
 
 
     @staticmethod
-    def _construct_query(users: List[str], after: Optional[datetime] = None, before: Optional[datetime] = None) -> str:
+    def _construct_query(users: List[str], after: Optional[datetime] = None, before: Optional[datetime] = None, use_updated: bool = False) -> str:
         """
         Constructs a GitHub Search Query
-        that returns pull requests made by the passed users.
+        that returns pull requests made by the passed users and options.
 
         Examples
         --------
             type:pr author:user1
             type:pr author:user2 updated:<=2021-01-01
             type:pr author:user1 author:user2 updated:2021-01-01..2021-03-01
 
         All dates are inclusive.
-        See GitHub Docs for full optons https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests
+        See GitHub Docs for full options https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests
         """
         query: List[str] = []
-
         query.append('type:pr')
 
         for u in users:
             query.append('author:' + u)
 
+        time_filter = 'created'
+        if use_updated:
+            time_filter = 'updated'
+
+        logger.debug('using time filter %s', time_filter)
+
         if before and after:
-            query.append(f"updated:{after.strftime('%Y-%m-%d')}..{before.strftime('%Y-%m-%d')}")
+            query.append(f"{time_filter}:{after.strftime('%Y-%m-%d')}..{before.strftime('%Y-%m-%d')}")
         elif before:
-            query.append(f"updated:<={before.strftime('%Y-%m-%d')}")
+            query.append(f"{time_filter}:<={before.strftime('%Y-%m-%d')}")
         elif after:
-            query.append(f"updated:>={after.strftime('%Y-%m-%d')}")
+            query.append(f"{time_filter}:>={after.strftime('%Y-%m-%d')}")
 
         return ' '.join(query)
 
     def _move_column_to_end(self, df: pd.DataFrame) -> pd.DataFrame:
         for col in self._move_to_end_columns:
             try:
                 df.insert(len(df.columns)-1, col, df.pop(col))
```

### Comparing `prfiesta-0.7.0/prfiesta/environment.py` & `prfiesta-0.8.0/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.7.0/prfiesta/output.py` & `prfiesta-0.8.0/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.7.0/pyproject.toml` & `prfiesta-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.7.0"
+version = "0.8.0"
 description = "Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
-documentation = "https://github.com/kiran94/prfiesta/README.md"
+documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
 keywords = [ "pull-request", "pull-request-review", "performance-review" ]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Utilities",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Version Control :: Git"
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pygithub = "^1.58.1"
 click = "^8.1.3"
 pandas = "^2.0.1"
 pyarrow = "^11.0.0"
```

### Comparing `prfiesta-0.7.0/PKG-INFO` & `prfiesta-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.7.0
+Version: 0.8.0
 Summary: Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: natural (>=0.2.0,<0.3.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pygithub (>=1.58.1,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: urllib3 (<2)
-Project-URL: Documentation, https://github.com/kiran94/prfiesta/README.md
+Project-URL: Documentation, https://github.com/kiran94/prfiesta/blob/main/README.md
 Project-URL: Repository, https://github.com/kiran94/prfiesta
 Description-Content-Type: text/markdown
 
 # prfiesta 🦜🥳
 
-[![main](https://github.com/kiran94/prfiesta/actions/workflows/main.yml/badge.svg)](https://github.com/kiran94/prfiesta/actions/workflows/main.yml) ![GitHub](https://img.shields.io/github/license/kiran94/prfiesta)
+[![main](https://github.com/kiran94/prfiesta/actions/workflows/main.yml/badge.svg)](https://github.com/kiran94/prfiesta/actions/workflows/main.yml) ![GitHub](https://img.shields.io/github/license/kiran94/prfiesta) [![PyPI](https://img.shields.io/pypi/v/prfiesta)](https://pypi.org/project/prfiesta/)
 
 > Collect and Analyze Individual Contributor Pull Requests
 
 `prfiesta` allows you to collect, analyze and celebrate pull requests made by an individual 🎉.
 
 It can be used by engineers or managers to gain insights into all the great work the contributor has made over a specified period of time. A great use case of this tool is during a performance review process when you want to perform analysis on all the contributions made over the year.
 
 ## Install
 
-```
-TODO
+```bash
+python -m pip install prfiesta
 ```
 
 Dependencies:
 
 - Python 3.8+
 
 ## Usage
@@ -51,20 +56,23 @@
 ```bash
 # Authenticate yourself
 export GITHUB_TOKEN=... # or GITHUB_ENTERPRISE_TOKEN
 
 # Get all pull requests for a user
 prfiesta -u kiran94
 
-# Get all pull requests for a user a date
+# Get all pull requests for a user created after a date
 prfiesta -u kiran94 --after 2023-01-01
 
-# Get all pull requests for a user between two dates
+# Get all pull requests for a user created between two dates
 prfiesta -u kiran94 --after 2023-01-01 --before 2023-06-01
 
+# Get all pull requests for a user updated after a date
+prfiesta -u kiran94 --after 2023-01-01 --use_updated
+
 # Get all pull requests with a custom output file name
 prfiesta -u kiran94 --output my_pull_requests.csv
 
 # Get all pull requests in parquet format with a custom file name
 prfiesta -u kiran94 --output_type parquet --output my_pull_requests.parquet
 
 # Get all pull requests for more then one user
@@ -76,18 +84,17 @@
 # Get help
 prfiesta --help
 ```
 
 You can also leverage `prfiesta` directly in your own application:
 
 ```python
-from datetime import datetime
-
 import pandas as pd
 
+from datetime import datetime
 from prfiesta.collectors.github import GitHubCollector
 
 github = GitHubCollector()
 frame: pd.DataFrame = github.collect('kiran94', 'user2', after=datetime(2023, 1, 1))
 
 print(frame)
 ```
@@ -97,14 +104,20 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
+### Time Filter
+
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` time dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+
+See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
+
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](./docs/analysis.md).
 
 ## Using GitHub Enterprise
 
 If you trying to fetch data from a [GitHub Enterprise](https://docs.github.com/en/enterprise-cloud@latest/rest/enterprise-admin?apiVersion=2022-11-28) server, then much of the same functionality should work the same. You just need to make sure that:
```

