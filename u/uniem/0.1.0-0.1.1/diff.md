# Comparing `tmp/uniem-0.1.0.tar.gz` & `tmp/uniem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.1.0.tar", max compression
+gzip compressed data, was "uniem-0.1.1.tar", max compression
```

## Comparing `uniem-0.1.0.tar` & `uniem-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-09 07:54:15.399692 uniem-0.1.0/LICENSE
--rw-r--r--   0        0        0      501 2023-05-12 10:14:33.536387 uniem-0.1.0/README.md
--rw-r--r--   0        0        0      586 2023-05-12 07:36:32.757911 uniem-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-05-12 10:16:25.758032 uniem-0.1.0/uniem/__init__.py
--rw-r--r--   0        0        0     4220 2023-05-09 10:57:19.511416 uniem-0.1.0/uniem/criteria.py
--rw-r--r--   0        0        0     3925 2023-05-10 09:35:44.683411 uniem-0.1.0/uniem/data.py
--rw-r--r--   0        0        0      430 2023-05-09 10:34:04.808537 uniem-0.1.0/uniem/data_structures.py
--rw-r--r--   0        0        0    10414 2023-05-12 10:15:37.987387 uniem-0.1.0/uniem/model.py
--rw-r--r--   0        0        0     5850 2023-05-10 03:05:23.472230 uniem-0.1.0/uniem/trainer.py
--rw-r--r--   0        0        0      348 2023-05-10 07:15:57.082768 uniem-0.1.0/uniem/types.py
--rw-r--r--   0        0        0      621 2023-05-10 07:07:11.507943 uniem-0.1.0/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-05-12 10:16:41.056944 uniem-0.1.0/uniem/version.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 uniem-0.1.0/setup.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 uniem-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 07:54:15.399692 uniem-0.1.1/LICENSE
+-rw-r--r--   0        0        0      598 2023-05-15 03:14:34.188003 uniem-0.1.1/README.md
+-rw-r--r--   0        0        0      607 2023-05-22 10:36:44.346256 uniem-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-05-12 10:16:25.758032 uniem-0.1.1/uniem/__init__.py
+-rw-r--r--   0        0        0     5950 2023-05-18 03:50:32.557213 uniem-0.1.1/uniem/criteria.py
+-rw-r--r--   0        0        0     8443 2023-05-22 06:43:10.136944 uniem-0.1.1/uniem/data.py
+-rw-r--r--   0        0        0      430 2023-05-09 10:34:04.808537 uniem-0.1.1/uniem/data_structures.py
+-rw-r--r--   0        0        0    11889 2023-05-22 10:36:08.591891 uniem-0.1.1/uniem/model.py
+-rw-r--r--   0        0        0     5850 2023-05-22 06:30:59.048879 uniem-0.1.1/uniem/trainer.py
+-rw-r--r--   0        0        0      680 2023-05-19 09:54:21.001026 uniem-0.1.1/uniem/types.py
+-rw-r--r--   0        0        0      621 2023-05-10 07:07:11.507943 uniem-0.1.1/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-05-22 10:36:54.260085 uniem-0.1.1/uniem/version.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 uniem-0.1.1/setup.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 uniem-0.1.1/PKG-INFO
```

### Comparing `uniem-0.1.0/LICENSE` & `uniem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.1.0/pyproject.toml` & `uniem-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "uniem"
-version = "0.1.0"
+version = "0.1.1"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 torch = "^2.0.0"
 transformers = "^4.28.0"
 accelerate = "^0.19.0"
 tqdm = "^4.65.0"
 typer = {extras = ["all"], version = "^0.9.0"}
+datasets = "^2.12.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 blue = "^0.9.1"
 ruff = "^0.0.265"
 isort = "^5.12.0"
```

### Comparing `uniem-0.1.0/uniem/criteria.py` & `uniem-0.1.1/uniem/criteria.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,59 +3,75 @@
 
 class ContrastLoss(torch.nn.Module):
     def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
 
 
-class PairSoftmaxContrastLoss(ContrastLoss):
-    def __init__(self, temperature: float = 0.05):
-        super().__init__()
-        self.temperature = temperature
-        self._cross_entropy_loss = torch.nn.CrossEntropyLoss()
-
+class PairCoSentLoss(ContrastLoss):
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
         sim_matrix = sim_matrix / self.temperature
-        labels = torch.arange(sim_matrix.size(0), device=text_embeddings.device, dtype=torch.long)
-        loss = self._cross_entropy_loss(sim_matrix, labels)
+        sim_matrix_diag = sim_matrix.diag()
+        sim_matrix_diff = sim_matrix - sim_matrix_diag.unsqueeze(1)
+        loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
         return loss
 
 
-class PairSigmoidContrastLoss(ContrastLoss):
+class TripletCoSentLoss(ContrastLoss):
+    def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
+        super().__init__(temperature)
+        self.add_swap_loss = add_swap_loss
+        if self.add_swap_loss:
+            self._pair_contrast_softmax_loss = PairCoSentLoss(temperature)
+        else:
+            self._pair_contrast_softmax_loss = None
+
+    def forward(
+        self,
+        text_embeddings: torch.Tensor,
+        text_pos_embeddings: torch.Tensor,
+        text_neg_embeddings: torch.Tensor,
+    ) -> torch.Tensor:
+        sim_pos_vector = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
+        sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
+        sim_matrix = torch.cat([sim_pos_vector.unsqueeze(1), sim_neg_matrix], dim=1)
+        sim_matrix = sim_matrix / self.temperature
+        sim_matrix_diff = sim_matrix - sim_matrix[:, 0].unsqueeze(1)
+        loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
+        if self._pair_contrast_softmax_loss:
+            loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
+        return loss
+
+
+class PairSoftmaxContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
+        self._cross_entropy_loss = torch.nn.CrossEntropyLoss()
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
-        batch_size = text_embeddings.size(0)
         sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
         sim_matrix = sim_matrix / self.temperature
-        sim_matrix_diag = sim_matrix.diag()
-
-        sim_diff_matrix = sim_matrix_diag.unsqueeze(1) - sim_matrix
-        diag_mask = torch.eye(sim_matrix.size(0), dtype=torch.bool, device=sim_matrix.device)
-        sim_diff_matrix = sim_diff_matrix.masked_fill(diag_mask, 1e9)
-
-        loss = -torch.log(torch.sigmoid(sim_diff_matrix)).sum() / (batch_size**2 - batch_size)
+        labels = torch.arange(sim_matrix.size(0), device=text_embeddings.device, dtype=torch.long)
+        loss = self._cross_entropy_loss(sim_matrix, labels)
         return loss
 
 
 class TripletSoftmaxContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
-        super().__init__()
-        self.temperature = temperature
+        super().__init__(temperature)
         self.add_swap_loss = add_swap_loss
         if self.add_swap_loss:
             self._pair_contrast_softmax_loss = PairSoftmaxContrastLoss(temperature)
         else:
             self._pair_contrast_softmax_loss = None
 
     def forward(
@@ -71,31 +87,54 @@
         labels = torch.zeros(sim_matrix.size(0), dtype=torch.long, device=sim_matrix.device)
         loss = torch.nn.CrossEntropyLoss()(sim_matrix, labels)
         if self._pair_contrast_softmax_loss:
             loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
         return loss
 
 
-class TripletSigmoidContrastLoss(ContrastLoss):
-    def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
+class PairSigmoidContrastLoss(ContrastLoss):
+    def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
+
+    def forward(
+        self,
+        text_embeddings: torch.Tensor,
+        text_pos_embeddings: torch.Tensor,
+    ) -> torch.Tensor:
+        batch_size = text_embeddings.size(0)
+        sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
+        sim_matrix = sim_matrix / self.temperature
+        sim_matrix_diag = sim_matrix.diag()
+
+        sim_diff_matrix = sim_matrix_diag.unsqueeze(1) - sim_matrix
+        diag_mask = torch.eye(sim_matrix.size(0), dtype=torch.bool, device=sim_matrix.device)
+        sim_diff_matrix = sim_diff_matrix.masked_fill(diag_mask, 1e9)
+
+        loss = -torch.log(torch.sigmoid(sim_diff_matrix)).sum() / (batch_size**2 - batch_size)
+        return loss
+
+
+class TripletSigmoidContrastLoss(ContrastLoss):
+    def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
+        super().__init__(temperature)
         self.add_swap_loss = add_swap_loss
         if self.add_swap_loss:
             self._pair_contrast_sigmoid_loss = PairSigmoidContrastLoss(temperature)
         else:
             self._pair_contrast_sigmoid_loss = None
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
         text_neg_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_pos_vector = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
+        sim_pos_vector = sim_pos_vector / self.temperature
         sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
+        sim_neg_matrix = sim_neg_matrix / self.temperature
         sim_diff_matrix = sim_pos_vector.unsqueeze(1) - sim_neg_matrix
-        sim_diff_matrix = sim_diff_matrix / self.temperature
         loss = -torch.log(torch.sigmoid(sim_diff_matrix)).mean()
         if self._pair_contrast_sigmoid_loss:
             loss += self._pair_contrast_sigmoid_loss(text_pos_embeddings, text_embeddings)
         return loss
```

### Comparing `uniem-0.1.0/uniem/model.py` & `uniem-0.1.1/uniem/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,38 +9,58 @@
 from transformers import AutoConfig, AutoModel, AutoTokenizer, PreTrainedModel
 
 from uniem.criteria import (
     PairSigmoidContrastLoss,
     PairSoftmaxContrastLoss,
     TripletSigmoidContrastLoss,
     TripletSoftmaxContrastLoss,
+    PairCoSentLoss,
+    TripletCoSentLoss,
 )
 from uniem.types import Tokenizer
 
 T = TypeVar('T')
 
 
 class EmbeddingStrategy(str, Enum):
     cls = 'cls'
     last_mean = 'last_mean'
     first_last_mean = 'first_last_mean'
     embedding_last_mean = 'embedding_last_mean'
+    last_weighted = 'last_weighted'
+
+
+class LossType(str, Enum):
+    sigmoid = 'sigmoid'
+    softmax = 'softmax'
+    cosent = 'cosent'
 
 
 def creat_mask_from_input_ids(input_ids: torch.Tensor, pad_token_id: int) -> torch.Tensor:
     return input_ids != pad_token_id
 
 
 def mean_pooling(hidden_state: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
     if mask is None:
         return torch.mean(hidden_state, dim=1)
     mask = mask.float()
     return torch.sum(hidden_state * mask.unsqueeze(-1), dim=1) / torch.sum(mask, dim=-1, keepdim=True)
 
 
+def load_hf_pretrained_model(model_name_or_path: str) -> PreTrainedModel:
+    config = AutoConfig.from_pretrained(model_name_or_path)
+    if config.model_type == 't5':
+        from transformers import T5EncoderModel
+
+        pretrained_model = T5EncoderModel.from_pretrained(model_name_or_path)
+    else:
+        pretrained_model = AutoModel.from_pretrained(model_name_or_path)
+    return pretrained_model  # type: ignore
+
+
 StrategyEmbedderClsMap: dict[EmbeddingStrategy, Type['Embedder']] = {}
 
 
 class Embedder(torch.nn.Module):
     embedding_strategy: ClassVar[EmbeddingStrategy]
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
@@ -62,16 +82,16 @@
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         raise NotImplementedError
 
     def save_pretrained(self, path: str | Path):
         self.encoder.save_pretrained(path)
 
     @classmethod
-    def from_pretrained(cls, path: str | Path):
-        encoder = AutoModel.from_pretrained(path)
+    def from_pretrained(cls, model_name_or_path: str):
+        encoder = load_hf_pretrained_model(model_name_or_path)
         return cls(encoder)
 
     @property
     def max_length(self):
         return self.encoder.config.max_position_embeddings
 
 
@@ -86,16 +106,14 @@
         return embeddings
 
 
 class ClsEmbedder(Embedder):
     embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.cls
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        if mask is None:
-            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids).last_hidden_state[:, 0]
         return embeddings
 
 
 class FirstLastEmbedder(Embedder):
     embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.first_last_mean
 
@@ -121,114 +139,117 @@
             mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
         static_embeddings = self.embedding_layer(input_ids)
         mean_last_embeddings = mean_pooling(self.encoder(input_ids).last_hidden_state, mask)
         mean_static_embeddings = mean_pooling(static_embeddings, mask)
         return (mean_last_embeddings + mean_static_embeddings) / 2
 
 
+class LastWeightedEmbedder(Embedder):
+    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.last_weighted
+
+    def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
+        super().__init__(encoder, pad_token_id)
+        self.embedding_layer = self.encoder.get_input_embeddings()
+
+    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
+        if mask is None:
+            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
+        weights = (torch.arange(input_ids.shape[1], device=input_ids.device) + 1).float()
+        embeddings = self.encoder(input_ids).last_hidden_state
+        embeddings = embeddings * mask.unsqueeze(-1).float() * weights.unsqueeze(0).unsqueeze(-1)
+        embeddings = torch.sum(embeddings, dim=1) / torch.sum(weights * mask, dim=-1, keepdim=True)
+        return embeddings
+
+
 class AutoEmbedder:
     @classmethod
-    def from_pretrained(cls, path: str | Path):
-        config = AutoConfig.from_pretrained(path)
-        if config.model_type == 't5':
-            from transformers import T5EncoderModel
-
-            encoder = T5EncoderModel.from_pretrained(path)
-        else:
-            encoder = AutoModel.from_pretrained(path)
-        encoder = cast(PreTrainedModel, encoder)
+    def from_pretrained(cls, model_name_or_path: str | Path):
+        encoder = load_hf_pretrained_model(str(model_name_or_path))
         embedder_cls = StrategyEmbedderClsMap[EmbeddingStrategy(encoder.config.uniem_embedding_strategy)]
         return embedder_cls(encoder)
 
 
 class EmbedderForTrain(torch.nn.Module):
-    def __init__(self, embedder: Embedder, chunk_size: int = 8):
+    def __init__(self, embedder: Embedder):
         super().__init__()
         self.embedder = embedder
-        self.chunk_size = chunk_size
-
-    def chunk_embedder_forward(self, input_ids: torch.Tensor) -> torch.Tensor:
-        num_chunks = (input_ids.size(0) // self.chunk_size) + 1
-        if num_chunks <= 1:
-            return self.embedder(input_ids)
-
-        chunks = torch.chunk(input_ids, num_chunks, dim=0)
-        embeddings = [self.embedder(chunk) for chunk in chunks]
-        embeddings = torch.cat(embeddings, dim=0)
-        return embeddings
 
 
 class EmbedderForPairTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
         temperature: float = 0.05,
-        use_sigmoid: bool = False,
+        loss_type: LossType | str = LossType.softmax,
         embedding_strategy: EmbeddingStrategy | str = EmbeddingStrategy.last_mean,
-        chunk_size: int = 8,
     ):
-        pretrained_model = AutoModel.from_pretrained(model_name_or_path)
+        pretrained_model = load_hf_pretrained_model(model_name_or_path)
         embedder = StrategyEmbedderClsMap[EmbeddingStrategy(embedding_strategy)](pretrained_model)
-        super().__init__(embedder, chunk_size)
-        if use_sigmoid:
+        super().__init__(embedder)
+        loss_type = LossType(loss_type)
+        if loss_type == LossType.sigmoid:
             self.criterion = PairSigmoidContrastLoss(temperature)
-        else:
+        elif loss_type == LossType.softmax:
             self.criterion = PairSoftmaxContrastLoss(temperature)
+        elif loss_type == LossType.cosent:
+            self.criterion = PairCoSentLoss(temperature)
 
     def forward(self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pos_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings)
         return {'loss': loss}
 
 
 class EmbedderForTripletTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
         temperature: float = 0.05,
-        use_sigmoid: bool = False,
+        loss_type: LossType | str = LossType.softmax,
         embedding_strategy: EmbeddingStrategy | str = EmbeddingStrategy.last_mean,
-        chunk_size: int = 8,
+        add_swap_loss: bool = False,
     ):
-        pretrained_model = AutoModel.from_pretrained(model_name_or_path)
+        pretrained_model = load_hf_pretrained_model(model_name_or_path)
         embedder = StrategyEmbedderClsMap[EmbeddingStrategy(embedding_strategy)](pretrained_model)
-        super().__init__(embedder, chunk_size)
-        if use_sigmoid:
-            self.criterion = TripletSigmoidContrastLoss(temperature)
-        else:
-            self.criterion = TripletSoftmaxContrastLoss(temperature)
-        self.chunk_size = chunk_size
+        super().__init__(embedder)
+        loss_type = LossType(loss_type)
+        if loss_type == LossType.sigmoid:
+            self.criterion = TripletSigmoidContrastLoss(temperature, add_swap_loss)
+        elif loss_type == LossType.softmax:
+            self.criterion = TripletSoftmaxContrastLoss(temperature, add_swap_loss)
+        elif loss_type == LossType.cosent:
+            self.criterion = TripletCoSentLoss(temperature, add_swap_loss)
 
     def forward(
         self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor, text_neg_ids: torch.Tensor
     ) -> dict[str, torch.Tensor]:
-        text_embeddings = self.chunk_embedder_forward(text_ids)
-        text_pos_embeddings = self.chunk_embedder_forward(text_pos_ids)
-        text_neg_embeddings = self.chunk_embedder_forward(text_neg_ids)
+        text_embeddings = self.embedder(text_ids)
+        text_pos_embeddings = self.embedder(text_pos_ids)
+        text_neg_embeddings = self.embedder(text_neg_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings, text_neg_embeddings)
         return {'loss': loss}
 
 
 def generate_batch(data: Iterable[T], batch_size: int = 32) -> Generator[list[T], None, None]:
     iterator = iter(data)
     while batch := list(islice(iterator, batch_size)):
         yield batch
 
 
 class UniEmbedder:
     PROGRESS_BAR_THRESHOLD = 1000
 
-    def __init__(self, embedder: Embedder, tokenizer: Tokenizer, max_legnth: int | None = None, device: str | None = None):
+    def __init__(self, embedder: Embedder, tokenizer: Tokenizer, max_length: int | None = None, device: str | None = None):
         super().__init__()
         self.embedder = embedder.eval()
         if device:
             self.embedder = self.embedder.to(device)
         self.tokenizer = tokenizer
-        self.max_length = max_legnth or self.tokenizer.model_max_length
+        self.max_length = max_length or self.embedder.encoder.config.max_length
 
     def __call__(self, sentences: list[str], batch_size: int = 32):
         return self.encode(sentences, batch_size)
 
     def encode(self, sentences: list[str], batch_size: int = 32, progress_bar: Literal['auto'] | bool = 'auto'):
         embeddings: list[np.ndarray] = []
         if progress_bar == 'auto':
@@ -237,30 +258,44 @@
         for batch in tqdm.tqdm(
             generate_batch(sentences, batch_size),
             disable=not progress_bar,
             total=len(sentences) // batch_size,
             unit='batch',
             desc='Encoding',
         ):
-            input_ids = self.tokenizer(batch, padding=True, truncation=True, return_tensors='pt')['input_ids']
+            encodes = self.tokenizer(
+                batch,
+                padding=True,
+                truncation=True,
+                return_tensors='pt',
+                return_attention_mask=True,
+                max_length=self.max_length,
+            )
+
+            input_ids = encodes['input_ids']
             input_ids = cast(torch.Tensor, input_ids)
             input_ids = input_ids.to(self.embedder.encoder.device)
+
+            attention_mask = encodes['attention_mask']
+            attention_mask = cast(torch.Tensor, attention_mask)
+            attention_mask = attention_mask.to(self.embedder.encoder.device)
+
             with torch.inference_mode():
-                batch_embeddings = self.embedder(input_ids)
+                batch_embeddings = self.embedder(input_ids, mask=attention_mask)
                 batch_embeddings = cast(torch.Tensor, batch_embeddings)
             embeddings.extend([i.cpu().numpy() for i in batch_embeddings])
         return embeddings
 
     def encode_single(self, sentence: str):
         return self.encode([sentence])[0]
 
     @classmethod
-    def from_pretrained(cls, model_name_or_path: str, max_legnth: int | None = None, device: str | None = None):
+    def from_pretrained(cls, model_name_or_path: str, max_length: int | None = None, device: str | None = None):
         encoder = AutoEmbedder.from_pretrained(model_name_or_path)
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
         if device is None:
             device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        return cls(encoder, tokenizer, max_legnth=max_legnth, device=device)
+        return cls(encoder, tokenizer, max_length=max_length, device=device)
 
     def save_pretrained(self, ouptut_dir: str):
         self.embedder.save_pretrained(ouptut_dir)
         self.tokenizer.save_pretrained(ouptut_dir)
```

### Comparing `uniem-0.1.0/uniem/trainer.py` & `uniem-0.1.1/uniem/trainer.py`

 * *Files identical despite different names*

### Comparing `uniem-0.1.0/uniem/utils.py` & `uniem-0.1.1/uniem/utils.py`

 * *Files identical despite different names*

### Comparing `uniem-0.1.0/setup.py` & `uniem-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 ['uniem']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['accelerate>=0.19.0,<0.20.0',
+ 'datasets>=2.12.0,<3.0.0',
  'torch>=2.0.0,<3.0.0',
  'tqdm>=4.65.0,<5.0.0',
  'transformers>=4.28.0,<5.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'uniem',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'unified embedding model',
-    'long_description': "# uniem\nunified embedding model\n\n# Usage\n\n```python\nfrom uniem import UniEmbedder\n\n\nsentences = ['Hello, World!', '你好，世界！']\nembedder = UniEmbedder()\nembeddings = embedder(sentences)\n```\n\n## Train Your Model\n\n1. create virtual environment\n```bash\nconda create -n uniem python=3.10\n```\n2. install uniem\n```bash\npip install -e .\n```\n3. get help\n```bash\npython scripts/train_medi.py --help\n```\n4. train embedding model\n```bash\npython scripts/train_medi.py <model_path_or_name> <data_file>\n```\n",
+    'long_description': "# uniem\nunified embedding model\n\n\n## Install\n\n```\npip install uniem\n```\n\n## Usage\n\n```python\nfrom uniem import UniEmbedder\n\nembedder = UniEmbedder.from_pretrained('uniem/base-softmax-last-mean')\nembeddings = embedder.encode(['Hello World!', '你好,世界!'])\n```\n\n## Train Your Model\n\n1. create virtual environment\n```bash\nconda create -n uniem python=3.10\n```\n2. install uniem\n```bash\npip install -e .\n```\n3. get help\n![](./docs/imgs/medi-help.png)\n```bash\npython scripts/train_medi.py --help\n```\n4. train embedding model\n```bash\npython scripts/train_medi.py <model_path_or_name> <data_file>\n```\n",
     'author': 'wangyuxin',
     'author_email': 'wangyuxin@mokahr.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `uniem-0.1.0/PKG-INFO` & `uniem-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.1.0
+Version: 0.1.1
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: accelerate (>=0.19.0,<0.20.0)
+Requires-Dist: datasets (>=2.12.0,<3.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # uniem
 unified embedding model
 
-# Usage
+
+## Install
+
+```
+pip install uniem
+```
+
+## Usage
 
 ```python
 from uniem import UniEmbedder
 
-
-sentences = ['Hello, World!', '你好，世界！']
-embedder = UniEmbedder()
-embeddings = embedder(sentences)
+embedder = UniEmbedder.from_pretrained('uniem/base-softmax-last-mean')
+embeddings = embedder.encode(['Hello World!', '你好,世界!'])
 ```
 
 ## Train Your Model
 
 1. create virtual environment
 ```bash
 conda create -n uniem python=3.10
 ```
 2. install uniem
 ```bash
 pip install -e .
 ```
 3. get help
+![](./docs/imgs/medi-help.png)
 ```bash
 python scripts/train_medi.py --help
 ```
 4. train embedding model
 ```bash
 python scripts/train_medi.py <model_path_or_name> <data_file>
 ```
```

