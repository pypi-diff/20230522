# Comparing `tmp/transformer_smaller_training_vocab-0.2.3.tar.gz` & `tmp/transformer_smaller_training_vocab-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_smaller_training_vocab-0.2.3.tar", max compression
+gzip compressed data, was "transformer_smaller_training_vocab-0.2.4.tar", max compression
```

## Comparing `transformer_smaller_training_vocab-0.2.3.tar` & `transformer_smaller_training_vocab-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-03-25 14:34:50.115062 transformer_smaller_training_vocab-0.2.3/LICENSE
--rw-r--r--   0        0        0     6918 2023-03-25 14:34:50.115062 transformer_smaller_training_vocab-0.2.3/README.md
--rw-r--r--   0        0        0     1666 2023-03-25 14:36:11.143247 transformer_smaller_training_vocab-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      220 2023-03-25 14:34:50.115062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/__init__.py
--rw-r--r--   0        0        0     2608 2023-03-25 14:34:50.115062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/contextual_reduce.py
--rw-r--r--   0        0        0      154 2023-03-25 14:34:50.115062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/logging_utils.py
--rw-r--r--   0        0        0     2444 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/modify_model.py
--rw-r--r--   0        0        0      719 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/modify_tokenizer.py
--rw-r--r--   0        0        0        0 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/py.typed
--rw-r--r--   0        0        0      756 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/token_stats.py
--rw-r--r--   0        0        0      717 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py
--rw-r--r--   0        0        0     1520 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py
--rw-r--r--   0        0        0      573 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py
--rw-r--r--   0        0        0     3452 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py
--rw-r--r--   0        0        0      479 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_roberta.py
--rw-r--r--   0        0        0      546 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py
--rw-r--r--   0        0        0      802 2023-03-25 14:34:50.119062 transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/utils.py
--rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 transformer_smaller_training_vocab-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-22 13:19:12.829801 transformer_smaller_training_vocab-0.2.4/LICENSE
+-rw-r--r--   0        0        0     6918 2023-05-22 13:19:12.829801 transformer_smaller_training_vocab-0.2.4/README.md
+-rw-r--r--   0        0        0     2790 2023-05-22 13:19:55.574382 transformer_smaller_training_vocab-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/__init__.py
+-rw-r--r--   0        0        0     7713 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/contextual_reduce.py
+-rw-r--r--   0        0        0      154 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/logging_utils.py
+-rw-r--r--   0        0        0     2444 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/modify_model.py
+-rw-r--r--   0        0        0      719 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/modify_tokenizer.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/py.typed
+-rw-r--r--   0        0        0      756 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/token_stats.py
+-rw-r--r--   0        0        0      716 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py
+-rw-r--r--   0        0        0      566 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py
+-rw-r--r--   0        0        0     3444 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py
+-rw-r--r--   0        0        0      472 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_roberta.py
+-rw-r--r--   0        0        0      539 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py
+-rw-r--r--   0        0        0     1115 2023-05-22 13:19:12.833801 transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/utils.py
+-rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 transformer_smaller_training_vocab-0.2.4/PKG-INFO
```

### Comparing `transformer_smaller_training_vocab-0.2.3/LICENSE` & `transformer_smaller_training_vocab-0.2.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Benedikt Fuchs
+Copyright (c) 2023 Benedikt Fuchs
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `transformer_smaller_training_vocab-0.2.3/README.md` & `transformer_smaller_training_vocab-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/modify_model.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/modify_model.py`

 * *Files identical despite different names*

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/modify_tokenizer.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/modify_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict
+from typing import Dict, List
 
 from transformers import PreTrainedTokenizer
 
 from transformer_smaller_training_vocab.transformer_set_vocab import set_vocab
 
 
 def reduce_tokenizer(tokenizer: PreTrainedTokenizer, used_token_ids: List[int]) -> Dict[str, int]:
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/token_stats.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/token_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Union, List, Sequence
+from typing import List, Sequence, Union
 
 from transformers import PreTrainedTokenizer
-from transformers.tokenization_utils_base import TextInput, PreTokenizedInput, TextInputPair, PreTokenizedInputPair
+from transformers.tokenization_utils_base import PreTokenizedInput, PreTokenizedInputPair, TextInput, TextInputPair
 
 
 def get_token_stats(
     tokenizer: PreTrainedTokenizer,
     texts: Sequence[Union[TextInput, PreTokenizedInput, TextInputPair, PreTokenizedInputPair]],
 ) -> List[int]:
     used = set()
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from transformer_smaller_training_vocab.transformer_set_vocab.auto_set_vocab import register_set_vocab, set_vocab
 from transformer_smaller_training_vocab.transformer_set_vocab.set_vocab_bert import set_bert_vocab
 from transformer_smaller_training_vocab.transformer_set_vocab.set_vocab_fast_tokenizer import set_fast_tokenizer_vocab
 from transformer_smaller_training_vocab.transformer_set_vocab.set_vocab_roberta import set_roberta_vocab
 from transformer_smaller_training_vocab.transformer_set_vocab.set_vocab_xlm_roberta import set_xlm_roberta_vocab
 
-
 __all__ = [
     "register_set_vocab",
     "set_vocab",
     "set_xlm_roberta_vocab",
     "set_roberta_vocab",
     "set_bert_vocab",
     "set_fast_tokenizer_vocab",
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/auto_set_vocab.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, TypeVar, Dict, Callable
+from typing import Callable, Dict, Type, TypeVar
 
 from transformers import PreTrainedTokenizer
 
 TOK = TypeVar("TOK", bound=PreTrainedTokenizer)
 TOK_FUNCTION = Callable[[TOK, Dict[str, int]], None]
 
 tokenizer_set_vocab_functions: Dict[Type[TOK], Callable[[TOK, Dict[str, int]], None]] = {}  # type: ignore[valid-type]
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 
 @register_set_vocab(BertTokenizer)
 def set_bert_vocab(tokenizer: BertTokenizer, vocab: Dict[str, int]) -> None:
     tokenizer.ids_to_tokens = collections.OrderedDict([(ids, tok) for tok, ids in vocab.items()])
     tokenizer.vocab = vocab
     tokenizer.wordpiece_tokenizer.vocab = vocab
-    tokenizer.added_tokens_encoder = {k: vocab[k] for k in tokenizer.added_tokens_encoder.keys()}
+    tokenizer.added_tokens_encoder = {k: vocab[k] for k in tokenizer.added_tokens_encoder}
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_fast_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
-from typing import Dict, Callable, Any
+from typing import Any, Callable, Dict
 
 from tokenizers import Tokenizer
 from transformers import PreTrainedTokenizerFast
 
 from transformer_smaller_training_vocab.transformer_set_vocab.auto_set_vocab import register_set_vocab
 
-
 SET_VOCAB_FUNCTION = Callable[[Dict[str, Any], Dict[str, int]], None]
 
 vocab_functions: Dict[str, SET_VOCAB_FUNCTION] = {}
 
 
 def register_vocab_function(name: str) -> Callable[[SET_VOCAB_FUNCTION], SET_VOCAB_FUNCTION]:
     def _decorator(fn: SET_VOCAB_FUNCTION) -> SET_VOCAB_FUNCTION:
@@ -73,12 +72,12 @@
 @register_vocab_function("BPE")
 def set_bpe_vocab(tokenizer_obj: Dict[str, Any], vocab: Dict[str, int]) -> None:
     # bpe tokenizer save merges next to the vocabulary and requires tokens for correct validation.
     # hence we don't delete tokens, but reorder them, so that the ids fit the requirement.
     old_vocab = tokenizer_obj["model"]["vocab"]
 
     new_vocab = vocab
-    for k in old_vocab.keys():
+    for k in old_vocab:
         if k not in new_vocab:
             new_vocab[k] = len(new_vocab)
 
     tokenizer_obj["model"]["vocab"] = new_vocab
```

### Comparing `transformer_smaller_training_vocab-0.2.3/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py` & `transformer_smaller_training_vocab-0.2.4/transformer_smaller_training_vocab/transformer_set_vocab/set_vocab_xlm_roberta.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from transformer_smaller_training_vocab.transformer_set_vocab.auto_set_vocab import register_set_vocab
 
 
 @register_set_vocab(XLMRobertaTokenizer)
 def set_xlm_roberta_vocab(tokenizer: XLMRobertaTokenizer, vocab: Dict[str, int]) -> None:
     tokenizer.fairseq_tokens_to_ids = vocab
     tokenizer.fairseq_ids_to_tokens = {v: k for k, v in tokenizer.fairseq_tokens_to_ids.items()}
-    tokenizer.added_tokens_encoder = {k: vocab[k] for k in tokenizer.added_tokens_encoder.keys()}
+    tokenizer.added_tokens_encoder = {k: vocab[k] for k in tokenizer.added_tokens_encoder}
```

### Comparing `transformer_smaller_training_vocab-0.2.3/PKG-INFO` & `transformer_smaller_training_vocab-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformer-smaller-training-vocab
-Version: 0.2.3
+Version: 0.2.4
 Summary: Temporary remove unused tokens during training to save ram and speed.
 Home-page: https://github.com/helpmefindaname/transformer-smaller-training-vocab
 License: MIT
 Author: Benedikt Fuchs
 Author-email: benedikt.fuchs.staw@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

