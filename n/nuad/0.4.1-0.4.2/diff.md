# Comparing `tmp/nuad-0.4.1.tar.gz` & `tmp/nuad-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuad-0.4.1.tar", last modified: Sun Mar 12 18:55:55 2023, max compression
+gzip compressed data, was "nuad-0.4.2.tar", last modified: Mon May 22 19:29:35 2023, max compression
```

## Comparing `nuad-0.4.1.tar` & `nuad-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 18:55:55.138579 nuad-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-03-12 18:55:47.000000 nuad-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-12 18:55:47.000000 nuad-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    27515 2023-03-12 18:55:55.138579 nuad-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    26997 2023-03-12 18:55:47.000000 nuad-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 18:55:55.138579 nuad-0.4.1/nuad/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)   358355 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/constraints.py
--rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/json_noindent_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8296 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/modifications.py
--rw-r--r--   0 runner    (1001) docker     (122)    56828 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/np.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 18:55:55.138579 nuad-0.4.1/nuad/nupack_viennaRNA_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (122)   251648 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/nupack_viennaRNA_parameter_files/dna_mathews1999.par
--rw-r--r--   0 runner    (1001) docker     (122)   380873 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/nupack_viennaRNA_parameter_files/dna_mathews2004.par
--rw-r--r--   0 runner    (1001) docker     (122)   115224 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (122)    31635 2023-03-12 18:55:47.000000 nuad-0.4.1/nuad/vienna_nupack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-12 18:55:55.138579 nuad-0.4.1/nuad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    27515 2023-03-12 18:55:55.000000 nuad-0.4.1/nuad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-12 18:55:55.000000 nuad-0.4.1/nuad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-12 18:55:55.000000 nuad-0.4.1/nuad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-12 18:55:55.000000 nuad-0.4.1/nuad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-12 18:55:55.000000 nuad-0.4.1/nuad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-12 18:55:47.000000 nuad-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-12 18:55:55.138579 nuad-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-03-12 18:55:47.000000 nuad-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:29:35.053551 nuad-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-05-22 19:29:26.000000 nuad-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-22 19:29:26.000000 nuad-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    27499 2023-05-22 19:29:35.053551 nuad-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    26981 2023-05-22 19:29:26.000000 nuad-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:29:35.049551 nuad-0.4.2/nuad/
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   375716 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/json_noindent_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8296 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/modifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56332 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/np.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:29:35.053551 nuad-0.4.2/nuad/nupack_viennaRNA_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (122)   251648 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/nupack_viennaRNA_parameter_files/dna_mathews1999.par
+-rw-r--r--   0 runner    (1001) docker     (122)   380873 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/nupack_viennaRNA_parameter_files/dna_mathews2004.par
+-rw-r--r--   0 runner    (1001) docker     (122)   115196 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-22 19:29:26.000000 nuad-0.4.2/nuad/vienna_nupack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:29:35.053551 nuad-0.4.2/nuad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    27499 2023-05-22 19:29:34.000000 nuad-0.4.2/nuad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-22 19:29:35.000000 nuad-0.4.2/nuad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:29:34.000000 nuad-0.4.2/nuad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-22 19:29:34.000000 nuad-0.4.2/nuad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-22 19:29:34.000000 nuad-0.4.2/nuad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-22 19:29:26.000000 nuad-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:29:35.053551 nuad-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-22 19:29:26.000000 nuad-0.4.2/setup.py
```

### Comparing `nuad-0.4.1/LICENSE` & `nuad-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/PKG-INFO` & `nuad-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuad
-Version: 0.4.1
+Version: 0.4.2
 Summary: nuad stands for "NUcleic Acid Designer". Enables one to specify constraints on a DNA (or RNA) nanostructure made from synthetic DNA/RNA and then attempts to find concrete DNA sequences that satisfy the constraints.
 Home-page: https://github.com/UC-Davis-molecular-computing/nuad
 Author: David Doty
 Author-email: doty@ucdavis.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -138,15 +138,15 @@
 
 - `Domain`: A `Domain` represents a contiguous subsequence of DNA. A single `Domain` represents both the DNA sequence and its complement. For instance there is one `Domain` with name `a`, with two versions: unstarred (`a`) and starred (`a*`). If the DNA sequence of `a` is 5'-CCCAA-3', then the DNA sequence of `a*` is 3'-GGGTT-5'. 
 
 - `DomainPool`: Each `Domain` is assigned a single `DomainPool`, which can be thought of as a "source of DNA sequences" for the `Domain`. (See exceptions below.) The sequence design algorithm will take DNA sequences from this source when attempting to find DNA sequences to assign to `Domain`'s to satisfy all constraints. Each `DomainPool` has a fixed length. Since each `Domain` only has one `DomainPool`, this means that each `Domain` has a fixed length as well. If no other constraints are specified, then the `DomainPool` simply provides all DNA sequences of that length. Though you will generally not call this method yourself, the method `DomainPool.generate_sequence()` returns a sequence from the pool. This method can be called infinitely many times (i.e., sequences can repeat, though the exact period after which they repeat is an unspecified implementation detail.)
 
   - There are two types of `Domain`'s with no associated `DomainPool`. One type is a `Domain` with the field `fixed` set to `True` by calling the method `Domain.set_fixed_sequence()`, which has some fixed DNA sequence that cannot be changed. A fixed `Domain` has no `DomainPool`.)
 
-  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.dependent and https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.subdomains.
+  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://nuad.readthedocs.io/en/latest/#constraints.Domain.dependent and https://nuad.readthedocs.io/en/latest/#constraints.Domain.subdomains.
 
 - `Strand`: A `Strand` contains an ordered list `domains` of `Domain`'s, together with an identification of which `Domain`'s are starred in this `Strand`, the latter specified as a set `starred_domain_indices` of indices (starting at 0) into the list `domains`. For example, the `Strand` consisting of `Domain`'s `a`, `b*`, `c`, `b`, `d*`, in that order, would have `domains = [a, b, c, b, d]` and `starred_domain_indices = {1, 4}`.
 
 - `Design`: This describes the whole system. Generally you will have one `Design`, which is composed of a list of `Strand`'s.
 
 - `Constraint`: There are several kinds of constraint objects. Not all of them are related in the type hierarchy. 
 
@@ -155,15 +155,15 @@
 
     - **"soft" constraints:**  All other constraints are subclasses of the abstract superclass `Constraint`. These constrains are "softer": sequences violating the constraints are allowed to be assigned to `Domain`'s. The sequence design algorithm steadily improves the design by changing sequences until all of these constraints are satisfied. The different subtypes of the base class `Constraint` correspond to different parts of the `Design` that are being evaluated by the `Constraint`. The types are:
 
         - `SingularConstraint`: This is an abstract superclass of the following concrete subclasses. The difference with the other abstract superclass `BulkConstraint` is explained in `BulkConstraint` below.
         
             - `DomainConstraint`: This only looks at a single `Domain`. In practice this is not used much, since there's not much information in a `Domain` other than its DNA sequence, so a `SequenceConstraint` or `NumpyConstraint` typically would already have filtered out any DNA sequence not satisfying such a constraint.
 
-            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://dnadsd.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
+            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://nuad.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
 
             - `DomainPairConstraint`: This evaluates a pair of `Domain`'s.
 
             - `StrandPairConstraint`: This evaluates a pair of `Strand`'s.
 
             - `ComplexConstraint`: This evaluates a tuple of `Strand`'s of arbitrary size.
 
@@ -179,15 +179,15 @@
 
     The `BulkConstraint` subclasses `DomainsConstraint`, `StrandsConstraint`, `DomainPairsConstraint`, `StrandPairsConstraint` use a different function, called `evaluate_bulk`, which take as input a list of "`Design` parts" (e.g., a list of pairs of `Strand`'s for a `StrandPairsConstraint`). The return value is of type `List[Tuple[DesignPart, float, str]]`, i.e., a list of triples, where each triple is `(part, excess, summary)`.
     
     `part` is the individual part of the design that caused a problem. Generally it will be one of the elements of the list passed to `evaluate_bulk`, though the returned list could be smaller than the input list. This is because some parts may satisfy the constraint, and generally the only parts returned from `evaluate_bulk` are those that violated the constraint. `excess` and `summary` have the same interpretation as with the "singular" constraints.
 
     The search algorithm evaluates the constraints, and for each violated constraint, it turns the `excess` value into a "score" by first passing it through the "score transfer function", which by default squares the value, and then multiplies by the value `Constraint.weight` (by default 1). The goal of the search is to minimize the sum of scores across all violated `Constraint`'s. The reason that the score is squared is that this leads the search algorithm to (slightly) favor reducing the excess of constraint violations that are "more in excess", i.e., it would reduce the total score more to reduce an excess from 4 to 3 (reducing the score from 4<sup>2</sup>=16 to 3<sup>2</sup>=9, a reduction of 16-9=7) than to reduce an excess from 2 to 1 (which reduces 2<sup>2</sup>=4 to 1<sup>2</sup>=1, a reduction of only 4-1=3).
 
-    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_dna_sequences](https://dnadsd.readthedocs.io/en/latest/#search.search_for_dna_sequences).
+    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_sequences](https://nuad.readthedocs.io/en/latest/#search.search_for_sequences).
 
 
 ## Constraint evaluations must be pure functions of their inputs
 
 For all constraints, it is critical that the `evaluate` or `evaluate_bulk` functions be *pure* functions of their inputs: the return value should depend only on the parameters passed to the function. For example, a `StrandPairConstraint` takes two strands as input, and its `(excess, summary)` return values should depend *only* on those two strands. Similarly, a `StrandsConstraint`, whose `evaluate_bulk` function takes a list of strands as input, should return a list of tuples, where each tuple represents a violation of a strand that depends only on that strand. This is required because nuad does an optimization in which constraints are only evaluated if they depend on parts of the design that contain the domain(s) that changed in the current iteration.
 
 For example, suppose there are 100 strands, but only 3 strands contain the domain `x`, and `x` is the domain whose DNA sequence is changed in the current search iteration. Then each `StrandConstraint` `s` will be evaluated only on those 3 strands, on the assumption that the other 97 strands would have the same output of the function `s.evaluate` as before.
```

### Comparing `nuad-0.4.1/README.md` & `nuad-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 - `Domain`: A `Domain` represents a contiguous subsequence of DNA. A single `Domain` represents both the DNA sequence and its complement. For instance there is one `Domain` with name `a`, with two versions: unstarred (`a`) and starred (`a*`). If the DNA sequence of `a` is 5'-CCCAA-3', then the DNA sequence of `a*` is 3'-GGGTT-5'. 
 
 - `DomainPool`: Each `Domain` is assigned a single `DomainPool`, which can be thought of as a "source of DNA sequences" for the `Domain`. (See exceptions below.) The sequence design algorithm will take DNA sequences from this source when attempting to find DNA sequences to assign to `Domain`'s to satisfy all constraints. Each `DomainPool` has a fixed length. Since each `Domain` only has one `DomainPool`, this means that each `Domain` has a fixed length as well. If no other constraints are specified, then the `DomainPool` simply provides all DNA sequences of that length. Though you will generally not call this method yourself, the method `DomainPool.generate_sequence()` returns a sequence from the pool. This method can be called infinitely many times (i.e., sequences can repeat, though the exact period after which they repeat is an unspecified implementation detail.)
 
   - There are two types of `Domain`'s with no associated `DomainPool`. One type is a `Domain` with the field `fixed` set to `True` by calling the method `Domain.set_fixed_sequence()`, which has some fixed DNA sequence that cannot be changed. A fixed `Domain` has no `DomainPool`.)
 
-  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.dependent and https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.subdomains.
+  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://nuad.readthedocs.io/en/latest/#constraints.Domain.dependent and https://nuad.readthedocs.io/en/latest/#constraints.Domain.subdomains.
 
 - `Strand`: A `Strand` contains an ordered list `domains` of `Domain`'s, together with an identification of which `Domain`'s are starred in this `Strand`, the latter specified as a set `starred_domain_indices` of indices (starting at 0) into the list `domains`. For example, the `Strand` consisting of `Domain`'s `a`, `b*`, `c`, `b`, `d*`, in that order, would have `domains = [a, b, c, b, d]` and `starred_domain_indices = {1, 4}`.
 
 - `Design`: This describes the whole system. Generally you will have one `Design`, which is composed of a list of `Strand`'s.
 
 - `Constraint`: There are several kinds of constraint objects. Not all of them are related in the type hierarchy. 
 
@@ -142,15 +142,15 @@
 
     - **"soft" constraints:**  All other constraints are subclasses of the abstract superclass `Constraint`. These constrains are "softer": sequences violating the constraints are allowed to be assigned to `Domain`'s. The sequence design algorithm steadily improves the design by changing sequences until all of these constraints are satisfied. The different subtypes of the base class `Constraint` correspond to different parts of the `Design` that are being evaluated by the `Constraint`. The types are:
 
         - `SingularConstraint`: This is an abstract superclass of the following concrete subclasses. The difference with the other abstract superclass `BulkConstraint` is explained in `BulkConstraint` below.
         
             - `DomainConstraint`: This only looks at a single `Domain`. In practice this is not used much, since there's not much information in a `Domain` other than its DNA sequence, so a `SequenceConstraint` or `NumpyConstraint` typically would already have filtered out any DNA sequence not satisfying such a constraint.
 
-            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://dnadsd.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
+            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://nuad.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
 
             - `DomainPairConstraint`: This evaluates a pair of `Domain`'s.
 
             - `StrandPairConstraint`: This evaluates a pair of `Strand`'s.
 
             - `ComplexConstraint`: This evaluates a tuple of `Strand`'s of arbitrary size.
 
@@ -166,15 +166,15 @@
 
     The `BulkConstraint` subclasses `DomainsConstraint`, `StrandsConstraint`, `DomainPairsConstraint`, `StrandPairsConstraint` use a different function, called `evaluate_bulk`, which take as input a list of "`Design` parts" (e.g., a list of pairs of `Strand`'s for a `StrandPairsConstraint`). The return value is of type `List[Tuple[DesignPart, float, str]]`, i.e., a list of triples, where each triple is `(part, excess, summary)`.
     
     `part` is the individual part of the design that caused a problem. Generally it will be one of the elements of the list passed to `evaluate_bulk`, though the returned list could be smaller than the input list. This is because some parts may satisfy the constraint, and generally the only parts returned from `evaluate_bulk` are those that violated the constraint. `excess` and `summary` have the same interpretation as with the "singular" constraints.
 
     The search algorithm evaluates the constraints, and for each violated constraint, it turns the `excess` value into a "score" by first passing it through the "score transfer function", which by default squares the value, and then multiplies by the value `Constraint.weight` (by default 1). The goal of the search is to minimize the sum of scores across all violated `Constraint`'s. The reason that the score is squared is that this leads the search algorithm to (slightly) favor reducing the excess of constraint violations that are "more in excess", i.e., it would reduce the total score more to reduce an excess from 4 to 3 (reducing the score from 4<sup>2</sup>=16 to 3<sup>2</sup>=9, a reduction of 16-9=7) than to reduce an excess from 2 to 1 (which reduces 2<sup>2</sup>=4 to 1<sup>2</sup>=1, a reduction of only 4-1=3).
 
-    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_dna_sequences](https://dnadsd.readthedocs.io/en/latest/#search.search_for_dna_sequences).
+    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_sequences](https://nuad.readthedocs.io/en/latest/#search.search_for_sequences).
 
 
 ## Constraint evaluations must be pure functions of their inputs
 
 For all constraints, it is critical that the `evaluate` or `evaluate_bulk` functions be *pure* functions of their inputs: the return value should depend only on the parameters passed to the function. For example, a `StrandPairConstraint` takes two strands as input, and its `(excess, summary)` return values should depend *only* on those two strands. Similarly, a `StrandsConstraint`, whose `evaluate_bulk` function takes a list of strands as input, should return a list of tuples, where each tuple represents a violation of a strand that depends only on that strand. This is required because nuad does an optimization in which constraints are only evaluated if they depend on parts of the design that contain the domain(s) that changed in the current iteration.
 
 For example, suppose there are 100 strands, but only 3 strands contain the domain `x`, and `x` is the domain whose DNA sequence is changed in the current search iteration. Then each `StrandConstraint` `s` will be evaluated only on those 3 strands, on the assumption that the other 97 strands would have the same output of the function `s.evaluate` as before.
```

### Comparing `nuad-0.4.1/nuad/constraints.py` & `nuad-0.4.2/nuad/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import dataclasses
 import enum
 import os
 import math
 import json
 from decimal import Decimal
 from typing import List, Set, Dict, Callable, Iterable, Tuple, Collection, TypeVar, Any, \
-    cast, Generic, DefaultDict, FrozenSet, Iterator, Sequence, Type
+    cast, Generic, DefaultDict, FrozenSet, Iterator, Sequence, Type, Optional
 from dataclasses import dataclass, field, InitVar
 from abc import ABC, abstractmethod
 from collections import defaultdict
 import itertools
 import logging
 from multiprocessing.pool import ThreadPool
 from numbers import Number
@@ -136,33 +136,44 @@
 
     p8064 = "p8064"
     """Variant of M13mp18 that is 8064 bases long. Available from, for example
 
     https://www.tilibit.com/collections/scaffold-dna/products/single-stranded-scaffold-dna-type-p8064
     """
 
+    p8634 = "p8634"
+    """Variant of M13mp18 that is 8634 bases long. At the time of this writing, not listed as available
+    from any biotech vender, but Tilibit will make it for you if you ask. 
+    (https://www.tilibit.com/pages/contact-us)
+    """
+
+
     def length(self) -> int:
         """
         :return: length of this variant of M13 (e.g., 7249 for variant :data:`M13Variant.p7249`)
         """
         if self is M13Variant.p7249:
             return 7249
         if self is M13Variant.p7560:
             return 7560
         if self is M13Variant.p8064:
             return 8064
+        if self is M13Variant.p8634:
+            return 8634
         raise AssertionError('should be unreachable')
 
     def scadnano_variant(self) -> sc.M13Variant:
         if self is M13Variant.p7249:
             return sc.M13Variant.p7249
         if self is M13Variant.p7560:
             return sc.M13Variant.p7560
         if self is M13Variant.p8064:
             return sc.M13Variant.p8064
+        if self is M13Variant.p8634:
+            return sc.M13Variant.p8634
         raise AssertionError('should be unreachable')
 
 
 def m13(rotation: int = 5587, variant: M13Variant = M13Variant.p7249) -> str:
     """
     The M13mp18 DNA sequence (commonly called simply M13).
 
@@ -269,20 +280,20 @@
         substrings.append(substring)
 
     return substrings
 
 
 def default_score_transfer_function(x: float) -> float:
     """
-    A quadratic transfer function.
+    A cubic transfer function.
     
     :return:
-        max(0.0, x^2)
+        max(0.0, x^3)
     """
-    return max(0.0, x ** 2)
+    return max(0.0, x ** 3)
 
 
 logger = logging.Logger('dsd', level=logging.DEBUG)
 """
 Global logger instance used throughout dsd.
 
 Call ``logger.removeHandler(logger.handlers[0])`` to stop screen output (assuming that you haven't added
@@ -374,15 +385,15 @@
 @dataclass  # type: ignore
 class NumpyFilter(ABC):
     """
     Abstract base class for numpy filters. A "filter" is a hard constraint applied to sequences
     for a :any:`Domain`; a sequence not passing the filter is never allowed to be assigned to
     a :any:`Domain`. This constrasts with the various subclasses of :any:`Constraint`, which
     are different in two ways: 1) they can apply to large parts of the design than just a domain,
-    e.g., a :any:`Strand` or a pair of :any:`Domain`'s, and 2) they are "soft" constraint that are
+    e.g., a :any:`Strand` or a pair of :any:`Domain`'s, and 2) they are "soft" constraints that are
     allowed to be violated during the course of the search.
 
     A :any:`NumpyFilter` is one that can be efficiently encoded
     as numpy operations on 2D arrays of bytes representing DNA sequences, through the class
     :any:`np.DNASeqList` (which uses such a 2D array as the field :py:data:`np.DNASeqList.seqarr`).
 
     Subclasses should set the value :data:`NumpyFilter.name`, inherited from this class.
@@ -570,24 +581,24 @@
         all_bits = [nn.base2bits[base] for base in self.bases]
 
         if seqs.seqlen <= self.distance_from_end:
             raise ValueError(f'cannot specify distance from end of {self.distance_from_end} '
                              f'when sequences only have length {seqs.seqlen}')
 
         if self.five_prime:
-            good_left = np.zeros(shape=len(seqs), dtype=np.bool)
+            good_left = np.zeros(shape=len(seqs), dtype=bool)
             left = seqs.seqarr[:, self.distance_from_end]
             for bits in all_bits:
                 if good_left is None:
                     good_left = (left == bits)
                 else:
                     good_left |= (left == bits)
 
         if self.three_prime:
-            good_right = np.zeros(shape=len(seqs), dtype=np.bool)
+            good_right = np.zeros(shape=len(seqs), dtype=bool)
             right = seqs.seqarr[:, -1 - self.distance_from_end]
             for bits in all_bits:
                 if good_right is None:
                     good_right = (right == bits)
                 else:
                     good_right |= (right == bits)
 
@@ -635,15 +646,15 @@
 
     def remove_violating_sequences(self, seqs: nn.DNASeqList) -> nn.DNASeqList:
         """Remove sequences that don't have one of the given bases at the given position."""
         assert isinstance(self.bases, list)
         if not 0 <= self.position < seqs.seqlen:
             raise ValueError(f'position must be between 0 and {seqs.seqlen} but it is {self.position}')
         mid = seqs.seqarr[:, self.position]
-        good = np.zeros(shape=len(seqs), dtype=np.bool)
+        good = np.zeros(shape=len(seqs), dtype=bool)
         for base in self.bases:
             good |= (mid == nn.base2bits[base])
         seqarr_pass = seqs.seqarr[good]
         return nn.DNASeqList(seqarr=seqarr_pass)
 
 
 @dataclass
@@ -704,15 +715,15 @@
         assert isinstance(self.substrings, list)
         sub_len = len(self.substrings[0])
         sub_ints = [[nn.base2bits[base] for base in sub] for sub in self.substrings]
         pow_arr = [4 ** k for k in range(sub_len)]
         sub_vals = np.dot(sub_ints, pow_arr)
         toeplitz = nn.create_toeplitz(seqs.seqlen, sub_len, self.indices)
         convolution = np.dot(toeplitz, seqs.seqarr.transpose())
-        pass_all = np.ones(seqs.numseqs, dtype=np.bool)
+        pass_all = np.ones(seqs.numseqs, dtype=bool)
         for sub_val in sub_vals:
             pass_sub = np.all(convolution != sub_val, axis=0)
             pass_all = pass_all & pass_sub
         seqarr_pass = seqs.seqarr[pass_all]
         return nn.DNASeqList(seqarr=seqarr_pass)
 
 
@@ -4288,19 +4299,16 @@
     is satisfied, and setting it to a positive value means the constraint is violated. The interpretation
     is that the larger `excess` is, the more the constraint is violated.
     
     For example, a common value for excess is the amount by which the NUPACK complex free energy exceeds
     a threshold.
     """
 
-    summary: str = ''
-    """
-    This string is displayed in the text report on constraints, after the name of the "part" (e.g.,
-    strand, pair of domains, pair of strands).
-    """
+    _summary: Optional[str] = None
+
 
     value: pint.Quantity[Decimal] | None = None
     """
     If this is a "numeric" constraint, i.e., checking some number such as the complex free energy of a 
     strand and comparing it to a threshold, this is the "raw" value. It is optional, but if specified,
     then the raw values can be plotted in a Jupyter notebook by the function :meth:`display_report`.
     
@@ -4324,23 +4332,41 @@
                  excess: float,
                  summary: str | None = None,
                  value: float | str | pint.Quantity[Decimal] | None = None) -> None:
         self.excess = excess
         if summary is None:
             if value is None:
                 raise ValueError('at least one of value or summary must be specified')
-            self.summary = str(value)
+            # note summary getter calculates summary from value if summary is None,
+            # so no need to set it here
         else:
-            self.summary = summary
+            self._summary = summary
         if value is not None:
             self.value = parse_and_normalize_quantity(value)
 
         self.score = 0.0
         self.part = None  # type:ignore
 
+    @property
+    def summary(self) -> str:
+        """
+        This string is displayed in the text report on constraints, after the name of the "part" (e.g.,
+        strand, pair of domains, pair of strands).
+
+        It can be set explicitly, or calculated from :data:`Result.value` if not set explicitly.
+        """
+        if self._summary is None:
+            return str(self.value)
+        else:
+            return self._summary
+
+    @summary.setter
+    def summary(self, summary: str) -> None:
+        self._summary = summary
+
 
 def parse_and_normalize_quantity(quantity: float | int | str | pint.Quantity) \
         -> pint.Quantity[Decimal]:
     if isinstance(quantity, (str, float, int)):
         quantity = ureg.Quantity(quantity)
     quantity = normalize_quantity(quantity)
     return quantity
@@ -4349,17 +4375,18 @@
 def Q_(qty: int | str | Decimal | float, unit: str | pint.Unit) -> pint.Quantity[Decimal]:  # noqa
     # Convenient constructor for units, eg, :code:`Q_(5.0, 'nM')`.
     # Ensures that the quantity is a Decimal.
     if isinstance(qty, Decimal):
         return ureg.Quantity(qty, unit)
     else:
         # we convert to string to avoid floating-point weirdness. For example
-        # ureg.Quantity(Decimal(-2.1), 'kcal/mol') gives
+        #   ureg.Quantity(Decimal(-2.1), 'kcal/mol') gives
         #   -2.100000000000000088817841970012523233890533447265625 kilocalorie / mole,
-        # but ureg.Quantity(Decimal(str(-2.1)), 'kcal/mol') gives
+        # whereas
+        #   ureg.Quantity(Decimal(str(-2.1)), 'kcal/mol') gives
         #   -2.1 kilocalorie / mole,
         qty_str = str(qty)
         return ureg.Quantity(Decimal(qty_str), unit)
 
 
 def normalize_quantity(quantity: pint.Quantity, compact: bool = False) -> pint.Quantity[Decimal]:
     """
@@ -4392,15 +4419,15 @@
         quantity = Q_(mag_norm, quantity.units)
     return quantity
 
 
 @dataclass(eq=False)
 class SingularConstraint(Constraint[DesignPart], Generic[DesignPart], ABC):
     evaluate: Callable[[Tuple[str, ...], DesignPart | None],
-                       Result[DesignPart]] = lambda _: _raise_unreachable()
+    Result[DesignPart]] = lambda _: _raise_unreachable()
     """
     Essentially a wrapper for a function that evaluates the :any:`Constraint`. 
     It takes as input a tuple of DNA sequences 
     (Python strings) and an optional :any:`Part`, where :any:`Part` is one of 
     :any:`Domain`, :any:`Strand`, :any:`DomainPair`, :any:`StrandPair`, or :any:`Complex`
     (the latter being an alias for arbitrary-length tuple of :any:`Strand`'s).
 
@@ -4459,15 +4486,15 @@
         result.part = part
         return result
 
 
 @dataclass(eq=False)
 class BulkConstraint(Constraint[DesignPart], Generic[DesignPart], ABC):
     evaluate_bulk: Callable[[Sequence[DesignPart]],
-                            List[Result]] = lambda _: _raise_unreachable()
+    List[Result]] = lambda _: _raise_unreachable()
 
     def call_evaluate_bulk(self, parts: Sequence[DesignPart]) -> List[Result]:
         results: List[Result[DesignPart]] = (self.evaluate_bulk)(parts)  # noqa
         # apply weight and transfer scores
         for result, part in zip(results, parts):
             if result.excess < 0.0:
                 result.excess = 0.0
@@ -4689,15 +4716,15 @@
 
     Unlike other constraints, which specify either :data:`Constraint._evaluate` or
     :data:`Constraint._evaluate_bulk`, a :any:`DesignConstraint` leaves both of these unspecified and
     specifies :data:`DesignConstraint._evaluate_design` instead.
     """
 
     evaluate_design: Callable[[Design, Iterable[Domain]],
-                              List[Tuple[DesignPart, float, str]]] = lambda _: _raise_unreachable()
+    List[Tuple[DesignPart, float, str]]] = lambda _: _raise_unreachable()
     """
     Evaluates the :any:`Design` (first argument), possibly taking into account which :any:`Domain`'s have
     changed in the last iteration (second argument).
     
     Returns a list of tuples (`part`, `score`, `summary`), 
     one tuple per violation of the :any:`DesignConstraint`.
     
@@ -5702,14 +5729,412 @@
         parallel=parallel,
         strands=strands,
         pairs=pairs,
         ignore_missing_thresholds=ignore_missing_thresholds,
     )
 
 
+def longest_complementary_subsequences_python_loop(arr1: np.ndarray, arr2: np.ndarray,
+                                                   gc_double: bool) -> List[int]:
+    """
+    Like :func:`longest_complementary_subsequences`, but uses a Python loop instead of numpy operations.
+    This is slower, but is easier to understand and useful for testing.
+    """
+    lcs_sizes = []
+    for s1, s2 in zip(arr1, arr2):
+        s1len = s1.shape[0]
+        s2len = s2.shape[0]
+        table = np.zeros(shape=(s1len + 1, s2len + 1), dtype=np.int8)
+        for i in range(s1len):
+            for j in range(s2len):
+                b1 = s1[i]
+                b2 = s2[j]
+                if b1 + b2 == 3:
+                    weight = 1
+                    if gc_double and (b1 == 1 or b1 == 2):
+                        weight = 2
+                    table[i + 1][j + 1] = weight + table[i][j]
+                else:
+                    table[i + 1][j + 1] = max(table[i + 1][j], table[i][j + 1])
+        lcs_size = table[s1len][s2len]
+        lcs_sizes.append(lcs_size)
+    return lcs_sizes
+
+
+def longest_complementary_subsequences_two_loops(arr1: np.ndarray, arr2: np.ndarray,
+                                                 gc_double: bool) -> List[int]:
+    """
+    Calculate length of longest common subsequences between `arr1[i]` and `arr2[i]`
+    for each i, storing in returned list `result[i]`.
+
+    This uses two nested Python loops to calculate the whole dynamic programming table.
+    :func:`longest_complementary_subsequences` is slightly faster because it maintains only the diagonal
+    of the DP table, and uses numpy vectorized operations to calculate the next diagonal of the table.
+
+    When used for DNA sequences, this assumes `arr2` has been reversed along axis 1, i.e.,
+    the sequences in `arr1` are assumed to be oriented 5' --> 3', and the sequences in `arr2`
+    are assumed to be oriented 3' --> 5'.
+
+    Args:
+        arr1: 2D array of DNA sequences, with each sequence represented as a 1D array of 0, 1, 2, 3
+              corresponding to A, C, G, T, respectively, with each row being a single DNA sequence
+              oriented 5' --> 3'.
+        arr2: 2D array of DNA sequences, with each row being a single DNA sequence
+              oriented 3' --> 5'.
+        gc_double: Whether to double the score for G-C base pairs.
+
+    Returns:
+        list `ret` of ints, where `ret[i]` is the length of the longest complementary subsequence
+        between `arr1[i]` and `arr2[i]`.
+    """
+    assert arr1.shape[0] == arr2.shape[0]
+    num_pairs = arr1.shape[0]
+    s1len = arr1.shape[1]
+    s2len = arr2.shape[1]
+    max_length = max(s1len, s2len)
+    dtype = np.min_scalar_type(max_length)  # e.g., uint8 for 0-255, uint16 for 256-65535, etc.
+    table = np.zeros(shape=(num_pairs, s1len + 1, s2len + 1), dtype=dtype)
+
+    # convert arr2 to complement and search for longest common subsequence (instead of complementary)
+    arr2 = 3 - arr2
+
+    for i in range(s1len):
+        for j in range(s2len):
+            bases1 = arr1[:, i]
+            bases2 = arr2[:, j]
+
+            equal_idxs = bases1 == bases2
+            if gc_double:
+                gc_idxs = np.logical_or(bases1[equal_idxs] == 1, bases1[equal_idxs] == 2)
+                weight = np.ones(len(bases1[equal_idxs]), dtype=dtype)
+                weight[gc_idxs] = 2
+                table[equal_idxs, i + 1, j + 1] = weight + table[equal_idxs, i, j]
+            else:
+                table[equal_idxs, i + 1, j + 1] = 1 + table[equal_idxs, i, j]
+
+            noncomp_idxs = np.logical_not(equal_idxs)
+            rec1 = table[noncomp_idxs, i + 1, j]
+            rec2 = table[noncomp_idxs, i, j + 1]
+            table[noncomp_idxs, i + 1, j + 1] = np.maximum(rec1, rec2)
+
+    lcs_sizes = table[:, s1len, s2len]
+
+    return lcs_sizes
+
+
+def longest_complementary_subsequences(arr1: np.ndarray, arr2: np.ndarray, gc_double: bool) -> List[int]:
+    """
+    Calculate length of longest common subsequences between `arr1[i]` and `arr2[i]`
+    for each i, storing in returned list `result[i]`.
+
+    Unlike :func:`longest_complementary_subsequences_two_loops`, this uses only one Python loop,
+
+    When used for DNA sequences, this assumes `arr2` has been reversed along axis 1, i.e.,
+    the sequences in `arr1` are assumed to be oriented 5' --> 3', and the sequences in `arr2`
+    are assumed to be oriented 3' --> 5'.
+
+    Args:
+        arr1: 2D array of DNA sequences, with each sequence represented as a 1D array of 0, 1, 2, 3
+              corresponding to A, C, G, T, respectively, with each row being a single DNA sequence
+              oriented 5' --> 3'.
+        arr2: 2D array of DNA sequences, with each row being a single DNA sequence
+              oriented 3' --> 5'.
+        gc_double: Whether to double the score for G-C base pairs.
+
+    Returns:
+        list `ret` of ints, where `ret[i]` is the length of the longest complementary subsequence
+        between `arr1[i]` and `arr2[i]`.
+    """
+    assert arr1.shape[0] == arr2.shape[0]
+    num_pairs = arr1.shape[0]
+    s1len = arr1.shape[1]
+    s2len = arr2.shape[1]
+    assert s1len == s2len  # for now, assume same length, but should be relaxed
+
+    max_length = max(s1len, s2len)
+    dtype = np.min_scalar_type(max_length)  # e.g., uint8 for 0-255, uint16 for 256-65535, etc.
+
+    # convert arr2 to WC complement and search for longest common subsequence (instead of complementary)
+    arr2 = 3 - arr2
+
+    length_prev_prev = length_prev = s1len
+    prev_prev_larger = s1len % 2 == 0
+    if prev_prev_larger:
+        length_prev_prev += 1
+    else:
+        length_prev += 1
+
+    # using this spreadsheet to visual DP table:
+    # https://docs.google.com/spreadsheets/d/1FIOgQYFSJ_6r3ThBivDjf0epUxVLgk0xlQnQS6TUeSw/
+    diag_prev_prev = np.zeros(shape=(num_pairs, length_prev_prev), dtype=dtype)
+    diag_prev = np.zeros(shape=(num_pairs, length_prev), dtype=dtype)
+
+    # do dynamic programming to figure out longest complementary subsequence,
+    # maintaining only the diagonal of the table and the previous two diagonals
+
+    # allocate these arrays just once to avoid re-allocating new memory each iteration
+    # they are used for telling which bases are equal between the two sequences
+    eq_idxs_larger = np.zeros((num_pairs, s1len + 1), dtype=bool)
+    eq_idxs_smaller = np.zeros((num_pairs, s1len), dtype=bool)
+    gc_idxs_larger = np.zeros((num_pairs, s1len + 1), dtype=bool)
+    gc_idxs_smaller = np.zeros((num_pairs, s1len), dtype=bool)
+    for i in range(0, 2 * s1len, 2):
+        diag_cur = update_diagonal(arr1, arr2, diag_prev, diag_prev_prev,
+                                   eq_idxs_larger if prev_prev_larger else eq_idxs_smaller,
+                                   gc_idxs_larger if prev_prev_larger else gc_idxs_smaller,
+                                   i, prev_prev_larger, gc_double)
+        if i < 2 * s1len - 2:
+            diag_next = update_diagonal(arr1, arr2, diag_cur, diag_prev,
+                                        eq_idxs_larger if not prev_prev_larger else eq_idxs_smaller,
+                                        gc_idxs_larger if not prev_prev_larger else gc_idxs_smaller,
+                                        i + 1, not prev_prev_larger, gc_double)
+            diag_prev = diag_next
+        diag_prev_prev = diag_cur
+
+    middle_idx = s1len // 2
+    lcs_sizes = diag_prev_prev[:, middle_idx]
+
+    return lcs_sizes
+
+
+def update_diagonal(arr1: np.ndarray, arr2: np.ndarray,
+                    diag_prev: np.ndarray, diag_prev_prev: np.ndarray,
+                    eq_idxs: np.ndarray,
+                    gc_idxs: np.ndarray,
+                    i: int, prev_prev_larger: bool, gc_double: bool) -> np.ndarray:
+    s1len = arr1.shape[1]
+    s2len = arr2.shape[1]
+    assert s1len == s2len  # for now, assume same length, but should be relaxed
+
+    # determine which bases in arr1 and arr2 are equal;
+    # compute LCS for that case and store in diag_eq
+    # creates view, not copy, so don't modify!
+    eq_idxs[:, :] = False
+    if i < s1len:
+        sub1 = arr1[:, i::-1]  # indices i, i-1, ..., 0
+        sub2 = arr2[:, :i + 1]  # indices 0, 1,   ..., i
+    else:
+        sub1 = arr1[:, :i - s1len:-1]  # indices s1len-1,   s1len-2, , ..., s1len-i
+        sub2 = arr2[:, i - s1len + 1:]  # indices s1len-i+1, s1len-i+2, ..., s1len-1
+
+    # need to set eq_idxs only on entries "within" the DP table, not the padded 0s on the edges
+    # see https://docs.google.com/spreadsheets/d/1FIOgQYFSJ_6r3ThBivDjf0epUxVLgk0xlQnQS6TUeSw for example
+
+    if i < s1len:
+        start = (s1len - i) // 2
+    else:
+        start = (i - s1len) // 2 + 1
+    end = s1len - start
+    if not prev_prev_larger:
+        end -= 1
+    # TODO: if there's a way to avoid allocating new memory for the Boolean array eq, that will save time.
+    #  With 10,000 pairs of sequences, each of length 64, this takes 1/4 the time if we just set
+    #  eq_idxs[:, start:end + 1] = True, compared to computing sub1==sub2 allocating new memory for eq
+    #  (not sure if the computation or the memory allocation dominates, however)
+    eq = sub1 == sub2
+    eq_idxs[:, start:end + 1] = eq
+
+    # don't want to allocate new memory, but give variable a better name
+    # to reflect that we are looking at the case where the bases are equal
+    # XXX: note that this is modifying diag_prev_prev,
+    # so only safe to do this after we aren't using it anymore
+    diag_cur = diag_prev_prev
+    diag_cur[eq_idxs] += 1
+    if gc_double:
+        gc_idxs[:, start:end + 1] = np.logical_and(np.logical_or(sub1 == 1, sub1 == 2), eq)
+        diag_cur[gc_idxs] += 1
+
+    # now take maximum with immediately previous diagonal
+    if prev_prev_larger:
+        # diag_cur is 1 larger than diag_prev
+        diag_cur_L = diag_cur[:, :-1]
+        diag_cur_R = diag_cur[:, 1:]
+        np.maximum(diag_cur_L, diag_prev, out=diag_cur_L)  # looks "above" in DP table
+        np.maximum(diag_cur_R, diag_prev, out=diag_cur_R)  # looks "left" in DP table
+    else:
+        # diag_cur is 1 smaller than diag_prev
+        diag_prev_L = diag_prev[:, :-1]
+        diag_prev_R = diag_prev[:, 1:]
+        np.maximum(diag_cur, diag_prev_L, out=diag_cur)  # looks "above" in DP table
+        np.maximum(diag_cur, diag_prev_R, out=diag_cur)  # looks "left" in DP table
+
+    return diag_cur
+
+
+def lcs(seqs1: Sequence[str], seqs2: Sequence[str], gc_double: bool) -> List[int]:
+    arr1 = nn.seqs2arr(seqs1)
+    arr2 = nn.seqs2arr(seqs2)
+    arr2 = np.flip(arr2, axis=1)
+    return longest_complementary_subsequences(arr1, arr2, gc_double)
+
+
+def lcs_loop(s1: str, s2: str, gc_double: bool) -> int:
+    arr1 = nn.seqs2arr([s1])
+    arr2 = nn.seqs2arr([s2[::-1]])
+    return longest_complementary_subsequences_python_loop(arr1, arr2, gc_double)[0]
+
+
+def lcs_strand_pairs_constraint(
+        *,
+        threshold: int,
+        weight: float = 1.0,
+        score_transfer_function: Callable[[float], float] = default_score_transfer_function,
+        description: str | None = None,
+        short_description: str = 'lcs strand pairs',
+        pairs: Iterable[Tuple[Strand, Strand]] | None = None,
+        check_strand_against_itself: bool = True,
+        gc_double: bool = True,
+) -> StrandPairsConstraint:
+    """
+    TODO: describe
+
+    Args
+        threshold:
+
+        weight:
+
+        score_transfer_function:
+
+        description:
+
+        short_description:
+
+        pairs:
+
+        gc_double: Whether to weigh G-C base pairs as double (i.e., they count for 2 instead of 1).
+
+    Returns
+        A :any: StrandPairsConstraint` that checks given pairs of :any:`Strand`'s for excessive
+        interaction due to having long complementary subsequences.
+    """
+    if description is None:
+        description = f'Longest complementary subsequence between strands is > {threshold}'
+
+    def evaluate_bulk(strand_pairs: Iterable[StrandPair]) -> List[Result]:
+        # import time
+        # start_eb = time.time()
+
+        seqs1 = [pair.strand1.sequence() for pair in strand_pairs]
+        seqs2 = [pair.strand2.sequence() for pair in strand_pairs]
+        arr1 = nn.seqs2arr(seqs1)
+        arr2 = nn.seqs2arr(seqs2)
+        arr2_rev = np.flip(arr2, axis=1)
+
+        # start = time.time()
+        lcs_sizes = longest_complementary_subsequences(arr1, arr2_rev, gc_double)
+        # lcs_sizes = longest_complementary_subsequences_two_loops(arr1, arr2_rev, gc_double)
+        # end = time.time()
+
+        results = []
+        for lcs_size in lcs_sizes:
+            excess = lcs_size - threshold
+            value = f'{lcs_size}'
+            result = Result(excess=excess, value=value)
+            results.append(result)
+
+        # end_eb = time.time()
+        # elapsed_ms = int(round((end - start) * 1000, 0))
+        # elapsed_eb_ms = int(round((end_eb - start_eb) * 1000, 0))
+        # print(f'\n{elapsed_ms} ms to measure LCS of {len(seqs1)} pairs')
+        # print(f'{elapsed_eb_ms} ms to run evaluate_bulk')
+
+        return results
+
+    pairs_tuple = None
+    if pairs is not None:
+        pairs_tuple = tuple(pairs)
+
+    return StrandPairsConstraint(
+        description=description,
+        short_description=short_description,
+        weight=weight,
+        score_transfer_function=score_transfer_function,
+        evaluate_bulk=evaluate_bulk,
+        pairs=pairs_tuple,
+        check_strand_against_itself=check_strand_against_itself,
+    )
+
+
+def lcs_strand_pairs_constraints_by_number_matching_domains(
+        *,
+        thresholds: Dict[int, int],
+        weight: float = 1.0,
+        score_transfer_function: Callable[[float], float] = default_score_transfer_function,
+        descriptions: Dict[int, str] | None = None,
+        short_descriptions: Dict[int, str] | None = None,
+        parallel: bool = False,
+        strands: Iterable[Strand] | None = None,
+        pairs: Iterable[Tuple[Strand, Strand]] | None = None,
+        gc_double: bool = True,
+        parameters_filename: str = '',
+        ignore_missing_thresholds: bool = False,
+) -> List[StrandPairsConstraint]:
+    """
+    TODO
+    """
+    if parameters_filename != '':
+        raise ValueError('should not specify parameters_filename when calling '
+                         'lcs_strand_pairs_constraints_by_number_matching_domains; '
+                         'it is only listed as a parameter for technical reasons relating to code resuse '
+                         'with other constraints that use that parameter')
+
+    def lcs_strand_pairs_constraint_with_dummy_parameters(
+            *,
+            threshold: float,
+            temperature: float = nv.default_temperature,
+            weight: float = 1.0,
+            score_transfer_function: Callable[[float], float] = default_score_transfer_function,
+            description: str | None = None,
+            short_description: str = 'lcs strand pairs',
+            parallel: bool = False,
+            pairs: Iterable[Tuple[Strand, Strand]] | None = None,
+            parameters_filename: str = nv.default_vienna_rna_parameter_filename
+    ) -> StrandPairsConstraint:
+        threshold_int = int(threshold)
+        return lcs_strand_pairs_constraint(
+            threshold=threshold_int,
+            weight=weight,
+            score_transfer_function=score_transfer_function,
+            description=description,
+            short_description=short_description,
+            pairs=pairs,
+            check_strand_against_itself=True,
+            # TODO: rewrite signature of other strand pair constraints to include this
+            gc_double=gc_double,
+        )
+
+    if descriptions is None:
+        descriptions = {
+            num_matching: (f'Longest complementary subsequence between strands is > {threshold}' +
+                           f'\nfor strands with {num_matching} complementary '
+                           f'{"domain" if num_matching == 1 else "domains"}')
+            for num_matching, threshold in thresholds.items()
+        }
+
+    if short_descriptions is None:
+        short_descriptions = {
+            num_matching: f'LCS{num_matching}comp'
+            for num_matching, threshold in thresholds.items()
+        }
+
+    return _strand_pairs_constraints_by_number_matching_domains(
+        constraint_creator=lcs_strand_pairs_constraint_with_dummy_parameters,
+        thresholds=thresholds,
+        temperature=-1,
+        weight=weight,
+        score_transfer_function=score_transfer_function,
+        descriptions=descriptions,
+        short_descriptions=short_descriptions,
+        parallel=parallel,
+        strands=strands,
+        pairs=pairs,
+        ignore_missing_thresholds=ignore_missing_thresholds,
+    )
+
+
 def rna_duplex_strand_pairs_constraint(
         *,
         threshold: float,
         temperature: float = nv.default_temperature,
         weight: float = 1.0,
         score_transfer_function: Callable[[float], float] = default_score_transfer_function,
         description: str | None = None,
@@ -7511,15 +7936,15 @@
             raise ValueError(
                 f"Multiple instances of domain in a complex is not allowed "
                 f"when its complement is also in the complex. "
                 f"Violating domain: {domain_name_complement}")
     # End Input Validation #
 
     addr_to_starting_base_pair_idx: Dict[StrandDomainAddress,
-                                         int] = _get_addr_to_starting_base_pair_idx(strand_complex)
+    int] = _get_addr_to_starting_base_pair_idx(strand_complex)
     all_bound_domain_addresses.update(_get_implicitly_bound_domain_addresses(
         strand_complex, nonimplicit_base_pairs_domain_names))
 
     # Set of all bound domain endpoints to check.
     base_pair_domain_endpoints_to_check: Set[_BasePairDomainEndpoint] = set()
 
     for (domain_addr, comple_addr) in all_bound_domain_addresses.items():
```

### Comparing `nuad-0.4.1/nuad/json_noindent_serializer.py` & `nuad-0.4.2/nuad/json_noindent_serializer.py`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/nuad/modifications.py` & `nuad-0.4.2/nuad/modifications.py`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/nuad/np.py` & `nuad-0.4.2/nuad/np.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,85 @@
 def seq2arr(seq: str, base2bits_local: Dict[str, int] | None = None) -> np.ndarray:
     """Convert seq (string with DNA alphabet) to numpy array with integers 0,1,2,3."""
     if base2bits_local is None:
         base2bits_local = base2bits
     return np.array([base2bits_local[base] for base in seq], dtype=np.ubyte)
 
 
+# this was about 5 times slower than the new implementation of `seqs2arr` below
+# def seqs2arr_old(seqs: Sequence[str]) -> np.ndarray:
+#     """Return numpy 2D array converting the given DNA sequences to integers."""
+#     if len(seqs) == 0:
+#         return np.empty((0, 0), dtype=np.ubyte)
+#     if isinstance(seqs, str):
+#         raise ValueError('seqs must be a sequence of strings, not a single string')
+#     seq_len = len(seqs[0])
+#     for seq in seqs:
+#         if len(seq) != seq_len:
+#             raise ValueError('All sequences in seqs must be equal length')
+#     num_seqs = len(seqs)
+#     arr = np.empty((num_seqs, seq_len), dtype=np.ubyte)
+#     for i in range(num_seqs):
+#         arr[i] = [base2bits[base] for base in seqs[i]]
+#     return arr
+
+
 def seqs2arr(seqs: Sequence[str]) -> np.ndarray:
     """Return numpy 2D array converting the given DNA sequences to integers."""
     if len(seqs) == 0:
         return np.empty((0, 0), dtype=np.ubyte)
+    if isinstance(seqs, str):
+        raise ValueError('seqs must be a sequence of strings, not a single string')
+
+    # check equal length of each sequence (a bit faster than a Python loop,
+    # e.g., 3.5 ms for 10^5 seqs compared to 5 ms with Python loop)
     seq_len = len(seqs[0])
-    for seq in seqs:
-        if len(seq) != seq_len:
-            raise ValueError('All sequences in seqs must be equal length')
+    lengths_it = map(len, seqs)
+    lengths_arr = np.fromiter(lengths_it, dtype=int)
+    if np.any(lengths_arr != seq_len):
+        raise ValueError('All sequences in seqs must be equal length')
+
     num_seqs = len(seqs)
-    arr = np.empty((num_seqs, seq_len), dtype=np.ubyte)
-    for i in range(num_seqs):
-        arr[i] = [base2bits[base] for base in seqs[i]]
-    return arr
+
+    # the code below is about 5 times faster than the old implementation (commented out above)
+    seqs_cat = ''.join(seqs)
+    seqs_cat = seqs_cat.upper()
+
+    seqs_cat_bytes = seqs_cat.encode()
+    seqs_cat_byte_array = bytearray(seqs_cat_bytes)
+    arr1d = np.frombuffer(seqs_cat_byte_array, dtype=np.ubyte)
+    # arr1d = np.fromstring(seqs_cat_bytes, dtype=np.ubyte) # generates warning about using frombuffer
+
+    # convert ASCII bytes for 'A', 'C', 'G', 'T' to 0, 1, 2, 3, respectively
+
+    # code below is magical to me, but it works and is slightly faster than more obvious ways:
+    # https://stackoverflow.com/a/35464758
+    from_values = np.array([ord(base) for base in ['A', 'C', 'G', 'T']])
+    to_values = np.arange(4)
+    sort_idx = np.argsort(from_values)
+    idx = np.searchsorted(from_values, arr1d, sorter=sort_idx)
+    arr1d = to_values[sort_idx][idx]
+
+    # this is a bit slower than the code above, e.g., 75 ms compared to 55 ms for 10^5 sequences
+    # for i, base in enumerate(['A', 'C', 'G', 'T']):
+    #     idxs_with_base = arr2d == ord(base)
+    #     arr2d[idxs_with_base] = i
+
+    arr2d = arr1d.reshape((num_seqs, seq_len))
+
+    return arr2d
+
+
+def arr2seqs(arr: np.ndarray) -> List[str]:
+    """Return list of strings converting the given numpy array of integers to DNA sequences."""
+    return [''.join(bits2base[base] for base in row) for row in arr]
 
 
 def arr2seq(arr: np.ndarray) -> str:
+    """Return string converting the given numpy array of integers to DNA sequence."""
     bases_ch = [bits2base[base] for base in arr]
     return ''.join(bases_ch)
 
 
 def make_array_with_all_sequences(length: int, digits: Sequence[int]) -> np.ndarray:
     num_digits = len(digits)
     num_seqs = num_digits ** length
@@ -84,15 +139,15 @@
     Uses the encoding described in the documentation for DNASeqList. The result
     is a 2D array, where each row represents a DNA sequence, and that row
     has one byte per base."""
 
     if len(bases) == 0:
         raise ValueError('bases cannot be empty')
     if not set(bases) <= {'A', 'C', 'G', 'T'}:
-        raise ValueError(f"bases must be a subset of {'A', 'C', 'G', 'T'}; cannot be {bases}")
+        raise ValueError(f"bases must be a subset of {{A, C, G, T}}; cannot be {bases}")
 
     base_bits = [base2bits[base] for base in bases]
     digits = np.array(base_bits, dtype=np.ubyte)
 
     return make_array_with_all_sequences(length, digits)
     # num_bases = len(bases)
     # num_seqs = num_bases ** length
@@ -453,15 +508,15 @@
     numa2s = a2s.shape[0]
     len_a1 = len(a1)
     len_a2 = a2s.shape[1]
     counter = np.zeros(shape=(len_a1 + 1, numa2s, len_a2 + 1), dtype=np.int)
 
     for i1 in range(len(a1)):
         idx = (a2s == a1[i1])
-        idx_shifted = np.insert(idx, 0, np.zeros(numa2s, dtype=np.bool), axis=1)
+        idx_shifted = np.insert(idx, 0, np.zeros(numa2s, dtype=bool), axis=1)
         counter[i1 + 1, idx_shifted] = counter[i1, idx] + 1
 
     counter = np.swapaxes(counter, 0, 1)
 
     counter_flat = counter.reshape(numa2s, (len_a1 + 1) * (len_a2 + 1))
     idx_longest_raveled = np.argmax(counter_flat, axis=1)
     len_longest = counter_flat[np.arange(counter_flat.shape[0]), idx_longest_raveled]
@@ -514,15 +569,15 @@
     counter = np.zeros(shape=(len_a1 + 1, numpairs, len_a2 + 1), dtype=np.int)
 
     for i1 in range(len_a1):
         a1s_cp_col = a1s[:, i1].reshape(numpairs, 1)
         a1s_cp_col_rp = np.repeat(a1s_cp_col, len_a2, axis=1)
 
         idx = (a2s == a1s_cp_col_rp)
-        idx_shifted = np.hstack([np.zeros(shape=(numpairs, 1), dtype=np.bool), idx])
+        idx_shifted = np.hstack([np.zeros(shape=(numpairs, 1), dtype=bool), idx])
         counter[i1 + 1, idx_shifted] = counter[i1, idx] + 1
 
     counter = np.swapaxes(counter, 0, 1)
 
     counter_flat = counter.reshape(numpairs, (len_a1 + 1) * (len_a2 + 1))
     idx_longest_raveled = np.argmax(counter_flat, axis=1)
     len_longest = counter_flat[np.arange(counter_flat.shape[0]), idx_longest_raveled]
@@ -562,28 +617,28 @@
 
     for i1 in range(len_a1):
         a1s_col = a1s[:, i1].reshape(numpairs, 1)
         a1s_col_rp = np.repeat(a1s_col, len_a2, axis=1)
 
         # find matching chars and extend length of substring
         match_idxs = (a2s == a1s_col_rp)
-        match_shifted_idxs = np.hstack([np.zeros(shape=(numpairs, 1), dtype=np.bool), match_idxs])
+        match_shifted_idxs = np.hstack([np.zeros(shape=(numpairs, 1), dtype=bool), match_idxs])
         counter[i1 + 1, match_shifted_idxs] = counter[i1, match_idxs] + 1
 
         if i1 > 0:
             # calculate energy if matching substring has length > 1
             prev_bases = a1s[:, i1 - 1]
             cur_bases = a1s[:, i1]
             loops = (prev_bases << 2) + cur_bases
             latest_energies = loop_energies[loops].reshape(numpairs, 1)
             latest_energies_rp = np.repeat(latest_energies, len_a2, axis=1)
-            match_idxs_false_at_end = np.hstack([match_idxs, np.zeros(shape=(numpairs, 1), dtype=np.bool)])
+            match_idxs_false_at_end = np.hstack([match_idxs, np.zeros(shape=(numpairs, 1), dtype=bool)])
             both_match_idxs = match_idxs_false_at_end & prev_match_shifted_idxs
             prev_match_shifted_shifted_idxs = np.hstack(
-                [np.zeros(shape=(numpairs, 1), dtype=np.bool), prev_match_shifted_idxs])[:, :-1]
+                [np.zeros(shape=(numpairs, 1), dtype=bool), prev_match_shifted_idxs])[:, :-1]
             both_match_shifted_idxs = match_shifted_idxs & prev_match_shifted_shifted_idxs
             energies[i1 + 1, both_match_shifted_idxs] = energies[i1, both_match_idxs] + latest_energies_rp[
                 both_match_idxs]
 
         #         prev_match_idxs = match_idxs
         prev_match_shifted_idxs = match_shifted_idxs
 
@@ -672,15 +727,15 @@
 
     def __init__(self,
                  length: int | None = None,
                  num_random_seqs: int | None = None,
                  shuffle: bool = False,
                  alphabet: Collection[str] = ('A', 'C', 'G', 'T'),
                  seqs: Sequence[str] | None = None,
-                 seqarr: np.ndarray = None,
+                 seqarr: np.ndarray | None = None,
                  filename: str | None = None,
                  rng: np.random.Generator = default_rng,
                  hamming_distance_from_sequence: Tuple[int, str] | None = None):
         """
         Creates a set of DNA sequences, all of the same length.
 
         Create either all sequences of a given length if seqs is not specified,
@@ -1065,22 +1120,22 @@
         good = (mid == base2bits[base])
         seqarrpass = self.seqarr[good]
         return DNASeqList(seqarr=seqarrpass)
 
     def filter_substring(self, subs: Sequence[str]) -> DNASeqList:
         """Remove any sequence with any elements from subs as a substring."""
         if len(set([len(sub) for sub in subs])) != 1:
-            raise ValueError('All substrings in subs must be equal length: %s' % subs)
+            raise ValueError(f'All substrings in subs must be equal length: {subs}')
         sublen = len(subs[0])
         subints = [[base2bits[base] for base in sub] for sub in subs]
         powarr = [4 ** k for k in range(sublen)]
         subvals = np.dot(subints, powarr)
         toeplitz = create_toeplitz(self.seqlen, sublen)
         convolution = np.dot(toeplitz, self.seqarr.transpose())
-        passall = np.ones(self.numseqs, dtype=np.bool)
+        passall = np.ones(self.numseqs, dtype=bool)
         for subval in subvals:
             passsub = np.all(convolution != subval, axis=0)
             passall = passall & passsub
         seqarrpass = self.seqarr[passall]
         return DNASeqList(seqarr=seqarrpass)
 
     def filter_seqs_by_g_quad(self) -> DNASeqList:
@@ -1119,15 +1174,15 @@
             if idx < 0:
                 raise ValueError(f'index must be nonnegative, but {idx} is not; all indices = {indices}')
             if idx >= seqlen - (sublen - 1):
                 raise ValueError(f'index must be less than {seqlen - (sublen - 1)}, '
                                  f'but {idx} is not; all indices = {indices}')
     num_rows = len(rows)
     num_cols = seqlen
-    toeplitz = np.zeros((num_rows, num_cols), dtype=np.int)
+    toeplitz = np.zeros((num_rows, num_cols), dtype=int)
     toeplitz[:, 0:sublen] = [powarr] * num_rows
     shift = list(rows)
     for i in range(len(rows)):
         toeplitz[i] = np.roll(toeplitz[i], shift[i])
     return toeplitz
 
 
@@ -1205,104 +1260,25 @@
 
 def wcenergies_str(seqs: Sequence[str], temperature: float, negate: bool = False) -> List[float]:
     seqarr = seqs2arr(seqs)
     return list(calculate_wc_energies(seqarr, temperature, negate))
 
 
 def wcenergy_str(seq: str, temperature: float, negate: bool = False) -> float:
-    seqarr = seqs2arr([seq])
-    return list(calculate_wc_energies(seqarr, temperature, negate))[0]
-
-
-def hash_ndarray(arr: np.ndarray) -> int:
-    writeable = arr.flags.writeable
-    if writeable:
-        arr.flags.writeable = False
-    h = hash(bytes(arr.data))  # hash(arr.data)
-    arr.flags.writeable = writeable
-    return h
-
-
-CACHE_WC = False
-_calculate_wc_energies_cache: np.ndarray | None = None
-_calculate_wc_energies_cache_hash: int = 0
+    return wcenergies_str([seq], temperature, negate)[0]
 
 
 def calculate_wc_energies(seqarr: np.ndarray, temperature: float, negate: bool = False) -> np.ndarray:
     """Calculate and store in an array all energies of all sequences in seqarr
     with their Watson-Crick complements."""
-    global _calculate_wc_energies_cache
-    global _calculate_wc_energies_cache_hash
-    if CACHE_WC and _calculate_wc_energies_cache is not None:
-        if _calculate_wc_energies_cache_hash == hash_ndarray(seqarr):
-            return _calculate_wc_energies_cache
     loop_energies = calculate_loop_energies(temperature, negate)
     left_index_bits = seqarr[:, :-1] << 2
     right_index_bits = seqarr[:, 1:]
     pair_indices = left_index_bits + right_index_bits
     pair_energies = loop_energies[pair_indices]
     energies: np.ndarray = np.sum(pair_energies, axis=1)
-    if CACHE_WC:
-        _calculate_wc_energies_cache = energies
-        _calculate_wc_energies_cache_hash = hash_ndarray(_calculate_wc_energies_cache)
     return energies
 
 
 def wc_arr(seqarr: np.ndarray) -> np.ndarray:
-    """Return numpy array of complements of sequences in `seqarr`."""
+    """Return numpy array of reverse complements of sequences in `seqarr`."""
     return (3 - seqarr)[:, ::-1]
-
-
-def prefilter_length_10_11(low_dg: float, high_dg: float, temperature: float, end_gc: bool,
-                           convert_to_list: bool = True) \
-        -> Tuple[List[str], List[str]] | Tuple[DNASeqList, DNASeqList]:
-    """Return sequences of length 10 and 11 with wc energies between given values."""
-    s10: DNASeqList = DNASeqList(length=10)
-    s11: DNASeqList = DNASeqList(length=11)
-    s10 = s10.filter_energy(low=low_dg, high=high_dg, temperature=temperature)
-    s11 = s11.filter_energy(low=low_dg, high=high_dg, temperature=temperature)
-    forbidden_subs = [f'{a}{b}{c}{d}' for a in ['G', 'C']
-                      for b in ['G', 'C']
-                      for c in ['G', 'C']
-                      for d in ['G', 'C']]
-    s10 = s10.filter_substring(forbidden_subs)
-    s11 = s11.filter_substring(forbidden_subs)
-    if end_gc:
-        print(
-            'Removing any domains that end in either A or T; '
-            'also ensuring every domain has an A or T within 2 indexes of the end')
-        s10 = s10.filter_end_gc()
-        s11 = s11.filter_end_gc()
-    for seqs in (s10, s11):
-        if len(seqs) == 0:
-            raise ValueError(
-                f'low_dg {low_dg:.2f} and high_dg {high_dg:.2f} too strict! '
-                f'no sequences of length {seqs.seqlen} found')
-    return (s10.to_list(), s11.to_list()) if convert_to_list else (s10, s11)
-
-
-def all_cats(seq: Sequence[int], seqs: Sequence[int]) -> np.ndarray:
-    """
-    Return all sequences obtained by concatenating seq to either end of a sequence in seqs.
-
-    For example,
-
-    .. code-block:: Python
-
-        all_cats([0,1,2,3], [[3,3,3], [0,0,0]])
-
-    returns the numpy array
-
-    .. code-block:: Python
-
-        [[0,1,2,3,3,3,3],
-         [3,3,3,0,1,2,3],
-         [0,1,2,3,0,0,0],
-         [0,0,0,0,1,2,3]]
-    """
-    seqarr = np.asarray([seq])
-    seqsarr = np.asarray(seqs)
-    ar = seqarr.repeat(seqsarr.shape[0], axis=0)
-    ret = np.concatenate((seqsarr, ar), axis=1)
-    ret2 = np.concatenate((ar, seqsarr), axis=1)
-    ret = np.concatenate((ret, ret2))
-    return ret
```

### Comparing `nuad-0.4.1/nuad/nupack_viennaRNA_parameter_files/dna_mathews1999.par` & `nuad-0.4.2/nuad/nupack_viennaRNA_parameter_files/dna_mathews1999.par`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/nuad/nupack_viennaRNA_parameter_files/dna_mathews2004.par` & `nuad-0.4.2/nuad/nupack_viennaRNA_parameter_files/dna_mathews2004.par`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/nuad/search.py` & `nuad-0.4.2/nuad/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -863,25 +863,25 @@
     (In this case, those sequences are not checked against any :any:`NumpyFilter`'s
     or :any:`SequenceFilter`'s in the :any:`Design`, since those checks are applied prior to
     assigning DNA sequences to any :any:`Domain`.)
 
     The function has some side effects. It writes a report on the optimal sequence assignment found so far
     every time a new improve assignment is found.
 
-    Whenever a new optimal sequence assignment is found, the following are written to files:
-    - DNA sequences of each strand are written to a text file .
-    - the whole dsd design
-    - a report on the DNA sequences indicating how well they do on constraints.
+    Whenever a new optimal sequence assignment is found, the following are also be written to files:
+
+    * DNA sequences of each strand are written to a text file .
+    * the whole design itself
+    * a report on the DNA sequences indicating how well they do on constraints.
 
     :param design:
         The :any:`Design` containing the :any:`Domain`'s to which to assign DNA sequences
         and the :any:`Constraint`'s that apply to them
     :param params:
-        A :any:`SearchParameters` object with attributes that can be called within this function
-        for flexibility.
+        A :any:`SearchParameters` object with attributes that can be used to specify options for the search.
 
     """
 
     if params.random_seed is not None:
         logger.info(f'using random seed of {params.random_seed}; '
                     f'use this same seed to reproduce this run')
 
@@ -1809,17 +1809,16 @@
                     self.num_violations_nonfixed -= 1
 
         self.reset_new()
 
         _assert_violations_are_accurate(self.evaluations, self.violations)
 
     def update_scores_and_counts(self) -> None:
-        """
-        :return: Total score of all evaluations.
-        """
+        # return: Total score of all evaluations.
+
         self.total_score = self.total_score_fixed = self.total_score_nonfixed = 0.0
         self.num_evaluations = self.num_evaluations_nonfixed = self.num_evaluations_fixed = 0
         self.num_violations = self.num_violations_nonfixed = self.num_violations_fixed = 0
 
         # count evaluations
         for evaluation in values_2d(self.evaluations):
             self.num_evaluations += 1
@@ -1945,19 +1944,19 @@
 
     score: float
 
     result: nc.Result
 
     def __init__(self, constraint: Constraint, violated: bool, part: DesignPart, domains: Iterable[Domain],
                  score: float, summary: str, result: nc.Result) -> None:
-        # :param constraint:
+        # constraint:
         #     :any:`Constraint` that was violated to result in this
-        # :param domains:
+        # domains:
         #     :any:`Domain`'s that were involved in violating :py:data:`Evaluation.constraint`
-        # :param score:
+        # score:
         #     total "score" of this violation, typically something like an excess energy over a
         #     threshold, squared, multiplied by the :data:`Constraint.weight`
         self.constraint = constraint
         self.violated = violated
         self.part = part
         self.domains = frozenset(domains)
         self.score = score
@@ -2196,15 +2195,15 @@
         same as argument `bins` to matplotlib.pyplot.hist:
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.yscale.html
         Can either be a single value to apply to all charts,
         or a dict mapping a constraint to a value,
         with the same rules as `xlims`
     """
     import matplotlib.pyplot as plt
-    from IPython.display import display, Markdown
+    from IPython.display import display, Markdown  # noqa
 
     def dm(obj):
         display(Markdown(obj))
 
     if xlims is None:
         xlims = {}
     if ylims is None:
@@ -2224,15 +2223,15 @@
         else:
             reports_without_values.append(report)
     num_figs = len(reports_with_values)
 
     for report in reports_without_values:
         part_type_name = report.constraint.part_name()
         dm(f'## {report.constraint.description}')
-        dm(f'### {report.num_violations}/{report.num_evaluations}  (\#violations/\#evaluations)')
+        dm(f'### {report.num_violations}/{report.num_evaluations}  (\#violations/\#evaluations)')  # noqa
         for viol in report.violations:
             print(f'  {part_type_name} {viol.part.name}: {viol.summary}')
 
     for i, (report, quantities) in enumerate(reports_with_values):
         quantities = [ev.result.value for ev in report.evaluations if ev.result.value is not None]
         assert len(quantities) > 0
```

### Comparing `nuad-0.4.1/nuad/stopwatch.py` & `nuad-0.4.2/nuad/stopwatch.py`

 * *Files identical despite different names*

### Comparing `nuad-0.4.1/nuad/vienna_nupack.py` & `nuad-0.4.2/nuad/vienna_nupack.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import itertools
 import os
 import logging
 import random
 import subprocess as sub
 import sys
 from multiprocessing.pool import ThreadPool
-from pathos.pools import ProcessPool
 from typing import Sequence, Tuple, List, Iterable
 
 import numpy as np
 
 import nuad.constraints as nc
 
 os_is_windows = sys.platform == 'win32'
@@ -133,56 +132,61 @@
     return dg
 
 
 def tupleize(seqs: str | Iterable[str]) -> Tuple[str, ...]:
     return (seqs,) if isinstance(seqs, str) else tuple(seqs)
 
 
-def pfunc_parallel(
-        pool: ProcessPool,
-        all_seqs: Sequence[str | Tuple[str, ...]],
-        temperature: float = default_temperature,
-        sodium: float = default_sodium,
-        magnesium: float = default_magnesium,
-        strand_association_penalty: bool = True,
-) -> Tuple[float]:
-    num_seqs = len(all_seqs)
-    if num_seqs == 0:
-        return tuple()
-
-    all_seqs = tuple(tupleize(seqs) for seqs in all_seqs)
-
-    first_seqs = all_seqs[0]
-
-    bases = sum(len(seq) for seq in first_seqs)
-    num_cores = nc.cpu_count(logical=True)
-
-    # these thresholds were measured empirically; see notebook nuad_parallel_time_trials.ipynb
-    call_sequential = (len(all_seqs) == 1
-                       or (bases <= 30 and num_seqs <= 50)
-                       or (bases <= 40 and num_seqs <= 40)
-                       or (bases <= 50 and num_seqs <= 30)
-                       or (bases <= 75 and num_seqs <= 20)
-                       or (bases <= 100 and num_seqs <= 10)
-                       or (bases <= 125 and num_seqs <= 4)
-                       or (bases <= 150 and num_seqs <= 3)
-                       or (num_seqs <= 1)
-                       )
-
-    def calculate_energies_sequential(all_tuples: Sequence[Tuple[str, ...]]) -> Tuple[float]:
-        return tuple(pfunc(seqs, temperature, sodium, magnesium, strand_association_penalty)
-                     for seqs in all_tuples)
-
-    if call_sequential:
-        return calculate_energies_sequential(all_seqs)
-
-    lists_of_sequence_pairs = nc.chunker(all_seqs, num_chunks=num_cores)
-    lists_of_energies = pool.map(calculate_energies_sequential, lists_of_sequence_pairs)
-    energies = nc.flatten(lists_of_energies)
-    return tuple(energies)
+try:
+    from pathos.pools import ProcessPool
+
+    def pfunc_parallel(
+            pool: ProcessPool,
+            all_seqs: Sequence[str | Tuple[str, ...]],
+            temperature: float = default_temperature,
+            sodium: float = default_sodium,
+            magnesium: float = default_magnesium,
+            strand_association_penalty: bool = True,
+    ) -> Tuple[float]:
+        num_seqs = len(all_seqs)
+        if num_seqs == 0:
+            return tuple()
+
+        all_seqs = tuple(tupleize(seqs) for seqs in all_seqs)
+
+        first_seqs = all_seqs[0]
+
+        bases = sum(len(seq) for seq in first_seqs)
+        num_cores = nc.cpu_count(logical=True)
+
+        # these thresholds were measured empirically; see notebook nuad_parallel_time_trials.ipynb
+        call_sequential = (len(all_seqs) == 1
+                           or (bases <= 30 and num_seqs <= 50)
+                           or (bases <= 40 and num_seqs <= 40)
+                           or (bases <= 50 and num_seqs <= 30)
+                           or (bases <= 75 and num_seqs <= 20)
+                           or (bases <= 100 and num_seqs <= 10)
+                           or (bases <= 125 and num_seqs <= 4)
+                           or (bases <= 150 and num_seqs <= 3)
+                           or (num_seqs <= 1)
+                           )
+
+        def calculate_energies_sequential(all_tuples: Sequence[Tuple[str, ...]]) -> Tuple[float]:
+            return tuple(pfunc(seqs, temperature, sodium, magnesium, strand_association_penalty)
+                         for seqs in all_tuples)
+
+        if call_sequential:
+            return calculate_energies_sequential(all_seqs)
+
+        lists_of_sequence_pairs = nc.chunker(all_seqs, num_chunks=num_cores)
+        lists_of_energies = pool.map(calculate_energies_sequential, lists_of_sequence_pairs)
+        energies = nc.flatten(lists_of_energies)
+        return tuple(energies)
+except ModuleNotFoundError as e:
+    raise e
 
 
 def nupack_complex_base_pair_probabilities(strand_complex: 'nc.Complex',  # circular import causes problems
                                            temperature: float = default_temperature,
                                            sodium: float = default_sodium,
                                            magnesium: float = default_magnesium) -> np.ndarray:
     """
```

### Comparing `nuad-0.4.1/nuad.egg-info/PKG-INFO` & `nuad-0.4.2/nuad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuad
-Version: 0.4.1
+Version: 0.4.2
 Summary: nuad stands for "NUcleic Acid Designer". Enables one to specify constraints on a DNA (or RNA) nanostructure made from synthetic DNA/RNA and then attempts to find concrete DNA sequences that satisfy the constraints.
 Home-page: https://github.com/UC-Davis-molecular-computing/nuad
 Author: David Doty
 Author-email: doty@ucdavis.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -138,15 +138,15 @@
 
 - `Domain`: A `Domain` represents a contiguous subsequence of DNA. A single `Domain` represents both the DNA sequence and its complement. For instance there is one `Domain` with name `a`, with two versions: unstarred (`a`) and starred (`a*`). If the DNA sequence of `a` is 5'-CCCAA-3', then the DNA sequence of `a*` is 3'-GGGTT-5'. 
 
 - `DomainPool`: Each `Domain` is assigned a single `DomainPool`, which can be thought of as a "source of DNA sequences" for the `Domain`. (See exceptions below.) The sequence design algorithm will take DNA sequences from this source when attempting to find DNA sequences to assign to `Domain`'s to satisfy all constraints. Each `DomainPool` has a fixed length. Since each `Domain` only has one `DomainPool`, this means that each `Domain` has a fixed length as well. If no other constraints are specified, then the `DomainPool` simply provides all DNA sequences of that length. Though you will generally not call this method yourself, the method `DomainPool.generate_sequence()` returns a sequence from the pool. This method can be called infinitely many times (i.e., sequences can repeat, though the exact period after which they repeat is an unspecified implementation detail.)
 
   - There are two types of `Domain`'s with no associated `DomainPool`. One type is a `Domain` with the field `fixed` set to `True` by calling the method `Domain.set_fixed_sequence()`, which has some fixed DNA sequence that cannot be changed. A fixed `Domain` has no `DomainPool`.)
 
-  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.dependent and https://dnadsd.readthedocs.io/en/latest/#constraints.Domain.subdomains.
+  - The other type is a `Domain` with the field `dependent` set the `True` (by assigning the field directly). Such a domain is dependent for its sequence on the sequence of some other `Domain` with `dependent = False` that either contains it as a subsequence, or is contained in it as a subsequence. For example, one can declare the domain `a` is independent (has `dependent = False`), with length 8, and has dependent subdomains `b` and `c` of length 5 and 3. `a` would have a `DomainPool`, and if `a` is assigned sequence AAACCGTT, then `b` is automatically assigned sequence AAACC, and `c` is automatically assigned sequence GTT. Such subdomains are assigned via the field `Domain.subdomains`; see the API documentation for more details: https://nuad.readthedocs.io/en/latest/#constraints.Domain.dependent and https://nuad.readthedocs.io/en/latest/#constraints.Domain.subdomains.
 
 - `Strand`: A `Strand` contains an ordered list `domains` of `Domain`'s, together with an identification of which `Domain`'s are starred in this `Strand`, the latter specified as a set `starred_domain_indices` of indices (starting at 0) into the list `domains`. For example, the `Strand` consisting of `Domain`'s `a`, `b*`, `c`, `b`, `d*`, in that order, would have `domains = [a, b, c, b, d]` and `starred_domain_indices = {1, 4}`.
 
 - `Design`: This describes the whole system. Generally you will have one `Design`, which is composed of a list of `Strand`'s.
 
 - `Constraint`: There are several kinds of constraint objects. Not all of them are related in the type hierarchy. 
 
@@ -155,15 +155,15 @@
 
     - **"soft" constraints:**  All other constraints are subclasses of the abstract superclass `Constraint`. These constrains are "softer": sequences violating the constraints are allowed to be assigned to `Domain`'s. The sequence design algorithm steadily improves the design by changing sequences until all of these constraints are satisfied. The different subtypes of the base class `Constraint` correspond to different parts of the `Design` that are being evaluated by the `Constraint`. The types are:
 
         - `SingularConstraint`: This is an abstract superclass of the following concrete subclasses. The difference with the other abstract superclass `BulkConstraint` is explained in `BulkConstraint` below.
         
             - `DomainConstraint`: This only looks at a single `Domain`. In practice this is not used much, since there's not much information in a `Domain` other than its DNA sequence, so a `SequenceConstraint` or `NumpyConstraint` typically would already have filtered out any DNA sequence not satisfying such a constraint.
 
-            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://dnadsd.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
+            - `StrandConstraint`: This evaluates a whole `Strand`. A common example is that NUPACK's `pfunc` should indicate a complex free energy above a certain threshold, indicating the `Strand` has little secondary structure. This example constraint is available in the library by calling [nupack_strand_complex_free_energy_constraint](https://nuad.readthedocs.io/en/latest/#constraints.nupack_strand_complex_free_energy_constraint).
 
             - `DomainPairConstraint`: This evaluates a pair of `Domain`'s.
 
             - `StrandPairConstraint`: This evaluates a pair of `Strand`'s.
 
             - `ComplexConstraint`: This evaluates a tuple of `Strand`'s of arbitrary size.
 
@@ -179,15 +179,15 @@
 
     The `BulkConstraint` subclasses `DomainsConstraint`, `StrandsConstraint`, `DomainPairsConstraint`, `StrandPairsConstraint` use a different function, called `evaluate_bulk`, which take as input a list of "`Design` parts" (e.g., a list of pairs of `Strand`'s for a `StrandPairsConstraint`). The return value is of type `List[Tuple[DesignPart, float, str]]`, i.e., a list of triples, where each triple is `(part, excess, summary)`.
     
     `part` is the individual part of the design that caused a problem. Generally it will be one of the elements of the list passed to `evaluate_bulk`, though the returned list could be smaller than the input list. This is because some parts may satisfy the constraint, and generally the only parts returned from `evaluate_bulk` are those that violated the constraint. `excess` and `summary` have the same interpretation as with the "singular" constraints.
 
     The search algorithm evaluates the constraints, and for each violated constraint, it turns the `excess` value into a "score" by first passing it through the "score transfer function", which by default squares the value, and then multiplies by the value `Constraint.weight` (by default 1). The goal of the search is to minimize the sum of scores across all violated `Constraint`'s. The reason that the score is squared is that this leads the search algorithm to (slightly) favor reducing the excess of constraint violations that are "more in excess", i.e., it would reduce the total score more to reduce an excess from 4 to 3 (reducing the score from 4<sup>2</sup>=16 to 3<sup>2</sup>=9, a reduction of 16-9=7) than to reduce an excess from 2 to 1 (which reduces 2<sup>2</sup>=4 to 1<sup>2</sup>=1, a reduction of only 4-1=3).
 
-    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_dna_sequences](https://dnadsd.readthedocs.io/en/latest/#search.search_for_dna_sequences).
+    The full search algorithm is described in the [API documentation for the function nuad.search.search_for_sequences](https://nuad.readthedocs.io/en/latest/#search.search_for_sequences).
 
 
 ## Constraint evaluations must be pure functions of their inputs
 
 For all constraints, it is critical that the `evaluate` or `evaluate_bulk` functions be *pure* functions of their inputs: the return value should depend only on the parameters passed to the function. For example, a `StrandPairConstraint` takes two strands as input, and its `(excess, summary)` return values should depend *only* on those two strands. Similarly, a `StrandsConstraint`, whose `evaluate_bulk` function takes a list of strands as input, should return a list of tuples, where each tuple represents a violation of a strand that depends only on that strand. This is required because nuad does an optimization in which constraints are only evaluated if they depend on parts of the design that contain the domain(s) that changed in the current iteration.
 
 For example, suppose there are 100 strands, but only 3 strands contain the domain `x`, and `x` is the domain whose DNA sequence is changed in the current search iteration. Then each `StrandConstraint` `s` will be evaluated only on those 3 strands, on the assumption that the other 97 strands would have the same output of the function `s.evaluate` as before.
```

### Comparing `nuad-0.4.1/setup.py` & `nuad-0.4.2/setup.py`

 * *Files identical despite different names*

