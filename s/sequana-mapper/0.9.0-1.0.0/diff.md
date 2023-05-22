# Comparing `tmp/sequana_mapper-0.9.0.tar.gz` & `tmp/sequana_mapper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_mapper-0.9.0.tar", last modified: Fri Apr 16 11:19:41 2021, max compression
+gzip compressed data, was "dist/sequana_mapper-1.0.0.tar", last modified: Mon May 22 11:44:48 2023, max compression
```

## Comparing `sequana_mapper-0.9.0.tar` & `sequana_mapper-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,26 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      128 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5702 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3633 2021-04-16 11:16:07.000000 sequana_mapper-0.9.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2021-04-16 09:53:13.000000 sequana_mapper-0.9.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5702 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1225 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      133 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-08-27 18:29:51.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_mapper.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2832 2021-04-16 11:12:26.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    23647 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/dag.png
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   102820 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/data2_R1_.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   106241 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/data2_R2_.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   117634 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/data_R1_.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   120952 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/data_R2_.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16122 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)       10 2021-04-16 10:01:31.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.amb
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)       51 2021-04-16 10:01:31.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.ann
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)    15988 2021-04-16 10:01:32.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.bwt
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)       23 2021-04-16 10:01:31.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.fai
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)     3975 2021-04-16 10:01:31.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.pac
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)     8000 2021-04-16 10:01:31.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/data/measles.fa.sa
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11238 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/logo.png
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     4134 2021-04-16 11:12:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8720 2021-04-16 11:10:47.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/mapper.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5221 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/multiqc_config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       61 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2825 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/sequana_pipelines/mapper/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      252 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3354 2021-04-16 11:15:57.000000 sequana_mapper-0.9.0/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2021-04-16 11:19:41.000000 sequana_mapper-0.9.0/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1691 2020-06-02 19:53:13.000000 sequana_mapper-0.9.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7626 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5216 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7626 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 11:44:47.000000 sequana_mapper-1.0.0/sequana_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3724 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    55200 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11238 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5235 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12190 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/mapper.rules
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/sequana_pipelines/mapper/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-22 11:44:48.000000 sequana_mapper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-05-22 11:44:41.000000 sequana_mapper-1.0.0/setup.py
```

### Comparing `sequana_mapper-0.9.0/PKG-INFO` & `sequana_mapper-1.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-Metadata-Version: 1.2
-Name: sequana_mapper
-Version: 0.9.0
-Summary: A simple mapper to map reads onto a reference. This is useful for quick QCs and also secondary analysis
-Home-page: https://github.com/sequana/
-Author: thomas cokelaer
-Author-email: thomas.cokelaer@pasteur.fr
-Maintainer: thomas cokelaer
-Maintainer-email: thomas.cokelaer@pasteur.fr
-License: new BSD
-Description: This is is the **mapper** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-        
-        :Overview: This is a simple pipeline to map several FastQ files onto a reference using different mappers/aligners
-        :Input: A set of FastQ files (illumina, pacbio, etc).
-        :Output: A set of BAM files (and/or bigwig) and HTML report
-        :Status: Production
-        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
-        
-            pip install sequana_mapper
-        
-        
-        Usage
-        ~~~~~
-        
-        ::
-        
-            sequana_pipelines_mapper --input-directory DATAPATH  --mapper bwa --create-bigwig
-            sequana_pipelines_mapper --input-directory DATAPATH  --mapper bwa --do-coverage
-        
-        This creates a directory with the pipeline and configuration file. You will then need 
-        to execute the pipeline::
-        
-            cd mapper
-            sh mapper.sh  # for a local run
-        
-        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-        
-            snakemake -s mapper.rules -c config.yaml --cores 4 --stats stats.txt
-        
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        This pipelines requires the following executable(s):
-        
-        - bamtools
-        - bwa
-        - multiqc
-        - sequana_coverage
-        - minimap2
-        - bowtie2
-        - deeptools
-        
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_mapper/master/sequana_pipelines/mapper/dag.png
-        
-        
-        Details
-        ~~~~~~~~~
-        
-        This pipeline runs **mapper** in parallel on the input fastq files (paired or not). 
-        A brief sequana summary report is also produced. When using **--pacbio** option, 
-        *-x map-pb* options ia automatically added to the config.yaml file and the
-        readtag is set to None. 
-        
-        
-        
-        Rules and configuration details
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_mapper/master/sequana_pipelines/mapper/config.yaml>`_
-        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-        
-        
-        Changelog
-        ~~~~~~~~~
-        
-        ========= ====================================================================
-        Version   Description
-        ========= ====================================================================
-        0.9.0     * fix issue with logger and increments requirements
-                  * add new option --pacbio to automatically set the options for 
-                    pacbio data (-x map-pb and readtag set to None)
-        0.8.13    * add the thread option in minimap2 case
-        0.8.12    * factorise multiqc rule
-        0.8.11    * Implemente the --from-project option and new framework
-                  * custom HTMrLl report
-        0.8.10    * change samtools_depth rule and switched to bam2cov to cope with null
-                    coverage 
-        0.8.9     * fix requirements
-        0.8.8     * fix pipeline rule for bigwig + renamed output_bigwig into
-                    create_bigwig; fix the multiqc config file
-        0.8.7     * fix config file creation (for bigwig)
-        0.8.6     * added bowtie2 mapper + bigwig as output, make coverage optional
-        0.8.5     * create a sym link to the HTML report. Better post cleaning.
-        0.8.4     * Fixing multiqc (synchronized with sequana updates) 
-        0.8.3     * add sequana_coverage rule. 
-        0.8.2     * add minimap2 mapper 
-        0.8.1     * fix bamtools stats rule to have different output name for multiqc
-        0.8.0     **First release.**
-        ========= ====================================================================
-        
-        
-Keywords: snakemake, sequana, bwa, bowtie2, minimap2
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
+
+.. image:: https://badge.fury.io/py/sequana-mapper.svg
+     :target: https://pypi.python.org/pypi/sequana_mapper
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+    :target: http://joss.theoj.org/papers/10.21105/joss.00352
+    :alt: JOSS (journal of open source software) DOI
+
+.. image:: https://github.com/sequana/mapper/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/sequana/mapper/actions/    
+
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
+
+This is the **mapper** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+
+:Overview: This is a simple pipeline to map several FastQ files onto a reference using different mappers/aligners
+:Input: A set of FastQ files (illumina, pacbio, etc).
+:Output: A set of BAM files (and/or bigwig) and HTML report
+:Status: Production
+:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+
+
+Installation
+~~~~~~~~~~~~
+
+If you already have all requirements, you can install the packages using pip::
+
+    pip install sequana_mapper --upgrade
+
+Usage
+~~~~~
+
+::
+
+    sequana_mapper --input-directory DATAPATH  --mapper bwa --create-bigwig
+    sequana_mapper --input-directory DATAPATH  --mapper bwa --do-coverage
+
+This creates a directory with the pipeline and configuration file. You will then need 
+to execute the pipeline::
+
+    cd mapper
+    sh mapper.sh  # for a local run
+
+This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+
+    snakemake -s mapper.rules -c config.yaml --cores 4 \
+        --wrapper-prefix https://raw.githubusercontent.com/sequana/sequana-wrappers/
+
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+
+Requirements
+~~~~~~~~~~~~
+
+This pipelines requires the following executable(s):
+
+- bamtools
+- bwa
+- multiqc
+- sequana_coverage
+- minimap2
+- bowtie2
+- deeptools
+
+.. image:: https://raw.githubusercontent.com/sequana/mapper/main/sequana_pipelines/mapper/dag.png
+
+
+Details
+~~~~~~~~~
+
+This pipeline runs **mapper** in parallel on the input fastq files (paired or not). 
+A brief sequana summary report is also produced. When using **--pacbio** option, 
+*-x map-pb* options is automatically added to the config.yaml file and the
+readtag is set to None. 
+
+
+
+Rules and configuration details
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/mapper/main/sequana_pipelines/mapper/config.yaml>`_
+to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+
+
+Changelog
+~~~~~~~~~
+
+========= ======================================================================
+Version   Description
+========= ======================================================================
+1.0.0     * Use latest sequana-wrappers and graphviz apptainer
+0.12.0    * Use latest pipetools and add singularity containers
+0.11.1    * Fix typo when setting coverage to True and allow untagged filenames
+0.11.0    * implement feature counts for capture-seq projects
+0.10.1    * remove getlogdir and getname
+0.10.0    * use new wrappers framework 
+0.9.0     * fix issue with logger and increments requirements
+          * add new option --pacbio to automatically set the options for 
+            pacbio data (-x map-pb and readtag set to None)
+0.8.13    * add the thread option in minimap2 case
+0.8.12    * factorise multiqc rule
+0.8.11    * Implemente the --from-project option and new framework
+          * custom HTMrLl report
+0.8.10    * change samtools_depth rule and switched to bam2cov to cope with null
+            coverage 
+0.8.9     * fix requirements
+0.8.8     * fix pipeline rule for bigwig + renamed output_bigwig into
+            create_bigwig; fix the multiqc config file
+0.8.7     * fix config file creation (for bigwig)
+0.8.6     * added bowtie2 mapper + bigwig as output, make coverage optional
+0.8.5     * create a sym link to the HTML report. Better post cleaning.
+0.8.4     * Fixing multiqc (synchronized with sequana updates) 
+0.8.3     * add sequana_coverage rule. 
+0.8.2     * add minimap2 mapper 
+0.8.1     * fix bamtools stats rule to have different output name for multiqc
+0.8.0     **First release.**
+========= ======================================================================
+
+
+Contribute & Code of Conduct
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To contribute to this project, please take a look at the 
+`Contributing Guidelines <https://github.com/sequana/sequana/blob/main/CONTRIBUTING.rst>`_ first. Please note that this project is released with a 
+`Code of Conduct <https://github.com/sequana/sequana/blob/main/CONDUCT.md>`_. By contributing to this project, you agree to abide by its terms.
+
```

### Comparing `sequana_mapper-0.9.0/sequana_pipelines/mapper/logo.png` & `sequana_mapper-1.0.0/sequana_pipelines/mapper/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_mapper-0.9.0/sequana_pipelines/mapper/main.py` & `sequana_mapper-1.0.0/sequana_pipelines/mapper/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,44 @@
+#
+#  This file is part of Sequana software
+#
+#  Copyright (c) 2016-2021 - Sequana Development Team
+##
+#  Distributed under the terms of the 3-clause BSD license.
+#  The full license is in the LICENSE file, distributed with this software.
+#
+#  website: https://github.com/sequana/sequana
+#  documentation: http://sequana.readthedocs.io
+#
+##############################################################################
 import sys
 import os
 import argparse
+import subprocess
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
+from sequana_pipetools import SequanaManager
 
 col = Colors()
 
 NAME = "mapper"
 
 
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
@@ -29,60 +47,65 @@
         so = InputOptions()
         so.add_options(self)
 
         so = GeneralOptions()
         so.add_options(self)
 
         pipeline_group = self.add_argument_group("pipeline")
-        pipeline_group.add_argument("--mapper", default='bwa',
-             choices=['bwa', 'minimap2', 'bowtie2'], 
-            help="Choose one of the valid mapper")
-        pipeline_group.add_argument("--reference-file", required=True,
-             help="You input reference file in fasta format")
-        pipeline_group.add_argument("--annotation-file",
-            help="Used by the sequana_coverage tool if provided" )
+        pipeline_group.add_argument(
+            "--mapper", default="bwa", choices=["bwa", "minimap2", "bowtie2"], help="Choose one of the valid mapper"
+        )
+        pipeline_group.add_argument("--reference-file", required=True, help="You input reference file in fasta format")
+        pipeline_group.add_argument("--annotation-file", help="Used by the sequana_coverage tool if provided")
+
+        pipeline_group.add_argument("--do-coverage", action="store_true", help="Use sequana_coverage (prokaryotes)")
 
-        pipeline_group.add_argument("--do-coverage", action="store_true",
-            help="Use sequana_coverage (prokaryotes)" )
+        pipeline_group.add_argument(
+            "--pacbio",
+            action="store_true",
+            help="If set, automatically set the input-readtag to None and set minimap2 options to -x map-pb",
+        )
 
-        pipeline_group.add_argument("--pacbio", action="store_true",
-            help="If set, automatically set the input-readtag to None and set minimap2 options to -x map-pb" )
+        pipeline_group.add_argument(
+            "--create-bigwig", action="store_true", help="create the bigwig files from the BAM files"
+        )
+        pipeline_group.add_argument(
+            "--capture-annotation-file",
+            help="SAF formatted file for capture efficiency calculation with featureCounts.",
+        )
 
-        pipeline_group.add_argument("--create-bigwig", action="store_true",
-            help="create the bigwig files from the BAM files" )
+        self.add_argument("--run", default=False, action="store_true", help="execute the pipeline directly")
 
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
-            if len(args_list)>2:
-                msg = "WARNING [sequana]: With --from-project option, " + \
-                        "pipeline and data-related options will be ignored."
+            if len(args_list) > 2:
+                msg = (
+                    "WARNING [sequana]: With --from-project option, "
+                    + "pipeline and data-related options will be ignored."
+                )
                 print(col.error(msg))
             for action in self._actions:
                 if action.required is True:
                     action.required = False
         options = super(Options, self).parse_args(*args)
         return options
 
 
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
@@ -108,16 +131,22 @@
         if options.create_bigwig:
             cfg.general.create_bigwig = True
 
         if options.pacbio:
             cfg.minimap2.options = " -x map-pb "
             cfg.input_readtag = ""
 
-
+        if options.capture_annotation_file:
+            cfg.feature_counts.do = True
+            cfg.feature_counts.options = "-F SAF "
+            cfg.feature_counts.gff = os.path.abspath(options.capture_annotation_file)
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
+    if options.run:
+        subprocess.Popen(["sh", "{}.sh".format(NAME)], cwd=options.workdir)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_mapper-0.9.0/sequana_pipelines/mapper/multiqc_config.yaml` & `sequana_mapper-1.0.0/sequana_pipelines/mapper/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_mapper-0.9.0/sequana_pipelines/mapper/schema.yaml` & `sequana_mapper-1.0.0/sequana_pipelines/mapper/schema.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,31 @@
     "input_readtag":
         type: str
         required: False
     "input_pattern":
         type: str
         required: True
 
+    "apptainers":
+        type: any
+
     "general":
         type: map
         mapping:
             "mapper":
                 type: str
                 enum: [bwa, minimap2, bowtie2]
             "reference_file":
                 type: str
             "annotation_file":
                 type: str
             "create_bigwig":
                 type: bool
 
-    "bwa_mem_mapping":
+    "bwa":
         type: map
         mapping:
             "index_algorithm":
                 type: str 
             "options":
                 type: str 
             "threads":
@@ -39,15 +42,19 @@
                 type: str 
 
     "multiqc":
         type: map
         mapping:
             "options":
                 type: str
-            "indir":
+            "modules":
+                type: str
+            "config_file":
+                type: str
+            "input_directory":
                 type: str
 
     "minimap2": 
         type: map
         mapping:
             "options":
                 type: str
@@ -101,18 +108,51 @@
             "cnv_clustering":
                 type: int
                 range: { min: -1 }
             "gc_window_size":
                 type: int
                 range: { min: 2}
 
-    "bowtie2_mapping_ref":
+    "bowtie2":
         type: map
         mapping:
             "options": 
                 type: str
             "threads": 
                 type: int
                 range: { min: 1 }
 
+    "bowtie2_index":
+        type: map
+        mapping:
+            "options": 
+                type: str
+            "threads": 
+                type: int
+                range: { min: 1 }
 
+    "bwa_index":
+        type: map
+        mapping:
+            "options": 
+                type: str
+            "threads": 
+                type: int
+                range: { min: 1 }
+
+    "feature_counts":
+        type: map
+        mapping:
+            "do":
+              type: bool
+            "options":
+                type: str
+            "gff":
+                type: str
+            "feature":
+                type: str
+            "attribute":
+                type: str
+            "threads":
+                type: int
+                range: { min: 1 }
```

