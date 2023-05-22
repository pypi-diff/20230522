# Comparing `tmp/sequana_revcomp-0.9.0.tar.gz` & `tmp/sequana_revcomp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_revcomp-0.9.0.tar", last modified: Tue Aug 30 21:20:48 2022, max compression
+gzip compressed data, was "dist/sequana_revcomp-1.0.0.tar", last modified: Mon May 22 20:39:52 2023, max compression
```

## Comparing `sequana_revcomp-0.9.0.tar` & `sequana_revcomp-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,23 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/.github/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/.github/workflows/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1390 2022-08-30 20:52:35.000000 sequana_revcomp-0.9.0/.github/workflows/main.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      965 2022-08-30 20:41:25.000000 sequana_revcomp-0.9.0/.github/workflows/pypi.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       70 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/.gitignore
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2022-08-30 20:40:02.000000 sequana_revcomp-0.9.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4765 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3502 2022-08-30 20:50:47.000000 sequana_revcomp-0.9.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2022-08-30 20:39:43.000000 sequana_revcomp-0.9.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      696 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/config.yaml
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     3721 2022-08-30 20:30:27.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        6 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1290 2022-08-30 20:36:53.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/revcomp.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      427 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/sequana_pipelines/revcomp/schema.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4765 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      691 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       72 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-08-30 19:56:06.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/sequana_revcomp.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      253 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3146 2022-08-30 20:54:28.000000 sequana_revcomp-0.9.0/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-08-30 21:20:48.000000 sequana_revcomp-0.9.0/singularity/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       56 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/singularity/Makefile
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      442 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/singularity/Singularity
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       54 2022-08-09 13:15:05.000000 sequana_revcomp-0.9.0/upload.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3721 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/revcomp.rules
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/sequana_pipelines/revcomp/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/sequana_revcomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-22 20:39:52.000000 sequana_revcomp-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-05-22 20:39:47.000000 sequana_revcomp-1.0.0/setup.py
```

### Comparing `sequana_revcomp-0.9.0/PKG-INFO` & `sequana_revcomp-1.0.0/sequana_revcomp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,136 +1,123 @@
-Metadata-Version: 2.1
-Name: sequana_revcomp
-Version: 0.9.0
+Metadata-Version: 1.2
+Name: sequana-revcomp
+Version: 1.0.0
 Summary: reverse complement a set of FastQ files
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: 
+        .. image:: https://badge.fury.io/py/sequana-revcomp.svg
+             :target: https://pypi.python.org/pypi/sequana_revcomp
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/revcomp/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/revcomp/actions/workflows    
+        
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        This is is the **revcomp** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+        
+        :Overview: revert and complement input Fast files
+        :Input: A set of FastQ files (paired or single-end) compressed or not
+        :Output: A set of reverse completed files
+        :Status: production
+        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+        
+        
+        
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        If you already have all requirements, you can install the packages using pip::
+        
+            pip install sequana_mapper --upgrade
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_revcomp --input-directory DATAPATH 
+        
+        This creates a directory with the pipeline and configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd revcomp
+            sh revcomp.sh  # for a local run
+            make clean
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s revcomp.rules -c config.yaml --cores 4 \
+                --wrapper-prefix https://raw.githubusercontent.com/sequana/sequana-wrappers/
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - seqtk
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs **seqtk** in parallel on the input fastq files.
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_revcomp/main/sequana_pipelines/revcomp/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ======================================================================
+        Version   Description
+        ========= ======================================================================
+        0.9.0     * set singularity container
+        0.8.4     * implemented --from-project option
+        0.8.3     * Uses new sequana framework to spee up --help calls
+                  * --threads option
+        0.8.2     Fix schema and rule. output files are now saved in the ./rc directory
+        0.8.1     Improve the --help message
+        0.8.0     First version from sequana 0.8.0
+        ========= ======================================================================
+        
 Keywords: fastq, reverse complement, snakemake, NGS,sequana
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE
-
-
-.. image:: https://badge.fury.io/py/sequana-revcomp.svg
-     :target: https://pypi.python.org/pypi/sequana_revcomp
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/revcomp/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/revcomp/actions/workflows    
-
-
-
-This is is the **revcomp** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-
-:Overview: revert and complement input Fast files
-:Input: A set of FastQ files (paired or single-end) compressed or not
-:Output: A set of reverse completed files
-:Status: production
-:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-:Authors: Thomas Cokelaer
-
-
-
-This is is the **fastqc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-
-:Overview: Runs fastqc and multiqc on a set of Sequencing data to produce control quality reports
-:Input: A set of FastQ files (paired or single-end) compressed or not
-:Output: an HTML file summary.html (individual fastqc reports, mutli-samples report)
-:Status: production
-:Wiki: https://github.com/sequana/fastqc/wiki
-:Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
-:Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
-
-
-Installation
-~~~~~~~~~~~~
-
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
-
-    pip install sequana_revcomp
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_pipelines_revcomp --input-directory DATAPATH 
-
-This creates a directory with the pipeline and configuration file. You will then need 
-to execute the pipeline::
-
-    cd revcomp
-    sh revcomp.sh  # for a local run
-    make clean
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s revcomp.rules -c config.yaml --cores 4 --stats stats.txt
-
-Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- seqtk
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs **seqtk** in parallel on the input fastq files.
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_revcomp/main/sequana_pipelines/revcomp/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-
-Changelog
-~~~~~~~~~
-
-========= ======================================================================
-Version   Description
-========= ======================================================================
-0.8.4     * implemented --from-project option
-0.8.3     * Uses new sequana framework to spee up --help calls
-          * --threads option
-0.8.2     Fix schema and rule. output files are now saved in the ./rc directory
-0.8.1     Improve the --help message
-0.8.0     First version from sequana 0.8.0
-========= ======================================================================
-
-
```

### Comparing `sequana_revcomp-0.9.0/README.rst` & `sequana_revcomp-1.0.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -6,67 +6,56 @@
     :target: http://joss.theoj.org/papers/10.21105/joss.00352
     :alt: JOSS (journal of open source software) DOI
 
 .. image:: https://github.com/sequana/revcomp/actions/workflows/main.yml/badge.svg
    :target: https://github.com/sequana/revcomp/actions/workflows    
 
 
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
 
 This is is the **revcomp** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
 
 :Overview: revert and complement input Fast files
 :Input: A set of FastQ files (paired or single-end) compressed or not
 :Output: A set of reverse completed files
 :Status: production
 :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-:Authors: Thomas Cokelaer
 
 
 
-This is is the **fastqc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-
-:Overview: Runs fastqc and multiqc on a set of Sequencing data to produce control quality reports
-:Input: A set of FastQ files (paired or single-end) compressed or not
-:Output: an HTML file summary.html (individual fastqc reports, mutli-samples report)
-:Status: production
-:Wiki: https://github.com/sequana/fastqc/wiki
-:Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
-:Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
 
 
 Installation
 ~~~~~~~~~~~~
 
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
-
-    pip install sequana_revcomp
+If you already have all requirements, you can install the packages using pip::
 
+    pip install sequana_mapper --upgrade
 
 Usage
 ~~~~~
 
 ::
 
-    sequana_pipelines_revcomp --input-directory DATAPATH 
+    sequana_revcomp --input-directory DATAPATH 
 
 This creates a directory with the pipeline and configuration file. You will then need 
 to execute the pipeline::
 
     cd revcomp
     sh revcomp.sh  # for a local run
     make clean
 
 This launch a snakemake pipeline. If you are familiar with snakemake, you can 
 retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
 
-    snakemake -s revcomp.rules -c config.yaml --cores 4 --stats stats.txt
+    snakemake -s revcomp.rules -c config.yaml --cores 4 \
+        --wrapper-prefix https://raw.githubusercontent.com/sequana/sequana-wrappers/
 
 Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
@@ -89,14 +78,15 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ======================================================================
 Version   Description
 ========= ======================================================================
+0.9.0     * set singularity container
 0.8.4     * implemented --from-project option
 0.8.3     * Uses new sequana framework to spee up --help calls
           * --threads option
 0.8.2     Fix schema and rule. output files are now saved in the ./rc directory
 0.8.1     Improve the --help message
 0.8.0     First version from sequana 0.8.0
 ========= ======================================================================
```

### Comparing `sequana_revcomp-0.9.0/sequana_pipelines/revcomp/main.py` & `sequana_revcomp-1.0.0/sequana_pipelines/revcomp/main.py`

 * *Files identical despite different names*

### Comparing `sequana_revcomp-0.9.0/sequana_pipelines/revcomp/revcomp.rules` & `sequana_revcomp-1.0.0/sequana_pipelines/revcomp/revcomp.rules`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     input:
         manager.getrawdata()
     output:
         "rc/{sample}.fastq.gz"
     log:
         temp("logs/{sample}.logs")
     container:
-        "https://zenodo.org/record/5729951/files/seqtk_1.3.0.img" 
+        config["apptainers"]["seqtk"]
     shell:
         """
         # -k means keep original data
         # the container does not contain pigz.
         #seqtk seq -r  {input}  | pigz -p {threads} -fk - --stdout > {output}  2> {log}
         seqtk seq -r  {input}  | gzip -fk -c > {output}  2> {log}
         """
```

### Comparing `sequana_revcomp-0.9.0/sequana_revcomp.egg-info/PKG-INFO` & `sequana_revcomp-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,123 @@
-Metadata-Version: 2.1
-Name: sequana-revcomp
-Version: 0.9.0
+Metadata-Version: 1.2
+Name: sequana_revcomp
+Version: 1.0.0
 Summary: reverse complement a set of FastQ files
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: 
+        .. image:: https://badge.fury.io/py/sequana-revcomp.svg
+             :target: https://pypi.python.org/pypi/sequana_revcomp
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/revcomp/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/revcomp/actions/workflows    
+        
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        This is is the **revcomp** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+        
+        :Overview: revert and complement input Fast files
+        :Input: A set of FastQ files (paired or single-end) compressed or not
+        :Output: A set of reverse completed files
+        :Status: production
+        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+        
+        
+        
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        If you already have all requirements, you can install the packages using pip::
+        
+            pip install sequana_mapper --upgrade
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_revcomp --input-directory DATAPATH 
+        
+        This creates a directory with the pipeline and configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd revcomp
+            sh revcomp.sh  # for a local run
+            make clean
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s revcomp.rules -c config.yaml --cores 4 \
+                --wrapper-prefix https://raw.githubusercontent.com/sequana/sequana-wrappers/
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - seqtk
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs **seqtk** in parallel on the input fastq files.
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_revcomp/main/sequana_pipelines/revcomp/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ======================================================================
+        Version   Description
+        ========= ======================================================================
+        0.9.0     * set singularity container
+        0.8.4     * implemented --from-project option
+        0.8.3     * Uses new sequana framework to spee up --help calls
+                  * --threads option
+        0.8.2     Fix schema and rule. output files are now saved in the ./rc directory
+        0.8.1     Improve the --help message
+        0.8.0     First version from sequana 0.8.0
+        ========= ======================================================================
+        
 Keywords: fastq, reverse complement, snakemake, NGS,sequana
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE
-
-
-.. image:: https://badge.fury.io/py/sequana-revcomp.svg
-     :target: https://pypi.python.org/pypi/sequana_revcomp
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/revcomp/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/revcomp/actions/workflows    
-
-
-
-This is is the **revcomp** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-
-:Overview: revert and complement input Fast files
-:Input: A set of FastQ files (paired or single-end) compressed or not
-:Output: A set of reverse completed files
-:Status: production
-:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-:Authors: Thomas Cokelaer
-
-
-
-This is is the **fastqc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-
-:Overview: Runs fastqc and multiqc on a set of Sequencing data to produce control quality reports
-:Input: A set of FastQ files (paired or single-end) compressed or not
-:Output: an HTML file summary.html (individual fastqc reports, mutli-samples report)
-:Status: production
-:Wiki: https://github.com/sequana/fastqc/wiki
-:Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
-:Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
-
-
-Installation
-~~~~~~~~~~~~
-
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
-
-    pip install sequana_revcomp
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_pipelines_revcomp --input-directory DATAPATH 
-
-This creates a directory with the pipeline and configuration file. You will then need 
-to execute the pipeline::
-
-    cd revcomp
-    sh revcomp.sh  # for a local run
-    make clean
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s revcomp.rules -c config.yaml --cores 4 --stats stats.txt
-
-Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- seqtk
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs **seqtk** in parallel on the input fastq files.
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_revcomp/main/sequana_pipelines/revcomp/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-
-Changelog
-~~~~~~~~~
-
-========= ======================================================================
-Version   Description
-========= ======================================================================
-0.8.4     * implemented --from-project option
-0.8.3     * Uses new sequana framework to spee up --help calls
-          * --threads option
-0.8.2     Fix schema and rule. output files are now saved in the ./rc directory
-0.8.1     Improve the --help message
-0.8.0     First version from sequana 0.8.0
-========= ======================================================================
-
-
```

### Comparing `sequana_revcomp-0.9.0/setup.py` & `sequana_revcomp-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # License: 3-clause BSD
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
-_MAJOR               = 0
-_MINOR               = 9
+_MAJOR               = 1
+_MINOR               = 0
 _MICRO               = 0
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
@@ -23,17 +23,17 @@
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
```

