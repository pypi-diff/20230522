# Comparing `tmp/mosek_license_server-0.1.2.tar.gz` & `tmp/mosek_license_server-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.1.2.tar", max compression
+gzip compressed data, was "mosek_license_server-0.1.3.tar", max compression
```

## Comparing `mosek_license_server-0.1.2.tar` & `mosek_license_server-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-21 05:39:44.781663 mosek_license_server-0.1.2/mosek_license/__init__.py
--rw-r--r--   0        0        0      499 2023-05-21 05:39:44.785663 mosek_license_server-0.1.2/mosek_license/license.py
--rw-r--r--   0        0        0      533 2023-05-21 05:40:02.209895 mosek_license_server-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-05-21 05:39:44.785663 mosek_license_server-0.1.2/readme.md
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 mosek_license_server-0.1.2/setup.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 mosek_license_server-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-22 15:43:36.887460 mosek_license_server-0.1.3/mosek_license/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-22 15:43:36.887460 mosek_license_server-0.1.3/mosek_license/license.py
+-rw-r--r--   0        0        0      533 2023-05-22 15:43:52.419585 mosek_license_server-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2362 2023-05-22 15:43:36.887460 mosek_license_server-0.1.3/readme.md
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 mosek_license_server-0.1.3/setup.py
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 mosek_license_server-0.1.3/PKG-INFO
```

### Comparing `mosek_license_server-0.1.2/pyproject.toml` & `mosek_license_server-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosek-license-server"
-version = "0.1.2"
+version = "0.1.3"
 description = "Expose a mosek license via a nginx server"
 authors = ["Thomas Schmelzer <thomas.schmelzer@gmail.com>"]
 license = "Apache 2.0"
 readme = "readme.md"
 repository = "https://github.com/tschm/mosek-license-server"
 packages = [{include = "mosek_license"}]
```

### Comparing `mosek_license_server-0.1.2/readme.md` & `mosek_license_server-0.1.3/readme.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 # Mosek License Server
 
+[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)
 [![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)
 
 Using a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license
 on a server to be accessible from various research machines without sharing the actual
 license file in the underlying repositories.
 
 This repository serves two purposes. It exposes the server but it is also the home
 for a little Python package to inject the license into your programs.
 
 We solve a common problem here. Assume $20$ researchers work on $50$ different strategies.
-Using local copies of the same license file is a tedious exercise as the file needs to get 
-updated once a year. 
+Using local copies of the same license file is a tedious exercise as
+he file needs to get updated once a year.
 Rather, each strategy would connect to the server to fetch a license using the mosek_license
 Python package. Once the strategy expires we only need to update the server.
 No change for the strategies is required.
 
 ## License server
 
-### Copy your license file into folder 
+### Copy your license file into folder
 
 Copy the license file you have received (from Mosek) into the license folder.
 Name it `mosek'.
 
+The file should look like
+
+```bash
+START_LICENSE
+VENDOR MOSEKLM
+# PSN-4183
+FEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...
+# PSN-4182
+FEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...
+END_LICENSE
+```
 
 ### Start the nginx server
 
 Share the license folder (after you have copied your personal Mosek license into)
 via
 
 ```bash
 docker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx
 ```
 
-The license will now be exposed via http://localhost:8080
+The license will now be exposed via `http://localhost:8080/mosek`
 
 As an alternative you can run the script
 
 ```bash
-./license_server.sh
+./start_server.sh
 ```
 
 ## The mosek_license module
 
 Install via
 
 ```bash
 pip install mosek-license-server
 ```
+
 and then
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
 license.upsert()
 
 # only now import mosek
 import mosek
 ```
-
```

### Comparing `mosek_license_server-0.1.2/setup.py` & `mosek_license_server-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['urllib3']
 
 setup_kwargs = {
     'name': 'mosek-license-server',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Expose a mosek license via a nginx server',
-    'long_description': "# Mosek License Server\n\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as the file needs to get \nupdated once a year. \nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder \n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via http://localhost:8080\n\nAs an alternative you can run the script\n\n```bash\n./license_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only now import mosek\nimport mosek\n```\n\n",
+    'long_description': "# Mosek License Server\n\n[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as\nhe file needs to get updated once a year.\nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder\n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\nThe file should look like\n\n```bash\nSTART_LICENSE\nVENDOR MOSEKLM\n# PSN-4183\nFEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...\n# PSN-4182\nFEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...\nEND_LICENSE\n```\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via `http://localhost:8080/mosek`\n\nAs an alternative you can run the script\n\n```bash\n./start_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\n\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only now import mosek\nimport mosek\n```\n",
     'author': 'Thomas Schmelzer',
     'author_email': 'thomas.schmelzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tschm/mosek-license-server',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mosek_license_server-0.1.2/PKG-INFO` & `mosek_license_server-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.1.2
+Version: 0.1.3
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
@@ -14,70 +14,82 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: urllib3
 Project-URL: Repository, https://github.com/tschm/mosek-license-server
 Description-Content-Type: text/markdown
 
 # Mosek License Server
 
+[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)
 [![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)
 
 Using a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license
 on a server to be accessible from various research machines without sharing the actual
 license file in the underlying repositories.
 
 This repository serves two purposes. It exposes the server but it is also the home
 for a little Python package to inject the license into your programs.
 
 We solve a common problem here. Assume $20$ researchers work on $50$ different strategies.
-Using local copies of the same license file is a tedious exercise as the file needs to get 
-updated once a year. 
+Using local copies of the same license file is a tedious exercise as
+he file needs to get updated once a year.
 Rather, each strategy would connect to the server to fetch a license using the mosek_license
 Python package. Once the strategy expires we only need to update the server.
 No change for the strategies is required.
 
 ## License server
 
-### Copy your license file into folder 
+### Copy your license file into folder
 
 Copy the license file you have received (from Mosek) into the license folder.
 Name it `mosek'.
 
+The file should look like
+
+```bash
+START_LICENSE
+VENDOR MOSEKLM
+# PSN-4183
+FEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...
+# PSN-4182
+FEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...
+END_LICENSE
+```
 
 ### Start the nginx server
 
 Share the license folder (after you have copied your personal Mosek license into)
 via
 
 ```bash
 docker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx
 ```
 
-The license will now be exposed via http://localhost:8080
+The license will now be exposed via `http://localhost:8080/mosek`
 
 As an alternative you can run the script
 
 ```bash
-./license_server.sh
+./start_server.sh
 ```
 
 ## The mosek_license module
 
 Install via
 
 ```bash
 pip install mosek-license-server
 ```
+
 and then
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
 license.upsert()
 
 # only now import mosek
 import mosek
 ```
 
-
```

