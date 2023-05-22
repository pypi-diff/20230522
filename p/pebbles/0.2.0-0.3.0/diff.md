# Comparing `tmp/pebbles-0.2.0.tar.gz` & `tmp/pebbles-0.3.0.tar.gz`

## Comparing `pebbles-0.2.0.tar` & `pebbles-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pebbles-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pebbles-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pebbles-0.2.0/.idea/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pebbles-0.2.0/src/pebbles/__init__.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pebbles-0.2.0/src/pebbles/countess.py
--rw-r--r--   0        0        0    12077 2020-02-02 00:00:00.000000 pebbles-0.2.0/src/pebbles/pebbles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     8621 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/test_pebbles.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/data/generate_test_sam.sh
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/data/map.bam
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/data/map.sam
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/data/query.fa
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pebbles-0.2.0/tests/data/ref.fa
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 pebbles-0.2.0/README.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pebbles-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 pebbles-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 pebbles-0.3.0/code_of_conduct.md
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pebbles-0.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pebbles-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pebbles-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pebbles-0.3.0/src/pebbles/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 pebbles-0.3.0/src/pebbles/countess.py
+-rw-r--r--   0        0        0    15863 2020-02-02 00:00:00.000000 pebbles-0.3.0/src/pebbles/pebbles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/test_pebbles.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/data/generate_test_sam.sh
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/data/map.bam
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/data/map.sam
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/data/query.fa
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pebbles-0.3.0/tests/data/ref.fa
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 pebbles-0.3.0/README.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pebbles-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pebbles-0.3.0/PKG-INFO
```

### Comparing `pebbles-0.2.0/.github/workflows/python-package.yml` & `pebbles-0.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/.github/workflows/python-publish.yml` & `pebbles-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/src/pebbles/countess.py` & `pebbles-0.3.0/src/pebbles/countess.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,49 +10,54 @@
     FileArrayParam,
     FileParam,
     FloatParam,
     MultiParam,
     StringParam,
     IntegerParam,
 )
-from countess.core.plugins import DaskInputPlugin
-from countess.utils.dask import concat_dataframes as concat_dask_dataframes
+from countess.core.plugins import PandasInputPlugin
 
 
-class CountSAMPlugin(DaskInputPlugin):
+class CountSAMPlugin(PandasInputPlugin):
     """Counts occurrences of alleles in a SAM file"""
 
     name = "SAM to Counts"
     title = "Count alleles in a SAM file (pebbles)"
     description = "Uses the Pebbles package to call variants from a SAM file to HGVS g. strings"
     version = VERSION
 
     file_types = [("SAM", "*.sam"),]
+    file_mode = 'r'
 
     parameters = {
         "max": IntegerParam("Maximum number of variants in a valid allele (read/alignment)", 1),
+        "min_quality": IntegerParam("Minimum quality score of alignment for a valid allele", 0),
     }
 
-    def read_file_to_dataframe(self, file_param, column_suffix="", row_limit=None):
+
+    def read_file_to_dataframe(self, file_param, logger, row_limit=None):
         records = {}
         count_column_name = "count"
-        if column_suffix:
-            count_column_name += "_" + str(column_suffix)
 
-        with pysam.AlignmentFile(file_param["filename"].value, 'r') as fh:
-            records = count_dict(fh, self.parameters["max"].value)
+        with pysam.AlignmentFile(file_param["filename"].value, self.file_mode) as fh:
+            records = count_dict(fh,
+                                 max_variants=self.parameters["max"].value,
+                                 min_quality=self.parameters["min_quality"].value,
+                                 row_limit=row_limit,
+                                 logger=logger)
 
         return pd.DataFrame.from_records(
             list(records.items()),  columns=("allele", count_column_name)
-        )
+            )
+
 
     def combine_dfs(self, dfs):
         """first concatenate the count dataframes, then group them by allele"""
 
-        combined_df = concat_dask_dataframes(dfs)
+        combined_df = pd.concat(dfs)
 
         if len(combined_df):
             combined_df = combined_df.groupby(by=["allele"]).sum()
 
         return combined_df
 
 class CountBAMPlugin(CountSAMPlugin):
@@ -60,25 +65,13 @@
 
     name = "BAM to Counts"
     title = "Count alleles in a BAM file (pebbles)"
     description = "Uses the Pebbles package to call variants from a BAM file to HGVS g. strings"
     version = VERSION
 
     file_types = [("BAM", "*.bam"),]
+    file_mode = 'rb'
 
     parameters = {
         "max": IntegerParam("Maximum number of variants in a valid allele (read/alignment)", 1),
+        "min_quality": IntegerParam("Minimum quality score of alignment for a valid allele", 0),
     }
-
-    def read_file_to_dataframe(self, file_param, column_suffix="", row_limit=None):
-        records = {}
-        count_column_name = "count"
-        if column_suffix:
-            count_column_name += "_" + str(column_suffix)
-
-        with pysam.AlignmentFile(file_param["filename"].value, 'rb') as fh:
-            records = count_dict(fh, self.parameters["max"].value)
-
-        return pd.DataFrame.from_records(
-            list(records.items()), columns=("allele", count_column_name)
-        )
-
```

### Comparing `pebbles-0.2.0/src/pebbles/pebbles.py` & `pebbles-0.3.0/src/pebbles/pebbles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,66 @@
 # Pebbles. Sister of BammBamm Flinstone
 # A per read bam mutation caller
 import argparse
 import collections
 import re
 import sys
+import traceback
 from collections import defaultdict
+from itertools import islice
 from collections.abc import Iterable, Mapping
-from typing import Tuple
+from typing import Tuple, Optional
 from pebbles import VERSION
 
 import pysam
 
 
+class Logger:
+    """Basic Logger compatible with CountESS.core.logger"""
+
+    def __init__(self, stdout=sys.stdout, stderr=sys.stderr, prefix: Optional[str] = None):
+        self.stdout = stdout
+        self.stderr = stderr
+        self.prefix = prefix
+
+    def progress(self, message: str = "Running", percentage: Optional[int] = None):
+        if self.prefix:
+            message = self.prefix + ": " + message
+        if percentage:
+            message += f" [{int(percentage):2d}%]"
+        self.stdout.write(f"{message}\n")
+
+    def log(self, level: str, message: str, detail: Optional[str] = None):
+        if self.prefix:
+            message = self.prefix + ": " + message
+        if detail:
+            message += " " + repr(detail)
+
+        self.stderr.write(message + "\n")
+
+    def info(self, message: str, detail: Optional[str] = None):
+        """Log a message at level info"""
+        self.log("info", message, detail)
+
+    def warning(self, message: str, detail: Optional[str] = None):
+        """Log a message at level warning"""
+        self.log("warning", message, detail)
+
+    def error(self, message: str, detail: Optional[str] = None):
+        """Log a message at level error"""
+        self.log("error", message, detail)
+
+    def exception(self, exception: Exception):
+        self.error(str(exception), detail="".join(traceback.format_exception(exception)))
+
+    def clear(self):
+        """Clear logs (if possible)"""
+        return None
+
+
 def expand_cigar(cigar: str) -> str:
     """Convert a compact cigar string with state counts eg '2S10M1I5M1D1M'
     to a fully expanded string of state operators eg 'SSMMMMMMMMMMIMMMMMDM'
     Supports the operators MIDNSHPX=
     see https://en.wikipedia.org/wiki/Sequence_alignment#Representations
 
         Arguments:
@@ -36,22 +81,22 @@
             o   cigar : a cigar string eg 80M5D10M10I
         Returns:
             o   string : gapped seqeunce
     """
     deletion_symbol = 'I' if is_reference else 'D'
     gapped = []
     xcigar = expand_cigar(cigar)
-    seq = list(seq)
+    seq_list = list(seq)
     for symbol in xcigar:
         if symbol == deletion_symbol:
             gapped.append('-')
         elif is_reference and symbol == 'S':
             gapped.append('-')
         else:
-            gapped.append(seq.pop(0))
+            gapped.append(seq_list.pop(0))
     return "".join(gapped)
 
 
 def expand_mdtag(mdtag: str) -> str:
     """Convert a SAM MD tag eg '6^TAG3G2' containing information on
     the reference sequence content not included in the read to a string
     of expanded match tokens '.' and reference states
@@ -123,46 +168,60 @@
                 nonref_bases += 1
             mutations.append(f'{refname}:g.{insstart}_{insstart + 1}ins{inserted}')
         if (expanded_cigar[i] == 'M' and expanded_engapped_md[i] != '.') or \
                 expanded_cigar[i] == 'X':
             mutant = ''
             reference = ''
             substart = i + pos + 1 + nonref_bases - softmasked
-            while expanded_cigar[i] in 'MX' and expanded_engapped_md[i] != '.':
+            while len(expanded_cigar) > i and expanded_cigar[i] in 'MX' and len(expanded_engapped_md) > i and expanded_engapped_md[i] != '.':
                 mutant += gapped_read[i]
                 reference += expanded_engapped_md[i]
                 i += 1
             if len(mutant) == 1:
                 mutations.append(f'{refname}:g.{substart}{reference}>{mutant}')
             else:
                 mutations.append(f'{refname}:g.{substart}_{i + pos + nonref_bases - softmasked}delins{mutant}')
         i += 1
     return mutations
 
 
-def call_mutations_from_pysam(pysamfile: collections.abc.Iterable) -> Tuple[str, list]:
+def call_mutations_from_pysam(pysamfile: collections.abc.Iterable,
+                              min_quality: int =0,
+                              logger: Optional[Logger] = None,
+                              ) -> Iterable[Tuple[str, list]]:
     """A generator function to call variants in all reads in a SAM/BAM
     file to HGVS format, on a per read basis.
     Assumes single end sequencing or merged paired end sequencing
+    qcfail, supplementary and unmapped segments are ignored
+
     Arguments:
         pysamfile: a pysam.AlignmentFile object
                    eg SAM pysam.AlignmentFile("data.sam", "r")
                       BAM pysam.AlignmentFile("data.bam", "rb")
+        min_quality:  the minimum mapping quality score for a reported allele. Default 0.
+        logger:    a logger object with a .warning() method such as CountESS.core.logger
+                   default: None
+
 
     Yields:
         a list of HGVS formatted variant events per read
     """
 
     for segment in pysamfile:
         if segment.is_qcfail or segment.is_supplementary or segment.is_unmapped:
             continue
+        if segment.mapping_quality < min_quality:
+            continue
         try:
             mdtag = segment.get_tag('MD')
         except KeyError:
-            print(f'skipping {segment.qname} as it has no MD tag')
+            if logger:
+                logger.warning(f'skipping {segment.qname} as it has no MD tag')
+            else:
+                print(f'skipping {segment.qname} as it has no MD tag')
             # skip reads with no MD tag
             continue
 
         mutations = call_mutations(segment.reference_name,
                                    segment.pos,
                                    engap(expand_mdtag(mdtag),
                                          segment.cigarstring,
@@ -180,51 +239,71 @@
     if len(variants) > 1:
         return variants[0].split(':g.')[0] + ':g.[' + ";".join([variant.split(':g.')[-1] for variant in variants]) + ']'
     else:
         return variants[0]
 
 
 def count_dict(pysamfile: Iterable,
-          max_variants: int =1,
-          ) -> Mapping[str, int]:
+               max_variants: int = 1,
+               row_limit: Optional[int] = None,
+               min_quality: int = 0,
+               logger: Optional[Logger] = None,
+               ) -> Mapping[str, int]:
     """
     Counts occurrences of alleles in a SAM or BAM file
 
     Arguments:
-        pysamfile - an iterable of alignment segment objects from pysam
-        max_variants - the maximum number of variants in a reported allele
+        pysamfile    : an iterable of alignment segment objects from pysam
+        max_variants : the maximum number of variants in a reported allele. Default 1
+        row_limit    : the maximum number of alignments to process. Default None (ie process all)
+        min_quality  : the minimum mapping quality score for a reported allele. Default 0
+        logger       : a logger object with a .progress() & .warning() method such as CountESS.core.logger
+                       default: None
+
 
     Returns:
         A dictionary keyed by allele HGVS strings of counts
     """
-    counts = defaultdict(int)
-    for readname,variants in call_mutations_from_pysam(pysamfile):
+    counts : dict[str,int] = defaultdict(int)
+    number = 0
+    for readname, variants in islice(call_mutations_from_pysam(pysamfile, min_quality, logger), row_limit):
+        number += 1
+        if logger and number % 1000 == 0:
+            logger.progress(f"Loading {pysamfile.filename.decode()}")
         if variants and len(variants) <= max_variants:
             counts[fix_multi_variants(variants)] += 1
+
+    if logger:
+        logger.progress(f"Loaded {pysamfile.filename.decode()}",100)
+        if len(counts) == 0 and row_limit is not None:
+            logger.warning(f"No mutations found in first {row_limit} alignments")
+
     return counts
 
 
 def count(pysamfile: Iterable,
-          max_variants: int =1,
+          max_variants: int = 1,
+          min_quality: int = 0,
           ) -> str:
     """
     Counts occurrences of alleles in a SAM or BAM file
 
     Arguments:
         pysamfile - an iterable of alignment segment objects from pysam
-        max_variants - the maximum number of variants in a reported allele
+        max_variants - the maximum number of variants in a reported allele. Default 1
+        min_quality - the minimum mapping quality score for a reported allele. Default 0
 
     Returns:
         A tsv formatted text string of allele HGVS description and counts
     """
-    counts = count_dict(pysamfile, max_variants)
+    counts = count_dict(pysamfile, max_variants=max_variants, min_quality=min_quality)
     return ''.join([f'{key}\t{counts[key]}\n' for key in counts])
 
 
-def cli(arguments: str = None) -> argparse.Namespace:
+def cli(arguments: Optional[str] = None) -> argparse.Namespace:
     """command line interface. Use pebbles -h to see help"""
     parser = argparse.ArgumentParser(description=f"pebbles v{VERSION}" + """
                   (                                                                
              /((/ ###((%*                                                       
             /%(((((@(((%&(                                                      
              @(#(((((%                      @,     &#(#&&   *                   
                 #%(((    (,              (*       @/@(**#&**                    
@@ -254,28 +333,38 @@
            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
     """, formatter_class=argparse.RawTextHelpFormatter)
     subparsers = parser.add_subparsers(dest='command')
     count = subparsers.add_parser('count',
                                   help='count occurrences of a variant')
     call = subparsers.add_parser('call',
-                                  help='count occurrences of a variant')
+                                 help='count occurrences of a variant')
     count.add_argument('--max',
                        type=int,
                        default=1,
                        help='Maximum number of variants in a read to include in count table'
                        )
+    count.add_argument('--min_quality',
+                       type=int,
+                       default=0,
+                       help='Minimum quality score required to count a variant'
+                       )
     count.add_argument('infile',
-                        type=str,
-                        help='a SAM or BAM format file of mapped single end reads',
-                        )
+                       type=str,
+                       help='a SAM or BAM format file of mapped single end reads',
+                       )
+    call.add_argument('--min_quality',
+                      type=int,
+                      default=0,
+                      help='Minimum quality score required to call a variant'
+                      )
     call.add_argument('infile',
-                        type=str,
-                        help='a SAM or BAM format file of mapped single end reads',
-                        )
+                      type=str,
+                      help='a SAM or BAM format file of mapped single end reads',
+                      )
     parser.add_argument('--version',
                         action='store_true',
                         help='print version information and exit')
     if arguments:
         args = parser.parse_args(arguments.split(' '))
     else:
         args = parser.parse_args()
@@ -291,16 +380,16 @@
     if args.infile.split('.')[-1].lower() == 'sam':
         infile = pysam.AlignmentFile(args.infile, "r")
     else:
         infile = pysam.AlignmentFile(args.infile, "rb")
 
     if args.command == 'call':
         print('readname\tvariants')
-        for x in call_mutations_from_pysam(infile):
+        for x in call_mutations_from_pysam(infile, min_quality=args.min_quality):
             print("\t".join([str(_) for _ in x]))
     elif args.command == 'count':
         print('variant\tcount')
-        print(count(infile, max_variants=args.max), end='')
+        print(count(infile, max_variants=args.max, min_quality=args.min_quality), end='')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pebbles-0.2.0/tests/test_pebbles.py` & `pebbles-0.3.0/tests/test_pebbles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import unittest
 import pathlib
 from pebbles.pebbles import *
 
 TEST_SAM = pathlib.Path(__file__).parent.joinpath("data/map.sam")
 TEST_BAM = pathlib.Path(__file__).parent.joinpath("data/map.bam")
-#TEST_CRAM = pathlib.Path(__file__).parent.joinpath("data/map.cram")
+
+
+# TEST_CRAM = pathlib.Path(__file__).parent.joinpath("data/map.cram")
 
 
 class PebblesTestCase(unittest.TestCase):
     def test_expand_cigar(self):
         self.assertEqual(expand_cigar('80M5D2M2I10M'), 'M' * 80 + 'D' * 5 + 'M' * 2 + 'I' * 2 + 'M' * 10)
         self.assertEqual(expand_cigar('2S4M5D2M2I10M'), 'SSMMMMDDDDDMMIIMMMMMMMMMM')
         pass
@@ -77,16 +79,16 @@
                'expanded_engapped_md': '.....................................................A...................................................',
                'expanded_cigar': 'MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM',
                'gapped_read': 'ACAGGCATGGGACCCTGCAGGGTTCTTGGCTTGGCGGCGGGACGAGAACGAGGTGACGACTCGGGCAAGCCTTTTTGTTTATACCAACAGCAACAACACAAAGGG'
                }), ['AY286018:g.59A>T'])
         self.assertEqual(call_mutations(
             **{'refname': 'AY286018', 'pos': 5,
                'expanded_engapped_md': '.....................................................A.....',
-               'expanded_cigar':       '=====================================================X=====',
-               'gapped_read':          'ACAGGCATGGGACCCTGCAGGGTTCTTGGCTTGGCGGCGGGACGAGAACGAGGTGACGA'
+               'expanded_cigar': '=====================================================X=====',
+               'gapped_read': 'ACAGGCATGGGACCCTGCAGGGTTCTTGGCTTGGCGGCGGGACGAGAACGAGGTGACGA'
                }), ['AY286018:g.59A>T'])
 
     def test_call_mutations_from_pysam(self):
         result = [call for call in call_mutations_from_pysam(pysam.AlignmentFile(TEST_SAM, "r"))]
         self.assertEqual(result,
                          [('WT', []),
                           ('16_18delGAC', ['AY286018:g.16_18delGAC']),
@@ -106,25 +108,62 @@
                           ('19_20delinsAG', ['AY286018:g.19_20delinsAG']),
                           ('19_20delinsAG', ['AY286018:g.19_20delinsAG']),
                           ('19_21delinsATG', ['AY286018:g.19_21delinsATG']),
                           ('59A>T', ['AY286018:g.59A>T']),
                           ('59A>T', ['AY286018:g.59A>T']),
                           ('42G>T;59A>T', ['AY286018:g.42G>T', 'AY286018:g.59A>T']),
                           ])
+        result = [call for call in call_mutations_from_pysam(pysam.AlignmentFile(TEST_BAM, "rb"), min_quality=61)]
+        self.assertEqual(result,[])
+
 
     def test_fix_multi_variants(self):
         self.assertEqual(fix_multi_variants(['AY286018:g.16_18delGAC', 'AY286018:g.59A>T']),
                          'AY286018:g.[16_18delGAC;59A>T]'
-                        )
+                         )
+
+    def test_count_dict(self):
+        self.assertEqual(count_dict(pysam.AlignmentFile(TEST_BAM, "rb")),
+                         {'AY286018:g.16_18delGAC': 1,
+                          'AY286018:g.18_19insATG': 1,
+                          'AY286018:g.19_20delinsAG': 2,
+                          'AY286018:g.19_21delinsATG': 1,
+                          'AY286018:g.59A>T': 2}
+                         )
+        self.assertEqual(count_dict(pysam.AlignmentFile(TEST_BAM, "rb"), row_limit=3),
+                         {'AY286018:g.16_18delGAC': 1,
+                          'AY286018:g.18_19insATG': 1}
+                         )
+        self.assertEqual(count_dict(pysam.AlignmentFile(TEST_BAM, "rb"), min_quality=61),
+                         {}
+                         )
 
     def test_count(self):
+        self.assertEqual(count(pysam.AlignmentFile(TEST_BAM, "rb"), min_quality=61),
+                        ''
+                         )
+        self.assertEqual(count(pysam.AlignmentFile(TEST_BAM, "rb"), min_quality=60),
+                         ('AY286018:g.16_18delGAC\t1\n'
+                          'AY286018:g.18_19insATG\t1\n'
+                          'AY286018:g.19_20delinsAG\t2\n'
+                          'AY286018:g.19_21delinsATG\t1\n'
+                          'AY286018:g.59A>T\t2\n')
+                         )
         self.assertEqual(count(pysam.AlignmentFile(TEST_BAM, "rb")),
                          ('AY286018:g.16_18delGAC\t1\n'
-                             'AY286018:g.18_19insATG\t1\n'
-                             'AY286018:g.19_20delinsAG\t2\n'
-                             'AY286018:g.19_21delinsATG\t1\n'
-                             'AY286018:g.59A>T\t2\n')
+                          'AY286018:g.18_19insATG\t1\n'
+                          'AY286018:g.19_20delinsAG\t2\n'
+                          'AY286018:g.19_21delinsATG\t1\n'
+                          'AY286018:g.59A>T\t2\n')
                          )
+        self.assertEqual(count(pysam.AlignmentFile(TEST_SAM, "r")),
+                         ('AY286018:g.16_18delGAC\t1\n'
+                          'AY286018:g.18_19insATG\t1\n'
+                          'AY286018:g.19_20delinsAG\t2\n'
+                          'AY286018:g.19_21delinsATG\t1\n'
+                          'AY286018:g.59A>T\t2\n')
+                         )
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pebbles-0.2.0/tests/data/map.bam` & `pebbles-0.3.0/tests/data/map.bam`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/tests/data/map.sam` & `pebbles-0.3.0/tests/data/map.sam`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/tests/data/query.fa` & `pebbles-0.3.0/tests/data/query.fa`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/tests/data/ref.fa` & `pebbles-0.3.0/tests/data/ref.fa`

 * *Files identical despite different names*

### Comparing `pebbles-0.2.0/README.md` & `pebbles-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Pebbles is a lightweight converter of BAM or SAM files to genomic HGVS. This means that the resulting
 calls will be in the format g.REFNAME:REFPOSITION and will not be corrected to be the most 3' variant 
 (due to the way most aligners work they will be 5' shifted on the + reference strand).
 For most uses you will want to process the output of pebbles with a HGVS validator and usually project
 them into a different coordinate space such as the c. coordinates of the gene/transcript of interest.
 This can be done with packages such as https://hgvs.readthedocs.io or websites like mutalyzer.nl
 
-Currently pebbles ignores quality scores and assumes all reads are a single unpaired unique observation.
+Currently pebbles ignores per base quality scores and assumes all reads are a single unpaired unique observation.
 In most uses it will be desirable to align overlaps for paired end sequencing and trim reads before calling.
 
 
 # Installation
 To install from PyPI using pip:
 
 ```shell
@@ -76,9 +76,47 @@
 AY286018:g.16_18delGAC  1
 AY286018:g.18_19insATG  1
 AY286018:g.19_20delinsAG    2
 AY286018:g.19_21delinsATG   1
 AY286018:g.59A>T    2
 ```
 
+For more detailed usage information see 
+```shell
+pebbles --help
+```
+
+# Usage as a CountESS plugin
+
+The CountESS project is a graphical workflow manager for analysing count based datasets, in particular Deep Mutational
+Scanning (DMS) and other Multiplex Assays of Variant Effects. CountESS is built with an entrypoint and inheritance
+based plugin system, that pebbles implements.
+
+To use pebbles in a CountESS workflow both Pebbles and CountESS need to be installed in the same python environment.
+Once correctly installed the BAM and SAM parsing workflow steps should automatically be detected by CountESS and made
+available in the user interface.
+
+For further information on CountESS see 
+[https://github.com/CountESS-Project/CountESS](https://github.com/CountESS-Project/CountESS)
+
+# Contributing to Pebbles
+Pebbles is licensed under the BSD-3-Clause license.  
+You are free to fork this repository under the terms of that license.
+If you have suggested changes please start by raising an issue in the issue tracker.
+Pull requests are welcome and will be included at the discretion of the author.
+Pull requests should be based on the 'develop' branch 
+(with the exception of bugfixes where develop has diverged from main).
+Bug reports should be made to the issue tracker.
+
+Difficulty in understanding how to use the software is a documentation bug, and should also be raised on the
+issue tracker so your question and my response are easily found by others.
+
+Pebbles aims to maintain a respectful and inclusive community and adopts the
+[contributor covenant v2.1](code_of_conduct.md)
+
+# Citing Pebbles
+
+Pebbles is currently unpublished. 
+The current release can be cited using the Zenodo DOI. 
+
 # License
 Pebbles is released under the BSD 3 Clause License https://opensource.org/license/bsd-3-clause/
```

### Comparing `pebbles-0.2.0/pyproject.toml` & `pebbles-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pebbles"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Matthew Wakefield", email="matthew.wakefield@unimelb.edu.au" },
 ]
 description = "A package for calling HGVS variants in single SAM/BAM alignments"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -15,14 +15,19 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
   "pysam >= 0.20.0",
 ]
 
+[project.optional-dependencies]
+countess = [
+    "countess >= 0.0.24, < 0.1"
+]
+
 [project.scripts]
 pebbles = "pebbles.pebbles:main"
 
 [project.entry-points.countess_plugins]
 count_SAM = "pebbles.countess:CountSAMPlugin"
 count_BAM = "pebbles.countess:CountBAMPlugin"
```

### Comparing `pebbles-0.2.0/PKG-INFO` & `pebbles-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pebbles
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package for calling HGVS variants in single SAM/BAM alignments
 Project-URL: Homepage, https://github.com/genomematt/pebbles
 Project-URL: Bug Tracker, https://github.com/genomematt/pebbles
 Author-email: Matthew Wakefield <matthew.wakefield@unimelb.edu.au>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Requires-Dist: pysam>=0.20.0
+Provides-Extra: countess
+Requires-Dist: countess<0.1,>=0.0.24; extra == 'countess'
 Description-Content-Type: text/markdown
 
 # pebbles
 
 Pebbles is a package for calling variants from single reads into HGVS format.
 
 In many use cases we are interested in calling variants from a single read rather than the more
@@ -26,15 +28,15 @@
 Pebbles is a lightweight converter of BAM or SAM files to genomic HGVS. This means that the resulting
 calls will be in the format g.REFNAME:REFPOSITION and will not be corrected to be the most 3' variant 
 (due to the way most aligners work they will be 5' shifted on the + reference strand).
 For most uses you will want to process the output of pebbles with a HGVS validator and usually project
 them into a different coordinate space such as the c. coordinates of the gene/transcript of interest.
 This can be done with packages such as https://hgvs.readthedocs.io or websites like mutalyzer.nl
 
-Currently pebbles ignores quality scores and assumes all reads are a single unpaired unique observation.
+Currently pebbles ignores per base quality scores and assumes all reads are a single unpaired unique observation.
 In most uses it will be desirable to align overlaps for paired end sequencing and trim reads before calling.
 
 
 # Installation
 To install from PyPI using pip:
 
 ```shell
@@ -93,9 +95,47 @@
 AY286018:g.16_18delGAC  1
 AY286018:g.18_19insATG  1
 AY286018:g.19_20delinsAG    2
 AY286018:g.19_21delinsATG   1
 AY286018:g.59A>T    2
 ```
 
+For more detailed usage information see 
+```shell
+pebbles --help
+```
+
+# Usage as a CountESS plugin
+
+The CountESS project is a graphical workflow manager for analysing count based datasets, in particular Deep Mutational
+Scanning (DMS) and other Multiplex Assays of Variant Effects. CountESS is built with an entrypoint and inheritance
+based plugin system, that pebbles implements.
+
+To use pebbles in a CountESS workflow both Pebbles and CountESS need to be installed in the same python environment.
+Once correctly installed the BAM and SAM parsing workflow steps should automatically be detected by CountESS and made
+available in the user interface.
+
+For further information on CountESS see 
+[https://github.com/CountESS-Project/CountESS](https://github.com/CountESS-Project/CountESS)
+
+# Contributing to Pebbles
+Pebbles is licensed under the BSD-3-Clause license.  
+You are free to fork this repository under the terms of that license.
+If you have suggested changes please start by raising an issue in the issue tracker.
+Pull requests are welcome and will be included at the discretion of the author.
+Pull requests should be based on the 'develop' branch 
+(with the exception of bugfixes where develop has diverged from main).
+Bug reports should be made to the issue tracker.
+
+Difficulty in understanding how to use the software is a documentation bug, and should also be raised on the
+issue tracker so your question and my response are easily found by others.
+
+Pebbles aims to maintain a respectful and inclusive community and adopts the
+[contributor covenant v2.1](code_of_conduct.md)
+
+# Citing Pebbles
+
+Pebbles is currently unpublished. 
+The current release can be cited using the Zenodo DOI. 
+
 # License
 Pebbles is released under the BSD 3 Clause License https://opensource.org/license/bsd-3-clause/
```

