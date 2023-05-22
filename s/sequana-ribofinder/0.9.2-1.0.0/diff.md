# Comparing `tmp/sequana_ribofinder-0.9.2.tar.gz` & `tmp/sequana_ribofinder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_ribofinder-0.9.2.tar", last modified: Mon Sep 28 13:00:09 2020, max compression
+gzip compressed data, was "dist/sequana_ribofinder-1.0.0.tar", last modified: Mon May 22 14:22:12 2023, max compression
```

## Comparing `sequana_ribofinder-0.9.2.tar` & `sequana_ribofinder-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      128 2020-09-25 19:46:10.000000 sequana_ribofinder-0.9.2/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4019 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2235 2020-09-28 12:58:56.000000 sequana_ribofinder-0.9.2/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       33 2020-09-28 12:59:44.000000 sequana_ribofinder-0.9.2/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      128 2020-09-25 19:46:10.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3075 2020-09-28 12:49:43.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    18938 2020-09-25 20:59:48.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/dag.png
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-25 19:46:10.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)   896937 2020-09-28 12:43:44.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/data/data_R1_.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9279 2020-09-28 12:47:30.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/data/feature.fasta
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     4875 2020-09-28 10:01:14.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4586 2020-09-25 21:37:33.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/multiqc_config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       15 2020-09-28 08:37:36.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6334 2020-09-28 12:51:43.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/ribofinder.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1698 2020-09-25 21:53:18.000000 sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/schema.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4019 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      855 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-09-25 20:53:02.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       33 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-09-28 13:00:08.000000 sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      256 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3321 2020-09-25 22:05:52.000000 sequana_ribofinder-0.9.2/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-09-28 13:00:09.000000 sequana_ribofinder-0.9.2/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1305 2020-09-28 12:56:23.000000 sequana_ribofinder-0.9.2/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    20253 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/dag.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5506 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4586 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12017 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/ribofinder.rules
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/test/test_main.py
```

### Comparing `sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/config.yaml` & `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # ==================[ Sections for the users ]================================
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
-input_directory: "."
+input_directory:
 input_readtag: _R[12]_
 input_pattern: '*fastq.gz'
 # =========================================== Sections for the users
 
 #############################################################################
 # Genome section:
 #
@@ -29,31 +29,27 @@
 #   it to True. Indexing is followed by force_indexing to make sure we do not
 #   erase the index files, which may be large.
 #
 #   Only one annotation file must be provided. If so, we extract the feature
 #   rRNA from the annotation, identifiy start/end and create fasta file on the
 #   fly. You may simply provide an input fasta file with rRNA if you have one.
 general:
-    aligner: bowtie1 
-    rRNA_file: ""
+    aligner: bowtie1
+    rRNA_file: ''
     rRNA_feature: rRNA
-    genbank_file: 
+    genbank_file: ''
     gff_file:
-    reference_file: 
-
-
-
-######################
-# if files are required for a pipeline and are within sequana or should
-# be downloaded before the pipeline provide them in this section
-# Note that sequana and url fields are followed by itemised files or links
-# using the front dashes
-requirements: ''
-
+    reference_file:
 
+apptainers:
+    sequana_ribofinder: "https://zenodo.org/record/7348115/files/sequana_ribofinder_0.12.0.img"
+    pigz: "https://zenodo.org/record/7346805/files/pigz_2.4.0.img"
+    bedtools: "https://zenodo.org/record/7346774/files/bedtools_2.30.0.img"
+    samtools: "https://zenodo.org/record/7215278/files/samtools_1.15.0.img"
+    graphviz:  "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
 
 #############################################################################
 # bowtie1_mapping_rna used to align reads against ribosomal RNA
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored
@@ -75,12 +71,13 @@
 # :Parameters:
 #
 # - options: any options recognised by multiqc
 # - output-directory: Create report in the specified output directory
 # - config_file: by default, we use sequana RNA-seq multiqc_config file. 
 #       If you want your own multiqc, fill this entry
 multiqc:
-    options: -f -x *_init_* -x *left_kept_reads* -x *fastqc_samples* -e htseq -e slamdunk
-    output_directory: multiqc
+    options: -f
+    input_directory: .
+    modules: ""
     config_file: multiqc_config.yaml
```

### Comparing `sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/main.py` & `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,30 @@
+#
+#  This file is part of Sequana software
+#
+#  Copyright (c) 2016 - Sequana Development Team
+#
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
-import shutil
+import subprocess
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
+from sequana_pipetools import SequanaManager
+from sequana import logger
 
 col = Colors()
 
 NAME = "ribofinder"
 
 
 class Options(argparse.ArgumentParser):
@@ -50,14 +65,16 @@
             default=None,
             help="""If provided, do not provide genbank""")
         pipeline_group.add_argument("--reference-file",
             default=None,
             help="""The required referenceto fetch features into""")
 
 
+        self.add_argument("--run", default=False, action="store_true",
+            help="execute the pipeline directly")
 
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
             if len(args_list)>2:
                 msg = "WARNING [sequana]: With --from-project option, " + \
                         "pipeline and data-related options will be ignored."
@@ -71,30 +88,24 @@
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
     # whatever needs to be called by all pipeline before the options parsing
-    from sequana_pipetools.options import before_pipeline
     before_pipeline(NAME)
 
-    # option parsing including common epil and og
+    # option parsing including common epilog
     options = Options(NAME, epilog=sequana_epilog).parse_args(args[1:])
 
-
-    from sequana.pipelines_common import SequanaManager
-
     # the real stuff is here
     manager = SequanaManager(options, NAME)
 
     # create the beginning of the command and the working directory
     manager.setup()
-    from sequana import logger
-    logger.level = options.level
 
     # fill the config file with input parameters
     if options.from_project is None:
         cfg = manager.config.config
 
         # --------------------------------------------------------- general
         cfg.general.aligner = options.aligner
@@ -105,34 +116,35 @@
         if options.genbank_file:
             cfg.general.genbank_file = os.path.abspath(options.genbank_file)
         if options.gff_file:
             cfg.general.gff_file = os.path.abspath(options.gff_file)
         if options.reference_file:
             cfg.general.reference_file = os.path.abspath(options.reference_file)
 
-
         if options.reference_file is None and options.rRNA_file is None:
             logger.error("You must provide a rRNA file or a reference_file")
             sys.exit(1)
 
         if options.reference_file:
             logger.info("checking your input GFF file and rRNA feature if provided")
             if options.genbank_file:
                 from sequana.genbank import GenBank
                 gbk = GenBank(options.genbank_file)
             if options.genbank_file is None and options.gff_file is None:
-                logger.error("You must provide an annotation (genbank-file or gff-file)")
-                sys.exit(1)
+                logger.error("Most probably you want to provide an annotation (genbank-file or gff-file)")
+                sys.exit(0)
 
         # ----------------------------------------------------  others
-        cfg.input_directory = os.path.abspath(options.input_directory)
         cfg.input_pattern = options.input_pattern
+        cfg.input_directory = os.path.abspath(options.input_directory)
         cfg.input_readtag = options.input_readtag
 
-
-
+        manager.exists(cfg.input_directory)
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
+    if options.run:
+        subprocess.Popen(["sh", '{}.sh'.format(NAME)], cwd=options.workdir)
+
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/multiqc_config.yaml` & `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-0.9.2/sequana_pipelines/ribofinder/schema.yaml` & `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/schema.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
         required: True
     "input_readtag":
         type: str
         required: True
     "input_pattern":
         type: str
         required: True
+    "apptainers":
+        type: any
 
     "general":
         type: map
         mapping:
             "aligner":
                 type: str
                 required: True
@@ -37,38 +39,38 @@
             "options":
                 type: str
             "threads":
                 type: int
                 required: True
                 range: { min: 1 }
 
-    'coverage':
+
+    'bowtie1_mapping_rna':
         type: map
         mapping:
             "do":
                 type: bool
-            "binSize":
-                type: int
-            "genomeSize":
-                type: int
-            "extendReads":
-                type: int
-            "minFragmentLength":
-                type: int
-            "maxFragmentLength":
-                type: int
+            "options":
+                type: str
             "threads":
                 type: int
                 required: True
-                range: { min: 1, max: 8 }
+                range: { min: 1}
 
-    'bowtie1_mapping_rna':
+    "multiqc":
         type: map
         mapping:
             "do":
-                type: bool
+              type: bool
             "options":
                 type: str
-            "threads":
-                type: int
-                required: True
-                range: { min: 1}
+            "config_file":
+                type: str
+            "input_directory":
+                type: str
+            "output_directory":
+                type: str
+            "modules":
+                type: str
+
+
+
```

### Comparing `sequana_ribofinder-0.9.2/sequana_ribofinder.egg-info/SOURCES.txt` & `sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 sequana_pipelines/ribofinder/config.yaml
 sequana_pipelines/ribofinder/dag.png
 sequana_pipelines/ribofinder/main.py
 sequana_pipelines/ribofinder/multiqc_config.yaml
 sequana_pipelines/ribofinder/requirements.txt
 sequana_pipelines/ribofinder/ribofinder.rules
 sequana_pipelines/ribofinder/schema.yaml
-sequana_pipelines/ribofinder/data/__init__.py
-sequana_pipelines/ribofinder/data/data_R1_.fastq.gz
-sequana_pipelines/ribofinder/data/feature.fasta
 sequana_ribofinder.egg-info/PKG-INFO
 sequana_ribofinder.egg-info/SOURCES.txt
 sequana_ribofinder.egg-info/dependency_links.txt
 sequana_ribofinder.egg-info/entry_points.txt
 sequana_ribofinder.egg-info/not-zip-safe
 sequana_ribofinder.egg-info/requires.txt
 sequana_ribofinder.egg-info/top_level.txt
```

### Comparing `sequana_ribofinder-0.9.2/test/test_main.py` & `sequana_ribofinder-1.0.0/test/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 import easydev
 import os
 import tempfile
 import subprocess
 import sys
-from sequana.pipelines_common import get_pipeline_location as getpath
 
-sharedir = getpath('ribofinder')
+from . import test_dir
 
+sharedir = f"{test_dir}/data"
 
 def test_standalone_subprocess():
     directory = tempfile.TemporaryDirectory()
-    cmd = """sequana_pipelines_ribofinder --input-directory {} 
+    cmd = """sequana_ribofinder --input-directory {} 
             --working-directory {} --force""".format(sharedir, directory.name)
     subprocess.call(cmd.split())
 
 
 def test_standalone_script():
     directory = tempfile.TemporaryDirectory()
     import sequana_pipelines.ribofinder.main as m
     sys.argv = ["test", "--input-directory", sharedir, 
             "--working-directory", directory.name, "--force", "--rRNA-file", sharedir+"feature.fasta"]
     m.main()
 
-def test_full():
+
+def test_full_rRNA_file():
     with tempfile.TemporaryDirectory() as directory:
         wk = directory
-
-        cmd = "sequana_pipelines_ribofinder --input-directory {} "
-        cmd += "--working-directory {}  --force --rRNA-file {}/feature.fasta"
-        cmd = cmd.format(sharedir, wk, sharedir)
-        print(cmd)
+        cmd = f"sequana_ribofinder --input-directory {sharedir} "
+        cmd += f"--working-directory {wk}  --force --rRNA-file {sharedir}/feature.fasta"
         subprocess.call(cmd.split())
+        stat = subprocess.call("sh ribofinder.sh".split(), cwd=wk)
+        assert os.path.exists(wk + "/summary.html")
 
+def test_full_rRNA_extract():
+    with tempfile.TemporaryDirectory() as directory:
+        wk = directory
+        cmd = f"sequana_ribofinder --input-directory {sharedir} "
+        cmd += f"--working-directory {wk}  --force --reference-file {sharedir}/Lepto.fa --gff-file {sharedir}/Lepto.gff"
+        subprocess.call(cmd.split())
         stat = subprocess.call("sh ribofinder.sh".split(), cwd=wk)
 
-        assert os.path.exists(wk + "/summary.html")
+
+        if os.path.exists(wk + "/summary.html"):
+            pass
+        else:
+            with open(f"{wk}/indexing/bowtie_rRNA.log", "r") as fout: 
+                print(fout.read())
+            raise IOError
 
 def test_version():
-    cmd = "sequana_pipelines_ribofinder --version"
+    cmd = "sequana_ribofinder --version"
     subprocess.call(cmd.split())
```

