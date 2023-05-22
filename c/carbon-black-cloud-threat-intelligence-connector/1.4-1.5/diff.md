# Comparing `tmp/carbon_black_cloud_threat_intelligence_connector-1.4.tar.gz` & `tmp/carbon_black_cloud_threat_intelligence_connector-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon_black_cloud_threat_intelligence_connector-1.4.tar", max compression
+gzip compressed data, was "carbon_black_cloud_threat_intelligence_connector-1.5.tar", max compression
```

## Comparing `carbon_black_cloud_threat_intelligence_connector-1.4.tar` & `carbon_black_cloud_threat_intelligence_connector-1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1507 2022-10-20 15:14:06.770040 carbon_black_cloud_threat_intelligence_connector-1.4/LICENSE
--rw-r--r--   0        0        0     3605 2022-10-20 15:14:06.770339 carbon_black_cloud_threat_intelligence_connector-1.4/README.md
--rw-r--r--   0        0        0      173 2023-01-10 14:27:18.906678 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 15:14:06.770961 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/cli/__init__.py
--rw-r--r--   0        0        0    11041 2022-10-20 15:14:06.771249 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/cli/connector.py
--rw-r--r--   0        0        0    11449 2022-10-20 15:14:06.771540 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/cli/wizard.py
--rw-r--r--   0        0        0     5617 2022-10-20 15:14:06.771781 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/importer.py
--rw-r--r--   0        0        0        0 2022-10-20 15:14:06.772037 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 15:14:06.772313 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v1/__init__.py
--rw-r--r--   0        0        0     7423 2022-10-20 15:14:06.772626 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v1/object_parsers.py
--rw-r--r--   0        0        0     9173 2022-10-20 15:14:06.772860 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v1/parser.py
--rw-r--r--   0        0        0        0 2022-10-20 15:14:06.773082 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v2/__init__.py
--rw-r--r--   0        0        0     9623 2022-10-20 15:14:06.773318 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v2/parser.py
--rw-r--r--   0        0        0     7666 2022-10-20 15:14:06.773582 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v2/pattern_parser.py
--rw-r--r--   0        0        0     4925 2022-10-20 15:14:06.773811 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/taxii_configurator.py
--rw-r--r--   0        0        0     5038 2022-10-20 15:14:06.774090 carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/utils.py
--rw-r--r--   0        0        0     1915 2023-01-10 14:27:18.909766 carbon_black_cloud_threat_intelligence_connector-1.4/pyproject.toml
--rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 carbon_black_cloud_threat_intelligence_connector-1.4/setup.py
--rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 carbon_black_cloud_threat_intelligence_connector-1.4/PKG-INFO
+-rw-r--r--   0        0        0     1507 2022-10-20 15:14:06.770040 carbon_black_cloud_threat_intelligence_connector-1.5/LICENSE
+-rw-r--r--   0        0        0     3605 2022-10-20 15:14:06.770339 carbon_black_cloud_threat_intelligence_connector-1.5/README.md
+-rw-r--r--   0        0        0      173 2023-05-22 12:35:14.143417 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 15:14:06.770961 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/cli/__init__.py
+-rw-r--r--   0        0        0    11041 2022-10-20 15:14:06.771249 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/cli/connector.py
+-rw-r--r--   0        0        0    11449 2022-10-20 15:14:06.771540 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/cli/wizard.py
+-rw-r--r--   0        0        0     5617 2022-10-20 15:14:06.771781 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/importer.py
+-rw-r--r--   0        0        0        0 2022-10-20 15:14:06.772037 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 15:14:06.772313 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v1/__init__.py
+-rw-r--r--   0        0        0     7423 2022-10-20 15:14:06.772626 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v1/object_parsers.py
+-rw-r--r--   0        0        0     9173 2022-10-20 15:14:06.772860 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v1/parser.py
+-rw-r--r--   0        0        0        0 2022-10-20 15:14:06.773082 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v2/__init__.py
+-rw-r--r--   0        0        0     9623 2022-10-20 15:14:06.773318 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v2/parser.py
+-rw-r--r--   0        0        0     7666 2022-10-20 15:14:06.773582 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v2/pattern_parser.py
+-rw-r--r--   0        0        0     4925 2022-10-20 15:14:06.773811 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/taxii_configurator.py
+-rw-r--r--   0        0        0     5038 2022-10-20 15:14:06.774090 carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/utils.py
+-rw-r--r--   0        0        0     1915 2023-05-22 12:35:14.145971 carbon_black_cloud_threat_intelligence_connector-1.5/pyproject.toml
+-rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 carbon_black_cloud_threat_intelligence_connector-1.5/setup.py
+-rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 carbon_black_cloud_threat_intelligence_connector-1.5/PKG-INFO
```

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/LICENSE` & `carbon_black_cloud_threat_intelligence_connector-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/README.md` & `carbon_black_cloud_threat_intelligence_connector-1.5/README.md`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/cli/connector.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/cli/connector.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/cli/wizard.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/importer.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/importer.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v1/object_parsers.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v1/object_parsers.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v1/parser.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v1/parser.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v2/parser.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v2/parser.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/stix_parsers/v2/pattern_parser.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/stix_parsers/v2/pattern_parser.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/taxii_configurator.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/taxii_configurator.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/cbc_importer/utils.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/cbc_importer/utils.py`

 * *Files identical despite different names*

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/pyproject.toml` & `carbon_black_cloud_threat_intelligence_connector-1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.mypy]
 ignore_missing_imports = true
 files = ["./cbc_importer/**/*.py", "./configurator/*.py"]
 
 [tool.poetry]
 name = "carbon-black-cloud-threat-intelligence-connector"
-version = "1.4"
+version = "1.5"
 description = "Carbon Black Cloud Threat Intelligence Connector"
 authors = ["Dimitar Ganev <dganev@vmware.com>" , "Emanuela Mitreva <emitreva@vmware.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 classifiers = [
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
```

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/setup.py` & `carbon_black_cloud_threat_intelligence_connector-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 entry_points = \
 {'console_scripts': ['cbc-threat-intel = cbc_importer.cli.connector:cli',
                      'cbc-threat-intel-wizard = cbc_importer.cli.wizard:cli']}
 
 setup_kwargs = {
     'name': 'carbon-black-cloud-threat-intelligence-connector',
-    'version': '1.4',
+    'version': '1.5',
     'description': 'Carbon Black Cloud Threat Intelligence Connector',
     'long_description': '# Threat Intelligence Connector for Carbon Black Cloud\n\nThis is a python project that can be used for ingesting Threat Intelligence from various STIX Feeds. The current supported versions of STIX Feeds are 1.x, 2.0 and 2.1.\nIt supports python >= 3.8\n\n[![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-threat-intelligence-connector/badge.svg?t=TczX1a)](https://coveralls.io/github/carbonblack/carbon-black-cloud-threat-intelligence-connector)\n[![Codeship Status for carbonblack/carbon-black-cloud-threat-intelligence-connector](https://app.codeship.com/projects/73a21e3d-2c23-4fa8-a611-ada9d9849f2c/status?branch=main)](https://app.codeship.com/projects/456985)\n\n## Installation\n\n```shell-session\n$ pip install carbon-black-cloud-threat-intelligence-connector\n$ cbc-threat-intel --help\nUsage: cbc-threat-intel [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  create-feed       Creates a feed in CBC\n  create-watchlist  Creates a Watchlist in CBC (from already created feed)\n  process-file      Process and import a single STIX content file into...\n  process-server    Process and import a TAXII Server (2.0/2.1/1.x)\n  version           Shows the version of the connector\n```\n\n## Documentation\n\nVisit the [developer network of Carbon Black Cloud](https://developer.carbonblack.com/reference/carbon-black-cloud/integrations/threat-intelligence-connector/) for more information of how to use the connector.\n\n## Developing the connector\n\nWe rely on pull requests to keep this project maintained. By participating in this project, you agree to abide by the VMware [code of conduct](CODE-OF-CONDUCT.md).\n\n### Setup\n\nIt is recommended to use Python3.8 / Python3.9 version for that project, assuming that you installed the deps with either virtualenv or poetry.\n\nFor a good code quality make sure to install the hooks from `pre-commit` as well.\n\n```shell-session\n$ pre-commit install\n```\n\n### Installation\n\nClone the repository\n\n```bash\n$ git clone https://github.com/carbonblack/carbon-black-cloud-threat-intelligence-connector.git\n$ cd carbon-black-cloud-threat-intelligence-connector/\n```\n\nYou can install this connector either via Poetry or using the `virtualenv`.\n\n#### Using [Poetry](https://python-poetry.org/docs/)\n\nYou will need to [install poetry](https://python-poetry.org/docs/#installation) first.\n\nTo install the connector run:\n\n```shell-session\n$ poetry install\n```\n\n#### Using [virtualenv](https://virtualenv.pypa.io/en/latest/)\n\nYou will need to [install virtualenv](https://virtualenv.pypa.io/en/latest/installation.html) first.\n\n```bash\n$ virtualenv venv\n...\n$ source ./venv/bin/activate\n(venv) $ pip install -r requirements.txt\n```\n\n### Tests\n\nThe tests can be run with the following command:\n\n```shell-session\n$ pytest ./tests/unit/\n```\nFor running the performance tests check out the [README](tests/performance/README.md)\n\n### Support\n\n1. View all API and integration offerings on the [Developer Network](https://developer.carbonblack.com) along with reference documentation, video tutorials, and how-to guides.\n2. Use the [Developer Community Forum](https://community.carbonblack.com/) to discuss issues and get answers from other API developers in the Carbon Black Community.\n3. Create a github issue for bugs and change requests or create a ticket with [Carbon Black Support](http://carbonblack.com/resources/support/).\n\n### Submitting a PR\n\nIt is strongly recommended to have written tests and documentation for your changes before submitting a PR to the project. Make sure to write good commit messages as well.\n',
     'author': 'Dimitar Ganev',
     'author_email': 'dganev@vmware.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `carbon_black_cloud_threat_intelligence_connector-1.4/PKG-INFO` & `carbon_black_cloud_threat_intelligence_connector-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-black-cloud-threat-intelligence-connector
-Version: 1.4
+Version: 1.5
 Summary: Carbon Black Cloud Threat Intelligence Connector
 License: BSD-2-Clause
 Keywords: connector,carbonblackcloud,stixtaxii,stix,taxii
 Author: Dimitar Ganev
 Author-email: dganev@vmware.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

