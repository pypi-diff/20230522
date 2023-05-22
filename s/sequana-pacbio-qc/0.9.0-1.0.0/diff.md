# Comparing `tmp/sequana_pacbio_qc-0.9.0.tar.gz` & `tmp/sequana_pacbio_qc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_pacbio_qc-0.9.0.tar", last modified: Tue Dec  1 13:17:22 2020, max compression
+gzip compressed data, was "dist/sequana_pacbio_qc-1.0.0.tar", last modified: Mon May 22 15:58:04 2023, max compression
```

## Comparing `sequana_pacbio_qc-0.9.0.tar` & `sequana_pacbio_qc-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5765 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3713 2020-12-01 13:16:55.000000 sequana_pacbio_qc-0.9.0/README.rst
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5765 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      805 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      145 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-11-28 18:23:36.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        8 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2020-06-02 19:54:21.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      821 2020-12-01 11:16:27.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/config.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-06-02 19:54:21.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/data/__init__.py
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)   363770 2020-06-02 19:54:21.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/data/lima_output.lbc32--lbc32.ccs.bam
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)   949820 2020-06-02 19:54:21.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/data/lima_output.lbc43--lbc43.ccs.bam
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     4782 2020-12-01 11:15:57.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5333 2020-12-01 11:53:47.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    10155 2020-12-01 12:03:32.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       16 2020-12-01 12:03:58.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      350 2020-12-01 11:17:20.000000 sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      255 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2776 2020-12-01 13:14:51.000000 sequana_pacbio_qc-0.9.0/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-12-01 13:17:22.000000 sequana_pacbio_qc-0.9.0/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1750 2020-12-01 13:11:25.000000 sequana_pacbio_qc-0.9.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4693 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    17653 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/dag.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4787 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5333 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14043 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2772 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/setup.py
```

### Comparing `sequana_pacbio_qc-0.9.0/PKG-INFO` & `sequana_pacbio_qc-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sequana_pacbio_qc
-Version: 0.9.0
+Version: 1.0.0
 Summary: QC on various type of pacbio data
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -13,46 +13,59 @@
         .. image:: https://badge.fury.io/py/sequana-pacbio-qc.svg
              :target: https://pypi.python.org/pypi/sequana_pacbio_qc
         
         .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
             :target: http://joss.theoj.org/papers/10.21105/joss.00352
             :alt: JOSS (journal of open source software) DOI
         
+        .. image:: https://github.com/sequana/pacbio_qc/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/pacbio_qc/actions/workflows    
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+           :target: http://joss.theoj.org/papers/10.21105/joss.00352
+           :alt: JOSS (journal of open source software) DOI
+        
+        |Codacy-Grade|
+        
         
         This is is the **pacbio_qc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
         
-        :Overview: Quality control for pacbio BAM files (raw data or CCS files)
-        :Input: BAM files provided by Pacbio Sequencers
+        :Overview: Quality control for pacbio datafiles (raw data or CCS files). 
+        
+        :Input: BAM files provided by Pacbio Sequencers. 
         :Output: HTML reports with various plots including taxonomic plot
         :Status: production
+        :Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
         :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
         
         
         Installation
         ~~~~~~~~~~~~
         
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
+        Just install this package::
         
             pip install sequana_pacbio_qc
         
+        You will need **samtools** and  **kraken2** (optional) for the taxonomic analysis.
+        
         
         Usage
         ~~~~~
         
         ::
         
-            sequana_pipelines_pacbio_qc --help
-            sequana_pipelines_pacbio_qc --input-directory DATAPATH
+            sequana_pacbio_qc --help
+            sequana_pacbio_qc --input-directory DATAPATH
         
         
-        iIf you want to filter out some BAM files, you may use the pattern in tab 'input data'.
+        If you want to filter out some BAM files, you may use the pattern in tab 'input data'.
         
         In the configuration tab, in the kraken section add as many databases
         as you wish. You may simply unset the first database to skip the taxonomy, which
         is experimental.
         
         
         This creates a directory with the pipeline and configuration file. You will then need
@@ -62,78 +75,90 @@
             sh pacbio_qc.sh  # for a local run
         
         This launch a snakemake pipeline. If you are familiar with snakemake, you can 
         retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
         
             snakemake -s pacbio_qc.rules -c config.yaml --cores 4 --stats stats.txt
         
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
         
         Requirements
         ~~~~~~~~~~~~
         
         This pipelines requires the following executable(s):
         
         - sequana
+        - samtools
         - kraken2
         - multiqc
         
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/dag.png
+        .. image:: https://raw.githubusercontent.com/sequana/pacbio_qc/main/sequana_pipelines/pacbio_qc/dag.png
         
         
         Details
         ~~~~~~~~~
         
         This pipeline takes as inputs a set of BAM files from Pacbio sequencers. It
         computes a set of basic statistics related to the read lengths. It also shows
-        some histograms related to the GC content, SNR of the diodes and the so-called ZMW
-        values. Finally, a quick taxonomy can be performed using Kraken. HTML reports
+        some histograms related to the GC content, SNR of the diodes and the number of passes
+        Finally, a quick taxonomy can be performed using Kraken. HTML reports
         are created for each sample as well as a multiqc summary page.
         
         Kraken databases are not provided with the pipeline. This step is optional and
-        not used by default. 
+        not used by default.
         
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.0     Uses latest wrappers and graphviz apptainers
+        0.11.0    Release to use latests sequana_pipetools framework
+        0.10.0    Update to use latest tools from sequana framework
         0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
                   modules (0.9.5)
         ========= ====================================================================
         
         
         Contribute & Code of Conduct
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         To contribute to this project, please take a look at the 
-        `Contributing Guidelines <https://github.com/sequana/sequana/blob/master/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
-        `Code of Conduct <https://github.com/sequana/sequana/blob/master/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
+        `Contributing Guidelines <https://github.com/sequana/sequana/blob/main/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+        `Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
         
         
         Rules and configuration details
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/config.yaml>`_
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/main/sequana_pipelines/pacbio_qc/config.yaml>`_
         to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
         
         
+        
+        .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/9b8355ff642f4de9acd4b270f8d14d10
+           :target: https://www.codacy.com/gh/sequana/pacbio_qc/dashboard
+        
+        
 Keywords: pacbio, snakemake, NGS, sequana
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
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
```

### Comparing `sequana_pacbio_qc-0.9.0/README.rst` & `sequana_pacbio_qc-1.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -3,46 +3,59 @@
 .. image:: https://badge.fury.io/py/sequana-pacbio-qc.svg
      :target: https://pypi.python.org/pypi/sequana_pacbio_qc
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
     :target: http://joss.theoj.org/papers/10.21105/joss.00352
     :alt: JOSS (journal of open source software) DOI
 
+.. image:: https://github.com/sequana/pacbio_qc/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/sequana/pacbio_qc/actions/workflows    
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
+
+|Codacy-Grade|
+
 
 This is is the **pacbio_qc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
 
-:Overview: Quality control for pacbio BAM files (raw data or CCS files)
-:Input: BAM files provided by Pacbio Sequencers
+:Overview: Quality control for pacbio datafiles (raw data or CCS files). 
+
+:Input: BAM files provided by Pacbio Sequencers. 
 :Output: HTML reports with various plots including taxonomic plot
 :Status: production
+:Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
 :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
 
 
 Installation
 ~~~~~~~~~~~~
 
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
+Just install this package::
 
     pip install sequana_pacbio_qc
 
+You will need **samtools** and  **kraken2** (optional) for the taxonomic analysis.
+
 
 Usage
 ~~~~~
 
 ::
 
-    sequana_pipelines_pacbio_qc --help
-    sequana_pipelines_pacbio_qc --input-directory DATAPATH
+    sequana_pacbio_qc --help
+    sequana_pacbio_qc --input-directory DATAPATH
 
 
-iIf you want to filter out some BAM files, you may use the pattern in tab 'input data'.
+If you want to filter out some BAM files, you may use the pattern in tab 'input data'.
 
 In the configuration tab, in the kraken section add as many databases
 as you wish. You may simply unset the first database to skip the taxonomy, which
 is experimental.
 
 
 This creates a directory with the pipeline and configuration file. You will then need
@@ -52,58 +65,67 @@
     sh pacbio_qc.sh  # for a local run
 
 This launch a snakemake pipeline. If you are familiar with snakemake, you can 
 retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
 
     snakemake -s pacbio_qc.rules -c config.yaml --cores 4 --stats stats.txt
 
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
 
 - sequana
+- samtools
 - kraken2
 - multiqc
 
-.. image:: https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/dag.png
+.. image:: https://raw.githubusercontent.com/sequana/pacbio_qc/main/sequana_pipelines/pacbio_qc/dag.png
 
 
 Details
 ~~~~~~~~~
 
 This pipeline takes as inputs a set of BAM files from Pacbio sequencers. It
 computes a set of basic statistics related to the read lengths. It also shows
-some histograms related to the GC content, SNR of the diodes and the so-called ZMW
-values. Finally, a quick taxonomy can be performed using Kraken. HTML reports
+some histograms related to the GC content, SNR of the diodes and the number of passes
+Finally, a quick taxonomy can be performed using Kraken. HTML reports
 are created for each sample as well as a multiqc summary page.
 
 Kraken databases are not provided with the pipeline. This step is optional and
-not used by default. 
+not used by default.
 
 
 Changelog
 ~~~~~~~~~
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.0.0     Uses latest wrappers and graphviz apptainers
+0.11.0    Release to use latests sequana_pipetools framework
+0.10.0    Update to use latest tools from sequana framework
 0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
           modules (0.9.5)
 ========= ====================================================================
 
 
 Contribute & Code of Conduct
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To contribute to this project, please take a look at the 
-`Contributing Guidelines <https://github.com/sequana/sequana/blob/master/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
-`Code of Conduct <https://github.com/sequana/sequana/blob/master/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
+`Contributing Guidelines <https://github.com/sequana/sequana/blob/main/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+`Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
 
 
 Rules and configuration details
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/config.yaml>`_
+Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/main/sequana_pipelines/pacbio_qc/config.yaml>`_
 to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
 
+
+
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/9b8355ff642f4de9acd4b270f8d14d10
+   :target: https://www.codacy.com/gh/sequana/pacbio_qc/dashboard
+
```

### Comparing `sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/PKG-INFO` & `sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sequana-pacbio-qc
-Version: 0.9.0
+Version: 1.0.0
 Summary: QC on various type of pacbio data
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -13,46 +13,59 @@
         .. image:: https://badge.fury.io/py/sequana-pacbio-qc.svg
              :target: https://pypi.python.org/pypi/sequana_pacbio_qc
         
         .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
             :target: http://joss.theoj.org/papers/10.21105/joss.00352
             :alt: JOSS (journal of open source software) DOI
         
+        .. image:: https://github.com/sequana/pacbio_qc/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/pacbio_qc/actions/workflows    
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+           :target: http://joss.theoj.org/papers/10.21105/joss.00352
+           :alt: JOSS (journal of open source software) DOI
+        
+        |Codacy-Grade|
+        
         
         This is is the **pacbio_qc** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
         
-        :Overview: Quality control for pacbio BAM files (raw data or CCS files)
-        :Input: BAM files provided by Pacbio Sequencers
+        :Overview: Quality control for pacbio datafiles (raw data or CCS files). 
+        
+        :Input: BAM files provided by Pacbio Sequencers. 
         :Output: HTML reports with various plots including taxonomic plot
         :Status: production
+        :Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
         :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
         
         
         Installation
         ~~~~~~~~~~~~
         
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
+        Just install this package::
         
             pip install sequana_pacbio_qc
         
+        You will need **samtools** and  **kraken2** (optional) for the taxonomic analysis.
+        
         
         Usage
         ~~~~~
         
         ::
         
-            sequana_pipelines_pacbio_qc --help
-            sequana_pipelines_pacbio_qc --input-directory DATAPATH
+            sequana_pacbio_qc --help
+            sequana_pacbio_qc --input-directory DATAPATH
         
         
-        iIf you want to filter out some BAM files, you may use the pattern in tab 'input data'.
+        If you want to filter out some BAM files, you may use the pattern in tab 'input data'.
         
         In the configuration tab, in the kraken section add as many databases
         as you wish. You may simply unset the first database to skip the taxonomy, which
         is experimental.
         
         
         This creates a directory with the pipeline and configuration file. You will then need
@@ -62,78 +75,90 @@
             sh pacbio_qc.sh  # for a local run
         
         This launch a snakemake pipeline. If you are familiar with snakemake, you can 
         retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
         
             snakemake -s pacbio_qc.rules -c config.yaml --cores 4 --stats stats.txt
         
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
         
         Requirements
         ~~~~~~~~~~~~
         
         This pipelines requires the following executable(s):
         
         - sequana
+        - samtools
         - kraken2
         - multiqc
         
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/dag.png
+        .. image:: https://raw.githubusercontent.com/sequana/pacbio_qc/main/sequana_pipelines/pacbio_qc/dag.png
         
         
         Details
         ~~~~~~~~~
         
         This pipeline takes as inputs a set of BAM files from Pacbio sequencers. It
         computes a set of basic statistics related to the read lengths. It also shows
-        some histograms related to the GC content, SNR of the diodes and the so-called ZMW
-        values. Finally, a quick taxonomy can be performed using Kraken. HTML reports
+        some histograms related to the GC content, SNR of the diodes and the number of passes
+        Finally, a quick taxonomy can be performed using Kraken. HTML reports
         are created for each sample as well as a multiqc summary page.
         
         Kraken databases are not provided with the pipeline. This step is optional and
-        not used by default. 
+        not used by default.
         
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.0     Uses latest wrappers and graphviz apptainers
+        0.11.0    Release to use latests sequana_pipetools framework
+        0.10.0    Update to use latest tools from sequana framework
         0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
                   modules (0.9.5)
         ========= ====================================================================
         
         
         Contribute & Code of Conduct
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         To contribute to this project, please take a look at the 
-        `Contributing Guidelines <https://github.com/sequana/sequana/blob/master/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
-        `Code of Conduct <https://github.com/sequana/sequana/blob/master/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
+        `Contributing Guidelines <https://github.com/sequana/sequana/blob/main/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+        `Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
         
         
         Rules and configuration details
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/master/sequana_pipelines/pacbio_qc/config.yaml>`_
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_pacbio_qc/main/sequana_pipelines/pacbio_qc/config.yaml>`_
         to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
         
         
+        
+        .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/9b8355ff642f4de9acd4b270f8d14d10
+           :target: https://www.codacy.com/gh/sequana/pacbio_qc/dashboard
+        
+        
 Keywords: pacbio, snakemake, NGS, sequana
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
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
```

### Comparing `sequana_pacbio_qc-0.9.0/sequana_pacbio_qc.egg-info/SOURCES.txt` & `sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+MANIFEST.in
 README.rst
+requirements.txt
 setup.cfg
 setup.py
 sequana_pacbio_qc.egg-info/PKG-INFO
 sequana_pacbio_qc.egg-info/SOURCES.txt
 sequana_pacbio_qc.egg-info/dependency_links.txt
 sequana_pacbio_qc.egg-info/entry_points.txt
 sequana_pacbio_qc.egg-info/not-zip-safe
 sequana_pacbio_qc.egg-info/requires.txt
 sequana_pacbio_qc.egg-info/top_level.txt
 sequana_pipelines/pacbio_qc/__init__.py
 sequana_pipelines/pacbio_qc/config.yaml
+sequana_pipelines/pacbio_qc/dag.png
 sequana_pipelines/pacbio_qc/main.py
 sequana_pipelines/pacbio_qc/multiqc_config.yaml
 sequana_pipelines/pacbio_qc/pacbio_qc.rules
 sequana_pipelines/pacbio_qc/requirements.txt
-sequana_pipelines/pacbio_qc/schema.yaml
-sequana_pipelines/pacbio_qc/data/__init__.py
-sequana_pipelines/pacbio_qc/data/lima_output.lbc32--lbc32.ccs.bam
-sequana_pipelines/pacbio_qc/data/lima_output.lbc43--lbc43.ccs.bam
-test/test_main.py
+sequana_pipelines/pacbio_qc/schema.yaml
```

### Comparing `sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/main.py` & `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # -*- coding: utf-8 -*-
 #
 #  This file is part of Sequana software
 #
-#  Copyright (c) 2016 - Sequana Development Team
-#
-#  File author(s):
-#      Thomas Cokelaer <thomas.cokelaer@pasteur.fr>
+#  Copyright (c) 2016-2023 - Sequana Development Team
 #
 #  Distributed under the terms of the 3-clause BSD license.
 #  The full license is in the LICENSE file, distributed with this software.
 #
 #  website: https://github.com/sequana/sequana
 #  documentation: http://sequana.readthedocs.io
 #
 ##############################################################################
 import sys
 import os
 import argparse
+import shutil
 import subprocess
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
+from sequana_pipetools import SequanaManager
 
 col = Colors()
 
 NAME = "pacbio_qc"
 
-# FIXME update sequana_pipetools
 class MyKrakenOptions():
     def __init__(self, group_name="section_kraken"):
         self.group_name = group_name
 
     def add_options(self, parser):
         group = parser.add_argument_group(self.group_name)
 
@@ -48,17 +47,20 @@
                 You may use several, in which case, an iterative taxonomy is
                 performed as explained in online sequana documentation""")
 
 
 class Options(argparse.ArgumentParser):
     def __init__(self, prog=NAME, epilog=None):
         usage = col.purple(sequana_prolog.format(**{"name": NAME}))
-        super(Options, self).__init__(usage=usage, prog=prog, description="",
+        super(Options, self).__init__(
+            usage=usage,
+            prog=prog,
+            description="",
             epilog=epilog,
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
         # add a new group of options to the parser
         so = SlurmOptions()
         so.add_options(self)
 
         # add a snakemake group of options to the parser
         so = SnakemakeOptions(working_directory=NAME)
@@ -94,23 +96,19 @@
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
     # whatever needs to be called by all pipeline before the options parsing
-    from sequana_pipetools.options import before_pipeline
     before_pipeline(NAME)
 
     # option parsing including common epilog
     options = Options(NAME, epilog=sequana_epilog).parse_args(args[1:])
 
-
-    from sequana.pipelines_common import SequanaManager
-
     # the real stuff is here
     manager = SequanaManager(options, NAME)
 
     # create the beginning of the command and the working directory
     manager.setup()
 
     # fill the config file with input parameters
@@ -128,17 +126,19 @@
             cfg.kraken.do = False
 
         if options.kraken_databases:
             cfg.kraken.databases =  [os.path.abspath(x)
                                      for x in options.kraken_databases]
             for this in options.kraken_databases:
                 manager.exists(this)
+            # if a DB is provided, let us update this field:
+            cfg.kraken.do = True
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
-    manager.teardown(check_fastq_files=False)
+    manager.teardown()
 
     if options.run:
         subprocess.Popen(["sh", '{}.sh'.format(NAME)], cwd=options.workdir)
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml` & `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-0.9.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules` & `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 #
 #  This file is part of Sequana software
 #
-#  Copyright (c) 2016-2020 - Sequana Development Team
+#  Copyright (c) 2016-2021 - Sequana Development Team
 #
 #  File author(s):
 #      Thomas Cokelaer <thomas.cokelaer@pasteur.fr>
 #
 #  Distributed under the terms of the 3-clause BSD license.
 #  The full license is in the LICENSE file, distributed with this software.
 #
@@ -14,87 +13,186 @@
 #  documentation: http://sequana.readthedocs.io
 #
 ##############################################################################
 
 import os
 
 from sequana import pacbio, sequana_data
-from sequana import snaketools as sm
+from sequana_pipetools import snaketools as sm
 
+# ========================================================= The main config file
 # This must be defined before the include
 configfile: "config.yaml"
+sequana_wrapper_branch = "main"
 
-# Generic include of some dynamic modules
 
-# A convenient manager
 def func(filename):
     # pacbio data are either BAM of FastQ files
     # if BAM, they may contain a .css.bam extension if the data is made of CCS
     # if output of LIMA tool, you may also have a barcode info such as
     # lbc32-lbc32 and so on. So a file may be called lima_output.lbc32.ccs.bam
     # and the next one lima_output.lb33.ccs.bam. Therefore the sample name is
     # only contaons in the barcode. Removing .ccs.bam is a solution
-    # So we will remove the first extension (e.g. .bam, .fastq) including
+    # So we will remove the first extension (e.g. .bam) including
     # possible compressed extension
     filename = filename.split("/")[-1]
     if filename.endswith(".bam"):
         return filename.rsplit(".bam")[0]
-    elif filename.endswith(".fastq"):
-        return filename.rsplit(".fastq")[0]
-    elif filename.endswith(".fastq.gz"):
-        return filename.rsplit(".fastq.gz")[0]
     else:
-        raise IOError("Input files must end in .bam, .fastq, or .fastq.gz")
-manager = sm.PipelineManagerGeneric("pacbio_qc", config, sample_func=func)
-manager.setup(globals(), mode="warning")
+        raise IOError("Input files must end in .bam")
 
 
-input_data = manager.getrawdata()
+# ================================================== The sequana pipeline manager
+manager = sm.PipelineManager("pacbio_qc", config, sample_func=func)
+if len(manager.samples) == 0:
+    logger.error("Could not find any sample")
+    sys.exit(1)
 
 
-to_clean = []
+# =========================================================  Final results
+rule pipeline:
+    input:
+        expand("{sample}/summary.html", sample=manager.samples),
+        ".sequana/rulegraph.svg",
+        "multiqc/multiqc_report.html", "summary.json"
+
+
+# =========================================================  bam to fasta (for kraken)
+if config['kraken']['do']:
+    rule bam_to_fasta:
+        input:
+            manager.getrawdata()
+        output:
+            temp("tmp/{sample}.fasta")
+        threads:
+            config['bam_to_fasta']['thread']
+        run:
+            from sequana import pacbio, FastQ
+            if input[0].endswith(".bam"):
+                p = pacbio.PacbioSubreads(input[0])
+                p.to_fasta(output[0], threads=threads)
+            else:
+                f = FastQ(input[0])
+                f.to_fasta(output[0])
+
+
+
+# Analysis the input BAM/Fastq , create pictures and summary file
+
+
+rule pacbio_quality:
+    """Pacbio quality control
+
+    Required input:
+        - __pacbio_quality__input : the input BAM file
+
+    Required output:
+        - __pacbio_quality__output_summary: summary_{sample}.json
+
+    Optional parameters:
+        - __pacbio_quality__images_directory: where to save PNG
+          images (default to ./images)
+
+    In addition to a summary file with basic statistics, this
+    rules creates 5 images with basic histograms about the read
+    lengths, the GC content, the ZMW information, the SNR of the
+    A,C,G,T nucleotides, and a 2D histogram of GC versus read length
+
+    References:
+        `sequana.pacbio <http://sequana.readthedocs.io/en/master/references.html#sequana.pacbio.PacbioSubreads>`_
+
+    """
+    input: manager.getrawdata()
+    params:
+        sample_name = "{sample}"
+    output:
+        read_len   = "{sample}/images/hist_read_len_{sample}.png",
+        GC_content = "{sample}/images/GC_content_{sample}.png",
+        ZMW        = "{sample}/images/ZMW_passes_{sample}.png",
+        SNR        = "{sample}/images/SNR_{sample}.png",
+        GC_vs_len  = "{sample}/images/GC_vs_len_{sample}.png",
+        summary    = "{sample}/sequana_summary_pacbio_qc_{sample}.json"
+    run:
+        from sequana import pacbio
+        import pylab
+        def setname(name):
+            return name
+        ########## labels for plots
+        short_name = input[0].replace(".bam","").split("/")[-1]
+        bam_pacbio = pacbio.PacbioSubreads(input[0])
+
+        ########## Read length
+        # individual histograms
+        bam_pacbio.hist_read_length(label=short_name)
+        pylab.title("")
+        pylab.legend()
+        pylab.savefig(setname(output.read_len))
+
+        ########## GC content
+        # individual histograms
+        bam_pacbio.hist_GC(label=short_name)
+        pylab.title("")
+        pylab.legend()
+        pylab.savefig(setname(output.GC_content))
+
+        ########## ZMW passes
+        # individual histograms
+        bam_pacbio.hist_nb_passes(label=short_name, bins=20)
+        pylab.title("")
+        pylab.legend()
+        pylab.savefig(setname(output.ZMW))
+
+        ########## SNR
+        # individual histograms
+        bam_pacbio.hist_snr()
+        pylab.title("")
+        pylab.savefig(setname(output.SNR))
+
+        # plot GC versus read length
+        bam_pacbio.plot_GC_read_len()
+        pylab.title("")
+        pylab.savefig(setname(output.GC_vs_len))
+
+        # summary
+        summary = bam_pacbio.summary()
+        with open(output.summary, "w") as fh:
+            summary.update(
+                {"images":
+                    {"hist_read_length": output.read_len,
+                    "hist_gc_content": output.GC_content,
+                    "hist_snr": output.SNR,
+                    "gc_vs_length": output.GC_vs_len,
+                    "hist_zmw": output.ZMW}
+                })
+            summary.update({'sample': params.sample_name})
+            summary.update({'generator': "sequana_pacbio_quality"})
+            json.dump(summary, fh, indent=True, sort_keys=True)
+        pylab.close()
+
 
-# Convert the BAM to fasta
-__bam_to_fasta__input_bam = input_data
-__bam_to_fasta__output_fasta = "{sample}.fasta"
-include: sm.modules["bam_to_fasta"]
-to_clean = []
 
 
-# Analysis the input Fasta , create pictures and summary file
-__pacbio_quality__input = input_data
-__pacbio_quality__sample_name = "{sample}"
-__pacbio_quality__output_summary = "{sample}/sequana_summary_pacbio_qc_{sample}.json"
-include: sm.modules["pacbio_quality"]
-to_clean.extend(expand(__bam_to_fasta__output_fasta, sample=manager.samples))
 
 
 # default output for the html_reports rule
 __html_report__input =  ["{sample}/sequana_summary_pacbio_qc_{sample}.json"]
 
 # Do we need the kraken output ? if so, fill variables
 extra_kraken = []
 if config['kraken']['do'] is True:
-    __kraken__html_output = "{sample}/kraken/kraken.html"
-    extra_kraken = expand(__kraken__html_output, sample=manager.samples)
-    __html_report__input +=  [__kraken__html_output]
-
-
-# Final results
-rule pipeline:
-    input:
-        expand("{sample}/summary.html", sample=manager.samples), 
-        ".sequana/rulegraph.svg",
-        "multiqc/multiqc_report.html", "summary.json"
+    extra_kraken = expand("{sample}/kraken/kraken.html", sample=manager.samples)
+    __html_report__input +=  ["{sample}/kraken/kraken.html"]
 
 
 # HTML reports
 rule html_report:
-    input:  __html_report__input
-    output: "{sample}/summary.html"
+    input:
+        __html_report__input
+    output:
+        "{sample}/summary.html"
     params:
         dir_kraken="{sample}/kraken",
         dir="{sample}"
     message: "create the pacbio BAM QC summary page"
     run:
         from sequana.modules_report.pacbio_input_bam import PacbioInputBAMModule as Module
 
@@ -110,122 +208,159 @@
 
         # Here, we just re-run the KrakenModule to get the HTML content
         # We do not want to save it
         if config['kraken']['do']:
             from sequana.modules_report.kraken import KrakenModule
             kr = KrakenModule(params.dir_kraken, output_filename=None)
             html = kr._get_summary_section()
-            #toreplace = "./kraken/kraken.html"
-            #target = params.dir_kraken + "kraken.html"
-            #html = html.replace(toreplace, target)
             m.sections.append({
               "name": "Taxonomic content",
               "anchor": "kraken",
               "content": html
             })
         # In the rule kraken:, a summary.html is created, which is overwritten
         # here
         m.create_html(output[0])
 
 
 # The kraken analysis
-rule kraken:
-    input: "{sample}.fasta"
-    output: "{sample}/kraken/kraken.html"
+rule sequana_taxonomy:
+    input:
+        "tmp/{sample}.fasta"
+    output:
+        "{sample}/kraken/kraken.html"
     params:
         databases=config['kraken']['databases']
-    threads: config['kraken']['thread']
-    run:
-        cmd = "sequana_taxonomy --file1 {input} --output-directory {wildcards.sample} --thread {threads} "
-        cmd += " --databases "
-        for dbname in params.databases:
-            cmd += " {} ".format(dbname)
-        shell(cmd)
+    container:
+        config['apptainers']['sequana']
+    threads:
+        config['kraken']['thread']
+    shell:
+        """
+
+        sequana_taxonomy --file1 {input} --output-directory {wildcards.sample} --thread {threads} --databases {params.databases}
+
+        """
+
+
+# ========================================================== multiqc
+
+
+sequana_multiqc_input = expand("{sample}/sequana_summary_pacbio_qc_{sample}.json", 
+    sample=manager.samples) + extra_kraken
+
+
+#config['multiqc']['options'] = config["multiqc"]["options"] + f" --comment '{comments}'"
+
 
-# FIXME resuse existing rules from sequana
 rule multiqc:
-    input: expand(__pacbio_quality__output_summary, sample=manager.samples) + extra_kraken
-    output: "multiqc/multiqc_report.html"
+    input:
+        sequana_multiqc_input
+    output:
+        "multiqc/multiqc_report.html"
     params:
-        config="multiqc_config.yaml"
-    run:
-        from subprocess import Popen
-        cmd = "multiqc . -f -m sequana_pacbio_qc -c {} -o multiqc".format(params.config)
-        process = Popen(cmd.split(), stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-        process.wait()
+       options=config['multiqc']['options'],
+       input_directory=config['multiqc']['input_directory'],
+       config_file=config['multiqc']['config_file'],
+       modules=config['multiqc']['modules']
+    log:
+       "multiqc/multiqc.log"
+    wrapper:
+       f"{sequana_wrapper_branch}/wrappers/multiqc"
 
 
 rule plotting_and_stats:
-    input: expand(__pacbio_quality__output_summary, sample=manager.samples)
+    input: expand("{sample}/sequana_summary_pacbio_qc_{sample}.json", sample=manager.samples)
+
     output: "summary.json"#, "summary.png"
     run:
+        import json
         from sequana.summary import Summary
         from sequana_pipelines.pacbio_qc import version
 
         summary = Summary("pacbioqc", caller="sequana_pacbio_qc", sample_name="multi samples")
         summary.description = "summary sequana_pacbio_qc pipeline"
         summary.pipeline_version = version
 
-        import json
         for filename in input:
             data = json.load(open(filename, 'r'))
             sample = data['sample']
             summary.data[sample] = data['read_stats']
             summary.data[sample]['sample'] = sample
 
         summary.to_json("summary.json")
 
 
 
-__rulegraph__input = manager.snakefile
-__rulegraph__output = ".sequana/rulegraph.svg"
-__rulegraph__mapper = {"multiqc": "../multiqc/multiqc_report.html"}
-include: sm.modules['rulegraph']
-localrules: rulegraph
+# ====================================================================== rulegraph
+
+rule rulegraph:
+    input: str(manager.snakefile)
+    output:
+        svg = "rulegraph/rulegraph.dot"
+    params:
+        mapper = {"multiqc": "../multiqc/multiqc_report.html"},
+        configname = "config.yaml"
+    wrapper:
+        f"{sequana_wrapper_branch}/wrappers/rulegraph"
+
 
+rule dot2svg:
+    input:
+        "rulegraph/rulegraph.dot"
+    output:
+        ".sequana/rulegraph.svg"
+    container:
+        config['apptainers']['graphviz']
+    shell:
+        """dot -Tsvg {input} -o {output}"""
 
 
-localrules: multiqc, rulegraph
+
+
+localrules: multiqc, rulegraph, plotting_and_stats
 
 
 onsuccess:
-    for this in to_clean:
-        try:os.remove(this)
-        except:pass
 
-    # This was create by calling Module but is not needed
+    # This was created by calling Module but is not needed
     shell('rm -rf css images js')
 
-
     from sequana import logger
-    logger.level = "INFO"
+    logger.setLevel("INFO")
 
     # This should create the stats plot and the Makefile
     manager.teardown()
     manager.clean_multiqc("multiqc/multiqc_report.html")
 
     # Now, the main HTML report
     import pandas as pd
     from sequana.utils.datatables_js import DataTable
     import json
 
-    # Summary table with links towards fastqc 
+    # Summary table with links towards fastqc
     data = json.load(open("summary.json", "r"))
     df = pd.DataFrame(data['data'])
     df = df.T
     del df['sample']
     df = df.reset_index().rename({'index': 'sample'}, axis=1)
-    for col in ['count', 'nb_reads', 'nb_bases', 'min', 'max', 'CCS_mean_passes', 'CCS_nb_reads']:
+    for col in ['count', 'nb_reads', 'nb_bases', 'min', 'max']:
         try: df[col] = [int(x) for x in df[col]]
         except: pass
-    for col in ['mean', 'mean_GC', 'std']:
+    for col in ['mean', 'mean_GC', 'std', "mean_passes"]:
         try: df[col] = [round(float(x), 2) for x in df[col]]
         except: pass
-    for col in ['25%','50%','75%']:
+    for col in ["25%","50%","75%", "count"]:
         del df[col]
+    df = df.rename({
+            "min":"min_read_length", 
+            "max":"max_read_length",
+            "std":"std_read_length",
+            "mean":"mean_length"}, axis=1)
+
 
     df['link'] = ["{}/summary.html".format(x) for x in df['sample']] 
 
     datatable = DataTable(df, 'pacbio_qc', index=False)
     datatable.datatable.datatable_options = {'paging': 'false',
                                               'buttons': ['copy', 'csv'],
                                              'bSort': 'true',
@@ -250,15 +385,15 @@
     js2 = datatable.create_javascript_function()
     htmltable2 = datatable.create_datatable(style="width: 20%; float:left" )
 
 
     from sequana.modules_report.summary import SummaryModule2
     data = {
             "name": manager.name,
-            "rulegraph": __rulegraph__output,
+            "rulegraph": ".sequana/rulegraph.svg",
             "stats": "stats.txt",
             "pipeline_version": vv
 
          }
 
     # Here the is main HTML page report
     contents = "<h2> General information</h2>"
@@ -276,13 +411,16 @@
     s = SummaryModule2(data, intro=contents)
 
 
     # finally, some cleanup
     shell("rm -rf rulegraph")   # embedded in report
     shell("chmod -R g+w .")
 
-
+onerror:
+    from sequana_pipetools.errors import PipeError
+    p = PipeError("pacbio_qc")
+    p.status()
```

### Comparing `sequana_pacbio_qc-0.9.0/setup.py` & `sequana_pacbio_qc-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-# -*- coding: utf-8 -*-
-# License: 3-clause BSD
-__revision__ = "$Id: $" # for the SVN Id
 from setuptools import setup, find_namespace_packages
 
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
     'license' : 'new BSD',
     'url' : "https://github.com/sequana/",
     'description': "QC on various type of pacbio data" ,
     'platforms' : ['Linux', 'Unix', 'MacOsX', 'Windows'],
     'keywords' : ['pacbio, snakemake, NGS, sequana'],
     'classifiers' : [
-          #'Development Status :: 4 - Beta',
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
 
@@ -40,35 +37,40 @@
     name             = "sequana_pacbio_qc",
     version          = version,
     maintainer       = metainfo['authors']['main'][0],
     maintainer_email = metainfo['authors']['main'][1],
     author           = metainfo['authors']['main'][0],
     author_email     = metainfo['authors']['main'][1],
     long_description = open("README.rst").read(),
+    long_description_content_type = "text/x-rst",
     keywords         = metainfo['keywords'],
     description      = metainfo['description'],
     license          = metainfo['license'],
     platforms        = metainfo['platforms'],
     url              = metainfo['url'],
     classifiers      = metainfo['classifiers'],
 
     # package installation
-    packages = ["sequana_pipelines.pacbio_qc",
-        'sequana_pipelines.pacbio_qc.data' ],
-
-    install_requires = "sequana",
+    packages = ["sequana_pipelines.pacbio_qc"],
 
+    install_requires = open("requirements.txt").read(),
+    extras_require={
+        "testing": [
+            "pytest",
+            "pytest-cov",
+            "pytest-xdist",
+            "coveralls",
+        ],
+    },
     # This is recursive include of data files
     exclude_package_data = {"": ["__pycache__"]},
     package_data = {
-        '': ['*.yaml', "*.rules", "*.json", "requirements.txt"],
-        'sequana_pipelines.pacbio_qc.data' : ['*.*'], 
+        '': ['*.yaml', "*.rules", "*.json", "requirements.txt", "*png", "*yml", "*smk"]
         },
 
     zip_safe=False,
 
     entry_points = {'console_scripts':[
-        'sequana_pipelines_pacbio_qc=sequana_pipelines.pacbio_qc.main:main',
         'sequana_pacbio_qc=sequana_pipelines.pacbio_qc.main:main']
     }
 
 )
```

