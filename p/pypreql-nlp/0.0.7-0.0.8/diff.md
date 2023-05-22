# Comparing `tmp/pypreql-nlp-0.0.7.tar.gz` & `tmp/pypreql-nlp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.7.tar", last modified: Thu May 18 02:09:59 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.8.tar", last modified: Mon May 22 03:26:30 2023, max compression
```

## Comparing `pypreql-nlp-0.0.7.tar` & `pypreql-nlp-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/cache_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/local_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_final_concepts.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_refine_filter.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/cache_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/local_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_final_concepts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_refine_filter.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/setup.py
```

### Comparing `pypreql-nlp-0.0.7/PKG-INFO` & `pypreql-nlp-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.7
+Version: 0.0.8
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.7/README.md` & `pypreql-nlp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.7/preql_nlp/cache_providers/local_sqlite.py` & `pypreql-nlp-0.0.8/preql_nlp/cache_providers/local_sqlite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from preql_nlp.cache_providers.base import BaseCache
+from preql_nlp.constants import logger
 import sqlite3
 
 DEFAULT_SQLITE_ADDRESS = "local_prompt_cache.db"
 
 
 
 class SqlliteCache(BaseCache):
 
 
     def __init__(self, sqlite_address: str = DEFAULT_SQLITE_ADDRESS):
         self.sqlite_address = sqlite_address
 
     
     def retrieve(self, prompt_hash: str) -> str | None:
-        print("checking for cache with prompt hash ", prompt_hash)
+        logger.info(f"checking for cache with prompt hash {prompt_hash}")
         con = sqlite3.connect(self.sqlite_address)
         cur = con.cursor()
         cur.execute(
             "create table if not exists prompt_cache (cache_id string, prompt_type string, response string)"
         )
         res = cur.execute(
             "select response, prompt_type from prompt_cache where cache_id = ?",
             (prompt_hash,),
         )
         current = res.fetchone()
         if current:
-            print("got cached response of type ", current[1])
+            logger.info(f"Got cached response of type {current[1]}")
             return current[0]
+        logger.info('No cache available for key')
         return None
 
 
 
-    def stash(self, prompt_hash: str, category: str, result: str):
+    def store(self, prompt_hash: str, category: str, result: str):
         con = sqlite3.connect(self.sqlite_address)
         cur = con.cursor()
         cur.execute(
             "create table if not exists prompt_cache (cache_id string, prompt_type string, response string)"
         )
         cur.execute(
             "insert into prompt_cache select ?, ?,  ?", (prompt_hash, category, result)
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/helpers.py` & `pypreql-nlp-0.0.8/preql_nlp/helpers.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.7/preql_nlp/main.py` & `pypreql-nlp-0.0.8/preql_nlp/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,287 +1,261 @@
+import uuid
+from typing import List, Union
+
+from preql.core.enums import BooleanOperator, Purpose
 from preql.core.models import (
-    Select,
-    ProcessedQuery,
+    Comparison,
     Concept,
-    OrderItem,
+    Conditional,
+    Environment,
     OrderBy,
     Ordering,
+    OrderItem,
+    ProcessedQuery,
+    Select,
+    WhereClause,
+    unique,
 )
 from preql.core.query_processor import process_query_v2
-from preql.core.enums import Purpose
-from typing import Iterable, List
-from collections import defaultdict
 
-from preql.core.models import Environment
-from preql_nlp.prompts import (
-    run_prompt,
-    SemanticToTokensPromptCase,
-    SelectionPromptCase,
-    SemanticExtractionPromptCase,
-    FilterRefinementCase,
-)
-from preql_nlp.constants import logger, DEFAULT_LIMIT
+from preql_nlp.constants import DEFAULT_LIMIT, logger
 from preql_nlp.models import (
+    ConceptSelectionResponse,
+    FilterResult,
+    FinalFilterResult,
+    FinalOrderResult,
     InitialParseResponse,
+    IntermediateParseResults,
     OrderResult,
-    FilterResult,
-    TokenInputs,
+    # TokenInputs,
     SemanticTokenResponse,
-    ConceptSelectionResponse,
-    IntermediateParseResults,
 )
-
-from preql.core.models import WhereClause, Conditional, Comparison
-from preql.core.enums import BooleanOperator
-
-
-from typing import Any
-
-import re
-import uuid
-
-
-def split_to_tokens(input_text: str) -> list[str]:
-    return list(set(re.split("\.|\_", input_text)))
-
-
-def build_token_list_by_purpose(concepts, purposes: Iterable[Purpose]) -> list[str]:
-    concepts = {k: v for k, v in concepts.items() if v.purpose in purposes}
-
-    unique = set(concepts.keys())
-    final = set()
-    # if a concept has another concept as a substring, remove
-    # to help restrict the size of the search space
-    for concept in unique:
-        # matched = [comparison  for comparison in unique if comparison in concept]
-        # filtered = [m for m in matched if m !=concept]
-        # if not filtered:
-        #     final.append(concept)
-        for x in split_to_tokens(concept):
-            final.add(x)
-    return list(final)
-
-
-def tokens_to_concept(
-    tokens: list[str],
-    concepts: List[str],
-    limits: int = 5,
-    universe: list[str] | None = None,
-):
-    tokens = list(set(tokens))
-    universe_list = list(set(universe or []))
-    mappings = {x: split_to_tokens(x) for x in concepts}
-    candidates = [x for x in concepts if all(token in mappings[x] for token in tokens)]
-    pickings = defaultdict(list)
-
-    if not candidates:
-        return None
-    tiers = set()
-    for candidate in candidates:
-        tier = sum(
-            [1 if token in mappings[candidate] else 0 for token in universe_list]
-        )
-        pickings[tier].append(candidate)
-        tiers.add(tier)
-    tier_list = sorted(list(tiers), key=lambda x: -x)
-
-    found: List[str] = []
-    while len(found) < limits and tier_list:
-        stier = tier_list.pop(0)
-        candidates = sorted(pickings[stier], key=lambda x: len(x))
-        required = limits - len(found)
-        found += candidates[:required]
-    return found
-
-
-def coerce_list_dict(input: Any) -> List[dict]:
-    if not isinstance(input, list):
-        raise ValueError("Input must be a list")
-    for x in input:
-        if not isinstance(x, dict):
-            raise ValueError("Input must be a list of dicts")
-    return input
-
-
-def coerce_list_str(input: Any) -> List[str]:
-    if not isinstance(input, list):
-        raise ValueError("Input must be a list")
-    for x in input:
-        if not isinstance(x, str):
-            raise ValueError("Input must be a list of dicts")
-    return input
-
-
-def coerce_initial_result(input) -> InitialParseResponse:
-    return InitialParseResponse.parse_obj(input)
+from preql_nlp.prompts import (
+    FilterRefinementCase,
+    SelectionPromptCase,
+    SemanticExtractionPromptCase,
+    SemanticToTokensPromptCase,
+    run_prompt,
+)
+from preql_nlp.tokenization import build_token_list_by_purpose, tokens_to_concept
 
 
-def get_phrase_from_x(x):
+def get_phrase_from_x(x: Union[str, FilterResult, OrderResult]):
     if isinstance(x, str):
         return x
     elif isinstance(x, FilterResult):
         return x.concept
     elif isinstance(x, OrderResult):
         return x.concept
     raise ValueError
 
 
+def tokenize_phrases(
+    phrase_list: List[str], tokens: List[str], session_uuid, log_info: bool
+) -> SemanticTokenResponse:
+    phrase_tokens: SemanticTokenResponse = run_prompt(  # type: ignore
+        SemanticToTokensPromptCase(phrases=phrase_list, tokens=tokens),
+        debug=True,
+        session_uuid=session_uuid,
+        log_info=log_info,
+    )
+    phrase_tokens.__root__ = [
+        x for x in phrase_tokens.__root__ if x.phrase in phrase_list
+    ]
+    return phrase_tokens
+
+
+def concept_names_from_token_response(
+    phrase_tokens: SemanticTokenResponse, concepts: dict[str, Concept]
+) -> list[str]:
+    token_universe = []
+    output: list[str] = []
+
+    for mapping in phrase_tokens:
+        token_universe += mapping.tokens
+    for mapping in phrase_tokens:
+        found = False
+        concepts_str_matches = tokens_to_concept(
+            mapping.tokens,
+            [c for c in concepts.keys()],
+            limits=5,
+            universe=token_universe,
+        )
+        if concepts_str_matches:
+            logger.info(f"For phrase {mapping.phrase} got {concepts_str_matches}")
+            output += concepts_str_matches
+            found = True
+            break
+        if not found:
+            raise ValueError(
+                f"Could not find concept for input {mapping.phrase} with tokens {mapping.tokens} and concepts {list(concepts.keys())}"
+            )
+    return output
+
+
+def enrich_filter(input: FinalFilterResult, log_info: bool, session_uuid):
+    if not (input.concept.metadata and input.concept.metadata.description):
+        return input
+    input.values = run_prompt(  # type: ignore
+        FilterRefinementCase(
+            values=input.values,
+            description=input.concept.metadata.description,
+        ),
+        session_uuid=session_uuid,
+        log_info=log_info,
+    ).new_values
+
+
 def discover_inputs(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
     log_info: bool = True,
 ) -> IntermediateParseResults:
-    # we work around prompt size issues and hallucination by doing a two phase discovery
-    # first we parse the question into metrics/dimensions
-    # then for each one, we match those to a token list
-    # and then we deterministically map the tokens back to the most relevant concept
-    # TODO: turn the third pass into a prompt
-    concepts = input_environment.concepts
-    debug = True
-    final_concept_list = list(concepts.keys())
-    metrics = build_token_list_by_purpose(concepts, (Purpose.METRIC,))
-    dimensions = build_token_list_by_purpose(
-        concepts, (Purpose.KEY, Purpose.PROPERTY, Purpose.CONSTANT)
-    )
+    # the core logic flow
 
+    # DETERMINSTIC: setup logging
+    # LLM: semantic extraction
+    # LLM: tokenization of all strings (reduce search space over all concepts)
+    # DETERMINISTIC: concept candidates from tokens (map reduced search space to candidates)
+    # LLM: final selection of concepts (final get the concept result we want)
+    # DETERMINISTIC: map phrases to final concepts
+    # LLM: enrich filter values
+    # DETERMINISTIC: return results
+
+    # DETERMINISTIC: setup logging
     session_uuid = uuid.uuid4()
+    env_concepts = input_environment.concepts
 
+    # LLM: semantic extraction
     parsed: InitialParseResponse = run_prompt(  # type:ignore
         SemanticExtractionPromptCase(input_text),
         debug=debug,
         log_info=log_info,
         session_uuid=session_uuid,
     )
-    filtering = build_token_list_by_purpose(
-        concepts, (Purpose.METRIC, Purpose.KEY, Purpose.CONSTANT, Purpose.PROPERTY)
-    )
-    order = list(set(filtering + metrics + dimensions))
-    token_inputs = TokenInputs(
-        metrics=metrics, dimensions=dimensions, order=order, filtering=filtering
-    )
 
-    output: List[str] = []
-    for field in ["metrics", "dimensions", "filtering", "order"]:
-        local_phrases = [get_phrase_from_x(x) for x in getattr(parsed, field)]
-        all_tokens = getattr(token_inputs, field)
-        phrase_tokens: SemanticTokenResponse = run_prompt(  # type: ignore
-            SemanticToTokensPromptCase(phrases=local_phrases, tokens=all_tokens),
-            debug=True,
-            session_uuid=session_uuid,
-            log_info=log_info,
+    # LLM: tokenization of all strings (reduce search space over all concepts)
+    concept_candidates = []
+    global_phrase_token_map = {}
+    for semantic_category, valid_purposes in {
+        "metrics": [Purpose.METRIC],
+        "dimensions": [Purpose.KEY, Purpose.PROPERTY, Purpose.CONSTANT],
+        "filtering": list(Purpose),
+        "order": list(Purpose),
+    }.items():
+        category_tokens = build_token_list_by_purpose(env_concepts, valid_purposes)
+        local_phrases = [
+            get_phrase_from_x(x) for x in getattr(parsed, semantic_category)
+        ]
+        # skip if we have no relevant phrases
+        if not local_phrases:
+            continue
+        token_mapping = tokenize_phrases(
+            local_phrases, category_tokens, log_info=log_info, session_uuid=session_uuid
         )
-        token_universe = []
-        for mapping in phrase_tokens:
-            token_universe += mapping.tokens
-        for mapping in phrase_tokens:
-            found = False
-            for universe in [token_universe]:
-                concepts = tokens_to_concept(
-                    mapping.tokens,
-                    [c for c in final_concept_list],
-                    limits=5,
-                    universe=universe,
-                )
-                if concepts:
-                    logger.info(f"For phrase {mapping.phrase} got {concepts}")
-                    output += concepts
-                    found = True
-                    break
-            if not found:
+
+        for item in token_mapping:
+            if not all([x in category_tokens] for x in item.tokens):
+                invalid = [x for x in item.tokens if x not in category_tokens]
                 raise ValueError(
-                    f"Could not find concept for input {mapping.phrase} with tokens {mapping.tokens}"
+                    f"Phrase {item.phrase} return invalid tokens {invalid}"
                 )
+            global_phrase_token_map[item.phrase] = item.tokens
+        concept_candidates += concept_names_from_token_response(
+            token_mapping, env_concepts
+        )
+
+    # DETERMINISTIC: concept candidates from tokens (map reduced search space to candidates)
     selections: ConceptSelectionResponse = run_prompt(  # type: ignore
-        SelectionPromptCase(concepts=output, question=input_text),
+        SelectionPromptCase(concept_names=concept_candidates, question=input_text),
         debug=debug,
         session_uuid=session_uuid,
         log_info=log_info,
     )
-    final = list(set(selections.matches))
+    selected_concepts = list(set(selections.matches))
 
-    for item in parsed.filtering:
-        instance = input_environment.concepts[item.concept]
-        if instance.metadata:
-            item.values = run_prompt(  # type: ignore
-                FilterRefinementCase(
-                    values=item.values,
-                    description=instance.metadata.description,
-                ),
-                debug=debug,
-                session_uuid=session_uuid,
-                log_info=log_info,
-            ).new_values
+    for selection in selected_concepts:
+        if selection not in env_concepts:
+            raise ValueError(
+                f"Returned concept {selection} that does not actually exist in environment!"
+            )
+
+    # DETERMINISTIC: map phrases to final concepts
+    phrase_to_concept_map: dict[str, Concept] = {}
+    for key, tokens in global_phrase_token_map.items():
+        mapped = tokens_to_concept(concepts=selected_concepts, tokens=tokens, limits=1)
+        if mapped:
+            phrase_to_concept_map[key] = env_concepts[mapped[0]]
+
+    final_ordering = [
+        FinalOrderResult(
+            concept=phrase_to_concept_map[order.concept], order=order.order
+        )
+        for order in parsed.order
+        if phrase_to_concept_map[order.concept]
+    ]
 
+    final_filters_pre = [
+        FinalFilterResult(
+            concept=phrase_to_concept_map[filter.concept],
+            operator=filter.operator,
+            values=filter.values,
+        )
+        for filter in parsed.filtering
+    ]
+
+    # LLM: enrich filter values
+    for item in final_filters_pre:
+        enrich_filter(item, log_info=log_info, session_uuid=session_uuid)
+    # DETERMINISTIC: return results
     return IntermediateParseResults(
-        select=final,
+        select=[env_concepts[c] for c in selected_concepts],
         limit=parsed.limit or 20,
-        order=parsed.order,
-        filtering=parsed.filtering,
+        order=final_ordering,
+        filtering=final_filters_pre,
     )
 
 
 def safe_limit(input: int | None) -> int:
     if not input:
         return DEFAULT_LIMIT
     if input in (-1, 0):
         return DEFAULT_LIMIT
     return input
 
 
-def safe_parse_order_item(
-    input: OrderResult, input_concepts: List[Concept]
-) -> OrderItem | None:
-    matched = [c for c in input_concepts if input.concept in c.address]
-    if not matched:
-        return None
-    try:
-        order = input.order
-    except Exception:
-        return None
-    return OrderItem(expr=matched[0], order=order)
-
-
 def parse_order(
-    input_concepts: List[Concept], ordering: List[OrderResult] | None
+    input_concepts: List[Concept], ordering: List[FinalOrderResult] | None
 ) -> OrderBy:
     default_order = [
         OrderItem(expr=c, order=Ordering.DESCENDING)
         for c in input_concepts
         if c.purpose == Purpose.METRIC
     ]
     if not ordering:
         return OrderBy(default_order)
     final = []
     for order in ordering:
-        parsed = safe_parse_order_item(order, input_concepts)
-        if parsed:
-            final.append(parsed)
+        final.append(OrderItem(expr=order.concept, order=order.order))
     return OrderBy(items=final)
 
 
-def parse_filter(
-    input: FilterResult, input_concepts: List[Concept]
-) -> Comparison | None:
-    matched = [c for c in input_concepts if input.concept in c.address]
-    if not matched:
-        return None
+def parse_filter(input: FinalFilterResult) -> Comparison | None:
     return Comparison(
-        left=matched[0],
+        left=input.concept,
         right=input.values[0] if len(input.values) == 1 else input.values,
         operator=input.operator,
     )
 
 
-def parse_filtering(
-    input_concepts: List[Concept], filtering: List[FilterResult]
-) -> WhereClause | None:
+def parse_filtering(filtering: List[FinalFilterResult]) -> WhereClause | None:
     base = []
     for item in filtering:
-        parsed = parse_filter(item, input_concepts)
+        parsed = parse_filter(item)
         if parsed:
             base.append(parsed)
     if not base:
         return None
     if len(base) == 1:
         return WhereClause(conditional=base[0])
     left: Conditional | Comparison = base.pop()
@@ -294,27 +268,29 @@
 
 def parse_query(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
     log_info: bool = True,
 ):
-    results = discover_inputs(
+    intermediate_results = discover_inputs(
         input_text, input_environment, debug=debug, log_info=log_info
     )
-    concepts = [input_environment.concepts[x] for x in results.select]
-    order = parse_order(concepts, results.order)
-    filtering = parse_filtering(concepts, results.filtering)
+    order = parse_order(intermediate_results.select, intermediate_results.order)
+
+    filtering = parse_filtering(intermediate_results.filtering)
+    # from preql.core.models import unique
+    # concepts = unique(concepts, 'address')
     if debug:
         print("Concepts found")
-        for c in concepts:
+        for c in intermediate_results.select:
             print(c.address)
     query = Select(
-        selection=concepts,
-        limit=safe_limit(results.limit),
+        selection=unique(intermediate_results.select, "address"),
+        limit=safe_limit(intermediate_results.limit),
         order_by=order,
         where_clause=filtering,
     )
     return query
 
 
 def build_query(
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/models.py` & `pypreql-nlp-0.0.8/preql_nlp/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 from pydantic import BaseModel
-from preql.core.enums import ComparisonOperator
-from preql.core.enums import Ordering
+from preql.core.enums import ComparisonOperator, Ordering
+from preql.core.models import Concept
 
-''''- metrics: a list of concepts from the question that should be aggregated
-- dimensions: a list of concepts from the question which are not metrics
-- limit: a number of records to limit the results to, -1 if none specified
-- order: a list of fields to order the results by, with the option to specify ascending or descending
-- filtering: a list of criteria to restrict the results by'''
-
-class TokenInputs(BaseModel):
-    """The inputs to the tokenization prompt"""
-    metrics:list[str]
-    dimensions:list[str]
-    order:list[str]
-    filtering:list[str]
+### Intermediate Models
 
 class FilterResult(BaseModel):
     """The result of the filter prompt"""
     concept:str
     values:list[str]
     operator:ComparisonOperator
 
+
+class FinalFilterResult(BaseModel):
+    concept:Concept
+    values:list[str]
+    operator:ComparisonOperator
+
 class OrderResult(BaseModel):
     """The result of the order prompt"""
     concept:str
     order: Ordering
 
+class FinalOrderResult(BaseModel):
+    """The processed result of the order prompt"""
+    concept:Concept
+    order: Ordering
+
 class InitialParseResponse(BaseModel):
     """The result of the initial parse"""
     metrics:list[str]
     dimensions:list[str]
     limit:int
     order:list[OrderResult]
     filtering:list[FilterResult]
 
     @property
     def selection(self)->list[str]:
         filtering = [f.concept for f in self.filtering]
         order = [x.concept for x in self.order]
-        return self.metrics + self.dimensions + filtering + order
+        return list(set(self.metrics + self.dimensions + filtering + order))
+
+
+class IntermediateParseResults(BaseModel):
+    select: list[Concept]
+    limit: int
+    order: list[FinalOrderResult]
+    filtering:list[FinalFilterResult]
 
 
+### Parse Result Models
+
 class SemanticTokenMatch(BaseModel):
     phrase: str
     tokens: list[str]
 
 class SemanticTokenResponse(BaseModel):
     __root__:list[SemanticTokenMatch]
 
@@ -55,19 +64,11 @@
         return self.__root__.__getitem__(idx)
 
 class ConceptSelectionResponse(BaseModel):
     matches:list[str]
     reasoning:str
 
 
-
-class IntermediateParseResults(BaseModel):
-    select: list[str]
-    limit: int
-    order: list[OrderResult]
-    filtering:list[FilterResult]
-
-
 class FilterRefinementResponse(BaseModel):
     new_values:list[str]
     old_values:list[str]
     reasoning:str
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.8/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_executor.py` & `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_executor.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from typing import List, Optional, Callable, Union, Type, overload
 import uuid
 import json
 import os
 from jinja2 import FileSystemLoader, Environment, Template
 from os.path import dirname
 
+PROMPT_STOPWORD = "<EOM>"
+
 loader = FileSystemLoader(searchpath=dirname(__file__))
 templates = Environment(loader=loader)
 
 
 def gen_hash(obj, keys: set[str]) -> str:
     """Generate a deterministic hash for an object across multiple runs"""
     import hashlib
@@ -45,53 +47,83 @@
 
     return m.digest().hex()
 
 
 class BasePreqlPromptCase(TemplatedPromptCase):
     parse_model: Type[BaseModel]
     template: Template
+    stopword = PROMPT_STOPWORD
 
     def __init__(
         self,
         category: str,
         fail_on_parse_error: bool = True,
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
-        super().__init__(category=category, evaluators=evaluators)
+        # this isn't actually the right way to pass through a stopword to the complete prompt
+        # so we're splitting in the response
+        # TODO: figure out how to do this when we figure out how to group prompts in one API call
+        super().__init__(
+            category=category,
+            evaluators=evaluators,
+            prompt_executor_kwargs={"stopword": PROMPT_STOPWORD},
+        )
         self._prompt_hash = str(uuid.uuid4())
         self.parsed = None
         self.fail_on_parse_error = fail_on_parse_error
+        self.retry_prompt = "User: That response was incorrectly formatted. Please return the same content as the first response with formatting fixed (eg. valid JSON) to conform with original request. System:\n"
         self.stash: BaseCache = SqlliteCache()
 
+    @classmethod
+    def parse_response(cls, response: str):
+        return cls.parse_model.parse_raw(response.split(cls.stopword)[0])
+
+    # def get_prompt_executor(self):
+    #     from langchain.chat_models import ChatOpenAI
+
+    #     model_name = os.environ.get("OPENAI_MODEL") or "text-davinci-003"
+    #     openai_api_key = os.environ.get("OPENAI_API_KEY")
+    #     self.prompt_executor_kwargs = {"model_name": model_name}
+    #     return ChatOpenAI(model_name=model_name, openai_api_key=openai_api_key)
+    #     # return ChatOpenAI()
+
     @retry_with_exponential_backoff
-    def execute_prompt(self, prompt_str):
+    def execute_prompt(self, prompt_str, skip_cache: bool = False):
         # if we already have a local result
         # skip hitting remote
         # TODO: make the cache provider pluggable and injected
         hash_val = gen_hash(self, self.attributes_used_for_hash)
         resp = self.stash.retrieve(hash_val)
-        if resp:
+        if resp and not skip_cache:
             self.response = resp
             return self.response
         self.response = self.prompt_executor(prompt_str)
-        self.stash.stash(hash_val, self.category, self.response)
+        self.stash.store(hash_val, self.category, self.response)
         return self.response
 
     def get_extra_template_context(self):
-        raise NotImplementedError("This class can't be used directly.")
+        return {"stopword": self.stopword}
+
+    def rerun(self):
+        self.prompt = self.prompt + self.response + "\n" + self.retry_prompt
+        self.execute_prompt(self.prompt, skip_cache=True)
 
     def post_run(self):
         try:
-            self.parsed = self.parse_model.parse_raw(self.response)
+            self.parsed = self.parse_response(self.response)
         except ValidationError as e:
-            print(self.render())
-            print("was unable to parse response using ", str(self.parse_model))
-            print(self.response)
-            if self.fail_on_parse_error:
-                raise e
+            self.rerun()
+            try:
+                self.parsed = self.parse_response(self.response)
+            except ValidationError:
+                print(self.render())
+                print("was unable to parse response using ", str(self.parse_model))
+                print(self.response)
+                if self.fail_on_parse_error:
+                    raise e
 
     def render(
         self,
     ):
         return self.template.render(**self.jinja_context)
 
 
@@ -106,15 +138,15 @@
         question: str,
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
         self.question = question
         super().__init__(category="semantic_extraction", evaluators=evaluators)
 
     def get_extra_template_context(self):
-        return {"question": self.question}
+        return {**super().get_extra_template_context(), "question": self.question}
 
 
 class SemanticToTokensPromptCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_semantic_to_tokens.jinja2")
     parse_model = SemanticTokenResponse
 
     attributes_used_for_hash = {"tokens", "phrases", "category", "template"}
@@ -122,44 +154,49 @@
     def __init__(
         self,
         tokens: List[str],
         phrases: List[str],
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
         self.tokens = sorted(tokens)
-        self.phrases = sorted(phrases)
+        # we need to ensure that we always have a list
+        # for chat-gpt to understand the prompt properly
+        # pad out the inputs with a random phrase
+        self.phrases = sorted(phrases + ["democratic elections"])
         super().__init__(category="semantic_to_tokens", evaluators=evaluators)
 
     def get_extra_template_context(self):
         return {
-            "tokens": ", ".join([f'"{c}"' for c in self.tokens]),
+            **super().get_extra_template_context(),
+            "tokens": ", ".join([f'"{c}"' for c in self.tokens if c]),
             "phrase_str": ", ".join([f'"{c}"' for c in self.phrases]),
         }
 
 
 class SelectionPromptCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_final_concepts.jinja2")
     parse_model = ConceptSelectionResponse
 
-    attributes_used_for_hash = {"question", "concepts", "category", "template"}
+    attributes_used_for_hash = {"question", "concept_names", "category", "template"}
 
     def __init__(
         self,
         question: str,
-        concepts: List[str],
+        concept_names: List[str],
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
         self.question = question
-        self.concepts = sorted(list(set(concepts)), key=lambda x: x)
+        self.concept_names = sorted(list(set(concept_names)), key=lambda x: x)
         super().__init__(evaluators=evaluators, category="selection")
         self.execution.score = None
 
     def get_extra_template_context(self):
         return {
-            "concept_string": ", ".join([f'"{c}"' for c in self.concepts]),
+            **super().get_extra_template_context(),
+            "concept_string": ", ".join([f'"{c}"' for c in self.concept_names]),
             "question": self.question,
         }
 
 
 class FilterRefinementCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_refine_filter.jinja2")
     parse_model = FilterRefinementResponse
@@ -174,14 +211,15 @@
     ):
         self.values = values
         self.description = description
         super().__init__(evaluators=evaluators, category="filter_refinement")
 
     def get_extra_template_context(self):
         return {
+            **super().get_extra_template_context(),
             "values": ", ".join([f'"{x}"' for x in self.values]),
             "description": self.description,
         }
 
 
 DATA_DIR = os.path.join(
     os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log_data"
@@ -212,15 +250,15 @@
                 os.path.join(DATA_DIR, str(session_uuid), prompt_hash + ".json")
             )
         )
         json.dump(data, f)
 
 
 @overload
-def run_prompt( # type: ignore
+def run_prompt(  # type: ignore
     prompt: SelectionPromptCase,
     debug: bool = False,
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
 ) -> ConceptSelectionResponse:
     ...
 
@@ -242,15 +280,15 @@
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
 ) -> SemanticTokenResponse:
     ...
 
 
 @overload
-def run_prompt( # type: ignore
+def run_prompt(  # type: ignore
     prompt: FilterRefinementCase,
     debug: bool = False,
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
 ) -> FilterRefinementResponse:
     ...
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_final_concepts.jinja2` & `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_final_concepts.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 * only return concepts provided by the user
 * concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
 * return the concepts that together best match the user question
 * reason about each match step by step, e.g. "first match the concept 'product' to the word 'product' in the question, then match the concept 'revenue' to the word 'revenue' in the question, and together these enable aggregating revenue by year"
 The output should be a VALID JSON blob with the following keys and values:
 * matches: a list of concepts from the user provided list that together best match the 
 * reasoning: a string explaining your step by step reasoning for the matches
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what product colors had the most revenue in 2024?"]
+
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what color products were the top sellers by revenue in 2024?"]
 System:
 {% raw %}{"matches": ["product.color", "order.revenue.sum", "order.year" ],
-"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color. Order year is required to filter to 2024." }
+"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color to determine the top. Order year is required to filter to 2024." }
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
 System:
 {"matches": ["order.state", "order.revenue.sum"],
 "reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
 System:
 {"matches": ["order.state", "order.revenue.avg"],
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2` & `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 System: You are a helpful AI that translates ambiguous business questions into structured outputs.
 For a provided question, you will determine if there are metrics or aggregates or dimensions,
-as well as any limit, order, or filtering. 
+as well as any limit, order, or filtering information required to accurately respond. 
 
-The output should be a VALID JSON blob with the following keys and values:
+
+The output should be a VALID JSON blob with the following keys and values followed by {{ stopword }}:
 - metrics: a list of concepts from the question that should be aggregated
 - dimensions: a list of concepts from the question which are not metrics
 - limit: a number of records to limit the results to, -1 if none specified
 - order: a list of  objects to order the results by, with the option to specify ascending or descending
 -- concept: a concept to order by
 -- order: the direction of ordering, "asc" or "desc"
 - filtering: a list of objects to filter the results on, where each object has the following keys:
 -- concept: a concept to filter on
 -- values: the value the concept is filtered to
--- operator: the comparison operator, one of "=", "in", "<", ">", "<=", or ">=". A between should be expressed as two inequalities. 
+-- operator: the comparison operator, one of "=", "in", "<", ">", "<=", "like", or ">=". A range, or between, should be expressed as two inequalities. 
 
+User: "How many people who love the color pink played frisbee on saturday??"
+System:
+{% raw %}{
+"metrics":["people count"],
+"dimensions": [],
+"limit": -1,
+"order": [],
+"filtering": [{"concept":"favorite color", "operator": "=", "values":["Pink"]}, {"concept":"day of week", "operator": "=", "values":["Saturday"]}, {"concept":"game played", "operator": "=", "values":["frisbee"]}]
+}{% endraw %}{{ stopword }}
 
 User: "What are the top 10 products by sales?"
 System:
 {% raw %}{
 "metrics":["sales"],
 "dimensions": ["products"],
 "limit": 10,
 "order": [{"concept":"sales", "order":"desc"}],
 "filtering": []
-}
+}{% endraw %}{{ stopword }}
 
 User: "What are the sales by line of business and state?"
-System:
+System:{% raw %}
 {
-"metrics":["average sales"],
+"metrics":["sales"],
 "dimensions": ["line of business", "state"],
 "limit": -1,
 "order": [],
 "filtering": []
-}
+}{% endraw %}{{ stopword }}
 
 User: "What is the average sales by state in the states of Wyoming and Texas?"
-System:
+System:{% raw %}
 {
 "metrics":["average sales"],
 "dimensions": ["state"],
 "limit": -1,
 "order": [],
 "filtering": [{"concept":"state", "operator": "in", "values":["Wyoming", "Texas"]}]
-}
+}{% endraw %}{{ stopword }}
 
-User: "What were sales between 2001 and 2020 in order of year?"
-System:
+User: "What were top selling products between 2001 and 2020 in order of year?"
+System:{% raw %}
 {
-"metrics":["sales"],
-"dimensions": ["year"],
+"metrics":["top selling"],
+"dimensions": ["year", "products"],
 "limit": -1,
 "order": [{"concept":"year", "order":"asc"}],
 "filtering": [{"concept":"year", "operator":">=", "values":["2001"]}, {"concept":"year", "operator":"<=", "values":["2020"]}]
-}{% endraw %}
+}{% endraw %}{{ stopword }}
 
 User: "{{ question }}"
 System:
```

### Comparing `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_refine_filter.jinja2` & `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_refine_filter.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 }
 {% endraw %}
 User: given the values ["Blue", "Red"], transform to match the following description: "An integer enum of colors. 1 = RED, 2 = BLUE, 3 = GREEN, 4 = YELLOW "
 System:
 {% raw %}
 {"new_values": [2, 1],
 "old_values": ["Blue", "Red"],
-"reasoning": "Tthe field is described as an enum mapping integers to colors. Blue is described as mapping to 2, and red to 1."
+"reasoning": "The field is described as an enum mapping integers to colors. Blue is described as mapping to 2, and red to 1."
 }
 {% endraw %}
 User: Given the values [{{ values }}], transform to match the following description: "{{ description }}"
 System:
```

### Comparing `pypreql-nlp-0.0.7/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.8/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.7
+Version: 0.0.8
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.7/pypreql_nlp.egg-info/SOURCES.txt` & `pypreql-nlp-0.0.8/pypreql_nlp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 preql_nlp/__init__.py
 preql_nlp/constants.py
 preql_nlp/helpers.py
 preql_nlp/main.py
 preql_nlp/models.py
 preql_nlp/monkeypatch.py
+preql_nlp/tokenization.py
 preql_nlp/cache_providers/__init__.py
 preql_nlp/cache_providers/base.py
 preql_nlp/cache_providers/local_sqlite.py
 preql_nlp/prompts/__init__.py
 preql_nlp/prompts/prompt_executor.py
 preql_nlp/prompts/prompt_final_concepts.jinja2
 preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
```

### Comparing `pypreql-nlp-0.0.7/setup.py` & `pypreql-nlp-0.0.8/setup.py`

 * *Files identical despite different names*

