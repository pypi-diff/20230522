# Comparing `tmp/peeling-0.1.0.tar.gz` & `tmp/peeling-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peeling-0.1.0.tar", last modified: Thu Mar 30 15:47:50 2023, max compression
+gzip compressed data, was "peeling-0.2.0.tar", last modified: Mon May 22 18:46:18 2023, max compression
```

## Comparing `peeling-0.1.0.tar` & `peeling-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-03-30 15:47:50.200512 peeling-0.1.0/
--rw-r--r--   0 pengxi     (501) staff       (20)     1518 2023-03-17 23:12:16.000000 peeling-0.1.0/LICENSE
--rw-r--r--   0 pengxi     (501) staff       (20)     9001 2023-03-30 15:47:50.200169 peeling-0.1.0/PKG-INFO
--rw-r--r--   0 pengxi     (501) staff       (20)     6912 2023-03-28 15:37:12.000000 peeling-0.1.0/README.md
-drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-03-30 15:47:50.192224 peeling-0.1.0/peeling/
--rw-r--r--   0 pengxi     (501) staff       (20)        0 2023-01-25 23:58:14.000000 peeling-0.1.0/peeling/__init__.py
--rw-r--r--   0 pengxi     (501) staff       (20)     1336 2023-03-22 16:09:24.000000 peeling-0.1.0/peeling/clipantherprocessor.py
--rwxr-xr-x   0 pengxi     (501) staff       (20)     6403 2023-03-22 16:09:30.000000 peeling-0.1.0/peeling/cliprocessor.py
--rwx------   0 pengxi     (501) staff       (20)      271 2023-03-22 16:09:35.000000 peeling-0.1.0/peeling/cliuniprotcommunicator.py
--rwx------   0 pengxi     (501) staff       (20)     3348 2023-03-22 16:09:41.000000 peeling-0.1.0/peeling/cliuserinputreader.py
--rwxr-xr-x   0 pengxi     (501) staff       (20)     3561 2023-03-22 16:09:08.000000 peeling-0.1.0/peeling/main.py
--rw-r--r--   0 pengxi     (501) staff       (20)     6145 2023-03-17 21:57:25.000000 peeling-0.1.0/peeling/pantherprocessor.py
--rw-r--r--   0 pengxi     (501) staff       (20)    10578 2023-03-17 21:54:15.000000 peeling-0.1.0/peeling/processor.py
--rw-r--r--   0 pengxi     (501) staff       (20)    12503 2023-03-22 16:17:47.000000 peeling-0.1.0/peeling/uniprotcommunicator.py
--rw-r--r--   0 pengxi     (501) staff       (20)     2079 2023-03-17 21:45:21.000000 peeling-0.1.0/peeling/userinputreader.py
--rw-r--r--   0 pengxi     (501) staff       (20)     1595 2023-03-22 16:10:09.000000 peeling-0.1.0/peeling/webpantherprocessor.py
--rwxr-xr-x   0 pengxi     (501) staff       (20)     5598 2023-03-22 16:10:14.000000 peeling-0.1.0/peeling/webprocessor.py
--rwxr-xr-x   0 pengxi     (501) staff       (20)     5639 2023-03-22 16:10:22.000000 peeling-0.1.0/peeling/webuniprotcommunicator.py
--rwx------   0 pengxi     (501) staff       (20)     1180 2023-03-22 16:10:28.000000 peeling-0.1.0/peeling/webuserinputreader.py
-drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-03-30 15:47:50.194953 peeling-0.1.0/peeling.egg-info/
--rw-r--r--   0 pengxi     (501) staff       (20)     9001 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/PKG-INFO
--rw-r--r--   0 pengxi     (501) staff       (20)      614 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/SOURCES.txt
--rw-r--r--   0 pengxi     (501) staff       (20)        1 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/dependency_links.txt
--rw-r--r--   0 pengxi     (501) staff       (20)       46 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/entry_points.txt
--rw-r--r--   0 pengxi     (501) staff       (20)      522 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/requires.txt
--rw-r--r--   0 pengxi     (501) staff       (20)        8 2023-03-30 15:47:50.000000 peeling-0.1.0/peeling.egg-info/top_level.txt
--rw-r--r--   0 pengxi     (501) staff       (20)     1408 2023-03-30 15:45:28.000000 peeling-0.1.0/pyproject.toml
--rw-r--r--   0 pengxi     (501) staff       (20)       38 2023-03-30 15:47:50.200688 peeling-0.1.0/setup.cfg
-drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-03-30 15:47:50.196345 peeling-0.1.0/test/
--rw-r--r--   0 pengxi     (501) staff       (20)    15513 2023-03-22 14:09:46.000000 peeling-0.1.0/test/test.py
+drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.089299 peeling-0.2.0/
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1518 2023-05-10 21:26:26.000000 peeling-0.2.0/LICENSE
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     9334 2023-05-22 18:46:18.088862 peeling-0.2.0/PKG-INFO
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     7202 2023-05-22 18:16:52.000000 peeling-0.2.0/README.md
+drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.079132 peeling-0.2.0/peeling/
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-10 21:26:26.000000 peeling-0.2.0/peeling/__init__.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     3169 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cellular_compartments.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1337 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/clipantherprocessor.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     6492 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliprocessor.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)      267 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     3464 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliuserinputreader.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     4803 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/main.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     6156 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/pantherprocessor.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    10823 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/processor.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    12249 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/uniprotcommunicator.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     2256 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/userinputreader.py
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1595 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webpantherprocessor.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     5620 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webprocessor.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     6498 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     1213 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webuserinputreader.py
+drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.087969 peeling-0.2.0/peeling.egg-info/
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     9334 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/PKG-INFO
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)      647 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/SOURCES.txt
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        1 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/dependency_links.txt
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)       46 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/entry_points.txt
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)      522 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/requires.txt
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        8 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/top_level.txt
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1479 2023-05-22 18:21:50.000000 peeling-0.2.0/pyproject.toml
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)       38 2023-05-22 18:46:18.089386 peeling-0.2.0/setup.cfg
+drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.088424 peeling-0.2.0/test/
+-rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    15513 2023-05-10 21:26:26.000000 peeling-0.2.0/test/test.py
```

### Comparing `peeling-0.1.0/LICENSE` & `peeling-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peeling-0.1.0/PKG-INFO` & `peeling-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.1.0
+Version: 0.2.0
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -27,20 +27,20 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
+Project-URL: Homepage, https://github.com/JaneliaSciComp/peeling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # PEELing
 
 
 ### Introduction
 In the evolutionary transition from unicellular to multicellular organisms, single cells assemble into highly organized tissues and cooperatively carry out physiological functions. To act as an integrated system, individual cells communicate with each other extensively through signaling at the cellular interface. Cell-surface signaling thus controls almost every aspect of the development, physiology, and pathogenesis of multicellular organisms. In situ cell-surface proteomics or `iPEEL` (in situ cell-surface proteome extraction by extracellular labeling; developed by [Li, Han et al., 2020](https://pubmed.ncbi.nlm.nih.gov/31955847/) — `PMID: 31955847` and [Shuster, Li et al., 2022](https://pubmed.ncbi.nlm.nih.gov/36220098/) — `PMID: 36220098`) provides a method for quantitatively profiling cell-surface proteomes in native tissues with cell-type and spatiotemporal specificities. 
 
@@ -70,48 +70,52 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the IDs to the latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). As of our testing, it will take dozens of seconds to minutes for the process. 
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
-Therefore, it is recommended to save the retrieved data when first time run it, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Remember to update the retrieved data periodically.
+Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
-To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'"
+To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
 ```
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates -p organism
 ```
 
 
 ### Options
 -h, --help    Show help message and exit
 
 -t, --tolerance    Tolerance of non-included ratios ratio, default is 0. (For example, in an experiment with 2 non-labelled controls and 3 labelled replicates, there are 6 replicate-to-control ratios. In the default algorithm, a protein must pass cutoff in all 6 ratios to be included in the final proteome. If the tolerance is set to 1, a protein is included in the final proteome if it passes cutoff in any 5 ratios. If the tolerance is set to 2, a protein is included in the final proteome if it passes cutoff in any 4 ratios.) 
 
 -o, --output    Directory to store output results, default is the current work directory
 
 -i, --ids    Latest_ids file directory including filename, e.g. data/id_mapping.tsv
 
--s, --surface    Annotation_surface file directory including filename, e.g. data/annotation_surface.tsv
+--tp, --true-positive   path to true positive annotation file, e.g. data/annotation_true_positive.tsv
 
--c, --cyto    Annotation_cyto file directory including filename, e.g. data/annotation_cyto.tsv
+--fp, --false-positive  path to false positive annotation file, e.g. data/annotation_false_positive.tsv
 
 -a, --cache    Save the data retrieved from UniProt on the local computer, true if specified
 
 -f, --format    The format of the output plots, default is png. Supported formats depend on the computation platform, use -h/--help to see supported formats
 
 -n, --nomap    No id mapping for local annotation files, true if specified
 
 -p, --panther    The organism from which the mass spec data is made, a required input for Panther enrichment analysis. Please refer to Panther's API page http://pantherdb.org/services/oai/pantherdb/supportedgenomes for supported organism. Choose the corresponding 'long_names', and wrap it by quotes, e.g. 'Homo sapiens'
+
+--cc, --cellular_compartment    Choose between: cs - cell surface [default], mt - mitochondria, nu - nucleus or ot - other. If other is chosen, the true positive (--tp) and false positive (--fp) files must be specified
+
+-v --verbose    Enables verbose debugging output
```

### Comparing `peeling-0.1.0/README.md` & `peeling-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,48 +30,52 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the IDs to the latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). As of our testing, it will take dozens of seconds to minutes for the process. 
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
-Therefore, it is recommended to save the retrieved data when first time run it, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Remember to update the retrieved data periodically.
+Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
-To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'"
+To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
 ```
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates -p organism
 ```
 
 
 ### Options
 -h, --help    Show help message and exit
 
 -t, --tolerance    Tolerance of non-included ratios ratio, default is 0. (For example, in an experiment with 2 non-labelled controls and 3 labelled replicates, there are 6 replicate-to-control ratios. In the default algorithm, a protein must pass cutoff in all 6 ratios to be included in the final proteome. If the tolerance is set to 1, a protein is included in the final proteome if it passes cutoff in any 5 ratios. If the tolerance is set to 2, a protein is included in the final proteome if it passes cutoff in any 4 ratios.) 
 
 -o, --output    Directory to store output results, default is the current work directory
 
 -i, --ids    Latest_ids file directory including filename, e.g. data/id_mapping.tsv
 
--s, --surface    Annotation_surface file directory including filename, e.g. data/annotation_surface.tsv
+--tp, --true-positive   path to true positive annotation file, e.g. data/annotation_true_positive.tsv
 
--c, --cyto    Annotation_cyto file directory including filename, e.g. data/annotation_cyto.tsv
+--fp, --false-positive  path to false positive annotation file, e.g. data/annotation_false_positive.tsv
 
 -a, --cache    Save the data retrieved from UniProt on the local computer, true if specified
 
 -f, --format    The format of the output plots, default is png. Supported formats depend on the computation platform, use -h/--help to see supported formats
 
 -n, --nomap    No id mapping for local annotation files, true if specified
 
 -p, --panther    The organism from which the mass spec data is made, a required input for Panther enrichment analysis. Please refer to Panther's API page http://pantherdb.org/services/oai/pantherdb/supportedgenomes for supported organism. Choose the corresponding 'long_names', and wrap it by quotes, e.g. 'Homo sapiens'
+
+--cc, --cellular_compartment    Choose between: cs - cell surface [default], mt - mitochondria, nu - nucleus or ot - other. If other is chosen, the true positive (--tp) and false positive (--fp) files must be specified
+
+-v --verbose    Enables verbose debugging output
```

### Comparing `peeling-0.1.0/peeling/clipantherprocessor.py` & `peeling-0.2.0/peeling/clipantherprocessor.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from peeling.pantherprocessor import PantherProcessor
 import logging
 import asyncio
+from peeling.pantherprocessor import PantherProcessor
 
 logger = logging.getLogger('peeling')
 
 
 class CliPantherProcessor(PantherProcessor):
     def __init__(self, organism, path):
         self.__organism = organism
@@ -38,8 +38,8 @@
             raise
         finally:
             await self._close_client()
 
 
     # implement abstract method
     def start(self):
-        asyncio.run(self._start())
+        asyncio.run(self._start())
```

### Comparing `peeling-0.1.0/peeling/cliprocessor.py` & `peeling-0.2.0/peeling/cliprocessor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from peeling.processor import Processor
 import os
 from datetime import datetime
 import pandas as pd
 import logging
 import asyncio
 import matplotlib.pyplot as plt
+from peeling.processor import Processor
 
 
 logger = logging.getLogger('peeling')
 
 
 class CliProcessor(Processor):
     def __init__(self, user_input_reader, uniprot_communicator):
@@ -29,111 +29,114 @@
             old_ids = list(mass_data.iloc[:, 0])
             if self.__ids is not None: # for annotation ids
                 old_ids_set = set(old_ids)
                 saved_ids_set = set(self.__ids['From'])
                 # logger.debug(f'before retrieve: {len(self.__ids)}')
                 to_retrieve = old_ids_set.difference(saved_ids_set)
                 # logger.debug(f'to retrieve: {len(to_retrieve)}')
-                
+
                 if len(to_retrieve) > 0:
                     old_ids = list(to_retrieve)
             retrieved_data = await self._get_uniprot_communicator().get_latest_id(old_ids)
             self.__ids = pd.concat([self.__ids, retrieved_data])
             # logger.debug(f'after concat: {len(self.__ids)}')
-              
+
         return self.__ids
 
-        
+
     # implement abstract method
     async def _get_annotation_data(self, type):
         '''
-        type: 'surface' or 'cyto'
+        type: 'true_positive' or 'false_positive'
         '''
-        if type == 'surface':
-            if self._get_user_input_reader().get_annotation_surface_filename() is not None: 
-                annotation = self._get_user_input_reader().get_annotation_surface() 
+        if type == 'true_positive':
+            if self._get_user_input_reader().get_true_positive_filename() is not None:
+                annotation = self._get_user_input_reader().get_annotation_true_positive()
                 annotation = pd.DataFrame(annotation.iloc[:, 0])
                 if not self._get_user_input_reader().get_id_mapping():
                     annotation.columns = ['From']
                     id_mapping_data = await self._get_id_mapping_data(annotation)
                     annotation = self._merge_id(annotation, id_mapping_data)
                     annotation.reset_index(inplace=True)
                     annotation = pd.DataFrame(annotation.iloc[:, 0])
                 annotation.columns = ['Entry']
             else: # retrieve annotation file from UniProt
-                annotation = await self._get_uniprot_communicator().get_annotation('surface')
+                annotation = await self._get_uniprot_communicator().get_annotation('true_positive')
                 annotation.dropna(subset=['Entry'], axis=0, how='any', inplace=True)
                 if self._get_user_input_reader().get_save():
-                    annotation.to_csv(f'{self.__path}/annotation_surface.tsv', sep='\t', index=False)
+                    annotation.to_csv(f'{self.__path}/annotation_true_positive.tsv', sep='\t', index=False)
                 annotation = annotation[['Entry']]
         else:
-            if self._get_user_input_reader().get_annotation_cyto_filename() is not None: 
-                annotation = self._get_user_input_reader().get_annotation_cyto() 
+            if self._get_user_input_reader().get_false_positive_filename() is not None:
+                annotation = self._get_user_input_reader().get_annotation_false_positive()
                 annotation = pd.DataFrame(annotation.iloc[:, 0])
                 if not self._get_user_input_reader().get_id_mapping():
                     annotation.columns = ['From']
                     id_mapping_data = await self._get_id_mapping_data(annotation)
                     annotation = self._merge_id(annotation, id_mapping_data)
                     annotation.reset_index(inplace=True)
                     annotation = pd.DataFrame(annotation.iloc[:, 0])
                 annotation.columns = ['Entry']
             else: # retrieve annotation file from UniProt
-                annotation = await self._get_uniprot_communicator().get_annotation('cyto')
+                annotation = await self._get_uniprot_communicator().get_annotation('false_positive')
                 annotation.dropna(subset=['Entry'], axis=0, how='any', inplace=True)
                 if self._get_user_input_reader().get_save():
-                    annotation.to_csv(f'{self.__path}/annotation_cyto.tsv', sep='\t', index=False)
+                    annotation.to_csv(f'{self.__path}/annotation_false_positive.tsv', sep='\t', index=False)
                 annotation = annotation[['Entry']]
-       
+
         return annotation
 
 
     # implement abstract method
     def _plot_supplemental(self, fig_name):
         plt.close()
 
 
     # implement abstract method
     def _construct_path(self):
         parent_path = os.path.join(self._get_user_input_reader().get_output_directory(), str(datetime.now()).replace(':','-').replace(' ','_'))
         if self._get_user_input_reader().get_save():
             retrieved_path = os.path.join(parent_path, "retrieved_data")
-            try: 
-                os.makedirs(retrieved_path, exist_ok=True) 
-            except OSError as error: 
+            try:
+                os.makedirs(retrieved_path, exist_ok=True)
+            except OSError as error:
                 logger.error(error)
         else:
             retrieved_path = None
         self.__path = retrieved_path
         return parent_path
 
 
     def _write_args(self, path):
         super()._write_args(path)
         with open(os.path.join(path, 'log.txt'), 'a') as f:
             ids = self._get_user_input_reader().get_latest_ids_filename()
             if ids is not None:
                 f.write(f'Latest_ids file: {ids}\n')
-            surface = self._get_user_input_reader().get_annotation_surface_filename()
-            if surface is not None:
-                f.write(f'Annotation_surface file: {surface}\n')
-            cyto = self._get_user_input_reader().get_annotation_cyto_filename()
-            if cyto is not None:
-                f.write(f'Annotation_cyto file: {cyto}\n')
+
+            true_positive = self._get_user_input_reader().get_true_positive_filename()
+            if true_positive is not None:
+                f.write(f'Annotation_true_positive file: {true_positive}\n')
+
+            false_positive = self._get_user_input_reader().get_false_positive_filename()
+            if false_positive is not None:
+                f.write(f'Annotation_false_positive file: {false_positive}\n')
+
             no_id_mapping = self._get_user_input_reader().get_id_mapping()
-            if (surface is not None) or (cyto is not None):
+            if (true_positive is not None) or (false_positive is not None):
                 f.write(f'No id mapping for local annotations: {no_id_mapping}\n')
-   
+
 
     # implement abstract method
     def start(self):
         data = self._get_user_input_reader().get_mass_data()
         parent_path = self._construct_path()
         data = self._mass_data_clean(data)
         asyncio.run(self._analyze(data, parent_path))
         if self._get_user_input_reader().get_save() and self._get_user_input_reader().get_latest_ids_filename() is None:
             self.__ids.to_csv(self.__path+'/latest_ids.tsv', sep='\t', index=False)
         self._write_args(parent_path)
         return parent_path
-    
 
-    def _set_surface_proteins_raw_data(self, df):
-        return
+
+    def _set_true_positive_proteins_raw_data(self, df):
+        return
```

### Comparing `peeling-0.1.0/peeling/cliuserinputreader.py` & `peeling-0.2.0/peeling/cliuserinputreader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pandas as pd
-from peeling.userinputreader import UserInputReader
 import logging
+from peeling.userinputreader import UserInputReader
 
 logger = logging.getLogger('peeling')
 
 
 class CliUserInputReader(UserInputReader):
-    def __init__(self, mass_filename, num_controls, num_replicates, output_directory, tolerance, ids_filename, annotation_surface_filename, annotation_cyto_filename, cache, plot_format, no_id_mapping):
-        super().__init__(num_controls, num_replicates, tolerance, plot_format)
+    def __init__(self, mass_filename, num_controls, num_replicates, output_directory, tolerance, ids_filename, true_positive_filename, false_positive_filename, cache, plot_format, no_id_mapping, cellular_compartment):
+        super().__init__(num_controls, num_replicates, tolerance, plot_format, cellular_compartment)
         self.__mass_filename = mass_filename
         self.__output_directory = output_directory
         self.__ids_filename = ids_filename
-        self.__annotation_surface_filename = annotation_surface_filename
-        self.__annotation_cyto_filename = annotation_cyto_filename
+        self.__true_positive_filename = true_positive_filename
+        self.__false_positive_filename = false_positive_filename
         self.__save = cache
         self.__no_id_mapping = no_id_mapping
 
 
     def __read_file(self, filename):
         try:
             df = pd.read_table(filename, sep='\t', header=0)
@@ -45,49 +45,49 @@
         return self.__mass_filename
     
 
     def get_latest_ids_filename(self):
         return self.__ids_filename
     
 
-    def get_annotation_surface_filename(self):
-        return self.__annotation_surface_filename
+    def get_true_positive_filename(self):
+        return self.__true_positive_filename
     
 
-    def get_annotation_cyto_filename(self):
-        return self.__annotation_cyto_filename
+    def get_false_positive_filename(self):
+        return self.__false_positive_filename
 
 
     def get_latest_ids(self):
         df = self.__read_file(self.__ids_filename)
         try:
             assert(df.shape[1] >= 2), 'Latest ids file should have at least two columns'
             logger.info('Read in %d rows from latest_ids file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
         
 
-    def get_annotation_surface(self):
-        df = self.__read_file(self.__annotation_surface_filename)
+    def get_annotation_true_positive(self):
+        df = self.__read_file(self.__true_positive_filename)
         try:
-            assert(df.shape[1] >= 1), 'Annotation_surface file should have at least one column containing ids of extracellular proteins'    
-            logger.info('Read in %d rows from annotation_surface file' % (len(df)))
+            assert(df.shape[1] >= 1), 'Annotation_true_positive file should have at least one column containing ids of proteins in your selected cellular compartment'
+            logger.info('Read in %d rows from annotation_true_positive file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
        
 
-    def get_annotation_cyto(self):
-        df = self.__read_file(self.__annotation_cyto_filename)
+    def get_annotation_false_positive(self):
+        df = self.__read_file(self.__false_positive_filename)
         try:
-            assert(df.shape[1] >= 1), 'Annotation_cyto file should have at least one column containing ids of intracellular proteins'    
-            logger.info('Read in %d rows from annotation_cyto file' % (len(df)))
+            assert(df.shape[1] >= 1), 'Annotation_false_positive file should have at least one column containing ids of proteins that are not found in your selected cellular compartment'
+            logger.info('Read in %d rows from annotation_false_positive file' % (len(df)))
             return df
         except AssertionError as e:
             logger.error(e)
             raise
 
     
     def get_output_directory(self):
@@ -95,8 +95,8 @@
 
 
     def get_save(self):
         return self.__save
     
 
     def get_id_mapping(self):
-        return self.__no_id_mapping
+        return self.__no_id_mapping
```

### Comparing `peeling-0.1.0/peeling/pantherprocessor.py` & `peeling-0.2.0/peeling/pantherprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,20 +150,20 @@
             logger.error(f'{ENRICH_CATEGORIES[annot_dataset]} failed.')
             logger.error(e)
             return (ENRICH_CATEGORIES[annot_dataset], 'failed')
 
 
     @abstractmethod
     def start(self):
-        raise NotImplemented()
+        raise NotImplementedError()
 
     
     @abstractmethod
     def _write_args(self):
-        raise NotImplemented()
+        raise NotImplementedError()
     
     
     def _set_organism_id(self, id):
         self.__organism_id = id
     
 
     def _get_path(self):
@@ -174,8 +174,8 @@
         return self.__organism_id
     
 
     async def _close_client(self):
         if self.__client is not None:
             await self.__client.aclose()
             self.__client = None
-        
+
```

### Comparing `peeling-0.1.0/peeling/processor.py` & `peeling-0.2.0/peeling/processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 logger = logging.getLogger('peeling')
 
 
 class Processor(ABC):
     def __init__(self, user_input_reader, uniprot_communicator):
         self.__user_input_reader = user_input_reader
         self.__uniprot_communicator = uniprot_communicator
-        
-    
+
+
     def _mass_data_clean(self, data):
         try:
             id_col = data.columns[0]
             data.rename(columns={id_col: 'From'}, inplace=True)
             data.replace('', np.nan, inplace=True) #for web, missing value is taken as '', won't be dropped
             data = data.dropna(axis=0, how='any')
             logger.info(f'After dropping rows with missing value: {len(data)}')
             assert(len(data) >= 1), 'Empty data after dropping missing values'
-        
+
             data.columns = [re.sub('[^a-zA-Z0-9_]', '_', name) for name in data.columns]
             data[data.columns[1:]] = data[data.columns[1:]].astype('float')
             return data
         except Exception as e:
             raise
-    
+
 
     def __make_heatmap(self, data, plot_path):
         data.set_index('From', inplace=True)
         corr = data.corr()
         #r2 = corr**2
         fig, ax = plt.subplots()
-        ax = sns.heatmap(corr, linewidth=0.5, annot=True, cmap="coolwarm", vmin=-1, vmax=1, square=True) 
+        ax = sns.heatmap(corr, linewidth=0.5, annot=True, cmap="coolwarm", vmin=-1, vmax=1, square=True)
         ax.tick_params(left=False, bottom=False)
         ax.set_xticklabels(ax.get_xticklabels(), rotation=50, ha='right')
         title = 'Pairwise Pearson Correlation Coefficient'
         plt.title(title)
         fig_name = title.replace(' ', '_')
         plt.savefig(f'{plot_path}/{fig_name}.{self.__user_input_reader.get_plot_format()}', bbox_inches='tight', dpi=130)
         data.reset_index(inplace=True)
@@ -68,92 +68,92 @@
         # logger.debug(f"After fillna: {np.sum(np.sum(mass_data[['From', 'Entry']].isnull()))}")
         updated_ids=np.sum(mass_data['From']!=mass_data['Entry'])
         logger.info(f'Mapped ids: {updated_ids}')
         mass_data.drop([mass_data.columns[0]], axis=1, inplace=True)
         mass_data.set_index('Entry', inplace=True)
         logger.info('Id mapping is done')
         return mass_data
-    
+
 
     @abstractmethod
     def _get_annotation_data(self, type):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
     def __merge_annotation(self, mass_data, annotation, type):
         '''
-        type: 'surface' or 'cyto'
+        type: 'true_positive' or 'false_positive'
         '''
         annotation['Add'] = 1
         annotation.drop_duplicates(keep='first', inplace=True)
         annotation.dropna(axis=0, how='any', inplace=True)
         annotation.set_index('Entry', inplace=True)
-        
+
         mass_data = mass_data.merge(annotation, how='left', left_index=True, right_index=True)
-        new_col_name = 'TP' if type=='surface' else 'FP'
+        new_col_name = 'TP' if type=='true_positive' else 'FP'
         mass_data.rename(columns={'Add': new_col_name}, inplace=True)
-        
+
         mass_data[new_col_name] = mass_data[new_col_name].fillna(0)
         logger.info(f'Adding annotation_{type} is done.')
         return mass_data
-    
+
 
     def __calculate_TPR_FPR_diff(self, data, col_to_sort):
         '''
-        Sort data on col_to_sort in descending order, calculate accumulative TPR, FPR and TPR-FPR. 
+        Sort data on col_to_sort in descending order, calculate accumulative TPR, FPR and TPR-FPR.
         Input
         data: df
         col_to_sort: int, the index of the column to sort
         return df
         '''
         col_name = data.columns[col_to_sort]
         data.sort_values(by=[col_name], ascending=False, inplace=True)
-        
-        TPR_col_name = "TPR"  
+
+        TPR_col_name = "TPR"
         FPR_col_name = "FPR"
         data[[TPR_col_name, FPR_col_name]] = data[['TP', 'FP']].cumsum()
         data[TPR_col_name] = data[TPR_col_name] / data['TP'].sum()
         data[FPR_col_name] = data[FPR_col_name] / data['FP'].sum()
-        data['TPR-FPR'] = data[TPR_col_name] - data[FPR_col_name] 
+        data['TPR-FPR'] = data[TPR_col_name] - data[FPR_col_name]
         return data
-    
+
 
     def __plot_line(self, data, output_dir, col_index):
         '''
         Make line plot of the last three columns (TPR, FPR, TPR-FPR)
         '''
         col_list = data.columns[-3:]
         plt.figure()
-        data[col_list].plot(use_index=False) 
-        
+        data[col_list].plot(use_index=False)
+
         plt.xlabel('Rank')
         plt.title('TPR, FPR, TPR-FPR')
         fig_name = f'TPR_FPR_{data.columns[col_index]}'
         plt.savefig(f'{output_dir}/{fig_name}.{self.__user_input_reader.get_plot_format()}', dpi=130)
         return fig_name
-    
+
 
     @abstractmethod
-    def _plot_supplemental(self, plt, fig_name):
+    def _plot_supplemental(self, fig_name):
         raise NotImplemented()
-    
+
 
     def __filter_by_max_TPR_FPR_diff(self, data, col_index):
         '''
         Set cut-off point to be the point with the maximal TPR-FPR; Set include = True if before or at this pos, False otherwise
         Return FPR, TPR of the cut-off point
         '''
         cut_off_pos = data.iloc[:, -1].argmax()
-        
+
         col_name = 'include_' + data.columns[col_index]
         data[col_name] = True
         data.iloc[cut_off_pos + 1:, -1] = False
         return cut_off_pos
-    
-    
+
+
     def __plot_roc(self, data, cut_off_pos, output_dir, col_index):
         '''
         Make ROC, calculate AUC, label the cut off point
         '''
         cutoff_fpr = data.iloc[cut_off_pos, -3]
         cutoff_tpr = data.iloc[cut_off_pos, -4]
         cutoff_protein_id = data.index[cut_off_pos]
@@ -165,94 +165,98 @@
         plt.ylabel('TPR')
         plt.text(0, 0.9, 'AUC = ' + str(round(auc(data.iloc[:, -3], data.iloc[:, -4]), 2)))
         plt.plot(cutoff_fpr, cutoff_tpr, marker='o', color='r')
         ax.annotate('Cut-off Rank: '+str(cut_off_pos)+'\nUniprot ID: '+cutoff_protein_id +'\nTPR='+str(round(cutoff_tpr,3))+', FPR='+str(round(cutoff_fpr,3)), (cutoff_fpr+0.05, cutoff_tpr-0.15))
         fig_name = f'ROC_{data.columns[col_index]}'
         plt.savefig(f'{output_dir}/{fig_name}.{self.__user_input_reader.get_plot_format()}', dpi=130)
         return fig_name
-    
 
-    def __get_surface_proteins(self, data, path, plots_path):
+
+    def __get_true_positive_proteins(self, data, path, plots_path):
         '''
-        If a protein is included in at least num_ctrl * num_rep - tolerance columns, output it as surface protein
-        
+        If a protein is included in at least num_ctrl * num_rep - tolerance columns, output it as true_positive protein
+
         Output
-        Accession ids of the surface proteins
+        Accession ids of the true_positive proteins
         '''
         total_col = self.__user_input_reader.get_num_controls() * self.__user_input_reader.get_num_replicates()
         start_col = 0
         threshold = total_col - self.__user_input_reader.get_tolerance()
-        
+
         for i in range(start_col, start_col + total_col):
             self.__calculate_TPR_FPR_diff(data, i)
             fig_name = self.__plot_line(data, plots_path, i)
             self._plot_supplemental(fig_name)
             cut_off_pos = self.__filter_by_max_TPR_FPR_diff(data, i)
             fig_name = self.__plot_roc(data, cut_off_pos, plots_path, i)
             self._plot_supplemental(fig_name)
             data.drop(data.columns[-4:-1], axis=1, inplace=True)
-        
+
         col_name = 'include_sum'
         data[col_name] = data.iloc[:, -total_col:].sum(axis=1)
-        
-        surface_proteins = data[data[col_name] >= threshold].iloc[:, :total_col+4]
-        surface_proteins.reset_index(inplace=True)
-        surface_proteins.dropna(subset='Entry', axis=0, how='any')
-        surface_proteins.drop_duplicates(subset='Entry', keep='first', inplace=True)
-        surface_proteins_raw_data =  surface_proteins
-        self._set_surface_proteins_raw_data(surface_proteins_raw_data)
-        surface_proteins = surface_proteins[['Entry', 'Gene Names', 'Protein names', 'Organism', 'Length']]
-
-        logger.info(f'{len(surface_proteins)} surface proteins found')
-        surface_proteins.to_csv(f'{path}/post-cutoff-proteome.tsv', sep='\t', index=False)
-        # save a txt file containing just surface protein ids separated by ',', so that easily copy to put in other web
-        proteins_str = ','.join(list(surface_proteins['Entry']))
+
+        true_positive_proteins = data[data[col_name] >= threshold].iloc[:, :total_col+4]
+        true_positive_proteins.reset_index(inplace=True)
+        true_positive_proteins.dropna(subset='Entry', axis=0, how='any')
+        true_positive_proteins.drop_duplicates(subset='Entry', keep='first', inplace=True)
+        true_positive_proteins_raw_data =  true_positive_proteins
+        self._set_true_positive_proteins_raw_data(true_positive_proteins_raw_data)
+        true_positive_proteins = true_positive_proteins[['Entry', 'Gene Names', 'Protein names', 'Organism', 'Length']]
+
+        logger.info(f'{len(true_positive_proteins)} true_positive proteins found')
+        true_positive_proteins.to_csv(f'{path}/post-cutoff-proteome.tsv', sep='\t', index=False)
+        # save a txt file containing just true_positive protein ids separated by ',', so that easily copy to put in other web
+        proteins_str = ','.join(list(true_positive_proteins['Entry']))
         with open(f'{path}/post-cutoff-proteome.txt', 'w') as f:
             f.write(proteins_str)
-    
+
 
     @abstractmethod
     def _construct_path(self):
         raise NotImplemented()
 
 
     async def _analyze(self, data, parent_path):
-        plots_path = os.path.join(parent_path, "plots") 
-        try: 
-            os.makedirs(plots_path) 
-        except OSError as error: 
+        plots_path = os.path.join(parent_path, "plots")
+        try:
+            os.makedirs(plots_path)
+        except OSError as error:
             logger.debug(error)
-        
+
         fig_name = self.__make_heatmap(data, plots_path)
         self._plot_supplemental(fig_name)
         id_mapping_data = await self._get_id_mapping_data(data)
         data = self._merge_id(data, id_mapping_data)
-        annotation_surface = await self._get_annotation_data('surface')
-        data = self.__merge_annotation(data, annotation_surface, 'surface')
-        annotation_cyto = await self._get_annotation_data('cyto')
-        data = self.__merge_annotation(data, annotation_cyto, 'cyto')
-        
-        self.__get_surface_proteins(data, parent_path, plots_path)
-    
+        annotation_true_positive = await self._get_annotation_data('true_positive')
+        data = self.__merge_annotation(data, annotation_true_positive, 'true_positive')
+        annotation_false_positive = await self._get_annotation_data('false_positive')
+        data = self.__merge_annotation(data, annotation_false_positive, 'false_positive')
+
+        self.__get_true_positive_proteins(data, parent_path, plots_path)
+
 
     def _write_args(self, path):
         with open(os.path.join(path, 'log.txt'), 'w') as f:
             f.write('Mass spec file: ' + str(self.__user_input_reader.get_mass_spec_filename()) + '\n')
+            cellular_compartment = self._get_user_input_reader().get_cellular_compartment()
+            if cellular_compartment is not None:
+                f.write(f'Cellular compartment: {cellular_compartment}\n')
             f.write(f'Number of controls: {self.__user_input_reader.get_num_controls()}\n')
             f.write(f'Number of replicates: {self.__user_input_reader.get_num_replicates()}\n')
             f.write(f'Tolerance: {self.__user_input_reader.get_tolerance()}\n')
             f.write(f'Plot format: {self.__user_input_reader.get_plot_format()}\n')
 
 
+
     @abstractmethod
     def start(self):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
     def _get_user_input_reader(self):
         return self.__user_input_reader
-    
-    
+
+
     def _get_uniprot_communicator(self):
         return self.__uniprot_communicator
-    
-    
+
+
```

### Comparing `peeling-0.1.0/peeling/uniprotcommunicator.py` & `peeling-0.2.0/peeling/uniprotcommunicator.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,53 +4,53 @@
 from urllib.parse import urlparse, parse_qs, urlencode
 import httpx
 import asyncio
 import csv
 import pandas as pd
 from abc import ABC, abstractmethod
 import logging
+from peeling.cellular_compartments import cellular_compartments
 
 logger = logging.getLogger('peeling')
 
+
+# surface = true positive
+# cyto = false positive
+
 TIME_OUT = 600
 MAX_KEEPALIVE_CONNECTIONS=10
 MAX_CONNECTIONS=15
 CONNECT_RETRY = 5
 MAX_CHECK_RETRY = 10
 POLLING_INTERVAL = 5
 API_URL = "https://rest.uniprot.org"
 
 CHUNK_SIZE = 2000 #TODO: tune CHUNK_SIZE
 
-# urls for cache have more fields (option for cli user to save retrieved data)
-SURFACE_URL_CACHE = "https://rest.uniprot.org/uniprotkb/search?compressed=true&fields=accession%2Creviewed%2Cid%2Cgene_names%2Corganism_name%2Ccc_subcellular_location&format=tsv&query=%28%28%28cc_scl_term%3ASL-0112%29%20OR%20%28cc_scl_term%3ASL-0243%29%20OR%20%28keyword%3AKW-0732%29%20OR%20%28cc_scl_term%3ASL-9906%29%20OR%20%28cc_scl_term%3ASL-9907%29%29%20AND%20%28reviewed%3Atrue%29%29&size=500"
-CYTO_URL_CACHE = "https://rest.uniprot.org/uniprotkb/search?compressed=true&fields=accession%2Creviewed%2Cid%2Cgene_names%2Corganism_name%2Ccc_subcellular_location&format=tsv&query=%28%28%28%28cc_scl_term%3ASL-0091%29%20OR%20%28cc_scl_term%3ASL-0173%29%20OR%20%28cc_scl_term%3ASL-0191%29%29%20AND%20%28reviewed%3Atrue%29%29%20NOT%20%28%28%28cc_scl_term%3ASL-0112%29%20OR%20%28cc_scl_term%3ASL-0243%29%20OR%20%28keyword%3AKW-0732%29%20OR%20%28cc_scl_term%3ASL-9906%29%20OR%20%28cc_scl_term%3ASL-9907%29%29%20AND%20%28reviewed%3Atrue%29%29%29&size=500"
-SURFACE_URL = "https://rest.uniprot.org/uniprotkb/search?compressed=true&fields=accession&format=tsv&query=%28%28%28cc_scl_term%3ASL-0112%29%20OR%20%28cc_scl_term%3ASL-0243%29%20OR%20%28keyword%3AKW-0732%29%20OR%20%28cc_scl_term%3ASL-9906%29%20OR%20%28cc_scl_term%3ASL-9907%29%29%20AND%20%28reviewed%3Atrue%29%29&size=500"
-CYTO_URL = "https://rest.uniprot.org/uniprotkb/search?compressed=true&fields=accession&format=tsv&query=%28%28%28%28cc_scl_term%3ASL-0091%29%20OR%20%28cc_scl_term%3ASL-0173%29%20OR%20%28cc_scl_term%3ASL-0191%29%29%20AND%20%28reviewed%3Atrue%29%29%20NOT%20%28%28%28cc_scl_term%3ASL-0112%29%20OR%20%28cc_scl_term%3ASL-0243%29%20OR%20%28keyword%3AKW-0732%29%20OR%20%28cc_scl_term%3ASL-9906%29%20OR%20%28cc_scl_term%3ASL-9907%29%29%20AND%20%28reviewed%3Atrue%29%29%29&size=500"
-
-
 class UniProtCommunicator(ABC):
-    def __init__(self, cache):
+    def __init__(self, cache=False, cellular_compartment='cs'):
         self.__save = cache
         self.__client = None
-        self.__annotation_surface = None
-        self.__annotation_cyto = None
-    
+        self._annotation_true_positive = None
+        self._annotation_false_positive = None
+        self.__cellular_compartment = cellular_compartments.get(cellular_compartment, None)
+        self._cc_code = cellular_compartment
+
 
     def __create_client(self):
         limits = httpx.Limits(max_keepalive_connections=MAX_KEEPALIVE_CONNECTIONS, max_connections=MAX_CONNECTIONS)
         transport = httpx.AsyncHTTPTransport(retries=CONNECT_RETRY)
         self.__client = httpx.AsyncClient(http2=True, timeout=TIME_OUT, limits=limits, transport=transport, event_hooks={'response': [self.__check_response]})
 
 
     async def __check_response(self, response):
         try:
             await response.aread()
             if response.status_code == 303:
-                return 
+                return
             response.raise_for_status()
         except httpx.HTTPStatusError:
             logger.info(response.json())
             raise
 
 
     async def __submit_id_mapping(self, ids):
@@ -70,34 +70,34 @@
 
 
     async def __check_id_mapping_results_ready(self, job_id):
         trial = 0
         while trial < MAX_CHECK_RETRY:
             trial += 1
             response = await self.__client.get(f"{API_URL}/idmapping/status/{job_id}")
-            if response.status_code == 303: 
+            if response.status_code == 303:
                 return response.headers.get('location')
-            j = response.json() 
+            j = response.json()
             if "jobStatus" in j:
                 if j["jobStatus"] == "RUNNING":
                     logger.debug(f"{job_id}: Retrying in {POLLING_INTERVAL}s")
                     await asyncio.sleep(POLLING_INTERVAL)
                 else:
                     raise Exception(j["jobStatus"])
             else:
-                return bool(j["results"] or j["failedIds"]) 
+                return bool(j["results"] or j["failedIds"])
         raise Exception('Reach max trials for check job status')
 
 
     async def __get_batch(self, batch_response, compressed):
-        batch_url = self.__get_next_link(batch_response.headers) 
+        batch_url = self.__get_next_link(batch_response.headers)
         while batch_url:
             batch_response = await self.__client.get(batch_url)
-            yield self.__decode_results(batch_response, compressed) 
-            batch_url = self.__get_next_link(batch_response.headers) 
+            yield self.__decode_results(batch_response, compressed)
+            batch_url = self.__get_next_link(batch_response.headers)
 
 
     def __combine_batches(self, all_results, batch_results):
         return all_results + batch_results[1:]
 
 
     # async def __get_id_mapping_results_link(self, job_id):
@@ -111,43 +111,44 @@
             decompressed = zlib.decompress(response.content, 16 + zlib.MAX_WBITS)
             return [line for line in decompressed.decode("utf-8").split("\n") if line]
         else:
             return [line for line in response.text.split("\n") if line]
 
 
     async def __get_id_mapping_results_search(self, url):
-        parsed = urlparse(url) 
+        parsed = urlparse(url)
         query = parse_qs(parsed.query)
-        file_format = "tsv" 
+        file_format = "tsv"
         query['format'] = file_format
-        size = 500 
+        size = 500
         query["size"] = size
         compressed = True
         query['compressed'] = compressed
         parsed = parsed._replace(query=urlencode(query, doseq=True))
         url = parsed.geturl()
         response = await self.__client.get(url)
         results = self.__decode_results(response, compressed)
         async for batch in self.__get_batch(response, compressed):
             results = self.__combine_batches(results, batch)
         return results
-    
+
 
     async def __get_annotation_results_search(self, url):
+        logger.debug(f'fetching data from: {url}')
         response = await self.__client.get(url)
         results = self.__decode_results(response, True)
         async for batch in self.__get_batch(response, True):
             results = self.__combine_batches(results, batch)
         return results
 
 
     def __get_data_frame_from_tsv_results(self, tsv_results):
         reader = csv.DictReader(tsv_results, delimiter="\t", quotechar='"')
         return pd.DataFrame(list(reader))
-    
+
 
     async def _retrieve_latest_id(self, old_ids, meta):
         start_time = datetime.now()
 
         if self.__client is None:
             self.__create_client()
 
@@ -156,15 +157,15 @@
             num_chunks = len(old_ids) // CHUNK_SIZE
             residual = len(old_ids) % CHUNK_SIZE
             num_chunks += 1 if residual>0 else 0
             chunks = [old_ids[CHUNK_SIZE*i:CHUNK_SIZE*(i+1)] if i<(num_chunks-1) else old_ids[CHUNK_SIZE*i:] for i in range(num_chunks)]
             logger.info(f'{len(old_ids)} ids are divided into {num_chunks} chunks with size {CHUNK_SIZE}')
             logger.info('Communicating with UniProt for id mapping...')
 
-            results_list = await asyncio.gather(*map(self.__retrieve_latest_id_chunk, chunks)) 
+            results_list = await asyncio.gather(*map(self.__retrieve_latest_id_chunk, chunks))
 
             failed_ids = 0
             no_mapping_ids_set = set()
             retrieved_ids = 0
             results_list_filtered = []
             for i, item in enumerate(results_list): #item may be list df or integer (len(chunk)) if mapping failed
                 if isinstance(item, int):
@@ -178,15 +179,15 @@
                         else: #all ids in this chunk didn't find mapping data
                             no_mapping_ids_set = no_mapping_ids_set.union(set(chunks[i]))
 
             meta['failed_id_mapping'] = failed_ids
             meta['no_id_mapping'] = no_mapping_ids_set
             logger.info(f'Retrieved {retrieved_ids} ids, {len(no_mapping_ids_set)} ids didn\'t find id mapping data, {failed_ids} ids failed for id mapping')
             logger.info(f'{datetime.now()-start_time} for id mapping')
-            
+
             return pd.concat(results_list_filtered)
         except Exception:
             raise
         finally:
             if self.__client is not None:
                 await self.__client.aclose()
                 self.__client = None
@@ -209,76 +210,96 @@
             return results_df
         except Exception as e:
             logger.error(e)
             return len(chunk)
 
 
     @abstractmethod
-    def get_latest_id():
-        raise NotImplemented()
+    def get_latest_id(self):
+        raise NotImplementedError()
 
-    
-    async def __retrieve_annotation_surface(self):
+
+    def __get_uniprot_url(self, type):
+        if not self.__cellular_compartment:
+            return None
+
+        if type == 'true_positive':
+            if self.__save:
+                logger.debug(f'using true_positive cache url for {self.__cellular_compartment.get("long_name")}')
+                return self.__cellular_compartment.get('true_positive_cache')
+            logger.debug(f'using true_positive url for {self.__cellular_compartment.get("long_name")}')
+            return self.__cellular_compartment.get('true_positive')
+        elif type == 'false_positive':
+            if self.__save:
+                logger.debug(f'using false_positive cache url for {self.__cellular_compartment.get("long_name")}')
+                return self.__cellular_compartment.get('false_positive_cache')
+            logger.debug(f'using false_positive url for {self.__cellular_compartment.get("long_name")}')
+            return self.__cellular_compartment.get('false_positive')
+        else:
+            raise Exception('__get_uniprot_url expects a type of either true_positive or false_positive')
+
+
+    async def __retrieve_annotation_true_positive(self):
         try:
-            logger.info('Retrieving annotation_surface file from UniProt...') 
-            url = SURFACE_URL_CACHE if self.__save else SURFACE_URL
+            logger.info('Retrieving annotation_true_positive file from UniProt...')
+            url = self.__get_uniprot_url('true_positive')
             results = await self.__get_annotation_results_search(url)
             results = self.__get_data_frame_from_tsv_results(results)
-            logger.info(f'Retrieved {len(results)} entries for annotation_surface')
-            self.__annotation_surface = results
+            logger.info(f'Retrieved {len(results)} entries for annotation_true_positive')
+            self._annotation_true_positive = results
         except Exception as e:
             logger.error(e)
-            logger.info(f'Retrieving annotation_surface failed')
-            raise   
+            logger.info(f'Retrieving annotation_true_positive failed')
+            raise
 
 
-    async def __retrieve_annotation_cyto(self):
+    async def __retrieve_annotation_false_positive(self):
         try:
-            logger.info('Retrieving annotation_cyto file from UniProt...')
-            url = CYTO_URL_CACHE if self.__save else CYTO_URL
+            logger.info('Retrieving annotation_false_positive file from UniProt...')
+            url = self.__get_uniprot_url('false_positive')
             results = await self.__get_annotation_results_search(url)
             results = self.__get_data_frame_from_tsv_results(results)
-            logger.info(f'Retrieved {len(results)} entries for annotation_cyto')
-            self.__annotation_cyto = results
+            logger.info(f'Retrieved {len(results)} entries for annotation_false_positive')
+            self._annotation_false_positive = results
         except Exception as e:
             logger.error(e)
-            logger.info(f'Retrieving annotation_cyto failed')
+            logger.info(f'Retrieving annotation_false_positive failed')
             raise
-    
+
 
     async def _retrieve_annotation(self):
         start_time = datetime.now()
 
         if self.__client is None:
             self.__create_client()
         try:
-            await asyncio.gather(self.__retrieve_annotation_surface(), self.__retrieve_annotation_cyto()) 
+            await asyncio.gather(self.__retrieve_annotation_true_positive(), self.__retrieve_annotation_false_positive())
             if not self.__save:
                 self.__shorten_annotation()
             logger.info(f'{datetime.now()-start_time} for retrieving annotations')
         except Exception:
             raise
         finally:
             if self.__client is not None:
                 await self.__client.aclose()
                 self.__client = None
-      
+
 
     async def get_annotation(self, type):
-        if self.__annotation_surface is None or self.__annotation_cyto is None:
+        if self._annotation_true_positive is None or self._annotation_false_positive is None:
                 await self._retrieve_annotation()
-        if type=='surface':
-            return self.__annotation_surface
-        elif type=='cyto':
-            return self.__annotation_cyto
-    
+        if type=='true_positive':
+            return self._annotation_true_positive
+        elif type=='false_positive':
+            return self._annotation_false_positive
+
 
     def __shorten_annotation(self):
-        self.__annotation_surface = self.__annotation_surface[['Entry']]
-        self.__annotation_cyto = self.__annotation_cyto[['Entry']]
-    
+        self._annotation_true_positive = self._annotation_true_positive[['Entry']]
+        self._annotation_false_positive = self._annotation_false_positive[['Entry']]
+
 
     def _set_annotation(self, data, type):
-        if type=='surface':
-            self.__annotation_surface = data
-        elif type=='cyto':
-            self.__annotation_cyto = data
+        if type=='true_positive':
+            self._annotation_true_positive = data
+        elif type=='false_positive':
+            self._annotation_false_positive = data
```

### Comparing `peeling-0.1.0/peeling/userinputreader.py` & `peeling-0.2.0/peeling/userinputreader.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,68 +2,71 @@
 import logging
 import matplotlib.pyplot as plt
 
 logger = logging.getLogger('peeling')
 
 
 class UserInputReader(ABC):
-    def __init__(self, num_controls, num_replicates, tolerance, plot_format):
+    def __init__(self, num_controls, num_replicates, tolerance, plot_format, cellular_compartment):
         self.__num_controls = num_controls
         self.__num_replicates = num_replicates
         self.__tolerance = tolerance
         self.__plot_format = plot_format
+        self.__cellular_compartment = 'cs' if cellular_compartment is None else cellular_compartment
         self.__check_init()
-    
+
 
     def __check_init(self):
         try:
             assert(self.__num_controls >= 1), '# Controls should be a positive integer'
             assert(self.__num_replicates >= 1), '# Replicates should be a positive integer'
             assert(self.__tolerance >= 0 and self.__tolerance <= self.__num_controls*self.__num_replicates), 'Tolerance should be an integer in [0, #controls * #replicates)'
             assert(self.__plot_format in set(plt.gcf().canvas.get_supported_filetypes().keys())), 'The plot format is invalid'
         except AssertionError as e:
             logger.error(e)
             raise
-    
-    
+
+
     def _check_file(self, df):
         try:
             assert(len(df) >= 1), 'The file is empty'
         except AssertionError as e:
             logger.error(e)
             raise
-    
+
 
     def _check_mass_spec_file(self, df):
         try:
             assert(df.shape[1] == self.__num_controls * self.__num_replicates + 1), 'The number of columns does not equal #replicates * #controls '
         except AssertionError as e:
             logger.error(e)
             logger.error('Check the input file is tab delimited (.tsv) and has correct data')
             raise
-    
+
 
     @abstractmethod
     def get_mass_data(self):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
     @abstractmethod
     def get_mass_spec_filename(self):
-        raise NotImplemented()
-    
+        raise NotImplementedError()
+
 
     def get_num_controls(self):
         return self.__num_controls
-    
+
 
     def get_num_replicates(self):
         return self.__num_replicates
-    
+
 
     def get_tolerance(self):
         return self.__tolerance
-    
+
 
     def get_plot_format(self):
         return self.__plot_format
-    
+
+    def get_cellular_compartment(self):
+        return self.__cellular_compartment
```

### Comparing `peeling-0.1.0/peeling/webpantherprocessor.py` & `peeling-0.2.0/peeling/webpantherprocessor.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from peeling.pantherprocessor import PantherProcessor
 import logging
+from peeling.pantherprocessor import PantherProcessor
 
 logger = logging.getLogger('peeling')
 
 
 class WebPantherProcessor(PantherProcessor):
     # overide superclass method
     def __init__(self, organism_id, unique_id):
```

### Comparing `peeling-0.1.0/peeling/webprocessor.py` & `peeling-0.2.0/peeling/webprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from peeling.processor import Processor
 import os
 #import shutil
 import uuid
 import logging
 import matplotlib.pyplot as plt
 import pandas as pd
+from peeling.processor import Processor
 
 
 logger = logging.getLogger('peeling')
 
 
 class WebProcessor(Processor):
     def __init__(self, *args):
         if len(args) == 2:
             user_input_reader, uniprot_communicator = args
             super().__init__(user_input_reader, uniprot_communicator)
             self.__uuid = None
             self.__web_plots_path = None
             self.__failed_id_mapping = 0
-            self.__surface_proteins_raw_data = None
+            self.__true_positive_proteins_raw_data = None
         elif len(args) == 3:
             unique_id, x, y = args
             self.__uuid = unique_id
             self.__x = x
             self.__y = y
         elif len(args) == 1:
             self.__uuid = args[0]
 
 
     #override superclass method
     def _mass_data_clean(self, data):
         data = super()._mass_data_clean(data)
-        data.to_csv(f'../results/{self.__uuid}/mass_spec_data.tsv', sep='\t', index=False) 
+        data.to_csv(f'../results/{self.__uuid}/mass_spec_data.tsv', sep='\t', index=False)
         return data
 
 
     # implement abstract method
     async def _get_id_mapping_data(self, mass_data):
         old_ids = list(mass_data.iloc[:, 0])
         meta={}
@@ -44,57 +44,57 @@
             self.__failed_id_mapping = meta['failed_id_mapping']
         return new_ids_df.copy()
 
 
     # implement abstract method
     async def _get_annotation_data(self, type):
         '''
-        type: 'surface' or 'cyto'
+        type: 'true_positive' or 'false_positive'
         '''
-        annotation = await self._get_uniprot_communicator().get_annotation(type) 
+        annotation = await self._get_uniprot_communicator().get_annotation(type)
         # logger.debug(f'\n{annotation.head()}')
         return annotation.copy()
-    
+
 
     # implement abstract method
-    def _plot_supplemental(self, fig_name): #plt, 
+    def _plot_supplemental(self, fig_name): #plt,
         plt.savefig(f'{self.__web_plots_path}/{fig_name}.jpeg', dpi=130, bbox_inches='tight')
         plt.close()
- 
+
 
     # implement abstract method
     def _construct_path(self):
         unique_id = str(uuid.uuid4())
         self.__uuid = unique_id
         parent_path = os.path.join('../results/', unique_id)
         results_path = os.path.join(parent_path, 'results')
         web_plots_path = os.path.join(parent_path, "web_plots")
         self.__web_plots_path = web_plots_path
-        try: 
-            os.makedirs(web_plots_path, exist_ok=True) 
-        except OSError as error: 
+        try:
+            os.makedirs(web_plots_path, exist_ok=True)
+        except OSError as error:
             logger.error(error)
         return results_path
-    
+
 
     # overriding method of super class
     def _write_args(self, path):
         super()._write_args(path)
         with open(os.path.join(path, 'log.txt'), 'a') as f:
             f.write('Failed id mapping: ' + str(self.__failed_id_mapping) + '\n')
 
-    
+
     # implement abstract method
     async def start(self):
         data = await self._get_user_input_reader().get_mass_data()
         results_path = self._construct_path()
         data = self._mass_data_clean(data)
         columns = list(data.columns[1:])
         await self._analyze(data, results_path)
-        self.__surface_proteins_raw_data.to_csv(f'../results/{self.__uuid}/post-cutoff-proteome_with_raw_data.tsv', sep='\t', index=False)
+        self.__true_positive_proteins_raw_data.to_csv(f'../results/{self.__uuid}/post-cutoff-proteome_with_raw_data.tsv', sep='\t', index=False)
         self._write_args(results_path)
         logger.info(f'Results saved at {self.__uuid}')
         #shutil.make_archive(f'../results/{self.__uuid}/results', 'zip', root_dir=f'../results/{self.__uuid}/results')
         #shutil.rmtree(f'../results/{self.__uuid}/results')
         return  self.__uuid, self.__failed_id_mapping, columns
 
 
@@ -142,9 +142,9 @@
                     format_line = format_line.strip()
                 return format_line[13:]
         except Exception as e:
             logger.error(e)
             raise
 
 
-    def _set_surface_proteins_raw_data(self, df):
-        self.__surface_proteins_raw_data = df
+    def _set_true_positive_proteins_raw_data(self, df):
+        self.__true_positive_proteins_raw_data = df
```

### Comparing `peeling-0.1.0/peeling/webuniprotcommunicator.py` & `peeling-0.2.0/peeling/webuniprotcommunicator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,112 @@
-from peeling.uniprotcommunicator import UniProtCommunicator
 import pandas as pd
 import numpy as np
 from datetime import datetime
 import logging
 import os
+from peeling.uniprotcommunicator import UniProtCommunicator
 
 logger = logging.getLogger('peeling')
 
 
 class WebUniProtCommunicator(UniProtCommunicator):
-    def __init__(self, cache=False):
-        super().__init__(cache)
+    def __init__(self, cache, cellular_compartment, tp_data=None, fp_data=None):
+        super().__init__(cache, cellular_compartment)
         self.__ids = None
         self.__track_update = 0
+        if isinstance(tp_data, pd.DataFrame) and isinstance(fp_data, pd.DataFrame):
+            self._annotation_true_positive = tp_data
+            self._annotation_false_positive = fp_data
+        else:
+            self.__init_annotations()
 
 
     # implement abstract method
     async def get_latest_id(self, old_ids, meta):
         if self.__ids is None:
             to_retrieve = old_ids
             logger.info('before retrieve, cached ids: 0')
 
         else:
             old_ids_set = set(old_ids)
             saved_ids_set = set(self.__ids['From'])
             to_retrieve = old_ids_set.difference(saved_ids_set)
             logger.info(f'before retrieve, cached ids: {len(self.__ids)}')
-        
+
         logger.info(f'to retrieve: {len(to_retrieve)}')
         if len(to_retrieve) > 0:
             retrieved_data = await self._retrieve_latest_id(list(to_retrieve), meta)
             retrieved_data = self.__add_no_mapping_ids(retrieved_data, meta)
-            # logger.debug(f'\n{retrieved_data.head()}')
+            logger.debug(f'\n{retrieved_data.head()}')
 
             self.__ids = pd.concat([self.__ids, retrieved_data])
             logger.info(f'after retrieve, cached ids: {len(self.__ids)}')
         return self.__ids[self.__ids['From'].isin(old_ids)]
 
 
     def __add_no_mapping_ids(self, retrieved_data, meta):
         # add ids that didn't find mapping data to cached ids, all fields are NaN
         no_mapping_ids = meta['no_id_mapping']
         if len(no_mapping_ids) > 0:
             no_mapping_ids = pd.DataFrame(list(no_mapping_ids), columns = ['From'])
             for col in retrieved_data.columns[1:]:
                 no_mapping_ids[col] = np.NaN
             retrieved_data = pd.concat([retrieved_data, no_mapping_ids])
-            # logger.debug(f'\n{no_mapping_ids.head()}')
+            logger.debug(f'\n{no_mapping_ids.head()}')
         return retrieved_data
- 
+
+
+    def __init_annotations(self):
+        annotation_types = ['true_positive', 'false_positive']
+        for annotation_type in annotation_types:
+            annotation_path = f'../retrieved_data/{self._cc_code}_annotation_{annotation_type}.tsv'
+            if os.path.exists(annotation_path):
+                annotation_data = pd.read_table(annotation_path, sep='\t', header=0)
+                logger.info(f'Read in {len(annotation_data)} entries from cached {self._cc_code}_annotation_{annotation_type} file')
+                self._set_annotation(annotation_data, annotation_type)
+            else:
+                logger.debug(f"*** didn't find cache in {annotation_path}")
+
 
     async def __initialize(self):
         start_time = datetime.now()
         logger.info('Initializing ...')
+        annotation_types = ['true_positive', 'false_positive']
         try:
             has_data = True
-            surface_path = '../retrieved_data/annotation_surface.tsv'
-            if os.path.exists(surface_path):
-                annotation_surface = pd.read_table(surface_path, sep='\t', header=0)
-                logger.info(f'Read in {len(annotation_surface)} entries from archived annotation_surface file')
-                self._set_annotation(annotation_surface, 'surface')
-            else:
-                has_data = False
+            for annotation_type in annotation_types:
+                annotation_path = f'../retrieved_data/{self._cc_code}_annotation_{annotation_type}.tsv'
+                if os.path.exists(annotation_path):
+                    annotation_data = pd.read_table(annotation_path, sep='\t', header=0)
+                    logger.info(f'Read in {len(annotation_data)} entries from cached {self._cc_code}_annotation_{annotation_type} file')
+                    self._set_annotation(annotation_data, annotation_type)
+                else:
+                    logger.debug(f"*** didn't find cache in {annotation_path}")
+                    has_data = False
 
-            cyto_path = '../retrieved_data/annotation_cyto.tsv'
-            if os.path.exists(cyto_path):
-                annotation_cyto = pd.read_table(cyto_path, sep='\t', header=0)
-                logger.info(f'Read in {len(annotation_cyto)} entries from archived annotation_cyto file')
-                self._set_annotation(annotation_cyto, 'cyto')
-            else:
-                has_data = False
-            
             if not has_data:
                 await self._retrieve_annotation()
-                surface = await self.get_annotation('surface')
-                surface.to_csv('../retrieved_data/annotation_surface.tsv', sep='\t', index=False)
-                cyto = await self.get_annotation('cyto')
-                cyto.to_csv('../retrieved_data/annotation_cyto.tsv', sep='\t', index=False)
+                for annotation_type in annotation_types:
+                    annotation_data = await self.get_annotation(annotation_type)
+                    annotation_data.to_csv(f'../retrieved_data/{self._cc_code}_annotation_{annotation_type}.tsv', sep='\t', index=False)
                 logger.info(f'Annotation files saved')
-        
+
             id_path = '../retrieved_data/latest_ids.tsv'
             if os.path.exists(id_path):
                 self.__ids = pd.read_table(id_path, sep='\t', header=0)
                 logger.info(f'Read in {len(self.__ids)} entries from archived latest_ids file')
-        
+
             end_time = datetime.now()
             logger.info(f'Initialization is done. Time: {end_time-start_time}')
-        
+
         except Exception as e:
             logger.error('Initialization failed')
             logger.info(e)
             raise
-        
+
 
 
     async def update_data(self):
         start_time = datetime.now()
         if self.__track_update == 0:
             try:
                 await self.__initialize()
@@ -111,22 +122,22 @@
                     updated_ids = self.__add_no_mapping_ids(updated_ids, meta)
                     num_diff = len(set(updated_ids['Entry']).difference(set(self.__ids['Entry'])))
                     logger.info(f'{num_diff} ids are updated')
                     self.__ids = updated_ids
                     self.__ids.to_csv('../retrieved_data/latest_ids.tsv', sep='\t', index=False)
                     logger.info('Latest_ids file saved')
                 await self._retrieve_annotation()
-                surface = await self.get_annotation('surface')
-                surface.to_csv('../retrieved_data/annotation_surface.tsv', sep='\t', index=False)
-                cyto = await self.get_annotation('cyto')
-                cyto.to_csv('../retrieved_data/annotation_cyto.tsv', sep='\t', index=False)
+                true_positive = await self.get_annotation('true_positive')
+                true_positive.to_csv(f'../retrieved_data/{self._cc_code}_annotation_true_positive.tsv', sep='\t', index=False)
+                false_positive = await self.get_annotation('false_positive')
+                false_positive.to_csv(f'../retrieved_data/{self._cc_code}_annotation_false_positive.tsv', sep='\t', index=False)
                 logger.info(f'Annotation files saved')
                 end_time = datetime.now()
                 logger.info(f'Update is done. Time: {end_time-start_time}')
                 self.__track_update += 1
             except Exception as e:
                 logger.error(e)
-        
-    
+
+
     # called in main.py, to export cached ids by api instead of waiting for update
     def get_ids(self):
-        return self.__ids
+        return self.__ids
```

### Comparing `peeling-0.1.0/peeling/webuserinputreader.py` & `peeling-0.2.0/peeling/webuserinputreader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from fastapi import UploadFile
 import pandas as pd
 import csv
-from peeling.userinputreader import UserInputReader
 import logging
+from peeling.userinputreader import UserInputReader
 
 logger = logging.getLogger('peeling')
 
 
 class WebUserInputReader(UserInputReader):
-    def __init__(self, mass_file:UploadFile, num_controls, num_replicates, tolerance, plot_format):
-        super().__init__(num_controls, num_replicates, tolerance, plot_format)
+    def __init__(self, mass_file:UploadFile, num_controls, num_replicates, tolerance, plot_format, cellular_compartment):
+        super().__init__(num_controls, num_replicates, tolerance, plot_format, cellular_compartment)
         self.__mass_file = mass_file
 
 
     async def __decode_uploadFile(self):
         bytes = await self.__mass_file.read()
         lines = [line for line in bytes.decode("utf-8").split("\n") if line]
         reader = csv.DictReader(lines, delimiter="\t", quotechar='"')
         df = pd.DataFrame(list(reader))
         logger.debug(f'\n{df.head()}')
-        self._check_file(df)        
+        self._check_file(df)
         return df
 
 
     # implement abstract method
     async def get_mass_data(self):
         data = await self.__decode_uploadFile()
         self._check_mass_spec_file(data)
         logger.info('Read in %d rows and %d columns from mass spec data' % data.shape)
         return data
-    
+
 
     # implement abstract method
     def get_mass_spec_filename(self):
-        return self.__mass_file.filename
+        return self.__mass_file.filename
```

### Comparing `peeling-0.1.0/peeling.egg-info/PKG-INFO` & `peeling-0.2.0/peeling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.1.0
+Version: 0.2.0
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -27,20 +27,20 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
+Project-URL: Homepage, https://github.com/JaneliaSciComp/peeling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # PEELing
 
 
 ### Introduction
 In the evolutionary transition from unicellular to multicellular organisms, single cells assemble into highly organized tissues and cooperatively carry out physiological functions. To act as an integrated system, individual cells communicate with each other extensively through signaling at the cellular interface. Cell-surface signaling thus controls almost every aspect of the development, physiology, and pathogenesis of multicellular organisms. In situ cell-surface proteomics or `iPEEL` (in situ cell-surface proteome extraction by extracellular labeling; developed by [Li, Han et al., 2020](https://pubmed.ncbi.nlm.nih.gov/31955847/) — `PMID: 31955847` and [Shuster, Li et al., 2022](https://pubmed.ncbi.nlm.nih.gov/36220098/) — `PMID: 36220098`) provides a method for quantitatively profiling cell-surface proteomes in native tissues with cell-type and spatiotemporal specificities. 
 
@@ -70,48 +70,52 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the IDs to the latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). As of our testing, it will take dozens of seconds to minutes for the process. 
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
-Therefore, it is recommended to save the retrieved data when first time run it, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Remember to update the retrieved data periodically.
+Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
-To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'"
+To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
 ```
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates -p organism
 ```
 
 
 ### Options
 -h, --help    Show help message and exit
 
 -t, --tolerance    Tolerance of non-included ratios ratio, default is 0. (For example, in an experiment with 2 non-labelled controls and 3 labelled replicates, there are 6 replicate-to-control ratios. In the default algorithm, a protein must pass cutoff in all 6 ratios to be included in the final proteome. If the tolerance is set to 1, a protein is included in the final proteome if it passes cutoff in any 5 ratios. If the tolerance is set to 2, a protein is included in the final proteome if it passes cutoff in any 4 ratios.) 
 
 -o, --output    Directory to store output results, default is the current work directory
 
 -i, --ids    Latest_ids file directory including filename, e.g. data/id_mapping.tsv
 
--s, --surface    Annotation_surface file directory including filename, e.g. data/annotation_surface.tsv
+--tp, --true-positive   path to true positive annotation file, e.g. data/annotation_true_positive.tsv
 
--c, --cyto    Annotation_cyto file directory including filename, e.g. data/annotation_cyto.tsv
+--fp, --false-positive  path to false positive annotation file, e.g. data/annotation_false_positive.tsv
 
 -a, --cache    Save the data retrieved from UniProt on the local computer, true if specified
 
 -f, --format    The format of the output plots, default is png. Supported formats depend on the computation platform, use -h/--help to see supported formats
 
 -n, --nomap    No id mapping for local annotation files, true if specified
 
 -p, --panther    The organism from which the mass spec data is made, a required input for Panther enrichment analysis. Please refer to Panther's API page http://pantherdb.org/services/oai/pantherdb/supportedgenomes for supported organism. Choose the corresponding 'long_names', and wrap it by quotes, e.g. 'Homo sapiens'
+
+--cc, --cellular_compartment    Choose between: cs - cell surface [default], mt - mitochondria, nu - nucleus or ot - other. If other is chosen, the true positive (--tp) and false positive (--fp) files must be specified
+
+-v --verbose    Enables verbose debugging output
```

### Comparing `peeling-0.1.0/peeling.egg-info/SOURCES.txt` & `peeling-0.2.0/peeling.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 peeling/__init__.py
+peeling/cellular_compartments.py
 peeling/clipantherprocessor.py
 peeling/cliprocessor.py
 peeling/cliuniprotcommunicator.py
 peeling/cliuserinputreader.py
 peeling/main.py
 peeling/pantherprocessor.py
 peeling/processor.py
```

### Comparing `peeling-0.1.0/peeling.egg-info/requires.txt` & `peeling-0.2.0/peeling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.1.0/pyproject.toml` & `peeling-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peeling"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="HHMI Janelia", email="peeling@janelia.hhmi.org" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
@@ -55,9 +55,12 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["peeling"]  # ["*"] by default
 exclude = []  # empty by default
 namespaces = false  # true by default
 
+[project.urls]
+Homepage = "https://github.com/JaneliaSciComp/peeling"
+
 [project.scripts]
 peeling = 'peeling.main:main'
```

### Comparing `peeling-0.1.0/test/test.py` & `peeling-0.2.0/test/test.py`

 * *Files identical despite different names*

