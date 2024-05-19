# Comparing `tmp/generate_sequences-0.0.7.tar.gz` & `tmp/generate_sequences-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.7.tar", last modified: Wed May  8 16:16:28 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.8.tar", last modified: Sun May 19 08:26:53 2024, max compression
```

## Comparing `generate_sequences-0.0.7.tar` & `generate_sequences-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.856396 generate_sequences-0.0.7/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.856396 generate_sequences-0.0.7/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:26:53.671061 generate_sequences-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-19 08:26:53.671061 generate_sequences-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:26:53.667061 generate_sequences-0.0.8/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/generate_sequences/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:26:53.667061 generate_sequences-0.0.8/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-19 08:26:53.000000 generate_sequences-0.0.8/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-19 08:26:53.000000 generate_sequences-0.0.8/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:26:53.000000 generate_sequences-0.0.8/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-19 08:26:53.000000 generate_sequences-0.0.8/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 08:26:53.000000 generate_sequences-0.0.8/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-19 08:24:46.000000 generate_sequences-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:26:53.671061 generate_sequences-0.0.8/setup.cfg
```

### Comparing `generate_sequences-0.0.7/LICENSE` & `generate_sequences-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.7/PKG-INFO` & `generate_sequences-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.7
+Version: 0.0.8
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -227,21 +227,23 @@
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.4.27; extra == "dev"
-Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
+Requires-Dist: furo==2024.5.6; extra == "dev"
+Requires-Dist: myst-parser<3.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
 Requires-Dist: sacrebleu==2.4.*; extra == "dev"
 Requires-Dist: sacremoses==0.1.*; extra == "dev"
 Requires-Dist: sentencepiece==0.2.*; extra == "dev"
 Requires-Dist: transformers<4.41,>=4.39; extra == "dev"
 
 # generate-sequences
+
+This package generates sequences from deep learning architectures. These architectures could be decoder-only, or encoder-decoder architectures.
```

### Comparing `generate_sequences-0.0.7/generate_sequences/generate.py` & `generate_sequences-0.0.8/generate_sequences/generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import heapq
-import warnings
 from typing import Callable, Iterator, List, Union
 
 import torch
 import torch.nn.functional as F
-import torch.utils
 from tqdm.auto import tqdm
 
 from generate_sequences.utils import sort_list_with_positions
 
 
 class BaseGenerator:
     def __init__(
@@ -20,25 +18,29 @@
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda" if torch.cuda.is_available() else "cpu",
         temperature: float = 1.0,
         use_tqdm: bool = True,
+        top_k_sampling: int = 0,
+        top_p_sampling: float = 0.0,
         multinomial_sampling: bool = False,
         sort_samples: bool = False,
     ) -> None:
         self.device = device
         self.use_tqdm = use_tqdm
         self.max_length = max_length
         self.batch_size = batch_size
         self.generation_forward = generation_forward
         self.eos_token_id = eos_token_id
         self.decoder_start_token_id = decoder_start_token_id
         self.temperature = temperature
+        self.top_k_sampling = top_k_sampling
+        self.top_p_sampling = top_p_sampling
         self.multinomial_sampling = multinomial_sampling
         self.sort_samples = sort_samples
 
     def get_batches(self, inputs: Union[List[torch.Tensor], List[str]]) -> Iterator[List[str]]:
         batched_inputs = inputs
         if self.sort_samples:
             sorted_inputs, inputs_positions = sort_list_with_positions(inputs)
@@ -57,24 +59,60 @@
         if not self.sort_samples:
             return outputs
         ordered_outputs = []
         for position in self.inputs_original_positions:
             ordered_outputs.append(outputs[position])
         return ordered_outputs
 
+    def sample_next_tokens(self, logits, num_tokens=1, min_tokens_to_keep=2):
+        if self.top_k_sampling > 0:
+            top_logits, _ = torch.topk(
+                logits,
+                min(self.top_k_sampling, logits.size(-1)),  # in case top_k_sampling > vocab
+                dim=-1,
+            )
+            logits[logits < top_logits[:, [-1]]] = -float("Inf")
+        if self.top_p_sampling > 0:
+            sorted_logits, sorted_indices = torch.sort(logits, descending=True)
+            cumulative_probs = torch.cumsum(F.softmax(sorted_logits, dim=-1), dim=-1)
+            sorted_indices_to_remove = cumulative_probs > self.top_p_sampling
+            if min_tokens_to_keep > 1:
+                # Keep at least min_tokens_to_keep (set to min_tokens_to_keep-1 because we add the first one below)
+                sorted_indices_to_remove[..., :min_tokens_to_keep] = 0
+            sorted_indices_to_remove[:, 1:] = sorted_indices_to_remove[:, :-1].clone()
+            sorted_indices_to_remove[:, 0] = 0
+            indices_to_remove = sorted_indices_to_remove.scatter(
+                1,
+                sorted_indices,
+                sorted_indices_to_remove,
+            )
+            logits[indices_to_remove] = -float("Inf")
+            # the above scatter is equevalent to:
+            # for i in range(logits.size(0)):
+            #     indices_to_remove = sorted_indices[i, sorted_indices_to_remove[i]]
+            #     logits[i, indices_to_remove] = -float("Inf")
+        logits = F.log_softmax(logits, dim=-1)
+        if self.multinomial_sampling:
+            next_tokens = torch.multinomial(
+                torch.exp(logits),
+                num_samples=num_tokens,
+            )
+            logits = logits.gather(-1, next_tokens)
+            # sort the sampled vector to make sure that the first num_beams samples are the best
+            logits, next_scores_indices = torch.sort(logits, descending=True, dim=1)
+            next_tokens = torch.gather(next_tokens, -1, next_scores_indices)
+        else:
+            logits, next_tokens = torch.topk(logits, num_tokens)
+        return logits, next_tokens
+
 
 class GreedyGenerator(BaseGenerator):
     @torch.no_grad()
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         outputs = []
-        # add user warning if temperature is not 1.0 that greedy search is not appropriate
-        if self.temperature != 1.0 and not self.multinomial_sampling:
-            warnings.warn(
-                "Temperature does not have an affect on Greedy search if multinomial sampling is set to False! If forgot to add multinomial sampling, set `multinomial_sampling=True` to the generator."
-            )
 
         for batch_inputs in self.get_batches(inputs):
             batch_size = len(batch_inputs)
             decoder_inputs = torch.full(
                 (batch_size, self.max_length),
                 self.eos_token_id,  # Pre-fill with EOS; only overwrite if generating
                 dtype=torch.long,
@@ -83,25 +121,17 @@
             decoder_inputs[:, 0] = self.decoder_start_token_id
             finished_mask = torch.zeros(batch_size, dtype=torch.bool, device=self.device)
 
             for step in range(1, self.max_length):
                 if finished_mask.all():
                     break  # Stop if all sequences are finished
                 batch_outputs = self.generation_forward(batch_inputs, decoder_inputs[:, :step])
-                batch_outputs = batch_outputs[:, -1, :]  # Get last tokens' outputs for the batch
-                next_tokens = batch_outputs / self.temperature
-                next_tokens = F.softmax(next_tokens, dim=-1)
-                # check for multinomial sampling
-                if self.multinomial_sampling:
-                    next_tokens = torch.multinomial(
-                        next_tokens,
-                        num_samples=1,
-                    ).squeeze()
-                else:
-                    next_tokens = torch.argmax(next_tokens, dim=-1)
+                logits = batch_outputs[:, -1, :] / self.temperature
+                _, next_tokens = self.sample_next_tokens(logits)
+                next_tokens = next_tokens.squeeze()
                 not_finished = ~finished_mask
                 decoder_inputs[not_finished, step] = next_tokens[not_finished]
                 finished_mask |= next_tokens == self.eos_token_id  # Update finished sequences
             outputs += decoder_inputs
         return self.restore_outputs_order(outputs)
 
 
@@ -121,30 +151,30 @@
     """Calculates the adjusted score of a node for beam sorting. Applies length penalty to score."""
     tokens = node.tokens
     if eos_token_id in tokens:
         tokens = tokens[1 : tokens.index(eos_token_id) + 1]
     return node.score / (len(tokens) ** length_penalty)
 
 
-# this implementation is inspired by:
-# https://hussainwali.medium.com/simple-implementation-of-beam-search-in-python-64b2d3e2fd7e
 class BeamSearchGenerator(BaseGenerator):
     def __init__(
         self,
         decoder_start_token_id: int,
         eos_token_id: int,
         generation_forward: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda" if torch.cuda.is_available() else "cpu",
         temperature: float = 1.0,
         use_tqdm: bool = True,
+        top_k_sampling: int = 0,
+        top_p_sampling: float = 0.0,
         multinomial_sampling: bool = False,
         sort_samples: bool = False,
         beam_width: int = 4,
         length_penalty: float = 1.0,
         beam_nodes_ordering_function: Callable[
             [BeamNode, int, float], float
         ] = default_beam_nodes_ordering_fn,
@@ -154,14 +184,16 @@
             eos_token_id,
             generation_forward,
             max_length,
             batch_size,
             device,
             temperature,
             use_tqdm,
+            top_k_sampling,
+            top_p_sampling,
             multinomial_sampling,
             sort_samples,
         )
         self.beam_width = beam_width
         self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
@@ -206,47 +238,37 @@
                 # beam width, taking the case where k < len(best_beams_nodes[0]), i.e. in the first step
                 beam_width = 1 if step == 0 else self.beam_width
                 for k in range(beam_width):
                     decoder_input_ids = torch.LongTensor(
                         [sample_best_nodes[k].tokens for sample_best_nodes in batch_best_nodes]
                     ).to(self.device)
                     batch_outputs = self.generation_forward(batch, decoder_input_ids)
-                    batch_outputs = batch_outputs[:, -1, :]
-                    batch_outputs = batch_outputs / self.temperature
-                    batch_outputs = F.log_softmax(batch_outputs, dim=-1)
-                    # check for multinomial sampling
-                    if self.multinomial_sampling:
-                        topk_indices = torch.multinomial(
-                            torch.exp(batch_outputs),
-                            self.beam_width,
-                            replacement=True,
-                        )
-                        topk_scores = batch_outputs.gather(1, topk_indices)
-                    else:
-                        topk_scores, topk_indices = torch.topk(batch_outputs, self.beam_width)
+                    logits = batch_outputs[:, -1, :] / self.temperature
+                    logits, next_tokens = self.sample_next_tokens(
+                        logits, num_tokens=self.beam_width
+                    )
                     for sample_index in range(len(batch)):
                         if batch_best_nodes[sample_index][k].tokens[-1] == self.eos_token_id:
                             next_nodes[sample_index] += [
                                 BeamNode(
                                     tokens=batch_best_nodes[sample_index][k].tokens
                                     + [self.eos_token_id],
                                     score=0,
                                 )
                             ] * self.beam_width
                         else:
                             next_nodes[sample_index] += [
                                 BeamNode(
                                     tokens=batch_best_nodes[sample_index][k].tokens
-                                    + [topk_indices[sample_index][i].item()],
+                                    + [next_tokens[sample_index][i].item()],
                                     score=batch_best_nodes[sample_index][k].score
-                                    + topk_scores[sample_index][i].item(),
+                                    + logits[sample_index][i].item(),
                                 )
                                 for i in range(self.beam_width)
                             ]
-
                 batch_best_nodes = next_nodes  # Update beams for the next time step
 
             batch_predictions = []
             for sample_nodes in batch_best_nodes:
                 best_node = max(
                     sample_nodes,
                     key=lambda node: self.beam_nodes_ordering_function(
```

### Comparing `generate_sequences-0.0.7/generate_sequences/utils.py` & `generate_sequences-0.0.8/generate_sequences/utils.py`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.7/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.8/generate_sequences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.7
+Version: 0.0.8
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -227,21 +227,23 @@
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.4.27; extra == "dev"
-Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
+Requires-Dist: furo==2024.5.6; extra == "dev"
+Requires-Dist: myst-parser<3.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
 Requires-Dist: sacrebleu==2.4.*; extra == "dev"
 Requires-Dist: sacremoses==0.1.*; extra == "dev"
 Requires-Dist: sentencepiece==0.2.*; extra == "dev"
 Requires-Dist: transformers<4.41,>=4.39; extra == "dev"
 
 # generate-sequences
+
+This package generates sequences from deep learning architectures. These architectures could be decoder-only, or encoder-decoder architectures.
```

### Comparing `generate_sequences-0.0.7/pyproject.toml` & `generate_sequences-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
   "pytest-sphinx",
   "pytest-cov",
   "twine>=1.11.0",
   "build",
   "setuptools",
   "wheel",
   "Sphinx>=4.3.0,<7.4.0",
-  "furo==2024.4.27",
-  "myst-parser>=1.0,<2.1",
+  "furo==2024.5.6",
+  "myst-parser>=1.0,<3.1",
   "sphinx-copybutton==0.5.2",
   "sphinx-autobuild==2021.3.14",
   "sphinx-autodoc-typehints==2.0.0",
   "packaging",
   "pre-commit==3.5.0",
   # added for testing
   "evaluate==0.4.*",
```

