# Comparing `tmp/baguette_verse-1.0.0.tar.gz` & `tmp/baguette_verse-1.0.5.tar.gz`

## Comparing `baguette_verse-1.0.0.tar` & `baguette_verse-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,69 @@
--rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/bake.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/metalib.py
--rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/toast.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/__init__.py
--rw-r--r--   0        0        0    24206 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/rack.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/__init__.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/compiler.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/cuckoo_api_list.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/logger.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17232 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    33256 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13655 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16621 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/extractor.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/evaluator.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0    30591 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/LICENSE
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/README.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    48653 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/logger.py
+-rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23846 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20635 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35115 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/LICENSE
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/README.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    48795 2020-02-02 00:00:00.000000 baguette_verse-1.0.5/PKG-INFO
```

### Comparing `baguette_verse-1.0.0/bake.py` & `baguette_verse-1.0.5/baguette/bakery/bake.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,530 +1,531 @@
 """
 This is a *magic* script to bake baguettes. Use -h/--help for usage.
 """
 
 
 
-
-
 def main():
     """
     Command line function to bake Cuckoo report(s). Use -h/--help for more info.
     """
 
-    if __name__ in ("__main__", "bake"):        # One for when started with Python, the other for when started with package command...
+    import logging
 
-        import logging
-        from baguette.bakery.logger import logger, set_level
-        set_level(logging.ERROR)
-
-        import argparse
-        from os import environ
-        import pathlib
-        from typing import Literal, Iterator
-        from baguette.bakery.compiler import compile
-        from baguette.bakery.source import filters
-        from baguette.bakery.source.colors import Color
-        from baguette.rack import BaguetteRack, TimeoutExit
-
-        parser = argparse.ArgumentParser(
-            description = 'Bakes Cuckoo reports into baguettes (gexf and pyt graphs).',
-            add_help = True,
-            conflict_handler = 'resolve',
-            epilog = """
-            Note that the format of input and outputs is quite flexible. Indeed you can :
-            give output folders for each output file, which will make all input have their output in these folders
-            - give a set of outputs for each input file, as long as they are given in the same place in the parameter sequences
-            - do the same with input folders and output folders, as long as they also come in the same order
-            - mix these options, again, as long as it has a meaning in the order they come.
-            - Note that if a given path does not exists, it is interpreted as a folder.
-            - Also, if an input path has the appropriate extension, it will be considered as a single input.
-            """
-            )
-
-        class PathSorter:
-
-            def __init__(self, pool : list[pathlib.Path | Literal["-"]], name : str) -> None:
-                self.pool = pool
-                self.name = name
-            
-            def __call__(self, arg : str):
-                if arg == "-":
-                    self.pool.append(arg)
-                    return
-                from glob import iglob
-                import re
-                magic_check = re.compile('([*?[])')
-                try:
-                    if magic_check.search(arg) is not None:
-                        self.pool.extend(pathlib.Path(path) for path in iglob(arg))
-                    else:
-                        self.pool.append(pathlib.Path(arg))
-                except:
-                    parser.error("invalid {} path : '{}'".format(self.name, arg))
+    from ..logger import logger, set_level
+    set_level(logging.ERROR)
 
-        reports : list[pathlib.Path | Literal["-"]] = []
-        baguettes : list[pathlib.Path | Literal["-"]] = []
-        visuals : list[pathlib.Path | Literal["-"]] = []
-        outputs : list[pathlib.Path | Literal["-"]] = []
-
-        def pool_size(arg : str) -> int:
-            """
-            Transforms a numeric argument in a number of process to use as a process pool.
-            It can be absolute, negative (relative to the number of CPUs) or 
-            """
-            from os import cpu_count
-            N = cpu_count()
-            if not N:
-                N = 1
+    import argparse
+    import pathlib
+    from os import environ
+    from typing import Iterator, Literal
+
+    from ..rack import BaguetteRack, TimeoutExit
+    from .compiler import compile
+    from .source import filters
+    from .source.colors import Color
+
+    parser = argparse.ArgumentParser(
+        description = 'Bakes Cuckoo reports into baguettes (gexf and pyt graphs).',
+        add_help = True,
+        conflict_handler = 'resolve',
+        epilog = """
+        Note that the format of input and outputs is quite flexible. Indeed you can :
+        give output folders for each output file, which will make all input have their output in these folders
+        - give a set of outputs for each input file, as long as they are given in the same place in the parameter sequences
+        - do the same with input folders and output folders, as long as they also come in the same order
+        - mix these options, again, as long as it has a meaning in the order they come.
+        - Note that if a given path does not exists, it is interpreted as a folder.
+        - Also, if an input path has the appropriate extension, it will be considered as a single input.
+        """
+        )
+
+    class PathSorter:
+
+        def __init__(self, pool : list[pathlib.Path | Literal["-"]], name : str) -> None:
+            self.pool = pool
+            self.name = name
+        
+        def __call__(self, arg : str):
+            if arg == "-":
+                self.pool.append(arg)
+                return
+            import re
+            from glob import iglob
+            magic_check = re.compile('([*?[])')
             try:
-                v = int(arg)
-                if v < 0:
-                    v = N - v
-                if v <= 0:
-                    parser.error("got a (too) negative value for process pool size : '{}'".format(arg))
+                if magic_check.search(arg) is not None:
+                    self.pool.extend(pathlib.Path(path) for path in iglob(arg))
+                else:
+                    self.pool.append(pathlib.Path(arg))
             except:
-                try:
-                    v = float(arg)
-                    if v <= 0:
-                        parser.error("got a negative relative process pool size : '{}'".format(arg))
-                    v = round(v * N)
-                except:
-                    parser.error("not a process pool size : '{}'".format(arg))
-            return v
+                parser.error("invalid {} path : '{}'".format(self.name, arg))
 
-        def time(arg : str) -> float:
-            from math import isnan
+    reports : list[pathlib.Path | Literal["-"]] = []
+    baguettes : list[pathlib.Path | Literal["-"]] = []
+    visuals : list[pathlib.Path | Literal["-"]] = []
+    outputs : list[pathlib.Path | Literal["-"]] = []
+
+    def pool_size(arg : str) -> int:
+        """
+        Transforms a numeric argument in a number of process to use as a process pool.
+        It can be absolute, negative (relative to the number of CPUs) or 
+        """
+        from os import cpu_count
+        N = cpu_count()
+        if not N:
+            N = 1
+        try:
+            v = int(arg)
+            if v < 0:
+                v = N - v
+            if v <= 0:
+                parser.error("got a (too) negative value for process pool size : '{}'".format(arg))
+        except:
             try:
                 v = float(arg)
-                if v <= 0 or isnan(v):
-                    parser.error("got a negative, null or nan maxtime")
-                return v
+                if v <= 0:
+                    parser.error("got a negative relative process pool size : '{}'".format(arg))
+                v = round(v * N)
             except:
-                parser.error("expected positive float for maxtime, got : '{}'".format(arg))
-
-        def paint_color(c : str) -> Color:
-            if c in dir(Color):
-                color = getattr(Color, c)
-                if not isinstance(color, Color):
-                    parser.error(f"not a valid color name : '{c}'")
-                return color
-            else:
-                # We can match colors in ALLL LANGUAGES!!!!
-                import re
-                color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
-                sep_re = r"(?:[ ,;:\|\&]+)"
-                inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
-                fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
-                if not fmatch:
-                    parser.error(f"could not understand color format : '{c}'")
-                r, g, b = fmatch.groups()
-
-                def is_float(s : str) -> bool:
-                    try:
-                        f = float(s)
-                        if not 0 <= f <= 1:
-                            return False
-                        return True
-                    except:
-                        return False
-                
-                def is_int(s : str) -> bool:
-                    try:
-                        i = int(s)
-                        if not 0 <= i <= 255:
-                            return False
-                        return True
-                    except:
-                        return False
-                
-                def is_hex(s : str) -> bool:
-                    try:
-                        i = int(s, base=16)
-                        if not 0 <= i <= 255:
-                            return False
-                        return True
-                    except:
-                        return False
-                    
-                if all(is_float(x) for x in (r, g, b)):
-                    r, g, b = float(r), float(g), float(b)
-                elif all(is_int(x) for x in (r, g, b)):
-                    r, g, b = int(r), int(g), int(b)
-                elif all(is_hex(x) for x in (r, g, b)):
-                    r, g, b = int(r, 16), int(g, 16), int(b, 16)
-                else:
-                    parser.error(f"could not understand color format : '{c}'")
+                parser.error("not a process pool size : '{}'".format(arg))
+        return v
 
-                return Color(r, g, b)
-
-        parser.add_argument("reports", type=PathSorter(reports, "report"), default=None, nargs="*" if "BAGUETTE_REPORTS" in environ else "+", help="Cuckoo report files (.json) to bake baguettes from. Can also be folders containing reports. Defaults to environment variable 'BAGUETTE_REPORTS' if set.")
-        parser.add_argument("--baguettes", type=PathSorter(baguettes, "baguette"), default=None, action="extend", nargs="*", help="the path(s) to the output baguette files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_BAGUETTES' or '-' if not set.")
-        parser.add_argument("--visuals", type=PathSorter(visuals, "visual"), default=None, action="extend", nargs="*", help="the path(s) to the output visual (Gephi) files (.gexf). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_VISUALS' or '-' if not set.")
-        parser.add_argument("-o", "--outputs", type=PathSorter(outputs, "output"), default=None, action="extend", nargs="*", help="the path to the result index folders (which end in .bag). They contain the index file (.pyt) which stores all the information about a given baguette. Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_OUTPUTS' or '.' if not set.")
-        parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
-        parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
-        parser.add_argument("-f", "--filters", type=str, default=[], choices=[name for name in dir(filters) if isinstance(getattr(filters, name), filters.Filter)], nargs="*", help="a list of filters that can be used when exporting the baguette to the visual file (.gexf).")
-        parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
-        parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
-        parser.add_argument("--skip_data_comparison", action="store_true", default=False, help="if enabled, the computation of the Levenshtein similarity between all Data nodes will be skipped.")
-        parser.add_argument("--skip_diff_comparison", action="store_true", default=False, help="same as skip_data_comparison but for Diff nodes.")
-        parser.add_argument("--background", type=paint_color, default=Color.black, help="If a color is given for background, the color settings which are close to the background color will be change to be more visible on background. Must be a valid color name or RGB values.")
-
-
-        args = parser.parse_args()
-
-        # Setting logging level
-
-        levels = {
-            0 : logging.ERROR,
-            1 : logging.WARNING,
-            2 : logging.INFO,
-            3 : logging.DEBUG
-        }
-        verbosity : Literal[0, 1, 2, 3] = min(3, args.verbosity)
-        set_level(levels[verbosity])
-
-        logger.info("Arguments parsed. Discovering jobs.")
+    def time(arg : str) -> float:
+        from math import isnan
+        try:
+            v = float(arg)
+            if v <= 0 or isnan(v):
+                parser.error("got a negative, null or nan maxtime")
+            return v
+        except:
+            parser.error("expected positive float for maxtime, got : '{}'".format(arg))
 
-        # Parsing jobs
+    def paint_color(c : str) -> Color:
+        if c in dir(Color):
+            color = getattr(Color, c.lower())
+            if not isinstance(color, Color):
+                parser.error(f"not a valid color name : '{c}'")
+            return color
+        else:
+            # We can match colors in ALLL LANGUAGES!!!!
+            import re
+            color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
+            sep_re = r"(?:[ ,;:\|\&]+)"
+            inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
+            fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
+            if not fmatch:
+                parser.error(f"could not understand color format : '{c}'")
+            r, g, b = fmatch.groups()
 
-        if not reports:
-            try:
-                reports = [pathlib.Path(environ["BAGUETTE_REPORTS"])]
-            except KeyError:
-                raise RuntimeError("Environment variable 'BAGUETTE_REPORTS' not found and there is no input...")
-            except:
-                parser.error("invalid report path in environment variable : '{}'".format(environ["BAGUETTE_REPORTS"]))
-        if not baguettes:
-            if "BAGUETTE_BAGUETTES" in environ:
+            def is_float(s : str) -> bool:
                 try:
-                    baguettes = [pathlib.Path(environ["BAGUETTE_BAGUETTES"])]
+                    f = float(s)
+                    if not 0 <= f <= 1:
+                        return False
+                    return True
                 except:
-                    parser.error("invalid baguettes path in environment variable : '{}'".format(environ["BAGUETTE_BAGUETTES"]))
-            else:
-                baguettes = ["-"]
-        if not visuals:
-            if "BAGUETTE_VISUALS" in environ:
+                    return False
+            
+            def is_int(s : str) -> bool:
                 try:
-                    visuals = [pathlib.Path(environ["BAGUETTE_VISUALS"])]
+                    i = int(s)
+                    if not 0 <= i <= 255:
+                        return False
+                    return True
                 except:
-                    parser.error("invalid visuals path in environment variable : '{}'".format(environ["BAGUETTE_VISUALS"]))
-            else:
-                visuals = ["-"]
-        if not outputs:
-            if "BAGUETTE_OUTPUTS" in environ:
+                    return False
+            
+            def is_hex(s : str) -> bool:
                 try:
-                    outputs = [pathlib.Path(environ["BAGUETTE_OUTPUTS"])]
+                    i = int(s, base=16)
+                    if not 0 <= i <= 255:
+                        return False
+                    return True
                 except:
-                    parser.error("invalid outputs path in environment variable : '{}'".format(environ["BAGUETTE_OUTPUTS"]))
+                    return False
+                
+            if all(is_float(x) for x in (r, g, b)):
+                r, g, b = float(r), float(g), float(b)
+            elif all(is_int(x) for x in (r, g, b)):
+                r, g, b = int(r), int(g), int(b)
+            elif all(is_hex(x) for x in (r, g, b)):
+                r, g, b = int(r, 16), int(g, 16), int(b, 16)
             else:
-                outputs = [pathlib.Path(".")]
+                parser.error(f"could not understand color format : '{c}'")
+
+            return Color(r, g, b)
 
-        class JobQueue:
+    parser.add_argument("reports", type=PathSorter(reports, "report"), default=None, nargs="*" if "BAGUETTE_REPORTS" in environ else "+", help="Cuckoo report files (.json) to bake baguettes from. Can also be folders containing reports. Defaults to environment variable 'BAGUETTE_REPORTS' if set.")
+    parser.add_argument("--baguettes", type=PathSorter(baguettes, "baguette"), default=None, action="extend", nargs="*", help="the path(s) to the output baguette files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_BAGUETTES' or '-' if not set.")
+    parser.add_argument("--visuals", type=PathSorter(visuals, "visual"), default=None, action="extend", nargs="*", help="the path(s) to the output visual (Gephi) files (.gexf). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_VISUALS' or '-' if not set.")
+    parser.add_argument("-o", "--outputs", type=PathSorter(outputs, "output"), default=None, action="extend", nargs="*", help="the path to the result index folders (which end in .bag). They contain the index file (.pyt) which stores all the information about a given baguette. Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_OUTPUTS' or '.' if not set.")
+    parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
+    parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
+    parser.add_argument("-f", "--filters", type=str, default=[], choices=[name for name in dir(filters) if isinstance(getattr(filters, name), filters.Filter)], nargs="*", help="a list of filters that can be used when exporting the baguette to the visual file (.gexf).")
+    parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
+    parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
+    parser.add_argument("--skip_data_comparison", action="store_true", default=False, help="if enabled, the computation of the Levenshtein similarity between all Data nodes will be skipped.")
+    parser.add_argument("--skip_diff_comparison", action="store_true", default=False, help="same as skip_data_comparison but for Diff nodes.")
+    parser.add_argument("--background", type=paint_color, default=Color.black, help="If a color is given for background, the color settings which are close to the background color will be changed to be more visible on that background. Must be a valid color name or RGB values.")
+
+
+    args = parser.parse_args()
+
+    # Setting logging level
+
+    levels = {
+        0 : logging.ERROR,
+        1 : logging.WARNING,
+        2 : logging.INFO,
+        3 : logging.DEBUG
+    }
+    verbosity : Literal[0, 1, 2, 3] = min(3, args.verbosity)
+    set_level(levels[verbosity])
 
+    logger.info("Arguments parsed. Discovering jobs.")
+
+    # Parsing jobs
+
+    if not reports:
+        try:
+            reports = [pathlib.Path(environ["BAGUETTE_REPORTS"])]
+        except KeyError:
+            raise RuntimeError("Environment variable 'BAGUETTE_REPORTS' not found and there is no input...")
+        except:
+            parser.error("invalid report path in environment variable : '{}'".format(environ["BAGUETTE_REPORTS"]))
+    if not baguettes:
+        if "BAGUETTE_BAGUETTES" in environ:
+            try:
+                baguettes = [pathlib.Path(environ["BAGUETTE_BAGUETTES"])]
+            except:
+                parser.error("invalid baguettes path in environment variable : '{}'".format(environ["BAGUETTE_BAGUETTES"]))
+        else:
+            baguettes = ["-"]
+    if not visuals:
+        if "BAGUETTE_VISUALS" in environ:
+            try:
+                visuals = [pathlib.Path(environ["BAGUETTE_VISUALS"])]
+            except:
+                parser.error("invalid visuals path in environment variable : '{}'".format(environ["BAGUETTE_VISUALS"]))
+        else:
+            visuals = ["-"]
+    if not outputs:
+        if "BAGUETTE_OUTPUTS" in environ:
+            try:
+                outputs = [pathlib.Path(environ["BAGUETTE_OUTPUTS"])]
+            except:
+                parser.error("invalid outputs path in environment variable : '{}'".format(environ["BAGUETTE_OUTPUTS"]))
+        else:
+            outputs = [pathlib.Path(".")]
+
+    class JobQueue:
+
+        """
+        These objects hold a series of grouped jobs.
+        """
+
+        def __init__(self, groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = []) -> None:
+            from copy import deepcopy
+            self.__groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = deepcopy(groups)
+            self.__last_group : list[pathlib.Path] = []
+            self.__active : bool = False
+        
+        def insert_group(self, group : list[pathlib.Path] | pathlib.Path | Literal["-"]):
             """
-            These objects hold a series of grouped jobs.
+            Creates an independant work group with given content, also creating a new active group for later use.
             """
-
-            def __init__(self, groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = []) -> None:
-                from copy import deepcopy
-                self.__groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = deepcopy(groups)
-                self.__last_group : list[pathlib.Path] = []
-                self.__active : bool = False
-            
-            def insert_group(self, group : list[pathlib.Path] | pathlib.Path | Literal["-"]):
-                """
-                Creates an independant work group with given content, also creating a new active group for later use.
-                """
-                if self.__active:
-                    self.__groups.append(self.__last_group)
-                self.__groups.append(group)
-                self.__last_group = []
-                self.__active = False
-            
-            def append_to_active_group(self, path : pathlib.Path):
-                """
-                Appends a file to the current group.
-                """
-                self.__last_group.append(path)
-                self.__active = True
-            
-            def new_group(self):
-                """
-                Adds the active group to the queue and creates a new empty active group.
-                """
-                if self.__active:
-                    self.__groups.append(self.__last_group)
-                self.__last_group = []
-                self.__active = True
-
-            def finalize(self):
-                """
-                Finalizes the queue, adding the currently active group to the queue if necessary.
-                """
-                if self.__active and self.__last_group:
-                    self.__groups.append(self.__last_group)
-            
-            def __iter__(self) -> Iterator[pathlib.Path | Literal["-"] | list[pathlib.Path]]:
-                """
-                Yields all the jobs in the queue.
-                """
-                yield from self.__groups
-            
-            def __len__(self) -> int:
-                """
-                Implements len(self).
-                """
-                return len(self.__groups)
-
-            def __getitem__(self, index : int) -> pathlib.Path | Literal["-"] | list[pathlib.Path]:
-                """
-                Implements self[index].
-                """
-                return self.__groups[index]
-
-
-        report_groups : JobQueue = JobQueue()
-        baguette_groups : JobQueue = JobQueue()
-        visual_groups : JobQueue = JobQueue()
-        output_groups : JobQueue = JobQueue()
-
-        def determine_type(path : pathlib.Path | Literal["-"], ext : str) -> Literal["folder", "file"]:
-            """
-            Determines if the given path should be interpreted as a folder or file path.
-            If it ends with the given extension and does not exist, it well be considered a file.
-            """
-            if path == "-":
-                return "folder"
-            elif ext and path.suffix == ext:
-                return "file"
-            if path.is_file():
-                return "file"
-            elif path.is_dir():
-                return "folder"
-            elif path.exists():
-                parser.error("given path exists and is neither a file or folder : '{}'".format(path))
-            else:
-                return "folder"
+            if self.__active:
+                self.__groups.append(self.__last_group)
+            self.__groups.append(group)
+            self.__last_group = []
+            self.__active = False
         
-        def create_name(folder : pathlib.Path) -> pathlib.Path:
+        def append_to_active_group(self, path : pathlib.Path):
             """
-            Given a path, this will return a (possibly) modified path that does not exist in the same folder.
+            Appends a file to the current group.
             """
-            if not folder.exists():
-                return folder
-            n = 0
-            ext = folder.suffix
-            if ext:
-                sfolder = str(folder)[:-len(ext)]
-            else:
-                sfolder = str(folder)
-            new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
-            while new_folder.exists():
-                n += 1
-                new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
-            return new_folder
-            
+            self.__last_group.append(path)
+            self.__active = True
+        
+        def new_group(self):
+            """
+            Adds the active group to the queue and creates a new empty active group.
+            """
+            if self.__active:
+                self.__groups.append(self.__last_group)
+            self.__last_group = []
+            self.__active = True
 
-        for r in reports:
-            if r == "-":
-                parser.error("cannot use automatic destination operator for input files.")
-            if determine_type(r, ".json") == "folder":
-                if r.exists():
-                    report_groups.insert_group([p for p in r.iterdir()])
-                else:
-                    parser.error("input folder/file does not exist : '{}'".format(r))
-            else:
-                if r.exists():
-                    report_groups.append_to_active_group(r)
-                else:
-                    parser.error("input file does not exist : '{}'".format(r))
-        report_groups.finalize()
+        def finalize(self):
+            """
+            Finalizes the queue, adding the currently active group to the queue if necessary.
+            """
+            if self.__active and self.__last_group:
+                self.__groups.append(self.__last_group)
         
-        for b in baguettes:
-            if determine_type(b, ".pyt") == "folder":
-                baguette_groups.insert_group(b)
-            else:
-                if b == "-":
-                    raise RuntimeError("How?")
-                baguette_groups.append_to_active_group(b)
-        baguette_groups.finalize()
-        if len(baguette_groups) == 1 and len(report_groups) > 1 and (isinstance(baguette_groups[0], pathlib.Path) or baguette_groups[0] == "-"):
-            baguette_groups = JobQueue([baguette_groups[0]] * len(report_groups))
-
-        for v in visuals:
-            if determine_type(v, ".gexf") == "folder":
-                visual_groups.insert_group(v)
-            else:
-                if v == "-":
-                    raise RuntimeError("How?")
-                visual_groups.append_to_active_group(v)
-        visual_groups.finalize()
-        if len(visual_groups) == 1 and len(report_groups) > 1 and (isinstance(visual_groups[0], pathlib.Path) or visual_groups[0] == "-"):
-            visual_groups = JobQueue([visual_groups[0]] * len(report_groups))
+        def __iter__(self) -> Iterator[pathlib.Path | Literal["-"] | list[pathlib.Path]]:
+            """
+            Yields all the jobs in the queue.
+            """
+            yield from self.__groups
         
-        for o in outputs:
-            if determine_type(o, ".bag") == "folder":
-                output_groups.insert_group(o)
-            else:
-                if o == "-":
-                    raise RuntimeError("How?")
-                output_groups.append_to_active_group(o)
-        output_groups.finalize()
-        if len(output_groups) == 1 and len(report_groups) > 1 and (isinstance(output_groups[0], pathlib.Path) or output_groups[0] == "-"):
-            output_groups = JobQueue([output_groups[0]] * len(report_groups))
-
-        # def printable_format(l) -> str:
-        #     return str(l) if not isinstance(l, list) else (str(l) if len(l) < 2 else "[...]")
-
-        # print("Sizes: {}, {}, {}, {}".format(len(report_groups), len(baguette_groups), len(visual_groups), len(output_groups)))
-        # print(list(printable_format(r) for r in report_groups))
-        # print(list(printable_format(b) for b in baguette_groups))
-        # print(list(printable_format(v) for v in visual_groups))
-        # print(list(printable_format(o) for o in output_groups))
-        # l1 = list(report_groups)
-        # l2 = list(baguette_groups) + [None] * (len(report_groups) - len(baguette_groups))
-        # l3 = list(visual_groups) + [None] * (len(report_groups) - len(visual_groups))
-        # l4 = list(output_groups) + [None] * (len(report_groups) - len(output_groups))
-        # for r, b, v, o in zip(l1, l2, l3, l4):
-        #     print("Work group:")
-        #     print("reports :", printable_format(r))
-        #     print("baguettes :", printable_format(b))
-        #     print("visuals :", printable_format(v))
-        #     print("outputs :", printable_format(o))
-        #     print("\n")
+        def __len__(self) -> int:
+            """
+            Implements len(self).
+            """
+            return len(self.__groups)
 
-        if len(report_groups) != len(baguette_groups) or len(report_groups) != len(visual_groups) or len(report_groups) != len(output_groups):
-            parser.error("different number of work groups in inputs/outputs.")
+        def __getitem__(self, index : int) -> pathlib.Path | Literal["-"] | list[pathlib.Path]:
+            """
+            Implements self[index].
+            """
+            return self.__groups[index]
+
+
+    report_groups : JobQueue = JobQueue()
+    baguette_groups : JobQueue = JobQueue()
+    visual_groups : JobQueue = JobQueue()
+    output_groups : JobQueue = JobQueue()
+
+    def determine_type(path : pathlib.Path | Literal["-"], ext : str) -> Literal["folder", "file"]:
+        """
+        Determines if the given path should be interpreted as a folder or file path.
+        If it ends with the given extension and does not exist, it well be considered a file.
+        """
+        if path == "-":
+            return "folder"
+        elif ext and path.suffix == ext:
+            return "file"
+        if path.is_file():
+            return "file"
+        elif path.is_dir():
+            return "folder"
+        elif path.exists():
+            parser.error("given path exists and is neither a file or folder : '{}'".format(path))
+        else:
+            return "folder"
+    
+    def create_name(folder : pathlib.Path) -> pathlib.Path:
+        """
+        Given a path, this will return a (possibly) modified path that does not exist in the same folder.
+        """
+        if not folder.exists():
+            return folder
+        n = 0
+        ext = folder.suffix
+        if ext:
+            sfolder = str(folder)[:-len(ext)]
+        else:
+            sfolder = str(folder)
+        new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
+        while new_folder.exists():
+            n += 1
+            new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
+        return new_folder
         
-        for r, b, v, o in zip(report_groups, baguette_groups, visual_groups, output_groups):
-            if not isinstance(r, list):
-                raise RuntimeError("How did we get here?")
-            n = len(r)
-            if isinstance(b, list) and len(b) != n:
-                parser.error("got a work group with different numbers of inputs and outputs.")
-            if isinstance(v, list) and len(v) != n:
-                parser.error("got a work group with different numbers of inputs and outputs.")
-            if isinstance(o, list) and len(o) != n:
-                parser.error("got a work group with different numbers of inputs and outputs.")
-
-        work : list[BaguetteRack] = []
-
-        def stripname(p : pathlib.Path) -> str:
-            """
-            Returns the name of the path without the exetension if it has one.
-            """
-            ext = p.suffix
-            if ext:
-                return p.name[:-len(ext)]
-            return p.name
-
-        for rgroup, bgroup, vgroup, ogroup in zip(report_groups, baguette_groups, visual_groups, output_groups):
-
-            if rgroup == "-":
-                parser.error("cannot use automatic destination operator for input files.")
-            elif isinstance(rgroup, pathlib.Path):      # Folder input
-                rgroup = list(rgroup.iterdir())         # Transform in file inputs
-
-            if ogroup == "-":
-                parser.error("cannot use automatic destination operator for output folders.")
-            elif isinstance(ogroup, pathlib.Path):      # Folder output
-                ogroup = [create_name(pathlib.Path(ogroup, stripname(r) + ".bag")) for r in rgroup]
-            
-            if bgroup == "-":                           # Magic destination:
-                bgroup = [None for _ in rgroup]         # To be determined later
-            elif isinstance(bgroup, pathlib.Path):      # Folder baguette destination
-                bgroup = [create_name(pathlib.Path(bgroup, stripname(r) + ".pyt")) for r in rgroup]       # Pre-compute the baguette paths with report names
-
-            if vgroup == "-":                           # Magic destination:
-                vgroup = [None for _ in rgroup]         # To be determined later
-            elif isinstance(vgroup, pathlib.Path):      # Folder visual destination
-                vgroup = [create_name(pathlib.Path(vgroup, stripname(r) + ".gexf")) for r in rgroup]       # Pre-compute the visual paths with report names
-            
-            for r, b, v, o in zip(rgroup, bgroup, vgroup, ogroup):
-                bg = BaguetteRack(o)
-                bg.report = r
-                bg.baguette = b if b is not None else (bg.working_directory / "baguette.pyt")
-                bg.visual = v if v is not None else (bg.working_directory / "visual.gexf")
-                bg.verbosity = verbosity
-                bg.skip_data_comparison = args.skip_data_comparison
-                bg.skip_diff_comparison = args.skip_diff_comparison
-                bg.filter_names = args.filters
-                bg.maxtime = args.maxtime
-                bg.perf = args.perf
-                bg.background_color = args.background
-                work.append(bg)
+
+    for r in reports:
+        if r == "-":
+            parser.error("cannot use automatic destination operator for input files.")
+        if determine_type(r, ".json") == "folder":
+            if r.exists():
+                report_groups.insert_group([p for p in r.iterdir()])
+            else:
+                parser.error("input folder/file does not exist : '{}'".format(r))
+        else:
+            if r.exists():
+                report_groups.append_to_active_group(r)
+            else:
+                parser.error("input file does not exist : '{}'".format(r))
+    report_groups.finalize()
+    
+    for b in baguettes:
+        if determine_type(b, ".pyt") == "folder":
+            baguette_groups.insert_group(b)
+        else:
+            if b == "-":
+                raise RuntimeError("How?")
+            baguette_groups.append_to_active_group(b)
+    baguette_groups.finalize()
+    if len(baguette_groups) == 1 and len(report_groups) > 1 and (isinstance(baguette_groups[0], pathlib.Path) or baguette_groups[0] == "-"):
+        baguette_groups = JobQueue([baguette_groups[0]] * len(report_groups))
+
+    for v in visuals:
+        if determine_type(v, ".gexf") == "folder":
+            visual_groups.insert_group(v)
+        else:
+            if v == "-":
+                raise RuntimeError("How?")
+            visual_groups.append_to_active_group(v)
+    visual_groups.finalize()
+    if len(visual_groups) == 1 and len(report_groups) > 1 and (isinstance(visual_groups[0], pathlib.Path) or visual_groups[0] == "-"):
+        visual_groups = JobQueue([visual_groups[0]] * len(report_groups))
+    
+    for o in outputs:
+        if determine_type(o, ".bag") == "folder":
+            output_groups.insert_group(o)
+        else:
+            if o == "-":
+                raise RuntimeError("How?")
+            output_groups.append_to_active_group(o)
+    output_groups.finalize()
+    if len(output_groups) == 1 and len(report_groups) > 1 and (isinstance(output_groups[0], pathlib.Path) or output_groups[0] == "-"):
+        output_groups = JobQueue([output_groups[0]] * len(report_groups))
+
+    # def printable_format(l) -> str:
+    #     return str(l) if not isinstance(l, list) else (str(l) if len(l) < 2 else "[...]")
+
+    # print("Sizes: {}, {}, {}, {}".format(len(report_groups), len(baguette_groups), len(visual_groups), len(output_groups)))
+    # print(list(printable_format(r) for r in report_groups))
+    # print(list(printable_format(b) for b in baguette_groups))
+    # print(list(printable_format(v) for v in visual_groups))
+    # print(list(printable_format(o) for o in output_groups))
+    # l1 = list(report_groups)
+    # l2 = list(baguette_groups) + [None] * (len(report_groups) - len(baguette_groups))
+    # l3 = list(visual_groups) + [None] * (len(report_groups) - len(visual_groups))
+    # l4 = list(output_groups) + [None] * (len(report_groups) - len(output_groups))
+    # for r, b, v, o in zip(l1, l2, l3, l4):
+    #     print("Work group:")
+    #     print("reports :", printable_format(r))
+    #     print("baguettes :", printable_format(b))
+    #     print("visuals :", printable_format(v))
+    #     print("outputs :", printable_format(o))
+    #     print("\n")
+
+    if len(report_groups) != len(baguette_groups) or len(report_groups) != len(visual_groups) or len(report_groups) != len(output_groups):
+        parser.error("different number of work groups in inputs/outputs.")
+    
+    for r, b, v, o in zip(report_groups, baguette_groups, visual_groups, output_groups):
+        if not isinstance(r, list):
+            raise RuntimeError("How did we get here?")
+        n = len(r)
+        if isinstance(b, list) and len(b) != n:
+            parser.error("got a work group with different numbers of inputs and outputs.")
+        if isinstance(v, list) and len(v) != n:
+            parser.error("got a work group with different numbers of inputs and outputs.")
+        if isinstance(o, list) and len(o) != n:
+            parser.error("got a work group with different numbers of inputs and outputs.")
+
+    work : list[BaguetteRack] = []
+
+    def stripname(p : pathlib.Path) -> str:
+        """
+        Returns the name of the path without the exetension if it has one.
+        """
+        ext = p.suffix
+        if ext:
+            return p.name[:-len(ext)]
+        return p.name
+
+    for rgroup, bgroup, vgroup, ogroup in zip(report_groups, baguette_groups, visual_groups, output_groups):
+
+        if rgroup == "-":
+            parser.error("cannot use automatic destination operator for input files.")
+        elif isinstance(rgroup, pathlib.Path):      # Folder input
+            rgroup = list(rgroup.iterdir())         # Transform in file inputs
+
+        if ogroup == "-":
+            parser.error("cannot use automatic destination operator for output folders.")
+        elif isinstance(ogroup, pathlib.Path):      # Folder output
+            ogroup = [create_name(pathlib.Path(ogroup, stripname(r) + ".bag")) for r in rgroup]
         
+        if bgroup == "-":                           # Magic destination:
+            bgroup = [None for _ in rgroup]         # To be determined later
+        elif isinstance(bgroup, pathlib.Path):      # Folder baguette destination
+            bgroup = [create_name(pathlib.Path(bgroup, stripname(r) + ".pyt")) for r in rgroup]       # Pre-compute the baguette paths with report names
+
+        if vgroup == "-":                           # Magic destination:
+            vgroup = [None for _ in rgroup]         # To be determined later
+        elif isinstance(vgroup, pathlib.Path):      # Folder visual destination
+            vgroup = [create_name(pathlib.Path(vgroup, stripname(r) + ".gexf")) for r in rgroup]       # Pre-compute the visual paths with report names
         
-        # Compile now...
-
-        from multiprocessing.pool import Pool
-        from threading import Lock, Thread
-
-        # All of this is because multiprocessing was coded with feet... Pool's async methods may freeze (deadlock maybe) on some platforms.
-
-        lock = Lock()
-        failed, timed_out, total = 0, 0, len(work)
-        def execute_single_job(P : Pool) -> bool:
-            nonlocal failed, timed_out
-            with lock:
-                if not work: 
-                    return False
-                br = work.pop()
-            try:
-                br = P.apply(compile, (br, ))
-            except KeyboardInterrupt as e:
-                from traceback import TracebackException
-                br.exception = TracebackException.from_exception(e)
-            if br.exception is None or not br.suppressed:
-                br.export()
-            if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
+        for r, b, v, o in zip(rgroup, bgroup, vgroup, ogroup):
+            bg = BaguetteRack(o)
+            bg.report = r
+            bg.baguette = b if b is not None else (bg.working_directory / "baguette.pyt")
+            bg.visual = v if v is not None else (bg.working_directory / "visual.gexf")
+            bg.verbosity = verbosity
+            bg.skip_data_comparison = args.skip_data_comparison
+            bg.skip_diff_comparison = args.skip_diff_comparison
+            bg.filter_names = args.filters
+            bg.maxtime = args.maxtime
+            bg.perf = args.perf
+            bg.background_color = args.background
+            work.append(bg)
+    
+    
+    # Compile now...
+
+    from multiprocessing.pool import Pool
+    from threading import Lock, Thread
+
+    # All of this is because multiprocessing was coded with feet... Pool's async methods may freeze (deadlock maybe) on some platforms.
+
+    lock = Lock()
+    failed, timed_out, total = 0, 0, len(work)
+    def execute_single_job(P : Pool) -> bool:
+        nonlocal failed, timed_out
+        with lock:
+            if not work: 
                 return False
-            elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
-                with lock:
-                    failed += 1
-                logger.error("Got a '{}' error during the baking of '{}'.".format(br.exception.exc_type.__name__, br.report.name))
-            elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
-                with lock:
-                    timed_out += 1
-            return True
-
-        def executor(P : Pool):
-            while execute_single_job(P):
-                pass
-        
-        threads : list[Thread] = []
+            br = work.pop()
         try:
-            with Pool(args.pool, maxtasksperchild = 1) as P:
-                for _ in range(args.pool):
-                    t = Thread(target = executor, args = (P, ), daemon = True)
-                    t.start()
-                    threads.append(t)
+            br = P.apply(compile, (br, ))
+        except KeyboardInterrupt as e:
+            from traceback import TracebackException
+            br.exception = TracebackException.from_exception(e)
+        if br.exception is None or not br.suppressed:
+            br.export()
+        if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
+            return False
+        elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
+            with lock:
+                failed += 1
+            logger.error("Got a '{}' error during the baking of '{}'.".format(br.exception.exc_type.__name__, br.report.name))
+        elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
+            with lock:
+                timed_out += 1
+        return True
 
-                for t in threads:
-                    t.join()
-            
-            success = total - failed - timed_out
-            if failed and success and timed_out:
-                print("{} failed baguettes, {} took too long and {} well-baked.".format(failed, timed_out, success))
-            elif failed and success:
-                print("{} failed baguettes, {} baked correctly.".format(failed, success))
-            elif timed_out and success:
-                print("{} baguettes took too long to bake, {} baked correctly.".format(timed_out, success))
-            elif failed and timed_out:
-                print("{} baguettes are failed and the {} others took too long to bake...".format(failed, timed_out))
-            elif failed:
-                print("All {} baguettes did not bake correctly...".format(failed))
-            elif timed_out:
-                print("All {} baguettes took too long to bake...".format(timed_out))
-            elif success:
-                print("All {} are well-baked!".format(success))
-        except KeyboardInterrupt:
-            print("Exiting.")
+    def executor(P : Pool):
+        while execute_single_job(P):
+            pass
+    
+    threads : list[Thread] = []
+    try:
+        with Pool(args.pool, maxtasksperchild = 1) as P:
+            for _ in range(args.pool):
+                t = Thread(target = executor, args = (P, ), daemon = True)
+                t.start()
+                threads.append(t)
+
+            for t in threads:
+                t.join()
+        
+        success = total - failed - timed_out
+        if failed and success and timed_out:
+            print("{} failed baguettes, {} took too long and {} well-baked.".format(failed, timed_out, success))
+        elif failed and success:
+            print("{} failed baguettes, {} baked correctly.".format(failed, success))
+        elif timed_out and success:
+            print("{} baguettes took too long to bake, {} baked correctly.".format(timed_out, success))
+        elif failed and timed_out:
+            print("{} baguettes are failed and the {} others took too long to bake...".format(failed, timed_out))
+        elif failed:
+            print("All {} baguettes did not bake correctly...".format(failed))
+        elif timed_out:
+            print("All {} baguettes took too long to bake...".format(timed_out))
+        elif success:
+            print("All {} are well-baked!".format(success))
+        if failed or timed_out:
+            exit(1)
+    except KeyboardInterrupt:
+        print("Exiting.")
+        exit(1)
             
 
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `baguette_verse-1.0.0/toast.py` & `baguette_verse-1.0.5/baguette/croutons/toast.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,477 +7,481 @@
 
 
 def main():
     """
     Command line function to toast baguettes. Use -h/--help for more info.
     """
 
-    if __name__ in ("__main__", "toast"):        # One for when started with Python, the other for when started with package command...
+    import logging
 
-        import logging
-        from baguette.bakery.logger import logger, set_level
-        set_level(logging.ERROR)
-
-        import argparse
-        from os import environ
-        import pathlib
-        from typing import Literal, Iterator
-        from baguette.bakery.source.colors import Color
-        from baguette.croutons.extractor import extract
-        from baguette.croutons.metalib.utils import entries
-        from baguette.rack import BaguetteRack, TimeoutExit
-
-        parser = argparse.ArgumentParser(
-            description = 'Toasts Baguettes, picking up interesting slices as defined by MetaGraphs patterns.',
-            add_help = True,
-            conflict_handler = 'resolve',
-            epilog = """
-            Note that the format of input and outputs is quite flexible. Indeed you can :
-            give output folders for each output file, which will make all input have their output in these folders
-            - give a set of outputs for each input file, as long as they are given in the same place in the parameter sequences
-            - do the same with input folders and output folders, as long as they also come in the same order
-            - mix these options, again, as long as it has a meaning in the order they come.
-            - Note that if a given path does not exists, it is interpreted as a folder, unless the name ends with the appropriate file extension.
-            """
-            )
-
-        class PathSorter:
-
-            def __init__(self, pool : list[pathlib.Path | Literal["-"]], name : str) -> None:
-                self.pool = pool
-                self.name = name
-            
-            def __call__(self, arg : str):
-                if arg == "-":
-                    self.pool.append(arg)
-                    return
-                from glob import iglob
-                import re
-                magic_check = re.compile('([*?[])')
-                try:
-                    if magic_check.search(arg) is not None:
-                        self.pool.extend(pathlib.Path(path) for path in iglob(arg))
-                    else:
-                        self.pool.append(pathlib.Path(arg))
-                except:
-                    parser.error("invalid {} path : '{}'".format(self.name, arg))
+    from ..logger import logger, set_level
+    set_level(logging.ERROR)
 
-        inputs : list[pathlib.Path | Literal["-"]] = []
-        extracted : list[pathlib.Path | Literal["-"]] = []
-
-        def pool_size(arg : str) -> int:
-            """
-            Transforms a numeric argument in a number of process to use as a process pool.
-            It can be absolute, negative (relative to the number of CPUs) or 
-            """
-            from os import cpu_count
-            N = cpu_count()
-            if not N:
-                N = 1
+    import argparse
+    import pathlib
+    from os import environ
+    from typing import Iterator, Literal
+
+    from ..bakery.source.colors import Color
+    from ..rack import BaguetteRack, TimeoutExit
+    from .extractor import extract
+    from .metalib.utils import entries
+
+    parser = argparse.ArgumentParser(
+        description = 'Toasts Baguettes, picking up interesting slices as defined by MetaGraphs patterns.',
+        add_help = True,
+        conflict_handler = 'resolve',
+        epilog = """
+        Note that the format of input and outputs is quite flexible. Indeed you can :
+        give output folders for each output file, which will make all input have their output in these folders
+        - give a set of outputs for each input file, as long as they are given in the same place in the parameter sequences
+        - do the same with input folders and output folders, as long as they also come in the same order
+        - mix these options, again, as long as it has a meaning in the order they come.
+        - Note that if a given path does not exists, it is interpreted as a folder, unless the name ends with the appropriate file extension.
+        """
+        )
+
+    class PathSorter:
+
+        def __init__(self, pool : list[pathlib.Path | Literal["-"]], name : str) -> None:
+            self.pool = pool
+            self.name = name
+        
+        def __call__(self, arg : str):
+            if arg == "-":
+                self.pool.append(arg)
+                return
+            import re
+            from glob import iglob
+            magic_check = re.compile('([*?[])')
             try:
-                v = int(arg)
-                if v < 0:
-                    v = N - v
-                if v <= 0:
-                    parser.error("got a (too) negative value for process pool size : '{}'".format(arg))
+                if magic_check.search(arg) is not None:
+                    self.pool.extend(pathlib.Path(path) for path in iglob(arg))
+                else:
+                    self.pool.append(pathlib.Path(arg))
             except:
-                try:
-                    v = float(arg)
-                    if v <= 0:
-                        parser.error("got a negative relative process pool size : '{}'".format(arg))
-                    v = round(v * N)
-                except:
-                    parser.error("not a process pool size : '{}'".format(arg))
-            return v
+                parser.error("invalid {} path : '{}'".format(self.name, arg))
+
+    inputs : list[pathlib.Path | Literal["-"]] = []
+    extracted : list[pathlib.Path | Literal["-"]] = []
 
-        def time(arg : str) -> float:
-            from math import isnan
+    def pool_size(arg : str) -> int:
+        """
+        Transforms a numeric argument in a number of process to use as a process pool.
+        It can be absolute, negative (relative to the number of CPUs) or 
+        """
+        from os import cpu_count
+        N = cpu_count()
+        if not N:
+            N = 1
+        try:
+            v = int(arg)
+            if v < 0:
+                v = N - v
+            if v <= 0:
+                parser.error("got a (too) negative value for process pool size : '{}'".format(arg))
+        except:
             try:
                 v = float(arg)
-                if v <= 0 or isnan(v):
-                    parser.error("got a negative, null or nan maxtime")
-                return v
+                if v <= 0:
+                    parser.error("got a negative relative process pool size : '{}'".format(arg))
+                v = round(v * N)
             except:
-                parser.error("expected positive float for maxtime, got : '{}'".format(arg))
+                parser.error("not a process pool size : '{}'".format(arg))
+        return v
 
-        def paint_color(c : str) -> Color:
-            if c in dir(Color):
-                color = getattr(Color, c)
-                if not isinstance(color, Color):
-                    parser.error(f"not a valid color name : '{c}'")
-                return color
-            else:
-                # We can match colors in ALLL LANGUAGES!!!!
-                import re
-                color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
-                sep_re = r"(?:[ ,;:\|\&]+)"
-                inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
-                fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
-                if not fmatch:
-                    parser.error(f"could not understand color format : '{c}'")
-                r, g, b = fmatch.groups()
-
-                def is_float(s : str) -> bool:
-                    try:
-                        f = float(s)
-                        if not 0 <= f <= 1:
-                            return False
-                        return True
-                    except:
+    def time(arg : str) -> float:
+        from math import isnan
+        try:
+            v = float(arg)
+            if v <= 0 or isnan(v):
+                parser.error("got a negative, null or nan maxtime")
+            return v
+        except:
+            parser.error("expected positive float for maxtime, got : '{}'".format(arg))
+
+    def paint_color(c : str) -> Color:
+        if c in dir(Color):
+            color = getattr(Color, c.lower())
+            if not isinstance(color, Color):
+                parser.error(f"not a valid color name : '{c}'")
+            return color
+        else:
+            # We can match colors in ALLL LANGUAGES!!!!
+            import re
+            color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
+            sep_re = r"(?:[ ,;:\|\&]+)"
+            inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
+            fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
+            if not fmatch:
+                parser.error(f"could not understand color format : '{c}'")
+            r, g, b = fmatch.groups()
+
+            def is_float(s : str) -> bool:
+                try:
+                    f = float(s)
+                    if not 0 <= f <= 1:
                         return False
-                
-                def is_int(s : str) -> bool:
-                    try:
-                        i = int(s)
-                        if not 0 <= i <= 255:
-                            return False
-                        return True
-                    except:
+                    return True
+                except:
+                    return False
+            
+            def is_int(s : str) -> bool:
+                try:
+                    i = int(s)
+                    if not 0 <= i <= 255:
                         return False
-                
-                def is_hex(s : str) -> bool:
-                    try:
-                        i = int(s, base=16)
-                        if not 0 <= i <= 255:
-                            return False
-                        return True
-                    except:
+                    return True
+                except:
+                    return False
+            
+            def is_hex(s : str) -> bool:
+                try:
+                    i = int(s, base=16)
+                    if not 0 <= i <= 255:
                         return False
-                    
-                if all(is_float(x) for x in (r, g, b)):
-                    r, g, b = float(r), float(g), float(b)
-                elif all(is_int(x) for x in (r, g, b)):
-                    r, g, b = int(r), int(g), int(b)
-                elif all(is_hex(x) for x in (r, g, b)):
-                    r, g, b = int(r, 16), int(g, 16), int(b, 16)
-                else:
-                    parser.error(f"could not understand color format : '{c}'")
+                    return True
+                except:
+                    return False
+                
+            if all(is_float(x) for x in (r, g, b)):
+                r, g, b = float(r), float(g), float(b)
+            elif all(is_int(x) for x in (r, g, b)):
+                r, g, b = int(r), int(g), int(b)
+            elif all(is_hex(x) for x in (r, g, b)):
+                r, g, b = int(r, 16), int(g, 16), int(b, 16)
+            else:
+                parser.error(f"could not understand color format : '{c}'")
 
-                return Color(r, g, b)
+            return Color(r, g, b)
 
-        parser.add_argument("inputs", type=PathSorter(inputs, "input"), default=None, nargs="*" if ("BAGUETTE_INPUTS" in environ or "BAGUETTE_OUTPUTS" in environ) else "+", help="Baguette folders. These should contain the index file resulting from the baking. Can also be folders baguette folders. Defaults to environment variable 'BAGUETTE_INPUTS' (or 'BAGUETTE_OUTPUTS') if set.")
-        parser.add_argument("--extracted", type=PathSorter(extracted, "extracted"), default=None, action="extend", nargs="*", help="the path(s) to the output extracted match files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_EXTRACTED' or '-' if not set.")
-        parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
-        parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
-        parser.add_argument("-p", "--pattern", type=str, action="extend", choices=["-"] + entries(), nargs="+", help="The metapath names (as in the source.metalib module) to search for. Leave empty or use '-' to search for all defined metagraphs.")
-        parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
-        parser.add_argument("--paint", type=paint_color, nargs="+", default=[], help="If a color is given for painting, the matches found will be painted in the visual.gexf file. Must be a valid color name or RGB values.")
-        parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
+    parser.add_argument("inputs", type=PathSorter(inputs, "input"), default=None, nargs="*" if ("BAGUETTE_INPUTS" in environ or "BAGUETTE_OUTPUTS" in environ) else "+", help="Baguette folders. These should contain the index file resulting from the baking. Can also be folders baguette folders. Defaults to environment variable 'BAGUETTE_INPUTS' (or 'BAGUETTE_OUTPUTS') if set.")
+    parser.add_argument("--extracted", type=PathSorter(extracted, "extracted"), default=None, action="extend", nargs="*", help="the path(s) to the output extracted match files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_EXTRACTED' or '-' if not set.")
+    parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
+    parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
+    parser.add_argument("-p", "--pattern", type=str, action="extend", choices=["-"] + entries(), nargs="+", help="The metapath names (as in the source.metalib module) to search for. Leave empty or use '-' to search for all defined metagraphs.")
+    parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
+    parser.add_argument("--paint", type=paint_color, nargs="+", default=[], help="If a color is given for painting, the matches found will be painted in the visual.gexf file. Must be a valid color name or RGB values.")
+    parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
 
-        args = parser.parse_args()
+    args = parser.parse_args()
 
-        # Setting logging level
+    # Setting logging level
 
-        levels = {
-            0 : logging.ERROR,
-            1 : logging.WARNING,
-            2 : logging.INFO,
-            3 : logging.DEBUG
-        }
-        verbosity : Literal[0, 1, 2, 3] = min(3, args.verbosity)
-        set_level(levels[verbosity])
+    levels = {
+        0 : logging.ERROR,
+        1 : logging.WARNING,
+        2 : logging.INFO,
+        3 : logging.DEBUG
+    }
+    verbosity : Literal[0, 1, 2, 3] = min(3, args.verbosity)
+    set_level(levels[verbosity])
 
-        logger.info("Arguments parsed. Discovering jobs.")
+    logger.info("Arguments parsed. Discovering jobs.")
 
-        # Parsing jobs
+    # Parsing jobs
 
-        if not inputs:
+    if not inputs:
+        try:
+            inputs = [pathlib.Path(environ["BAGUETTE_INPUTS"])]
+        except KeyError:
             try:
-                inputs = [pathlib.Path(environ["BAGUETTE_INPUTS"])]
+                inputs = [pathlib.Path(environ["BAGUETTE_OUTPUTS"])]
             except KeyError:
-                try:
-                    inputs = [pathlib.Path(environ["BAGUETTE_OUTPUTS"])]
-                except KeyError:
-                    raise RuntimeError("Environment variable 'BAGUETTE_INPUTS' not found and there is no input...")
+                raise RuntimeError("Environment variable 'BAGUETTE_INPUTS' not found and there is no input...")
+        except:
+            parser.error("invalid baguette input path in environment variable : '{}'".format(environ["BAGUETTE_INPUTS"] if "BAGUETTE_INPUTS" in environ else environ["BAGUETTE_OUTPUTS"]))
+    if not extracted:
+        if "BAGUETTE_EXTRACTED" in environ:
+            try:
+                extracted = [pathlib.Path(environ["BAGUETTE_EXTRACTED"])]
             except:
-                parser.error("invalid baguette input path in environment variable : '{}'".format(environ["BAGUETTE_INPUTS"] if "BAGUETTE_INPUTS" in environ else environ["BAGUETTE_OUTPUTS"]))
-        if not extracted:
-            if "BAGUETTE_EXTRACTED" in environ:
-                try:
-                    extracted = [pathlib.Path(environ["BAGUETTE_EXTRACTED"])]
-                except:
-                    parser.error("invalid extraction path in environment variable : '{}'".format(environ["BAGUETTE_EXTRACTED"]))
-            else:
-                extracted = ["-"]
+                parser.error("invalid extraction path in environment variable : '{}'".format(environ["BAGUETTE_EXTRACTED"]))
+        else:
+            extracted = ["-"]
+    
+    if not args.pattern:
+        args.pattern = entries()
+    if "-" in args.pattern and len(args.pattern) > 1:
+        parser.error("if '-' is given for pattern, it should be the only.")
+    if "-" in args.pattern:
+        args.pattern = entries()
+
+    if args.paint:
+        if len(args.paint) == 1:
+            args.paint *= len(args.pattern)
+        if len(args.paint) != len(args.pattern):
+            parser.error("expected one color or as many colors as patterns to match.")
+    
+    class JobQueue:
+
+        """
+        These objects hold a series of grouped jobs.
+        """
+
+        def __init__(self, groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = []) -> None:
+            from copy import deepcopy
+            self.__groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = deepcopy(groups)
+            self.__last_group : list[pathlib.Path] = []
+            self.__active : bool = False
         
-        if not args.pattern:
-            args.pattern = entries()
-        if "-" in args.pattern and len(args.pattern) > 1:
-            parser.error("if '-' is given for pattern, it should be the only.")
-        if "-" in args.pattern:
-            args.pattern = entries()
-
-        if args.paint:
-            if len(args.paint) == 1:
-                args.paint *= len(args.pattern)
-            if len(args.paint) != len(args.pattern):
-                parser.error("expected one color or as many colors as patterns to match.")
+        def insert_group(self, group : list[pathlib.Path] | pathlib.Path | Literal["-"]):
+            """
+            Creates an independant work group with given content, also creating a new active group for later use.
+            """
+            if self.__active:
+                self.__groups.append(self.__last_group)
+            self.__groups.append(group)
+            self.__last_group = []
+            self.__active = False
         
-        class JobQueue:
-
+        def append_to_active_group(self, path : pathlib.Path):
+            """
+            Appends a file to the current group.
+            """
+            self.__last_group.append(path)
+            self.__active = True
+        
+        def new_group(self):
             """
-            These objects hold a series of grouped jobs.
+            Adds the active group to the queue and creates a new empty active group.
             """
+            if self.__active:
+                self.__groups.append(self.__last_group)
+            self.__last_group = []
+            self.__active = True
 
-            def __init__(self, groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = []) -> None:
-                from copy import deepcopy
-                self.__groups : list[pathlib.Path | Literal["-"] | list[pathlib.Path]] = deepcopy(groups)
-                self.__last_group : list[pathlib.Path] = []
-                self.__active : bool = False
-            
-            def insert_group(self, group : list[pathlib.Path] | pathlib.Path | Literal["-"]):
-                """
-                Creates an independant work group with given content, also creating a new active group for later use.
-                """
-                if self.__active:
-                    self.__groups.append(self.__last_group)
-                self.__groups.append(group)
-                self.__last_group = []
-                self.__active = False
-            
-            def append_to_active_group(self, path : pathlib.Path):
-                """
-                Appends a file to the current group.
-                """
-                self.__last_group.append(path)
-                self.__active = True
-            
-            def new_group(self):
-                """
-                Adds the active group to the queue and creates a new empty active group.
-                """
-                if self.__active:
-                    self.__groups.append(self.__last_group)
-                self.__last_group = []
-                self.__active = True
-
-            def finalize(self):
-                """
-                Finalizes the queue, adding the currently active group to the queue if necessary.
-                """
-                if self.__active and self.__last_group:
-                    self.__groups.append(self.__last_group)
-            
-            def __iter__(self) -> Iterator[pathlib.Path | Literal["-"] | list[pathlib.Path]]:
-                """
-                Yields all the jobs in the queue.
-                """
-                yield from self.__groups
-            
-            def __len__(self) -> int:
-                """
-                Implements len(self).
-                """
-                return len(self.__groups)
-
-            def __getitem__(self, index : int) -> pathlib.Path | Literal["-"] | list[pathlib.Path]:
-                """
-                Implements self[index].
-                """
-                return self.__groups[index]
-
-
-        input_groups : JobQueue = JobQueue()
-        extracted_groups : JobQueue = JobQueue()
-
-        def determine_type(path : pathlib.Path | Literal["-"], ext : str) -> Literal["folder", "file"]:
-            """
-            Determines if the given path should be interpreted as a folder or file path.
-            If it ends with the given extension and does not exist, it well be considered a file.
-            """
-            if path == "-":
-                return "folder"
-            elif ext and path.suffix == ext:
-                return "file"
-            if path.is_file():
-                return "file"
-            elif path.is_dir():
-                return "folder"
-            elif path.exists():
-                parser.error("given path exists and is neither a file or folder : '{}'".format(path))
-            else:
-                return "folder"
+        def finalize(self):
+            """
+            Finalizes the queue, adding the currently active group to the queue if necessary.
+            """
+            if self.__active and self.__last_group:
+                self.__groups.append(self.__last_group)
         
-        def create_name(folder : pathlib.Path) -> pathlib.Path:
+        def __iter__(self) -> Iterator[pathlib.Path | Literal["-"] | list[pathlib.Path]]:
             """
-            Given a path, this will return a (possibly) modified path that does not exist in the same folder.
+            Yields all the jobs in the queue.
             """
-            if not folder.exists():
-                return folder
-            n = 0
-            ext = folder.suffix
-            if ext:
-                sfolder = str(folder)[:-len(ext)]
-            else:
-                sfolder = str(folder)
+            yield from self.__groups
+        
+        def __len__(self) -> int:
+            """
+            Implements len(self).
+            """
+            return len(self.__groups)
+
+        def __getitem__(self, index : int) -> pathlib.Path | Literal["-"] | list[pathlib.Path]:
+            """
+            Implements self[index].
+            """
+            return self.__groups[index]
+
+
+    input_groups : JobQueue = JobQueue()
+    extracted_groups : JobQueue = JobQueue()
+
+    def determine_type(path : pathlib.Path | Literal["-"], ext : str) -> Literal["folder", "file"]:
+        """
+        Determines if the given path should be interpreted as a folder or file path.
+        If it ends with the given extension and does not exist, it well be considered a file.
+        """
+        if path == "-":
+            return "folder"
+        elif ext and path.suffix == ext:
+            return "file"
+        if path.is_file():
+            return "file"
+        elif path.is_dir():
+            return "folder"
+        elif path.exists():
+            parser.error("given path exists and is neither a file or folder : '{}'".format(path))
+        else:
+            return "folder"
+    
+    def create_name(folder : pathlib.Path) -> pathlib.Path:
+        """
+        Given a path, this will return a (possibly) modified path that does not exist in the same folder.
+        """
+        if not folder.exists():
+            return folder
+        n = 0
+        ext = folder.suffix
+        if ext:
+            sfolder = str(folder)[:-len(ext)]
+        else:
+            sfolder = str(folder)
+        new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
+        while new_folder.exists():
+            n += 1
             new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
-            while new_folder.exists():
-                n += 1
-                new_folder = pathlib.Path(sfolder + "({})".format(n) + ext)
-            return new_folder
-            
+        return new_folder
+        
 
-        for i in inputs:
-            if i == "-":
-                parser.error("cannot use automatic destination operator for input baguette folders.")
-            if determine_type(i, ".bag") == "folder":
-                if i.exists():
-                    input_groups.insert_group([p for p in i.iterdir()])
-                else:
-                    parser.error("input folder does not exist : '{}'".format(i))
+    for i in inputs:
+        if i == "-":
+            parser.error("cannot use automatic destination operator for input baguette folders.")
+        if determine_type(i, ".bag") == "folder":
+            if i.exists():
+                input_groups.insert_group([p for p in i.iterdir()])
             else:
-                if i.exists():
-                    input_groups.append_to_active_group(i)
-                else:
-                    parser.error("input baguette folder does not exist : '{}'".format(i))
-        input_groups.finalize()
-        
-        for e in extracted:
-            if determine_type(e, ".pyt") == "folder":
-                extracted_groups.insert_group(e)
+                parser.error("input folder does not exist : '{}'".format(i))
+        else:
+            if i.exists():
+                input_groups.append_to_active_group(i)
             else:
-                if e == "-":
-                    raise RuntimeError("How?")
-                extracted_groups.append_to_active_group(e)
-        extracted_groups.finalize()
-        if len(extracted_groups) == 1 and len(input_groups) > 1 and (isinstance(extracted_groups[0], pathlib.Path) or extracted_groups[0] == "-"):
-            extracted_groups = JobQueue([extracted_groups[0]] * len(input_groups))
-
-        # def printable_format(l) -> str:
-        #     return str(l) if not isinstance(l, list) else (str(l) if len(l) < 2 else "[...]")
-
-        # print("Sizes: {}, {}, {}, {}".format(len(report_groups), len(baguette_groups), len(visual_groups), len(output_groups)))
-        # print(list(printable_format(r) for r in report_groups))
-        # print(list(printable_format(b) for b in baguette_groups))
-        # print(list(printable_format(v) for v in visual_groups))
-        # print(list(printable_format(o) for o in output_groups))
-        # l1 = list(report_groups)
-        # l2 = list(baguette_groups) + [None] * (len(report_groups) - len(baguette_groups))
-        # l3 = list(visual_groups) + [None] * (len(report_groups) - len(visual_groups))
-        # l4 = list(output_groups) + [None] * (len(report_groups) - len(output_groups))
-        # for r, b, v, o in zip(l1, l2, l3, l4):
-        #     print("Work group:")
-        #     print("reports :", printable_format(r))
-        #     print("baguettes :", printable_format(b))
-        #     print("visuals :", printable_format(v))
-        #     print("outputs :", printable_format(o))
-        #     print("\n")
-
-        if len(input_groups) != len(extracted_groups):
-            parser.error("different number of work groups in inputs/outputs.")
-        
-        for i, e in zip(input_groups, extracted_groups):
-            if not isinstance(i, list):
-                raise RuntimeError("How did we get here?")
-            n = len(i)
-            if isinstance(e, list) and len(e) != n:
-                parser.error("got a work group with different numbers of inputs and outputs.")
-
-        work : list[BaguetteRack] = []
-
-        def stripname(p : pathlib.Path) -> str:
-            """
-            Returns the name of the path without the exetension if it has one.
-            """
-            ext = p.suffix
-            if ext:
-                return p.name[:-len(ext)]
-            return p.name
-
-        for igroup, egroup in zip(input_groups, extracted_groups):
-
-            if igroup == "-":
-                parser.error("cannot use automatic destination operator for input files.")
-            elif isinstance(igroup, pathlib.Path):      # Folder input
-                igroup = list(igroup.iterdir())         # Transform in file inputs
-            
-            if egroup == "-":                           # Magic destination:
-                egroup = [None for _ in igroup]         # To be determined later
-            elif isinstance(egroup, pathlib.Path):      # Folder baguette destination
-                egroup = [create_name(pathlib.Path(egroup, stripname(r) + ".pyt")) for r in igroup]       # Pre-compute the baguette paths with report names
-            
-            for i, e in zip(igroup, egroup):
-                if not (i / "index.pyt").exists():
-                    parser.error("baguette folder does not have the appropriate index file : '{}' not found.".format(i / "index.pyt"))
-                if not (i / "index.pyt").is_file():
-                    parser.error("baguette folder does not have the appropriate index file : '{}' is not a file.".format(i / "index.pyt"))
-                bg = BaguetteRack.import_from(i / "index.pyt")
-                bg.extracted = e if e is not None else bg.working_directory / "extracted.pyt"
-                bg.pattern_names = args.pattern
-                bg.maxtime = args.maxtime
-                bg.perf = args.perf
-                bg.paint_color = args.paint
-                work.append(bg)
+                parser.error("input baguette folder does not exist : '{}'".format(i))
+    input_groups.finalize()
+    
+    for e in extracted:
+        if determine_type(e, ".pyt") == "folder":
+            extracted_groups.insert_group(e)
+        else:
+            if e == "-":
+                raise RuntimeError("How?")
+            extracted_groups.append_to_active_group(e)
+    extracted_groups.finalize()
+    if len(extracted_groups) == 1 and len(input_groups) > 1 and (isinstance(extracted_groups[0], pathlib.Path) or extracted_groups[0] == "-"):
+        extracted_groups = JobQueue([extracted_groups[0]] * len(input_groups))
+
+    # def printable_format(l) -> str:
+    #     return str(l) if not isinstance(l, list) else (str(l) if len(l) < 2 else "[...]")
+
+    # print("Sizes: {}, {}, {}, {}".format(len(report_groups), len(baguette_groups), len(visual_groups), len(output_groups)))
+    # print(list(printable_format(r) for r in report_groups))
+    # print(list(printable_format(b) for b in baguette_groups))
+    # print(list(printable_format(v) for v in visual_groups))
+    # print(list(printable_format(o) for o in output_groups))
+    # l1 = list(report_groups)
+    # l2 = list(baguette_groups) + [None] * (len(report_groups) - len(baguette_groups))
+    # l3 = list(visual_groups) + [None] * (len(report_groups) - len(visual_groups))
+    # l4 = list(output_groups) + [None] * (len(report_groups) - len(output_groups))
+    # for r, b, v, o in zip(l1, l2, l3, l4):
+    #     print("Work group:")
+    #     print("reports :", printable_format(r))
+    #     print("baguettes :", printable_format(b))
+    #     print("visuals :", printable_format(v))
+    #     print("outputs :", printable_format(o))
+    #     print("\n")
+
+    if len(input_groups) != len(extracted_groups):
+        parser.error("different number of work groups in inputs/outputs.")
+    
+    for i, e in zip(input_groups, extracted_groups):
+        if not isinstance(i, list):
+            raise RuntimeError("How did we get here?")
+        n = len(i)
+        if isinstance(e, list) and len(e) != n:
+            parser.error("got a work group with different numbers of inputs and outputs.")
+
+    work : list[BaguetteRack] = []
+
+    def stripname(p : pathlib.Path) -> str:
+        """
+        Returns the name of the path without the exetension if it has one.
+        """
+        ext = p.suffix
+        if ext:
+            return p.name[:-len(ext)]
+        return p.name
+
+    for igroup, egroup in zip(input_groups, extracted_groups):
+
+        if igroup == "-":
+            parser.error("cannot use automatic destination operator for input files.")
+        elif isinstance(igroup, pathlib.Path):      # Folder input
+            igroup = list(igroup.iterdir())         # Transform in file inputs
         
+        if egroup == "-":                           # Magic destination:
+            egroup = [None for _ in igroup]         # To be determined later
+        elif isinstance(egroup, pathlib.Path):      # Folder baguette destination
+            egroup = [create_name(pathlib.Path(egroup, stripname(r) + ".pyt")) for r in igroup]       # Pre-compute the baguette paths with report names
         
-        # Extract now...
-
-        from multiprocessing.pool import Pool
-        from threading import Lock, Thread
-
-        # All of this is because multiprocessing was coded with feet... Pool's async methods may freeze (deadlock maybe) on some platforms.
-
-        lock = Lock()
-        failed, timed_out, total = 0, 0, len(work)
-        def execute_single_job(P : Pool) -> bool:
-            nonlocal failed, timed_out
-            with lock:
-                if not work: 
-                    return False
-                br = work.pop()
-            try:
-                br = P.apply(extract, (br, ))
-            except KeyboardInterrupt as e:
-                from traceback import TracebackException
-                br.exception = TracebackException.from_exception(e)
-            if br.exception is None or not br.suppressed:
-                br.export()
-            if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
+        for i, e in zip(igroup, egroup):
+            if not (i / "index.pyt").exists():
+                parser.error("baguette folder does not have the appropriate index file : '{}' not found.".format(i / "index.pyt"))
+            if not (i / "index.pyt").is_file():
+                parser.error("baguette folder does not have the appropriate index file : '{}' is not a file.".format(i / "index.pyt"))
+            bg = BaguetteRack.import_from(i / "index.pyt")
+            bg.verbosity = args.verbosity
+            bg.extracted = e if e is not None else bg.working_directory / "extracted.pyt"
+            bg.pattern_names = args.pattern
+            bg.maxtime = args.maxtime
+            bg.perf = args.perf
+            bg.paint_color = args.paint
+            work.append(bg)
+    
+    
+    # Extract now...
+
+    from multiprocessing.pool import Pool
+    from threading import Lock, Thread
+
+    # All of this is because multiprocessing was coded with feet... Pool's async methods may freeze (deadlock maybe) on some platforms.
+
+    lock = Lock()
+    failed, timed_out, total = 0, 0, len(work)
+    def execute_single_job(P : Pool) -> bool:
+        nonlocal failed, timed_out
+        with lock:
+            if not work: 
                 return False
-            elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
-                with lock:
-                    failed += 1
-                logger.error("Got a '{}' error during the toasting of '{}'.".format(br.exception.exc_type.__name__, br.working_directory.name))
-            elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
-                with lock:
-                    timed_out += 1
-            return True
-
-        def executor(P : Pool):
-            while execute_single_job(P):
-                pass
-        
-        threads : list[Thread] = []
+            br = work.pop()
         try:
-            with Pool(args.pool, maxtasksperchild = 1) as P:
-                for _ in range(args.pool):
-                    t = Thread(target = executor, args = (P, ), daemon = True)
-                    t.start()
-                    threads.append(t)
+            br = P.apply(extract, (br, ))
+        except KeyboardInterrupt as e:
+            from traceback import TracebackException
+            br.exception = TracebackException.from_exception(e)
+        if br.exception is None or not br.suppressed:
+            br.export()
+        if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
+            return False
+        elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
+            with lock:
+                failed += 1
+            logger.error("Got a '{}' error during the toasting of '{}'.".format(br.exception.exc_type.__name__, br.working_directory.name))
+        elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
+            with lock:
+                timed_out += 1
+        return True
 
-                for t in threads:
-                    t.join()
-            
-            success = total - failed - timed_out
-            if failed and success and timed_out:
-                print("{} failed toasts, {} took too long and {} well-toasted.".format(failed, timed_out, success))
-            elif failed and success:
-                print("{} failed toasts, {} toasted correctly.".format(failed, success))
-            elif timed_out and success:
-                print("{} baguettes took too long to toast, {} toasted correctly.".format(timed_out, success))
-            elif failed and timed_out:
-                print("{} toasts are failed and the {} others took too long to toast...".format(failed, timed_out))
-            elif failed:
-                print("All {} baguettes did not toast correctly...".format(failed))
-            elif timed_out:
-                print("All {} baguettes took too long to toast...".format(timed_out))
-            elif success:
-                print("All {} are well-toasted!".format(success))
-        except KeyboardInterrupt:
-            print("Exiting.")
+    def executor(P : Pool):
+        while execute_single_job(P):
+            pass
+    
+    threads : list[Thread] = []
+    try:
+        with Pool(args.pool, maxtasksperchild = 1) as P:
+            for _ in range(args.pool):
+                t = Thread(target = executor, args = (P, ), daemon = True)
+                t.start()
+                threads.append(t)
+
+            for t in threads:
+                t.join()
+        
+        success = total - failed - timed_out
+        if failed and success and timed_out:
+            print("{} failed toasts, {} took too long and {} well-toasted.".format(failed, timed_out, success))
+        elif failed and success:
+            print("{} failed toasts, {} toasted correctly.".format(failed, success))
+        elif timed_out and success:
+            print("{} baguettes took too long to toast, {} toasted correctly.".format(timed_out, success))
+        elif failed and timed_out:
+            print("{} toasts are failed and the {} others took too long to toast...".format(failed, timed_out))
+        elif failed:
+            print("All {} baguettes did not toast correctly...".format(failed))
+        elif timed_out:
+            print("All {} baguettes took too long to toast...".format(timed_out))
+        elif success:
+            print("All {} are well-toasted!".format(success))
+        if failed or timed_out:
+            exit(1)
+    except KeyboardInterrupt:
+        print("Exiting.")
+        exit(1)
             
 
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `baguette_verse-1.0.0/baguette/rack.py` & `baguette_verse-1.0.5/baguette/rack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains utilities to manage BAGUETTE data.
+This module contains utilities to manage BAGUETTE data. For more information, look at the BaguetteRack class.
 """
 
 from pathlib import Path
 from traceback import TracebackException
 from typing import Any, Literal, TypeVar
 
 from .croutons.source.metagraph import MetaGraph
@@ -23,14 +23,15 @@
 
 T = TypeVar("T", bound="BaguetteRack")
 
 class BaguetteRack:
 
     """
     Baguette racks are just a utility to organize baguettes easily.
+    They have MANY properties that can be changed to manage BAGUETTEs.
     Remember to export() them before deleting them, as this will write the index file.
     """
 
     __slots__ = {
         "__working_directory" : "The absolute path to the working directory",
         "__index" : "The path to the index file. Can be relative to __working_directory",
         "__report" : "The path to the Cuckoo report file. Can be relative to __working_directory",
@@ -79,14 +80,16 @@
         self.__skip_diff_comparison : bool = False
         self.__exception : TracebackException | None = None
         self.__baked : bool = False
         self.__toasted : bool = False
         self.__verbosity : Literal[0, 1, 2, 3] = 0
         self.__maxtime : float = float("inf")
         self.__paint_color : list[Color] | None = None
+        self.__suppressed : bool = False
+        self.__background_color : Color = Color.black
         if working_directory is not None and not isinstance(working_directory, str | Path):
             raise TypeError("Expected Path, got " + repr(type(working_directory).__name__))
         if working_directory is not None:
             self.set_defaults(Path(working_directory))
         
     def set_defaults(self, working_directory : Path):
         """
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/compiler.py` & `baguette_verse-1.0.5/baguette/bakery/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         levels = {
             0 : logging.ERROR,
             1 : logging.WARNING,
             2 : logging.INFO,
             3 : logging.DEBUG
         }
         
-        from .logger import set_level, logger
+        from ..logger import set_level, logger
         set_level(levels[rack.verbosity])
 
         logger.debug("Just change worker's verbosity level.")
 
         import os
         from pickle import dump
         from .source.build import Builder
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/logger.py` & `baguette_verse-1.0.5/baguette/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-This module adds a strong logging system to the bakery package.
+This module adds an extensive logging system to the BAGUETTE system.
 """
 
 import logging
 import sys
 
 __all__ = ["logger", "stdout_handler", "standart_formatter", "set_level", "create_log_file"]
 
 
 
 
 
 logger = logging.getLogger()
 logger.setLevel(0)
 stdout_handler = logging.StreamHandler(sys.stdout)
-standart_formatter = logging.Formatter("%(levelname)-8s : %(module)-10s : %(asctime)-24s : %(message)s")
+standart_formatter = logging.Formatter("%(levelname)-8s : %(module)-11s : %(asctime)-23s : %(message)s")
 
 logger.addHandler(stdout_handler)
 stdout_handler.setFormatter(standart_formatter)
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/build.py` & `baguette_verse-1.0.5/baguette/bakery/source/build.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+"""
+This module defines the compiler interface. Look at the Builder class.
+"""
+
 from io import IOBase
-from ..logger import logger
-from typing import Any, Dict, Iterator, TypeVar
-from .utils import *
-from .graph import Graph
-from .event import Event
-from .types.execution.entities import Process, Call
-import os
 from threading import Lock
+from typing import Any, Dict, Iterator
+
+from ...logger import logger
+from .event import Event
+from .graph import Graph
+from .types.execution.entities import Call, Process
+from .utils import chrono
+
+__all__ = ["Builder", "build", "BuildingPhase"]
 
 
 
 
 
 class BuildingPhase(Event):
     
@@ -53,22 +59,26 @@
 
 
 
 
 
 class Builder:
 
+    """
+    This class handles the building of BAGUETTEs. Just give the source file to the constructor and call build().
+    """
+
     def __init__(self, data : str | IOBase | dict) -> None:
         if isinstance(data, str):
             try:
                 data = open(data, "r")
             except:
                 raise 
         if isinstance(data, IOBase):
-            from json import load, JSONDecodeError
+            from json import JSONDecodeError, load
             try:
                 data = load(data)
                 logger.info("File loaded and structured.")
             except JSONDecodeError:
                 raise
         if not isinstance(data, dict):
             raise TypeError("Expected dict or json file, got " + repr(data.__class__.__name__))
@@ -81,32 +91,32 @@
         """
         Returns the progress (between 0.0 and 1.0) of the current task.
         """
         return self._progress / self._target
 
     def calls(self) -> Iterator[Dict[str, Any]]:
         """
-        Yields all the calls' data.
+        Yields all the calls' data from the source file.
         """
         for process in self.data["behavior"]["processes"]:
             for call in process["calls"]:
                 yield call
 
     def machines(self) -> Iterator[Dict[str, str]]:
         """
-        Yields all the machines' data.
+        Yields all the machines' data from the source file.
         """
         if "domains" not in self.data["network"]:
             return
         for machine in self.data["network"]["domains"]:
             yield machine
 
     def hostIP(self) -> str:
         """
-        Returns the host machine's IP address.
+        Returns the host machine's IP address from the source file.
         """
         import re
         expr = re.compile(r"\[cuckoo.core.resultserver\] DEBUG: Now tracking machine (\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}) for task #\d+\n")
         for line in self.data["debug"]["cuckoo"]:
             if expr.search(line):
                 match = expr.search(line)
                 if match:
@@ -131,21 +141,24 @@
                 if p.PID == pid:
                     return p.executable
         raise RuntimeError("Could not find malware process")
         
 
     @chrono
     def build(self) -> None:
+        """
+        Builds the BAGUETTE from the source file.
+        """
         BuildingPhase("Initialization", 0).throw()
-        from .graph import Graph
-        from .types.execution import Thread, Call, FollowedBy, Process, NextSignificantCall
-        from .types.network import Host, SpawnedProcess
-        from .types.filesystem.integration import declare_existing_file
-        from .graph import find_or_create
+        from .graph import Graph, find_or_create
+        from .types.execution import (Call, FollowedBy, NextSignificantCall,
+                                      Process, Thread)
         from .types.execution.utils import CallHandler
+        from .types.filesystem.integration import declare_existing_file
+        from .types.network import Host, SpawnedProcess
         self.graph = Graph()
 
         with self.graph:
 
             BuildingPhase("Network Discovery", 0).throw()
             logger.info("Identifying machines.")
 
@@ -248,42 +261,25 @@
                     new = next_call
             
             # Extra building phases
             for i in range(BuildingPhase.finalizing_steps()):
                 logger.info("Running finalization phase #{}.".format(i + 1))
                 BuildingPhase("Finalizer", i).throw()
 
-    @chrono
-    def flush_graph(self):
-
-        logger.info("Flushing graph.")
-
-        from ..source.graph import Vertex, UniqueVertex, Edge, Arrow
-        Self = TypeVar("Self", bound = type)
-
-        def subclass_iterator(cls : Self) -> Iterator[Self]:
-            for c in cls.__subclasses__():
-                yield c
-                for ci in subclass_iterator(c):
-                    yield ci
-        
-        for cls in subclass_iterator(Vertex):
-            if cls != UniqueVertex:
-                logger.debug("Adding {} {} vertices to the graph.".format(len(cls), cls.__name__))
-                cls.add_vertices_to_graph(self.graph)
-        for cls in subclass_iterator(Edge):
-            if cls != Arrow:
-                logger.debug("Adding {} {} edges to the graph.".format(len(cls), cls.__name__))
-                cls.add_edges_to_graph(self.graph)
 
     @chrono
     def process_to_vertex(self, process : dict) -> Process:
+        """
+        Given the source data of a process, creates the corresponding Process node.
+        """
         from ..source.graph import find_or_create
-        from ..source.types.execution import Process, Thread, Call, HasChildProcess, HasThread, HasFirstCall, FollowedBy
-        from ..source.types.imports import Import, HasImport
+        from ..source.types.execution import (Call, FollowedBy,
+                                              HasChildProcess, HasFirstCall,
+                                              HasThread, Process, Thread)
+        from ..source.types.imports import HasImport, Import
         p : Process
         t : Thread
         a : Call
         p, _ = find_or_create(Process, PID = process["pid"])
         p.executable = process["process_path"]
         p.command = process["command_line"]
         p.start = process["first_seen"]
@@ -323,14 +319,17 @@
         p.start = min((t.start for t in p.threads), default=p.start)
         p.stop = max((t.stop for t in p.threads), default=p.start)
 
         return p
 
     @chrono
     def api_to_vertex(self, call : dict) -> Call:
+        """
+        Given the data from the source file, builds the corresponding Call node.
+        """
         from ..source.record import record
         from ..source.types.execution import Call
         a = Call()
         a.name = call["api"]
         a.category = call["category"]
         a.stacktrace = tuple(call["stacktrace"])
         a.status = call["status"]
@@ -341,18 +340,24 @@
         return a
 
 
 
 
 
 def build(file : str | IOBase) -> "Graph":
+    """
+    Shortcut function to directly build a BAGUETTE from a source file. Returns the freshly-baked BAGUETTE.
+    """
     if isinstance(file, str):
         file = open(file, "rb")
     try:
         b = Builder(file)
     except:
         raise TypeError("Expected file, got " + repr(file.__class__.__name__))
     b.build()
     return b.graph
 
 
-__all__ = ["Builder", "build"]
+
+
+
+del IOBase, Lock, Any, Dict, Iterator, logger, Event, Graph, Call, Process, chrono
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/colors.py` & `baguette_verse-1.0.5/baguette/bakery/source/colors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
-This module defines colors to be used for graphs.
+This module defines colors to be used for graphs. Look at the Color class.
 """
 
 from typing import Any, Iterable, Iterator, Tuple, Union
+from Viper.frozendict import frozendict
 
-__all__ = ["chart", "Color"]
+__all__ = ["Color"]
 
 
 
 
 
 __chart_init = {
     'black' : (0.0, 0.0, 0.0),
@@ -148,15 +149,15 @@
     'snow' : (1.0, 0.9803921568627451, 0.9803921568627451),
     'yellow' : (1.0, 1.0, 0.0),
     'lightyellow' : (1.0, 1.0, 0.8784313725490196),
     'ivory' : (1.0, 1.0, 0.9411764705882353),
     'white' : (1.0, 1.0, 1.0)
 }
 
-chart : dict[str, "Color"] = {}
+chart : frozendict[str, "Color"]
 
 
 
 
 
 class ColorType(type):
 
@@ -167,46 +168,60 @@
     def __getattribute__(self, name: str) -> "Color":
         """
         Implements getattr(Color, name).
         """
         try:
             return super().__getattribute__(name)
         except AttributeError:
-            if name in chart:
-                return chart[name]
+            if name in self.chart:
+                return self.chart[name]
             else:
                 raise AttributeError("type object " + repr(super().__getattribute__("__name__")) + " has no attribute " + repr(name))
             
     def __dir__(self) -> list[str]:
         """
         Implements dir(Color).
         """
-        return list(super().__dir__()) + list(chart)
-
+        return list(super().__dir__()) + list(self.chart)
+    
+    @property
+    def names(self) -> list[str]:
+        """
+        Returns the list of available color names.
+        """
+        return list(self.chart)
+    
+    chart : frozendict[str, "Color"] = frozendict()
+    inverted_chart : frozendict[tuple[int, int, int], str] = frozendict()
 
 
 
 
 class Color(metaclass = ColorType):
 
     """
     This class is used to describe colors.
+    They can be defined using RGB values (three float (0:1) or three int [0:255]) or using the color name:
+    >>> Color(1.0, 1.0, 1.0) is Color.white
+    True
+    
+    Use Color.names to list all the available color names.
     """
 
     __slots__ = ("R", "G", "B")
 
     def __new__(cls: type, r : int | float, g : int | float, b : int | float) -> "Color":
         if not isinstance(r, int | float) or not isinstance(g, int | float) or not isinstance(b, int | float):
             raise TypeError("Expected three int or float, got " + repr(r.__class__.__name__) + ", " + repr(g.__class__.__name__) + " and " + repr(b.__class__.__name__))
         if isinstance(r, int) and isinstance(g, int) and isinstance(b, int):
             r, g, b = r / 255, g / 255, b / 255
         r, g, b = float(r), float(g), float(b)
-        for name, value in chart.items():
-            if isinstance(value, Color) and (value.R, value.G, value.B) == (r, g, b):
-                return value
+        R, G, B = round(r * 255), round(g * 255), round(b * 255)
+        if (R, G, B) in Color.inverted_chart:
+            return Color.chart[Color.inverted_chart[R, G, B]]
         return super().__new__(cls)
 
 
     def __init__(self, r : int | float, g : int | float, b : int | float) -> None:
         if isinstance(r, int) and isinstance(g, int) and isinstance(b, int):
             r, g, b = r / 255, g / 255, b / 255
         r, g, b = float(r), float(g), float(b)
@@ -215,17 +230,16 @@
         self.R, self.G, self.B = r, g, b
     
 
     def __str__(self) -> str:
         """
         Implements str(self).
         """
-        for name, value in chart.items():
-            if Color(value.R, value.G, value.B) == self:
-                return "Color." + name
+        if self.to_int() in Color.inverted_chart:
+            return "Color." + Color.inverted_chart[self.to_int()]
         return "Color" + str((self.R, self.G, self.B))
     
 
     __repr__ = __str__
     
 
     def __eq__(self, o: object) -> bool:
@@ -364,10 +378,11 @@
         return Color(min(1.0, max(0.0, R)), min(1.0, max(0.0, G)), min(1.0, max(0.0, B)))
 
 
 
 
 
 # Convert color vectors of the __chart_init to Color objects in the real chart
-chart.update((name, Color(*value)) for name, value in __chart_init.items())
+ColorType.chart = frozendict((name, Color(*value)) for name, value in __chart_init.items())
+ColorType.inverted_chart = frozendict((color.to_int(), name) for name, color in ColorType.chart.items())
 
-del Any, Tuple, Union, ColorType, Iterable, Iterator, __chart_init
+del Any, Tuple, Union, ColorType, Iterable, Iterator, __chart_init, frozendict
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/config.py` & `baguette_verse-1.0.5/baguette/bakery/source/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains configuration objects for execution graphs.
+This module contains configuration objects for execution graphs. Look at the Setting class.
 """
 
 from abc import abstractmethod
 from typing import Any, Generic, Self, TypeVar
 from .colors import Color
 from Viper.meta.decorators import hybridmethod, staticproperty
 
@@ -14,22 +14,22 @@
 
 
 T = TypeVar("T")
 
 class Setting(Generic[T]):
 
     """
-    Just a class to hold settings for BAGUETTE. Cannot be used as such, you need to specialize it as a generic class of the type of object the setting will hold:
+    Just a class to hold settings for BAGUETTE. Cannot be used as such, you need to specialize it similarly to generic class of the type of object the setting will hold:
 
     >>> s = Setting(Color.white)
     ValueError: Cannot instanciate unspecialized Setting class
-    >>> ColorMap = Setting[Color]
-    >>> s = ColorMap(Color.white)
+    >>> ColorSetting = Setting[Color]
+    >>> s = ColorSetting(Color.white)
     >>> class A:
-    ...     x = ColorMap(Color.red)
+    ...     x = ColorSetting(Color.red)
     ... 
     >>> a = A()
     >>> a.x
     Color.red
     >>> a.x = 1
     TypeError: Expected Color, got 'int'
     >>> a.x = Color.yellow
@@ -37,22 +37,22 @@
     Color.yellow
     >>> A.x         # Note that settings are actually affected at a class level.
     Color.yellow
     >>> del a.x
     >>> a.x
     Color.red
     
-    The advantage of Settings over simple properties is that references are hold at the class level to all the settings declared in all class namespaces:
+    The advantage of Settings over simple properties is that references are held at the class level to all the settings declared in all classes namespaces:
 
     >>> Setting.list()
     {(<class '__main__.A'>, 'x'): <baguette.bakery.source.config.Setting[Color] object at 0x0000016345399590>}
-    >>> IntMap = Setting[int]
-    >>> IntMap.list()
+    >>> IntSetting = Setting[int]
+    >>> IntSetting.list()
     {}
-    >>> ColorMap.list()
+    >>> ColorSetting.list()
     {(<class '__main__.A'>, 'x'): <baguette.bakery.source.config.Setting[Color] object at 0x0000016345399590>}
     >>> a.x = Color.yellow
     >>> Setting.list()[A, "x"].value = Color.black
     >>> a.x
     Color.black
     """
 
@@ -93,15 +93,15 @@
         The type of value expected for this Setting.
         """
         raise NotImplementedError
 
     @property
     def value(self) -> T:
         """
-        The value that this Setting currently points to.
+        The value that this Setting currently holds.
         """
         return self.__current
     
     @value.setter
     def value(self, value : T):
         if not isinstance(value, self.cls):
             raise TypeError(f"Expected {self.cls.__name__}, got '{type(value).__name__}'")
@@ -152,15 +152,15 @@
             raise ValueError("Expected subclass of the class this setting is registered in.")
         cp = type(self)(self.__default)
         setattr(cls, name, cp)
         cp.__set_name__(cls, name)
         return cp
 
     def __set_name__(self, owner : type, name : str):
-        from ..logger import logger
+        from ...logger import logger
         logger.debug(f"New '{self.cls.__name__}' setting registered for class '{owner.__name__}' with name '{name}'.")
         Setting.__per_class[(owner, name)] = self
 
     def __get__(self, instance : Any, owner : type | None = None) -> T:
         return self.__current
     
     def __set__(self, instance : Any, value : T):
@@ -185,15 +185,15 @@
 
 
 
 def ajust_for_background_color(background_color : Color, tolerance : float = 0.15):
     """
     This function will change the values of the Color Settings to ajust those that would not be visible for a background of the given color.
     """
-    from ..logger import logger
+    from ...logger import logger
 
     for (cls, name), color_setting in ColorSetting.list().items():
         if sum((a - b) ** 2 for a, b in zip(color_setting.value, background_color)) ** 0.5 < tolerance:
             logger.info(f"Changing color setting '{cls.__name__}.{name}'.")
             color_setting.value = color_setting.value.negative_to(background_color)
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/event.py` & `baguette_verse-1.0.5/baguette/bakery/source/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 The event library. An event can be created by anyone, specifying any kind of data. Anybody can wait for any type of events.
+Look at the Event class.
 """
 
 from typing import Callable, Generic, Type, TypeVar
 from Viper.better_threading import Future
 from threading import Lock
 from .utils import chrono
 
@@ -15,14 +16,26 @@
 
 T = TypeVar("T", bound="Event")
 
 class Event(Generic[T]):
 
     """
     The base event class. Use its static methods to react to Events created.
+    To wait for an event of a specifice event class, just use:
+    >>> cls.wait()      # Returns the cls instance that was thrown.
+    To throw an event, use:
+    >>> event = cls()
+    >>> event.throw()
+
+    The event system works with class hierarchy:
+    >>> class MyEvent(Event):
+    ...     pass
+    ... 
+    >>> MyEvent.wait()  # Only waits for events that satisfy isinstance(event, MyEvent).
+    >>> Event.wait()    # Waits for any kind of event.
     """
 
     __waiting : dict[Type[T], list[Future[T]]] = {}
     __callbacks : dict[Type[T], list[Callable[[T], None]]] = {}
     __locks : dict[Type[T], Lock] = {}
 
     __slots__ = {}
@@ -35,15 +48,15 @@
 
     @chrono
     def throw(self : T) -> bool:
         """
         Triggers the Event. Everyone waiting for it will be awaken, and corresponding callbacks will be called.
         Returns True if anybody reacted to the event. Returns False otherwise.
         """
-        from ..logger import logger
+        from ...logger import logger
 
         def raise_multiple_exceptions(exceptions : list[BaseException]):
             """
             Raises all the exceptions in the given list, in order.
             """
             if not exceptions:
                 return
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/filters.py` & `baguette_verse-1.0.5/baguette/bakery/source/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This module defines basic graph filters. Use them to reduce the size of the graph by only keeping specific edges.
-To be used with compile.py, all custom Filters must be defined in this file!
+To be used with 'bake', all custom Filters must be defined in this file!
 """
 
 from typing import Callable, Iterable
 from .graph import Edge, Vertex, Graph
 from Viper.meta.iterable import InstanceReferencingClass
 from .utils import chrono, System
 from .types.registry import Key, KeyEntry, Handle
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/graph.py` & `baguette_verse-1.0.5/baguette/bakery/source/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-This module defines all graph-related objects.
+This module defines all graph-related base classes.
+Look at the classes Vertex, Edge, Arrow and Graph.
+Vertex, Edge and Arrow classes are heavily subclasses in BAGUETTE. Look at package 'baguette.bakery.source.types' to know more.
 """
 
 from threading import RLock, Thread
 from typing import Any, Callable, Iterable, Iterator, Optional, TypeVar, Union
 from .colors import Color
 from .config import ColorSetting, SizeSetting, SwitchSetting, WeightSetting
 from Viper.meta.iterable import InstanceReferencingClass
@@ -486,15 +488,15 @@
     
         
 
 
 class Arrow(Edge):
 
     """
-    An arrow for a graph. Links two vertices together.
+    An arrow (directed) for a graph. Links two vertices together.
     """
     
     def __repr__(self) -> str:
         """
         Implements repr(self).
         """
         return "arrow(" + repr(self.source) + ", " + repr(self.destination) + ")"
@@ -544,15 +546,24 @@
 
 
 
 class Graph:
 
     """
     A graph class. Add starting vertices and use explore() to complete the graph.
-    Graph can be used in context managers to append all Vertices and Edges created in the current thread to the context Graph.
+    Graph can be used in context managers to append all Vertices and Edges created in the current thread to the context Graph:
+    >>> G = Graph()
+    >>> with G:
+    ...     u = Vertex()
+    ...     e = Edge(u, u)
+    ... 
+    >>> u in G.vertices:
+    True
+    >>> e in G.edges:
+    True
     """
 
     __slots__ = {
         "vertices" : "The set of vertices in this graph",
         "edges" : "The set of edges in this graph",
         "data" : "A dictionary holding additional data for this graph"
     }
@@ -651,14 +662,25 @@
 
     def __len__(self) -> int:
         """
         Implements len(self). Returns the number of vertices.
         """
         return len(self.vertices)
     
+    def __contains__(self, vertex_or_edge : Vertex | Edge) -> bool:
+        """
+        Implements vertex_or_edge in self. Returns True if the given Vertex or Edge is in the Graph.
+        """
+        if isinstance(vertex_or_edge, Vertex):
+            return vertex_or_edge in self.vertices
+        elif isinstance(vertex_or_edge, Edge):
+            return vertex_or_edge in self.edges
+        else:
+            raise TypeError(f"Expected Vertex or Edge, got '{type(vertex_or_edge).__name__}'")
+    
     @property
     def n(self) -> int:
         """
         The number of vertices.
         """
         return len(self)
     
@@ -791,15 +813,15 @@
     #         e.source = translation[u]
     #         e.destination = translation[v]
     #         e.write()
     #     return cp
 
     def export(self, file : str, *, subgraph_supported : bool = False) -> None:
         """
-        Writes this graph under the GEXF format into file.
+        Writes this graph under the GEXF format into given file.
         """
         # List of possible attributes to include in visuals :
         # Node Size : proportional to radius! not surface area!
         # Color : R, G, B
         # Node Shape : Any of "disc", "square", "triangle" or "diamond"
         # Edge Thickness : same as weight?
         # Edge Shape : Any of "solid", "dotted", "dashed" or "double"
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/record.py` & `baguette_verse-1.0.5/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/utils.py` & `baguette_verse-1.0.5/baguette/bakery/source/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,31 @@
 
 
 
 
 
 @cache
 def extract_pickle_slots(o : type[Vertex | Edge]) -> Set[str]:
+    """
+    Internal function for pickling complex objects.
+    """
     s : set[str]
     if not hasattr(o, "__pickle_slots__"):
         s = set()
     else:
         s = set(o.__pickle_slots__) # type: ignore
     for b in s:
         if not isinstance(b, str):
             raise RuntimeError("__pickle_slots__ should only contain str, got a " + repr(type(b).__name__))
     return s.union(*[extract_pickle_slots(b) for b in o.__bases__])
 
 
 def path_factory(path : str) -> pathlib.PurePath:
     """
-    Returns the correct path factory class for the given graph (Either WindowsPurePath or PosixPurePath).
+    Returns the correct path factory class for the given graph (either WindowsPurePath or PosixPurePath).
     """
     from pathlib import PurePosixPath, PureWindowsPath
 
     from .graph import Graph
     platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
     if "windows" in platform:
         return PureWindowsPath(path)
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from functools import cache
 from types import ModuleType
 from .. import types as type_package
 from ..graph import Edge, Vertex
 
-__all__ = ["types", "relations", "relation_types"]
+__all__ = ["types", "relations", "relation_types", "baguette_structure"]
 
 
 
 
 
 @cache
 def types(mod : ModuleType = type_package) -> set[type[Vertex]]:
@@ -20,15 +20,15 @@
     """
     from ..graph import Vertex
     from types import ModuleType
 
     if not isinstance(mod, ModuleType):
         raise TypeError("Expected module or package, got " + repr(type(mod).__name__))
 
-    type_set = set()
+    type_set : set[type[Vertex]] = set()
     package_name = mod.__name__
 
     for name in dir(mod):
         value = getattr(mod, name)
         if isinstance(value, type) and issubclass(value, Vertex):
             type_set.add(value)
         elif isinstance(value, ModuleType):
@@ -49,25 +49,25 @@
     """
     from ..graph import Edge
     from types import ModuleType
 
     if not isinstance(mod, ModuleType):
         raise TypeError("Expected module or package, got " + repr(type(mod).__name__))
 
-    type_set = set()
+    type_set : set[type[Edge]] = set()
     package_name = mod.__name__
 
     for name in dir(mod):
         value = getattr(mod, name)
         if isinstance(value, type) and issubclass(value, Edge):
             type_set.add(value)
         elif isinstance(value, ModuleType):
             name = value.__name__.rpartition(".")[0]
             if name == package_name:
-                type_set.update(types(value))
+                type_set.update(relations(value))
     
     return type_set
 
 
 
 
 
@@ -77,17 +77,28 @@
     Given an Edge or Arrow subclass, gives the best type hints for the source and destination vertices.
     Defaults to (Vertex, Vertex) when no annotations exist.
     """
     from typing import get_type_hints
     from ..graph import Edge, Vertex
 
     if not isinstance(edge_class, type) or not issubclass(edge_class, Edge):
-        raise TypeError("Expected Edge subclass, got " + repr(type(edge_class).__name__))
+        raise TypeError("Expected Edge subclass, got " + repr(edge_class))
 
     hints = get_type_hints(edge_class)
     return hints.get("source", Vertex), hints.get("destination", Vertex)
+
+
+
+
+
+def baguette_structure():
+    """
+    A dynamic clone of 'baguette.croutons.source.utils.baguette_structure'.
+    """
+    from ....croutons.source.utils import baguette_structure
+    return baguette_structure()
     
 
 
 
 
 del cache, ModuleType, type_package, Edge, Vertex
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/data/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from typing import Iterator, Optional
 
-from ....logger import logger
+from .....logger import logger
 from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 from ...utils import chrono
 from ..filesystem.entities import File, Handle
 from ..network.entities import Connection, Socket
 from .utils import IOOperation
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/data/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...build import BuildingPhase
 from ...utils import chrono
 from ..filesystem.entities import File, Handle
 from ..network.entities import Connection, Socket
 from . import entities, relations
 
 __all__ = ["register_read_operation", "register_write_operation"]
@@ -87,15 +87,15 @@
     """
     When called with the right finalizing phase event, will cause all Diff nodes to compute their data attributes.
     """
     from time import time_ns
 
     from Viper.format import duration
 
-    from ....logger import logger
+    from .....logger import logger
     from ...config import CompilationParameters
     from .entities import Diff
     if e.major == "Finalizer" and e.minor == __N_diff_comparison_phase:
         logger.debug("Finalizing{} {} Diff nodes.".format(" and comparing" if not CompilationParameters.SkipLevenshteinForDiffNodes else "",len(Diff)))
         n = len(Diff)
         t0 = time_ns()
         t = t0
@@ -108,15 +108,15 @@
 @chrono
 def normalize_diff_nodes(e : BuildingPhase):
     """
     When called with the right finalizing phase event, will cause all Diff nodes to compare their diff file sizes and change their size accordingly.
     """
     from typing import Type
 
-    from ....logger import logger
+    from .....logger import logger
     from ...colors import Color
     from ...graph import Vertex
     from ..filesystem import File, Handle
     from ..network import Connection, Socket
     from .entities import Diff
 
     def project_range(x : float, sa : float, sb : float, da : float, db : float) -> float:
@@ -153,15 +153,15 @@
             d.color = Color.linear((Diff.diff_low_entropy_color, Diff.diff_high_entropy_color), (1 - d.glob_entropy / 8, d.glob_entropy / 8))
 
 @chrono
 def fuse_diff_nodes(e : BuildingPhase):
     """
     When called with the right finalizing phase event, will cause all identical Diff nodes to be merged with their size increasing.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Graph
     from .entities import Diff
 
     groups : dict[Diff, int] = {}
 
     def merge(u : Diff, v : Diff):
         """
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/data/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...config import WeightSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..filesystem.entities import File, Handle
 from ..network.entities import Connection, Socket
 from .entities import Data, Diff
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/execution/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from typing import Optional
 
-from ....logger import logger
+from .....logger import logger
 from ...colors import Color
 from ...config import ColorSetting, SizeSetting
 from ...graph import UniqueVertex, Vertex
 from ...utils import chrono
 
 __all__ = ["Process", "Thread", "Call"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/execution/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...build import BuildingPhase
 from ...utils import chrono
 from . import entities, relations
 from .utils import CallHandler
 
 __all__ = []
 
@@ -17,15 +17,15 @@
 logger.info("Loading integrations from {} library.".format(__name__.rpartition(".")[0].rpartition(".")[2]))
 
 @chrono
 def integrate_thread_creation(c : entities.Call):
     """
     Links a Thread vertex to the Call vertex (from another thread) that created it.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import find_or_create
     from .entities import Thread
     from .relations import InjectedThread, StartedThread
     if c.arguments.thread_identifier != 0:      # Should indicate that the call failed
         logger.debug("New thread detected.")
         t : Thread
         t, ok = find_or_create(Thread, TID = c.arguments.thread_identifier)
@@ -37,15 +37,15 @@
             InjectedThread(p, t)
 
 @chrono
 def integrate_process_creation(c : entities.Call):
     """
     Links a Process vertex to the Call vertex (from another process) that created it.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import find_or_create
     from .entities import Process
     from .relations import StartedProcess
     if c.arguments.process_identifier != 0:
         logger.debug("New process detected.")
         p : Process
         p, ok = find_or_create(Process, PID = c.arguments.process_identifier)
@@ -69,15 +69,15 @@
 __N_phase = BuildingPhase.request_finalizing_phase()
 
 @chrono
 def remove_cuckoo_phantom_processes(ev : BuildingPhase):
     """
     When called with the right finalizing phase event, will cause Process nodes which represent Cuckoo process (inital processes with no info available) to be erased.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Graph
     from ..network import Host, SpawnedProcess
     from .entities import Process
     if ev.major == "Finalizer" and ev.minor == __N_phase:
         logger.debug("Erasing Cuckoo phantom processes.")
         n = 0
         h = Host.current
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/execution/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...config import SwitchSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..filesystem.entities import Directory, File
 from .entities import Call, Process, Thread
 
 __all__ = ["HasChildProcess", "UsesAsArgument", "Runs", "HasThread", "HasFirstCall", "FollowedBy", "NextSignificantCall", "StartedThread", "InjectedThread", "StartedProcess"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 import pathlib
 
-from ....logger import logger
+from .....logger import logger
 from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["File", "Directory", "Handle"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
 from typing import Type
 
-from ....logger import logger
+from .....logger import logger
 from ...build import BuildingPhase
 from ...event import Event
 from ...graph import Arrow, Edge
 from ...utils import chrono
 from ..execution.entities import Call
 from ..execution.utils import CallHandler
 from . import entities, relations
@@ -73,15 +73,15 @@
 
 
 @chrono
 def integrate_file_creation(c : Call):
     """
     Creates a File/Directory vertex if it does not exists.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import File, Handle
     from .relations import CreatesFile, HasHandle, UsesFile
     if c.status == 1:
         logger.debug("File created.")
         if c.arguments.file_handle in __inverted_handles:
             h = __inverted_handles[c.arguments.file_handle]
         else:
@@ -124,15 +124,15 @@
         # if "FILE_READ"
 
 @chrono
 def integrate_file_opening(c : Call):
     """
     Creates an File/Directory vertex.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import File, Handle
     from .relations import HasHandle, Opens, UsesFile
     if c.status == 1:
         logger.debug("File opened.")
         if c.arguments.file_handle in __inverted_handles:
             h = __inverted_handles[c.arguments.file_handle]
         else:
@@ -159,28 +159,28 @@
         NewFile(f).throw()
 
 @chrono
 def integrate_file_closing(c : Call):
     """
     Connects a closing system call to the corresponding Handle.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .relations import Closes
     if c.status == 1 and c.arguments.handle in __inverted_handles:
         logger.debug("File closed.")
         h = __inverted_handles.pop(c.arguments.handle)
         __active_handles.pop(h)
         Closes(c, h)
 
 @chrono
 def integrate_file_reading(c : Call):
     """
     Creates a Data vertex, and links it to the Handle and Call vertices.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ..data import Data
     from ..data.integration import register_read_operation
     from .entities import File
     from .relations import Conveys, Reads
     if c.status == 1 and c.arguments.file_handle in __inverted_handles:
         logger.debug("Reading from file.")
         h = __inverted_handles[c.arguments.file_handle]
@@ -194,15 +194,15 @@
             register_read_operation(f, h, d.data, c.arguments.offset)
 
 @chrono
 def integrate_file_writing(c : Call):
     """
     Creates a Data vertex, and links it to the Handle and Call vertices.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ..data import Data
     from ..data.integration import register_write_operation
     from .entities import File
     from .relations import Conveys, Writes
     if c.status == 1 and c.arguments.file_handle in __inverted_handles:
         logger.debug("Writing to file.")
         h = __inverted_handles[c.arguments.file_handle]
@@ -216,15 +216,15 @@
             register_write_operation(f, h, d.data, c.arguments.offset)
     
 @chrono
 def integrate_file_copying(c : Call):
     """
     Creates a File vertex, and links it to the original file it was copied from.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import File
     from .relations import IsCopyiedInto
     if c.status == 1:
         logger.debug("Copying file.")
         if c.arguments.oldfilepath in __existing_files:
             fs = __existing_files[c.arguments.oldfilepath]
         else:
@@ -246,15 +246,15 @@
             __all_files[c.arguments.newfilepath].append(fd)
             NewFile(fd).throw()
         IsCopyiedInto(fs, fd)
 
 @chrono
 def integrate_file_deleting(c : Call):
     # You need to make it possible to have multiple times the same file name...
-    from ....logger import logger
+    from .....logger import logger
     from .entities import File
     if c.status == 1:
         logger.debug("Deleting file.")
         if c.arguments.filepath not in __existing_files:
             f = File()
             f.path = c.arguments.filepath
             __existing_files[c.arguments.filepath] = f
@@ -302,15 +302,15 @@
     """
     When all File nodes have been created, this will replace those which are actually directories into Directory nodes and build the file system tree.
     """
     # TODO : You will need to make a version of this which keeps track of when files/directories exists to make sure your file system tree is indeed a tree !!!
     from pathlib import PurePath
     from typing import Type
 
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Edge, Graph, find_or_create
     from ..execution import Runs
     from ..network import Host
     from .entities import Directory, File
     from .relations import Contains, HasDrive
 
     disappearing : set[Type[Edge]] = {Runs}
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/filesystem/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...graph import Arrow, Edge
 from ..data.entities import Data
 from ..execution.entities import Call, Process
 from ..network.entities import Host
 from .entities import Directory, File, Handle
 
 __all__ = ["UsesFile", "UsesDirectory", "Opens", "Closes", "CreatesFile", "CreatesDirectory", "DeletesFile", "DeletesDirectory", "Reads", "Writes", "Conveys", "HasDrive", "HasHandle", "Contains", "IsCopyiedInto"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/imports/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Import"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/imports/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...utils import chrono
 from ..filesystem.integration import NewFile
 from . import entities, relations
 
 __all__ = []
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/imports/relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...graph import Edge
 from ..execution.entities import Process
 from ..filesystem.entities import File
 from .entities import *
 
 __all__ = ["HasImport", "IsFile"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/network/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from collections import defaultdict
 from typing import Optional
 
 from Viper.meta.decorators import staticproperty
 
-from ....logger import logger
+from .....logger import logger
 from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Connection", "Socket", "Host"]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/network/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...utils import chrono
 from ..execution.entities import Call
 from ..execution.utils import CallHandler
 from . import entities, relations
 
 __all__ = []
 
@@ -21,15 +21,15 @@
 __inverted_handles : dict[int, entities.Socket] = {}
 
 @chrono
 def integrate_socket_creation(c : Call):
     """
     Creates a Socket vertex and links it to the call that created it.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import Socket
     from .relations import CreatesSocket, HasSocket
     if c.status == 1:
         logger.debug("Socket created.")
         s = Socket()
         __active_handles[s] = c.arguments.socket
         __inverted_handles[c.arguments.socket] = s
@@ -42,15 +42,15 @@
         HasSocket(c.thread.process, s)
 
 @chrono
 def integrate_socket_binding(c : Call):
     """
     Creates a Connection vertex and binds it to a local address.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import find_or_create
     from .entities import Connection, Host
     from .relations import Binds, Communicates, HasConnection
     if c.status == 1:
         logger.debug("Socket bound.")
         l = Connection()
         if c.arguments.socket in __inverted_handles:
@@ -69,15 +69,15 @@
             logger.error("I don't know how to handle this type of address:\n{}".format(s))
 
 @chrono
 def integrate_socket_connection(c : Call):
     """
     Sets the remote address of a connection.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import find_or_create
     from .entities import Connection, Host
     from .relations import Communicates, Connects, HasConnection
     if c.status == 1:
         logger.debug("Socket connected.")
         try:
             sock = c.arguments.socket
@@ -106,15 +106,15 @@
 
 
 @chrono
 def integrate_socket_listening(c : Call):
     """
     Sets the socket in listening mode.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .relations import ListensOn
     if c.status == 1:
         logger.debug("Socket listening.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
         else:
             logger.warning("Listening from non-existing socket.")
@@ -122,15 +122,15 @@
         ListensOn(c, s)
 
 @chrono
 def integrate_socket_accepting(c : Call):
     """
     Sets a connection remote address through an accept system call. Also creates a new socket object.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import find_or_create
     from .entities import Connection, Host, Socket
     from .relations import Accepts, Communicates, Duplicates, HasConnection
     if c.status == 1:
         logger.debug("Socket accepting connection.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
@@ -158,15 +158,15 @@
             l1.dest = b.dest
 
 @chrono
 def integrate_socket_close(c : Call):
     """
     Closes a socket and the connection linked to it.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .relations import Closes, CloseSocket
     if c.status == 1:
         logger.debug("Closing socket.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
         else:
             logger.warning("Closing non-existing socket.")
@@ -181,15 +181,15 @@
             logger.warning("Closing down unbound socket...")
 
 @chrono
 def integrate_socket_shutdown(c : Call):
     """
     Closes a connection.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .relations import Shutdown
     if c.status == 1:
         logger.debug("Closing socket.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
         else:
             logger.warning("Shuting down non-existing socket")
@@ -201,15 +201,15 @@
             logger.warning("Shuting down unbound socket...")
 
 @chrono
 def integrate_socket_send(c : Call):
     """
     Sends data through a connection.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ..data import Data
     from ..data.integration import register_write_operation
     from .relations import Conveys, Sends
     if c.status == 1:
         logger.debug("Sending data.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
@@ -229,15 +229,15 @@
             register_write_operation(l, s, c.arguments.buffer)
 
 @chrono
 def integrate_socket_recv(c : Call):
     """
     Receives data through a connection.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ..data import Data
     from ..data.integration import register_read_operation
     from .relations import Conveys, Receives
     if c.status == 1:
         logger.debug("Receiving data.")
         if c.arguments.socket in __inverted_handles:
             s = __inverted_handles[c.arguments.socket]
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/network/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...config import SwitchSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..data.entities import Data
 from ..execution.entities import Call, Process
 from .entities import Connection, Host, Socket
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/registry/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from abc import abstractmethod
 from types import NoneType
 from typing import Any, Callable, Generic, Optional, TypeVar
 
-from ....logger import logger
+from .....logger import logger
 from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Key", "KeyEntry", "Handle"]
 
 
@@ -56,15 +56,15 @@
             raise TypeError("Expected str, got " + repr(type(value).__name__))
         if "\\" in value:
             raise ValueError("'\\' not permitted in a registry key name")
         if len(value) > 255:
             raise ValueError("Key name is too long to be allowed by registry")
         self.__name = value.lower().title().replace("\x00", "\uFFFD")
         if not self.printable:
-            from ....logger import logger
+            from .....logger import logger
             from ...config import ColorSetting
             logger.info("Got an unprintable registry key.")
             self.color = self.unprintable_key_color
     
     @property
     def path(self) -> str:
         """
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/registry/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains integration protocols for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...build import BuildingPhase
 from ...utils import chrono
 from ..execution.entities import Call
 from ..execution.utils import CallHandler
 from . import entities, relations
 
 __all__ = []
@@ -81,15 +81,15 @@
 
 
 @chrono
 def integrate_key_opening(c : Call):
     """
     Creates a new Key node if necessary when a key is opened.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import Handle
     from .relations import HasHandle, UsesKey
     if c.status == 1:
         logger.debug("Opening registry key.")
         if c.arguments.regkey.lower() in __existing_keys:
             k = __existing_keys[c.arguments.regkey.lower()]
         else:
@@ -104,15 +104,15 @@
         __active_handles[h] = c.arguments.key_handle.lower()
         
 @chrono
 def integrate_key_enumeration(c : Call):
     """
     Finds the enumerated Key and sub-Key. Creates the sub-Key if it does not exist. Links the sub-Key to the Handle.
     """
-    from ....logger import logger
+    from .....logger import logger
     from .entities import Key
     from .relations import Discovered
     if c.status == 1:
         logger.debug("Enumerating from registry key.")
         k : Key
         sk : Key
         if c.arguments.key_handle.lower() not in __inverted_handles:
@@ -127,29 +127,29 @@
         Discovered(h, sk)
 
 @chrono
 def integrate_key_closing(c : Call):
     """
     Closes a Handle associated with a Key.
     """
-    from ....logger import logger
+    from .....logger import logger
     if c.status == 1:
         logger.debug("Closing key handle.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to close unseen key handle.")
             return
         h = __inverted_handles.pop(c.arguments.key_handle.lower())
         __active_handles.pop(h)
 
 @chrono 
 def integrate_key_deleting(c : Call):
     """
     Marks a registry Key as deleted.
     """
-    from ....logger import logger
+    from .....logger import logger
     if c.status == 1:
         logger.debug("Deleting registry key.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to delete key from unseen handle.")
             return
         k = __create_key_tree(c.arguments.regkey)
         k.color = k.deleted_key_color
@@ -160,15 +160,15 @@
             __deleted_entries[k].update(__existing_entries.pop(k))
 
 @chrono
 def integrate_key_value_querying(c : Call):
     """
     Creates a KeyEntry node and marks it as read by thea key Handle.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Graph
     from .entities import KeyEntry
     from .relations import ChangesTowards, HasEntry, QueriesEntry
     if c.status == 1:
         logger.debug("Querying key entry.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to query value with unseen key handle.")
@@ -217,15 +217,15 @@
         QueriesEntry(v, h)
 
 @chrono
 def integrate_key_value_setting(c : Call):
     """
     Creates a KeyEntry node and marks it as written by a key Handle.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Graph
     from .entities import KeyEntry
     from .relations import ChangesTowards, HasEntry, SetsEntry
     if c.status == 1:
         logger.debug("Setting key entry.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to set value with unseen key handle.")
@@ -271,15 +271,15 @@
         SetsEntry(h, v)
 
 @chrono
 def integrate_key_value_deleting(c : Call):
     """
     Creates a KeyEntry node and marks it as deleted by a key Handle.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...graph import Graph
     from .entities import KeyEntry
     from .relations import ChangesTowards, DeletesEntry, HasEntry
     if c.status == 1:
         logger.debug("Deleting key entry.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to set value with unseen key handle.")
@@ -360,15 +360,15 @@
 
 __N_referencing_phase = BuildingPhase.request_finalizing_phase()
 
 def find_filesystem_references(ev : BuildingPhase):
     """
     When called with the right finalizing phase event, will cause all KeyEntry nodes to link to File or Folder nodes that their value reference if these entries were modified.
     """
-    from ....logger import logger
+    from .....logger import logger
     from ...utils import is_path, parse_command_line, path_factory
     from ..filesystem import Contains, Directory, File, HasDrive
     from ..network import Host
     from .entities import KeyEntry, Key_SZ_Entry, Key_MULTI_SZ_Entry
     from .relations import DeletesEntry, ReferencesFileSystem, SetsEntry
     if ev.major == "Finalizer" and ev.minor == __N_referencing_phase:
         logger.debug("Finding references to filesystem in {} registry key entries.".format(len(KeyEntry)))
```

### Comparing `baguette_verse-1.0.0/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.5/baguette/bakery/source/types/registry/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
-from ....logger import logger
+from .....logger import logger
 from ...graph import Arrow, Edge
 from ..execution.entities import Process
 from ..filesystem.entities import Directory, File
 from ..network.entities import Host
 from .entities import Handle, Key, KeyEntry
 
 __all__ = ["HasSubKey", "HasEntry", "UsesKey", "HasHandle", "Discovered", "QueriesEntry", "SetsEntry", "DeletesEntry", "ChangesTowards", "ReferencesFileSystem"]
```

### Comparing `baguette_verse-1.0.0/baguette/croutons/extractor.py` & `baguette_verse-1.0.5/baguette/croutons/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         levels = {
             0 : logging.ERROR,
             1 : logging.WARNING,
             2 : logging.INFO,
             3 : logging.DEBUG
         }
         
-        from ..bakery.logger import set_level, logger
+        from ..logger import set_level, logger
         set_level(levels[rack.verbosity])
 
         logger.debug("Just change worker's verbosity level.")
 
         import os
         from pickle import dump, load, UnpicklingError
         from Viper.better_threading import Future, DaemonThread
```

### Comparing `baguette_verse-1.0.0/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.5/baguette/croutons/metalib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This is the MetaLib! It is a library for MetaGraphs, a pattern storage.
 
 All existing MetaGraphs are loaded with the package.
 To create new MetaGraphs, use the module croutons.metalib.interactive.
 """
 
-from ...bakery.logger import logger
+from ...logger import logger
 from .utils import entries, load
 
 logger.info("Loading MetaGraph library.")
 
 __all__ = []
```

### Comparing `baguette_verse-1.0.0/baguette/croutons/metalib/evaluator.py` & `baguette_verse-1.0.5/baguette/croutons/source/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
-This module defines an evaluator class, which is a pickable Python function.
+This module defines an evaluator class, which is a pickable Python function. Look at Evaluator.
 """
 
-from typing import Any, Generic, TypeVar, ParamSpec
+from typing import Any, Generic, TypeVar
+
+__all__ = ["Evaluator"]
+
 
 
 
 
 X = TypeVar("X")
 R = TypeVar("R")
 
@@ -53,18 +56,18 @@
             self.__compile()
         except SyntaxError as E:
             self.__code = old_code
             raise SyntaxError("Cannot set function code as it contains a syntax error.") from E
         self.__code = code
     
     def __str__(self) -> str:
-        return "lambda x : " + self.__code
+        return "x -> " + self.__code
     
     def __repr__(self) -> str:
-        return "Evaluator(" + repr(self.__code) + ")"
+        return f"Evaluator('{self.__code}')"
     
     def __call__(self, x : X) -> R:
         if not self.__compiled:
             raise RuntimeError("Tried to call an empty Evaluator")
         try:
             return self.__compiled(x)
         except BaseException as E:
@@ -73,8 +76,14 @@
     def __getstate__(self) -> dict[str, Any]:
         return {"code" : self.__code}
     
     def __setstate__(self, state : dict[str, Any]):
         self.__code = ""
         self.__compiled = None
         for name, value in state.items():
-            setattr(self, name, value)
+            setattr(self, name, value)
+
+
+
+
+
+del Any, Generic, TypeVar, X, R
```

### Comparing `baguette_verse-1.0.0/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.5/baguette/croutons/metalib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,8 +171,14 @@
             file = Path(file)
         except:
             raise ValueError("Invalid path : '{}'".format(file))
     if not isinstance(file, Path):
         raise TypeError("Expected path, got " + repr(type(file).__name__))
     from pickle import load
     with file.open("rb") as f:
-        return load(f)
+        return load(f)
+    
+
+
+
+
+del pathlib, MetaGraph
```

### Comparing `baguette_verse-1.0.0/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.5/baguette/croutons/source/metagraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 """
-This module defines MetaGraphs, MetaVertices, MetaEdges and MetaArrows.
+This module defines MetaGraphs, MetaVertices, MetaEdges and MetaArrows. They allow you to create graph patterns.
+Look at these classes.
 """
 
-from typing import Any, Callable, Iterable, Iterator, Optional, Self
-from ...bakery.source.graph import Arrow, Edge, Graph, UniqueVertex, Vertex
+from types import UnionType
+from typing import Any, Iterable, Iterator, Optional, Self
+
+from baguette.bakery.source.graph import Edge
+from baguette.croutons.source.evaluator import Evaluator
+
 from ...bakery.source.colors import Color
+from ...bakery.source.graph import Arrow, Edge, Graph, UniqueVertex, Vertex
 from ...bakery.source.types.execution import *
-from ...bakery.source.types.network import *
 from ...bakery.source.types.filesystem import *
-
-
-
+from ...bakery.source.types.network import *
+from .evaluator import Evaluator
 
 
 class MetaVertex(UniqueVertex):
 
     """
-    This class describes a type vertex. One or multiple Vertex subclasses can be associated to it.
+    This class describes a type vertex. One or multiple Vertex subclasses can be associated to it as well as additional conditions.
+    This class defines properties cls and condition which can be efficiently affected with a special syntax:
+    >>> MV = MetaVertex()
+    >>> MV.cls = (File, )
+    >>> MV.condition = Evaluator("lambda x : x.name.endswith('.exe')")
+
+    is equivalent to:
+    >>> MV = MetaVertex[File]("lambda x : x.name.endswith('.exe')")
     """
 
     @classmethod
-    def __class_getitem__(cls, cls_init):
+    def __class_getitem__(cls, cls_init : type[Vertex] | tuple[type[Vertex], ...] | UnionType) -> Self:
         try:
             Mv = cls()
             Mv.cls = cls_init
             return Mv
         except BaseException as E:
             raise E from None
 
@@ -32,22 +43,24 @@
         "__class" : "The class that this MetaVertex represents.",
         "__condition" : "An additional condition function. Takes a Vertex as an input and tells whether or not it can be a valid match (does not need to check type)",
         "__color" : "The Color forcefully set to this MetaVertex."
     }
 
     __pickle_slots__ = {
         "cls",
-        "condition"
+        "condition",
+        "color"
     }
 
     def __init__(self, *, parent: Optional[Vertex] = None) -> None:
         from ...bakery.source.colors import Color
+        from .evaluator import Evaluator
         super().__init__(parent=parent)
         self.__class : tuple[type[Vertex], ...] = (Vertex, )
-        self.__condition : Callable[[Vertex], bool] | bool = True
+        self.__condition : Evaluator[Vertex, bool] | None = None
         self.__color : Color | None = None
         self.edges : set[MetaEdge]
 
     @property
     def color(self) -> Color:
         """
         The color of this MetaVertex. Defaults to the average of the colors of all its Vertex classes.
@@ -72,20 +85,28 @@
     def cls(self) -> tuple[type[Vertex], ...]:
         """
         The classes that this vertex represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Vertex] | tuple[type[Vertex], ...]):
+    def cls(self, cls : type[Vertex] | tuple[type[Vertex], ...] | UnionType):
         """
         Sets the class(es) associated with this vertex.
         """
+        from types import UnionType
+
         from ...bakery.source.graph import Vertex
-        if isinstance(cls, type) and issubclass(cls, Vertex):
+        if isinstance(cls, UnionType):
+            args : tuple[type[Vertex]] = cls.__args__
+            for c in args:
+                if not isinstance(c, type) or not issubclass(c, Vertex):
+                    raise TypeError("Expected subclass of Vertex or tuple of subclasses, got a " + repr(c))
+            self.__class = args
+        elif isinstance(cls, type) and issubclass(cls, Vertex):
             self.__class = (cls, )
         elif isinstance(cls, tuple):
             for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Vertex):
                     raise TypeError("Expected subclass of Vertex or tuple of subclasses, got a " + repr(c))
             self.__class = cls
         else:
@@ -93,84 +114,123 @@
     
     @cls.deleter
     def cls(self):
         from ...bakery.source.graph import Vertex
         self.__class = (Vertex, )
 
     @property
-    def condition(self) -> Callable[[Vertex], bool] | bool:
+    def condition(self) -> Evaluator[Vertex, bool] | None:
         """
-        An additional condition to check when trying to match a Vertex to this MetaVertex.
+        An additional and optional condition to check when trying to match a Vertex to this MetaVertex.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Vertex], bool] | bool):
+    def condition(self, cond : Evaluator[Vertex, bool] | str):
         """
         Sets the additional condition function for this MetaVertex.
         """
-        if not callable(cond) and not isinstance(cond, bool):
-            raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
+        from .evaluator import Evaluator
+        if isinstance(cond, str):
+            try:
+                cond = Evaluator(cond)
+            except SyntaxError as e:
+                raise e from None
+        if not isinstance(cond, Evaluator):
+            raise TypeError(f"Expected Evaluator or str, got '{type(cond).__name__}'")
         self.__condition = cond
 
     @condition.deleter
     def condition(self):
-        self.__condition = True
+        self.__condition = None
     
     def match(self, v : Vertex) -> bool:
         """
         Returns True if the Vertex v has a matching type.
         """
-        return isinstance(v, self.__class) and (self.__condition(v) if callable(self.__condition) else self.__condition)
+        return isinstance(v, self.__class) and (self.__condition(v) if self.__condition else True)
     
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaVertex.
         """
         return " | ".join(c.__name__ for c in self.__class)
+    
+    def __call__(self, cond : Evaluator[Vertex, bool] | str) -> Self:
+        """
+        Implements self(cond). Sets the condition and returns self.
+        """
+        try:
+            self.condition = cond
+            return self
+        except BaseException as e:
+            raise e from None
+        
+    def __getstate__(self):
+        s = super().__getstate__()
+        if not s["condition"]:
+            s.pop("condition")
+        return s
+    
+    def __setstate__(self, state : dict[str, Any]):
+        self.__condition = None
+        super().__setstate__(state)
 
     @property
     def label(self) -> str:
-        return "Vertex[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"Vertex[{self.__get_cls_str()}]" + (f"({str(self.__condition)})" if self.__condition else "")
 
     def __str__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + ("*" if self.__condition else "")
     
     def __repr__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + (f"({repr(self.__condition.code)})" if self.__condition else "")
     
 
 
 
 
 class MetaEdge(Edge):
 
     """
     This class describes a type edge. One or multiple Edge subclasses can be associated to it.
     Note that a MetaEdge can represent a subclass of Arrow and in this case, the match can be made in both directions.
+    Like MetaVertices, MetaEdges have special syntaxes for setting the cls and condition attributes:
+    >>> U = MetaVertex[Directory]
+    >>> V = MetaVertex[File]
+    >>> UV = MetaEdge(U, V)
+    >>> UV.cls = (Contains, )
+    >>> UV.condition = Evaluator("lambda x : True")     # Dummy condition
+
+    is equivalent to:
+    >>> U = MetaVertex[Directory]
+    >>> V = MetaVertex[File]
+    >>> UV = MetaEdge(U, V)[contains]("lambda x : True")
     """
 
     __slots__ = {
         "__class" : "The class that this MetaEdge represents.",
         "__condition" : "An additional condition function. Takes an Edge as an input and tells whether or not it can be a valid match (does not need to check type)",
         "__color" : "The Color forcefully set to this MetaEdge."
     }
 
     __pickle_slots__ = {
         "cls",
-        "condition"
+        "condition",
+        "color"
     }
 
     def __init__(self, source: MetaVertex, destination: MetaVertex, *, auto_write: bool = True) -> None:
         from ...bakery.source.colors import Color
+        from .evaluator import Evaluator
         if not isinstance(source, MetaVertex) or not isinstance(destination, MetaVertex):
             raise TypeError("Expected two MetaVertices, got " + repr(type(source).__name__) + " and " + repr(type(destination).__name__))
         super().__init__(source, destination, auto_write=auto_write)
         self.__class : tuple[type[Edge], ...] = (Edge, )
-        self.__condition : Callable[[Edge], bool] | bool = True
+        self.__condition : Evaluator[Edge, bool] | None = None
         self.__color : Color | None = None
         self.source : MetaVertex
         self.destination : MetaVertex
 
     @property
     def color(self) -> Color:
         """
@@ -200,20 +260,28 @@
     def cls(self) -> tuple[type[Edge], ...]:
         """
         The classes that this edge represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Edge] | tuple[type[Edge], ...]):
+    def cls(self, cls : type[Edge] | tuple[type[Edge], ...] | UnionType):
         """
         Sets the class(es) associated with this edge.
         """
+        from types import UnionType
+
         from ...bakery.source.graph import Edge
-        if isinstance(cls, type) and issubclass(cls, Edge):
+        if isinstance(cls, UnionType):
+            args : tuple[type[Edge]] = cls.__args__
+            for c in args:
+                if not isinstance(c, type) or not issubclass(c, Edge):
+                    raise TypeError("Expected subclass of Edge or tuple of subclasses, got a " + repr(c))
+            self.__class = args
+        elif isinstance(cls, type) and issubclass(cls, Edge):
             self.__class = (cls, )
         elif isinstance(cls, tuple):
             for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Edge):
                     raise TypeError("Expected subclasses of Edge or tuple of subclasses, got a " + repr(c))
             self.__class = cls
         else:
@@ -221,101 +289,135 @@
         
     @cls.deleter
     def cls(self):
         from ...bakery.source.graph import Edge
         self.__class = (Edge, )
         
     @property
-    def condition(self) -> Callable[[Edge], bool] | bool:
+    def condition(self) -> Evaluator[Edge, bool] | None:
         """
         An additional condition to check when trying to match an Edge to this MetaEdge.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Edge], bool] | bool):
+    def condition(self, cond : Evaluator[Edge, bool] | str):
         """
         Sets the additional condition function for this MetaEdge.
         """
-        if not callable(cond) and not isinstance(cond, bool):
-            raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
+        from .evaluator import Evaluator
+        if isinstance(cond, str):
+            try:
+                cond = Evaluator(cond)
+            except SyntaxError as e:
+                raise e from None
+        if not isinstance(cond, Evaluator):
+            raise TypeError(f"Expected Evaluator or str, got '{type(cond).__name__}'")
         self.__condition = cond
     
     @condition.deleter
     def condition(self):
-        self.__condition = True
+        self.__condition = None
     
     def match(self, e : Edge) -> bool:
         """
         Returns True if the Egde e has a matching type.
         """
-        return isinstance(e, self.__class) and (self.__condition(e) if callable(self.__condition) else self.__condition)
+        return isinstance(e, self.__class) and (self.__condition(e) if self.__condition else True)
     
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaEdge.
         """
         return " | ".join(c.__name__ for c in self.cls)
+    
+    def __getstate__(self):
+        s = super().__getstate__()
+        if not s["condition"]:
+            s.pop("condition")
+        return s
+    
+    def __setstate__(self, state : dict[str, Any]):
+        self.__condition = None
+        super().__setstate__(state)
 
     @property
     def label(self) -> str:
-        return "Edge[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"Edge[{self.__get_cls_str()}]" + (f"({repr(self.__condition.code)})" if self.__condition else "")
 
     def __str__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + ("*" if self.__condition else "")
     
     def __repr__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + (f"({repr(self.__condition.code)})" if self.__condition else "")
 
-    def __getitem__(self, cls : type[Edge] | tuple[type[Edge], ...]) -> Self:
+    def __getitem__(self, cls : type[Edge] | tuple[type[Edge], ...] | UnionType) -> Self:
         try:
             self.cls = cls
             return self
         except BaseException as E:
             raise E from None
+        
+    def __call__(self, cond : Evaluator[Edge, bool] | str) -> Self:
+        try:
+            self.condition = cond
+            return self
+        except BaseException as e:
+            raise e from None
+
 
 
 
 
 class MetaArrow(Arrow, MetaEdge):
 
     """
     This class describes a type arrow. One or multiple Arrow subclasses can be associated to it.
+    It has the same syntax rules as MetaEdges.
     """
 
     __slots__ = {
         "__class" : "The class that this MetaArrow represents.",
         "__condition" : "An additional condition function. Takes an Arrow as an input and tells whether or not it can be a valid match (does not need to check type)"
     }
 
     __pickle_slots__ = {
         "cls",
         "condition"
     }
 
     def __init__(self, source: MetaVertex, destination: MetaVertex, *, auto_write: bool = True) -> None:
         from ...bakery.source.graph import Arrow
+        from .evaluator import Evaluator
         super().__init__(source, destination, auto_write=auto_write)
         self.__class : tuple[type[Arrow], ...] = (Arrow, )
-        self.__condition : Callable[[Arrow], bool] | bool = True
+        self.__condition : Evaluator[Arrow, bool] | None = None
 
     @property
     def cls(self) -> tuple[type[Arrow], ...]:
         """
         The classes that this arrow represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Arrow] | tuple[type[Arrow], ...]):
+    def cls(self, cls : type[Arrow] | tuple[type[Arrow], ...] | UnionType):
         """
         Sets the class(es) associated with this arrow.
         """
+        from types import UnionType
+
         from ...bakery.source.graph import Arrow
-        if isinstance(cls, type) and issubclass(cls, Arrow):
+        if isinstance(cls, UnionType):
+            args : tuple[type[Arrow]] = cls.__args__
+            for c in args:
+                if not isinstance(c, type) or not issubclass(c, Arrow):
+                    raise TypeError("Expected subclass of Arrow or tuple of subclasses, got a " + repr(c))
+            self.__class = args
+        elif isinstance(cls, type) and issubclass(cls, Arrow):
             self.__class = (cls, )
         elif isinstance(cls, tuple):
             for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Arrow):
                     raise TypeError("Expected subclasses of Arrow or tuple of subclasses, got a " + repr(c))
             self.__class = cls
         else:
@@ -323,66 +425,90 @@
         
     @cls.deleter
     def cls(self):
         from ...bakery.source.graph import Arrow
         self.__class = (Arrow, )
         
     @property
-    def condition(self) -> Callable[[Arrow], bool] | bool:
+    def condition(self) -> Evaluator[Arrow, bool] | None:
         """
-        An additional condition to check when trying to match an Edge to this MetaEdge.
+        An additional condition to check when trying to match an Arrow to this MetaArrow.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Arrow], bool] | bool):
+    def condition(self, cond : Evaluator[Arrow, bool] | str):
         """
-        Sets the additional condition function for this MetaEdge.
+        Sets the additional condition function for this MetaArrow.
         """
-        if not callable(cond) and not isinstance(cond, bool):
-            raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
+        from .evaluator import Evaluator
+        if isinstance(cond, str):
+            try:
+                cond = Evaluator(cond)
+            except SyntaxError as e:
+                raise e from None
+        if not isinstance(cond, Evaluator):
+            raise TypeError(f"Expected Evaluator or str, got '{type(cond).__name__}'")
         self.__condition = cond
     
     @condition.deleter
     def condition(self):
-        self.__condition = True
+        self.__condition = None
+    
+    def __setstate__(self, state : dict[str, Any]):
+        self.__condition = None
+        super().__setstate__(state)
     
     def match(self, a : Arrow) -> bool:
         """
         Returns True if the Arrow a has a matching type.
         """
-        return isinstance(a, self.__class) and (self.__condition(a) if callable(self.__condition) else self.__condition)
+        return isinstance(a, self.__class) and (self.__condition(a) if self.__condition else True)
 
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaArrow.
         """
         return " | ".join(c.__name__ for c in self.cls)
 
     @property
     def label(self) -> str:
-        return "Arrow[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"Arrow[{self.__get_cls_str()}]" + (f"({repr(self.__condition.code)})" if self.__condition else "")
     
     def __str__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + ("*" if self.__condition else "")
     
     def __repr__(self) -> str:
-        return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
+        return f"{type(self).__name__}[{self.__get_cls_str()}]" + (f"({repr(self.__condition.code)})" if self.__condition else "")
     
-    def __getitem__(self, cls : type[Arrow] | tuple[type[Arrow], ...]) -> Self:
+    def __getitem__(self, cls : type[Arrow] | tuple[type[Arrow], ...] | UnionType) -> Self:
         return super().__getitem__(cls)
     
+    def __call__(self, cond: Evaluator[Arrow, bool] | str) -> Self:
+        try:
+            self.condition = cond
+            return self
+        except BaseException as e:
+            raise e from None
+    
 
 
 
 
 class MetaGraph(Graph):
 
     """
     This particular type of graph can only contain MetaVertices, MetaEdges or MetaArrows. It can be used for normal graph exploration.
+    Note that contrary to normal Graphs, MetaGraphs can hold named vertices and edges:
+    >>> MG = MetaGraph()
+    >>> MG.File = MetaVertex[File]
+    >>> len(MG.vertices)
+    1
+    >>> mG.File
+    MetaVertex[File]
     """
 
     __slots__ = {
         "__named_objects" : "A dict holding named vertices and edges."
     }
 
     vertices : set[MetaVertex]
@@ -666,17 +792,18 @@
             yield Mu
             done.add(Mu)
          
     def search_iter(self, g : Graph) -> Iterator[Graph]:
         """
         Searches through g for all occurences of a subgraph that matches the metagraph.
         """
-        from ...bakery.source.graph import Graph
         from typing import Iterator
 
+        from ...bakery.source.graph import Graph
+
         # subgraphs : list[dict[MetaVertex | MetaEdge, Vertex | Edge]] = [{}]
         # next_subgraphs : list[dict[MetaVertex | MetaEdge, Vertex | Edge]] = []
 
         mapping = self.__neighborhood_mapper(g)
 
         self.__clear_mapper_deadends(mapping)
```

### Comparing `baguette_verse-1.0.0/.gitignore` & `baguette_verse-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/LICENSE` & `baguette_verse-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.0/README.md` & `baguette_verse-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use `pip` in the Python installation you want to use:
 
 ```$ pip install baguette-verse```
 
 BAGUETTE is a pure Python project, meaning that a BAGUETTE graph is a Python data structure and for now can only be manipulated using the Python interface described below.
 
+If you want to learn BAGUETTE interactively, once installed, you can just run this command to start the tutorial:
+
+```$ baguette.tutorial```
+
 ## Bakery
 
 **Bakery** is the package used to bake (compile) BAGUETTE graphs. For now, BAGUETTEs can only be made from Cuckoo execution reports. From that, the baker will create a BAGUETTE packaging:
 Inside of a ".bag" folder, you may find :
 - the "baguette.pyt" file which contains the **pickle** of the BAGUETTE graph
 - the "visual.gexf" file, which is a **visualizable** graph format to use with **[Gephi](https://gephi.org/)**
 - a "index.pyt" file which holds **metadata** about the given BAGUETTE.
```

### Comparing `baguette_verse-1.0.0/PKG-INFO` & `baguette_verse-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.0
+Version: 1.0.5
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -670,15 +670,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: levenshtein
 Requires-Dist: python-magic-bin; platform_system == 'Windows'
 Requires-Dist: python-magic; platform_system != 'Windows'
-Requires-Dist: viper-lib>=0.5.4
+Requires-Dist: viper-lib>=0.5.5
 Description-Content-Type: text/markdown
 
 # BAGUETTE-VERSE
 
 This is the BAGUETTE framework. BAGUETTE stands for **Behavioral Analysis Graph Using Execution Traces Towards Explanability**.
 BAGUETTE is a **heterogeneous graph** data structure used to represent the **behavior of malware samples**.
 
@@ -686,14 +686,18 @@
 
 BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use `pip` in the Python installation you want to use:
 
 ```$ pip install baguette-verse```
 
 BAGUETTE is a pure Python project, meaning that a BAGUETTE graph is a Python data structure and for now can only be manipulated using the Python interface described below.
 
+If you want to learn BAGUETTE interactively, once installed, you can just run this command to start the tutorial:
+
+```$ baguette.tutorial```
+
 ## Bakery
 
 **Bakery** is the package used to bake (compile) BAGUETTE graphs. For now, BAGUETTEs can only be made from Cuckoo execution reports. From that, the baker will create a BAGUETTE packaging:
 Inside of a ".bag" folder, you may find :
 - the "baguette.pyt" file which contains the **pickle** of the BAGUETTE graph
 - the "visual.gexf" file, which is a **visualizable** graph format to use with **[Gephi](https://gephi.org/)**
 - a "index.pyt" file which holds **metadata** about the given BAGUETTE.
```

