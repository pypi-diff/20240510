# Comparing `tmp/diffpass-0.0.1.tar.gz` & `tmp/diffpass-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffpass-0.0.1.tar", last modified: Wed May  8 22:09:50 2024, max compression
+gzip compressed data, was "diffpass-0.1.0.tar", last modified: Fri May 10 11:24:25 2024, max compression
```

## Comparing `diffpass-0.0.1.tar` & `diffpass-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-08 22:09:50.685526 diffpass-0.0.1/
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    11337 2023-08-31 17:21:49.000000 diffpass-0.0.1/LICENSE
--rw-rw-r--   0 lupo      (1001) lupo      (1001)      111 2023-08-31 17:21:49.000000 diffpass-0.0.1/MANIFEST.in
--rw-r--r--   0 lupo      (1001) lupo      (1001)     6601 2024-05-08 22:09:50.685526 diffpass-0.0.1/PKG-INFO
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     5464 2024-05-08 21:44:04.000000 diffpass-0.0.1/README.md
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-08 22:09:50.685526 diffpass-0.0.1/diffpass/
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       22 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/__init__.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    26659 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/_modidx.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    21824 2024-05-08 21:43:44.000000 diffpass-0.0.1/diffpass/base.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     3660 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/constants.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     9286 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/data_utils.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     1700 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/entropy_ops.py
--rw-r--r--   0 lupo      (1001) lupo      (1001)     5360 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/gumbel_sinkhorn_ops.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     1406 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/ipa_utils.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    23085 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/model.py
--rw-r--r--   0 lupo      (1001) lupo      (1001)     1291 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/msa_parsing.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     4621 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/sequence_similarity_ops.py
--rw-rw-r--   0 lupo      (1001) lupo      (1001)    14088 2024-05-08 21:43:45.000000 diffpass-0.0.1/diffpass/train.py
-drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-08 22:09:50.685526 diffpass-0.0.1/diffpass.egg-info/
--rw-r--r--   0 lupo      (1001) lupo      (1001)     6601 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/PKG-INFO
--rw-rw-r--   0 lupo      (1001) lupo      (1001)      553 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/SOURCES.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/dependency_links.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/entry_points.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-02-19 12:44:53.000000 diffpass-0.0.1/diffpass.egg-info/not-zip-safe
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       89 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/requires.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)        9 2024-05-08 22:09:50.000000 diffpass-0.0.1/diffpass.egg-info/top_level.txt
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     1101 2024-05-08 22:02:11.000000 diffpass-0.0.1/settings.ini
--rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-08 22:09:50.685526 diffpass-0.0.1/setup.cfg
--rw-rw-r--   0 lupo      (1001) lupo      (1001)     2596 2023-08-31 17:21:49.000000 diffpass-0.0.1/setup.py
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.479231 diffpass-0.1.0/
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    11337 2023-08-31 17:21:49.000000 diffpass-0.1.0/LICENSE
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)      111 2023-08-31 17:21:49.000000 diffpass-0.1.0/MANIFEST.in
+-rw-r--r--   0 lupo      (1001) lupo      (1001)    10887 2024-05-10 11:24:25.479231 diffpass-0.1.0/PKG-INFO
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     9745 2024-05-10 09:39:56.000000 diffpass-0.1.0/README.md
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.475231 diffpass-0.1.0/diffpass/
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       22 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/__init__.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    26907 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/_modidx.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    26072 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/base.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     3660 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/constants.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    10162 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/data_utils.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     1700 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/entropy_ops.py
+-rw-r--r--   0 lupo      (1001) lupo      (1001)     5360 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/gumbel_sinkhorn_ops.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     2263 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/ipa_utils.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    23338 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/model.py
+-rw-r--r--   0 lupo      (1001) lupo      (1001)     1291 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/msa_parsing.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     4621 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/sequence_similarity_ops.py
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)    17749 2024-05-10 11:24:12.000000 diffpass-0.1.0/diffpass/train.py
+drwxrwxr-x   0 lupo      (1001) lupo      (1001)        0 2024-05-10 11:24:25.475231 diffpass-0.1.0/diffpass.egg-info/
+-rw-r--r--   0 lupo      (1001) lupo      (1001)    10887 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/PKG-INFO
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)      553 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/SOURCES.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/dependency_links.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/entry_points.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        1 2024-02-19 12:44:53.000000 diffpass-0.1.0/diffpass.egg-info/not-zip-safe
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       89 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/requires.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)        9 2024-05-10 11:24:25.000000 diffpass-0.1.0/diffpass.egg-info/top_level.txt
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     1009 2024-05-10 11:22:19.000000 diffpass-0.1.0/settings.ini
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)       38 2024-05-10 11:24:25.479231 diffpass-0.1.0/setup.cfg
+-rw-rw-r--   0 lupo      (1001) lupo      (1001)     2596 2023-08-31 17:21:49.000000 diffpass-0.1.0/setup.py
```

### Comparing `diffpass-0.0.1/LICENSE` & `diffpass-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass/_modidx.py` & `diffpass-0.1.0/diffpass/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
                                      'diffpass.data_utils.create_groupwise_seq_records': ( 'data_utils.html#create_groupwise_seq_records',
                                                                                            'diffpass/data_utils.py'),
                                      'diffpass.data_utils.get_single_and_paired_seqs': ( 'data_utils.html#get_single_and_paired_seqs',
                                                                                          'diffpass/data_utils.py'),
                                      'diffpass.data_utils.one_hot_encode_msa': ( 'data_utils.html#one_hot_encode_msa',
                                                                                  'diffpass/data_utils.py'),
                                      'diffpass.data_utils.pad_msas_with_dummy_sequences': ( 'data_utils.html#pad_msas_with_dummy_sequences',
-                                                                                            'diffpass/data_utils.py')},
+                                                                                            'diffpass/data_utils.py'),
+                                     'diffpass.data_utils.remove_groups_not_in_both': ( 'data_utils.html#remove_groups_not_in_both',
+                                                                                        'diffpass/data_utils.py')},
             'diffpass.entropy_ops': { 'diffpass.entropy_ops.pointwise_shannon': ( 'entropy_ops.html#pointwise_shannon',
                                                                                   'diffpass/entropy_ops.py'),
                                       'diffpass.entropy_ops.smooth_mean_one_body_entropy': ( 'entropy_ops.html#smooth_mean_one_body_entropy',
                                                                                              'diffpass/entropy_ops.py'),
                                       'diffpass.entropy_ops.smooth_mean_two_body_entropy': ( 'entropy_ops.html#smooth_mean_two_body_entropy',
                                                                                              'diffpass/entropy_ops.py')},
             'diffpass.gumbel_sinkhorn_ops': { 'diffpass.gumbel_sinkhorn_ops.gumbel_matching': ( 'gumbel_sinkhorn_ops.html#gumbel_matching',
```

### Comparing `diffpass-0.0.1/diffpass/base.py` & `diffpass-0.1.0/diffpass/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,581 +1,649 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/base.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/model.ipynb.
 
 # %% auto 0
-__all__ = ['INGROUP_IDX_DTYPE', 'dccn', 'make_pbar', 'DiffPaSSResults', 'DiffPaSSModel']
+__all__ = ['IndexPair', 'IndexPairsInGroup', 'IndexPairsInGroups', 'GeneralizedPermutation', 'MatrixApply',
+           'PermutationConjugate', 'global_argmax_from_group_argmaxes', 'apply_hard_permutation_batch_to_similarity',
+           'TwoBodyEntropyLoss', 'MILoss', 'HammingSimilarities', 'Blosum62Similarities', 'BestHits',
+           'InterGroupSimilarityLoss', 'IntraGroupSimilarityLoss']
 
-# %% ../nbs/base.ipynb 3
+# %% ../nbs/model.ipynb 4
 # Stdlib imports
+from collections.abc import Iterable, Sequence
+from typing import Optional, Union, Iterator, Literal
 from copy import deepcopy
-from typing import Optional, Any, Sequence, Union
-from dataclasses import fields, dataclass
-
-# Progress bars
-from tqdm import tqdm
+from warnings import warn
+from functools import partial
 
 # NumPy
 import numpy as np
 
 # PyTorch
 import torch
-from torch.nn import Module
+from torch.nn import Module, ParameterList, Parameter
+from torch.nn.functional import softmax
 
 # DiffPaSS imports
-from diffpass.model import (
-    GeneralizedPermutation,
-    Blosum62Similarities,
-    HammingSimilarities,
-    BestHits,
+from .gumbel_sinkhorn_ops import gumbel_sinkhorn, gumbel_matching
+from diffpass.entropy_ops import (
+    smooth_mean_one_body_entropy,
+    smooth_mean_two_body_entropy,
+)
+from .constants import get_blosum62_data
+from diffpass.sequence_similarity_ops import (
+    smooth_hamming_similarities_dot,
+    smooth_hamming_similarities_cdist,
+    smooth_substitution_matrix_similarities_dot,
+    smooth_substitution_matrix_similarities_cdist,
+    soft_best_hits,
+    hard_best_hits,
 )
 
-# Constants
-INGROUP_IDX_DTYPE = np.int16
+# Type aliases
+IndexPair = tuple[int, int]  # Pair of indices
+IndexPairsInGroup = list[IndexPair]  # Pairs of indices in a group of sequences
+IndexPairsInGroups = list[IndexPairsInGroup]  # Pairs of indices in groups of sequences
+
+# %% ../nbs/model.ipynb 6
+def _consecutive_slices_from_sizes(group_sizes: Optional[Sequence[int]]) -> list[slice]:
+    if group_sizes is None:
+        return [slice(None)]
+    cumsum = np.cumsum(group_sizes).tolist()
+
+    return [slice(start, end) for start, end in zip([0] + cumsum, cumsum)]
+
+# %% ../nbs/model.ipynb 8
+class GeneralizedPermutation(Module):
+    """Generalized permutation layer implementing both soft and hard permutations."""
 
-# %% ../nbs/base.ipynb 4
-def dccn(x: torch.Tensor) -> np.ndarray:
-    return x.detach().clone().cpu().numpy()
-
-
-def make_pbar(epochs: int, show_pbar: bool) -> Any:
-    if show_pbar:
-        return tqdm(range(epochs + 1))
-    return range(epochs + 1)
-
-
-@dataclass
-class DiffPaSSResults:
-    # Optionally, log alphas for fine-grained information
-    log_alphas: Optional[list]
-    # Soft and hard permutations
-    soft_perms: Optional[list]
-    hard_perms: list
-    # Losses
-    hard_losses: list
-    soft_losses: list
-
-
-class DiffPaSSModel(Module):
-    allowed_permutation_cfg_keys = {
-        "tau",
-        "n_iter",
-        "noise",
-        "noise_factor",
-        "noise_std",
-    }
-    allowed_information_measures = {"MI", "TwoBodyEntropy"}
-    allowed_similarity_kinds = {"Hamming", "Blosum62"}
-    allowed_similarities_cfg_keys = {
-        "Hamming": {"use_dot", "p"},
-        "Blosum62": {"use_dot", "p", "use_scoredist", "aa_to_int", "gaps_as_stars"},
-    }
-    allowed_best_hits_cfg_keys = {"tau", "reciprocal"}
-
-    group_sizes: Sequence[int]
-    fixed_pairings: Optional[Sequence[Sequence[Sequence[int]]]]
-    permutation_cfg: Optional[dict[str, Any]]
-    effective_permutation_cfg_: dict[str, Any]
-    information_measure: str
-    similarity_kind: str
-    similarities_cfg: Optional[dict[str, Any]]
-    effective_similarities_cfg_: dict[str, Any]
-    permutation: GeneralizedPermutation
-    similarities: Union[Blosum62Similarities, HammingSimilarities]
-    compute_in_group_best_hits: bool
-    best_hits_cfg: Optional[dict[str, Any]]
-    effective_best_hits_cfg_: dict[str, Any]
-    best_hits: BestHits
-
-    single_fit_default_cfg = {
-        "epochs": 1,
-        "optimizer_name": "SGD",
-        "optimizer_kwargs": None,
-        "mean_centering": False,
-        "show_pbar": False,
-        "compute_final_soft": False,
-        "record_log_alphas": False,
-        "record_soft_perms": False,
-        "record_soft_losses": False,
-    }
-
-    @staticmethod
-    def reduce_num_tokens(x: torch.Tensor) -> torch.Tensor:
-        """Reduce the number of tokens in a one-hot encoded tensor."""
-        used_tokens = x.clone()
-        for _ in range(x.ndim - 1):
-            used_tokens = used_tokens.any(-2)
-
-        return x[..., used_tokens]
-
-    def validate_permutation_cfg(self, permutation_cfg: Optional[dict]) -> None:
-        if permutation_cfg is None:
-            return
-        if not set(permutation_cfg).issubset(self.allowed_permutation_cfg_keys):
-            raise ValueError(
-                f"Invalid keys in `permutation_cfg`: "
-                f"{set(permutation_cfg) - self.allowed_permutation_cfg_keys}"
-            )
-
-    def validate_information_measure(self, information_measure: str) -> None:
-        if information_measure not in self.allowed_information_measures:
-            raise ValueError(
-                f"Invalid information measure: {self.information_measure}. "
-                f"Allowed values are: {self.allowed_information_measures}"
-            )
-
-    def validate_similarity_kind(self, similarity_kind: str) -> None:
-        if similarity_kind not in self.allowed_similarity_kinds:
-            raise ValueError(
-                f"Invalid similarity kind: {self.similarity_kind}. "
-                f"Allowed values are: {self.allowed_similarity_kinds}"
-            )
-
-    def validate_similarities_cfg(self, similarities_cfg: Optional[dict]) -> None:
-        if similarities_cfg is None:
-            return
-        if not set(similarities_cfg).issubset(
-            self.allowed_similarities_cfg_keys[self.similarity_kind]
-        ):
-            raise ValueError(
-                f"Invalid keys in `similarities_cfg`: "
-                f"{set(similarities_cfg) - self.allowed_similarities_cfg_keys[self.similarity_kind]}"
-            )
-
-    def validate_best_hits_cfg(self, best_hits_cfg: Optional[dict]) -> None:
-        if best_hits_cfg is None:
-            return
-        if not set(best_hits_cfg).issubset(self.allowed_best_hits_cfg_keys):
-            raise ValueError(
-                f"Invalid keys in `best_hits_cfg`: "
-                f"{set(best_hits_cfg) - self.allowed_best_hits_cfg_keys}"
-            )
-
-    def init_permutation(
+    def __init__(
         self,
-        group_sizes: Sequence[int],
-        fixed_pairings: Optional[Sequence[Sequence[Sequence[int]]]] = None,
-        permutation_cfg: Optional[dict[str, Any]] = None,
+        *,
+        group_sizes: Iterable[int],
+        fixed_pairings: Optional[IndexPairsInGroups] = None,
+        tau: float = 1.0,
+        n_iter: int = 1,
+        noise: bool = False,
+        noise_factor: float = 1.0,
+        noise_std: bool = False,
+        mode: Literal["soft", "hard"] = "soft",
     ) -> None:
+        super().__init__()
         self.group_sizes = tuple(s for s in group_sizes)
-        self.fixed_pairings = fixed_pairings
-        self.permutation_cfg = permutation_cfg
 
-        # Validate GeneralizedPermutation config
-        self.validate_permutation_cfg(permutation_cfg)
-        if self.permutation_cfg is None:
-            self.effective_permutation_cfg_ = {}
-        else:
-            self.effective_permutation_cfg_ = deepcopy(self.permutation_cfg)
+        self.init_fixed_pairings_and_log_alphas(fixed_pairings)
 
-        self.permutation = GeneralizedPermutation(
-            group_sizes=self.group_sizes,
-            fixed_pairings=self.fixed_pairings,
-            mode="soft",
-            **self.effective_permutation_cfg_,
-        )
+        self.tau = tau
+        self.n_iter = n_iter
+        self.noise = noise
+        self.noise_factor = noise_factor
+        self.noise_std = noise_std
+        self.mode = mode
 
-    def init_similarities(
-        self, similarity_kind: str, similarities_cfg: Optional[dict[str, Any]] = None
+    def init_fixed_pairings_and_log_alphas(
+        self,
+        fixed_pairings: IndexPairsInGroups,
+        device: Optional[torch.device] = None,
     ) -> None:
-        self.validate_similarity_kind(similarity_kind)
-        self.similarity_kind = similarity_kind
-        self.validate_similarities_cfg(similarities_cfg)
-        self.similarities_cfg = similarities_cfg
-        if self.similarities_cfg is None:
-            self.effective_similarities_cfg_ = {}
-        else:
-            self.effective_similarities_cfg_ = deepcopy(self.similarities_cfg)
-        if similarity_kind == "Blosum62":
-            self.similarities = Blosum62Similarities(**self.effective_similarities_cfg_)
-        elif similarity_kind == "Hamming":
-            self.similarities = HammingSimilarities(**self.effective_similarities_cfg_)
-
-    def init_best_hits(self, best_hits_cfg: Optional[dict[str, Any]] = None) -> None:
-        self.validate_best_hits_cfg(best_hits_cfg)
-        self.best_hits_cfg = best_hits_cfg
-        if self.best_hits_cfg is None:
-            self.effective_best_hits_cfg_ = {}
-        else:
-            self.effective_best_hits_cfg_ = deepcopy(self.best_hits_cfg)
-        self.best_hits = BestHits(
-            group_sizes=self.group_sizes if self.compute_in_group_best_hits else None,
-            mode="soft",
-            **self.effective_best_hits_cfg_,
+        """Initialize fixed pairings and parameterization matrices."""
+        self._validate_fixed_pairings(fixed_pairings)
+        self.fixed_pairings = fixed_pairings
+
+        # Initialize parameterization matrices ('log-alphas')
+        # By default, initialize all parametrization matrices to zero
+        self.nonfixed_group_sizes_ = (
+            tuple(
+                s - num_efm
+                for s, num_efm in zip(
+                    self.group_sizes, self._effective_number_fixed_pairings
+                )
+            )
+            if self.fixed_pairings
+            else self.group_sizes
+        )
+        self.log_alphas = ParameterList(
+            [
+                Parameter(torch.zeros(s, s), requires_grad=bool(s))
+                for s in self.nonfixed_group_sizes_
+            ]
         )
+        self.to(device=device)
 
-    def validate_inputs(
-        self,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        *,
-        check_same_alphabet_size: bool = True,
+    def _validate_fixed_pairings(
+        self, fixed_pairings: Optional[IndexPairsInGroups] = None
     ) -> None:
-        """Validate input tensors representing aligned objects or (dis)similarity matrices."""
-        size_x, size_y = x.shape[0], y.shape[0]
-        if size_x != size_y:
-            raise ValueError(f"Size mismatch between x ({size_x}) and y ({size_y}).")
-
-        if self.are_inputs_msas:
-            if x.ndim != 3 or y.ndim != 3:
+        if fixed_pairings:
+            if len(fixed_pairings) != len(self.group_sizes):
                 raise ValueError(
-                    "Inputs must be 3D tensors of shape (n_samples, length, alphabet_size)."
+                    "If `fixed_pairings` is provided, it must have the same length as "
+                    "`group_sizes`."
                 )
-            _, alphabet_size_x = x.shape[1:]
-            _, alphabet_size_y = y.shape[1:]
-            if check_same_alphabet_size and (alphabet_size_x != alphabet_size_y):
-                raise ValueError("Inputs must have the same alphabet size.")
-        elif x.ndim != 2 or y.ndim != 2:
-            raise ValueError(
-                "Inputs must be 2D square tensors of shape (n_samples, n_samples)."
-            )
-        elif x.shape[1] != size_x or y.shape[1] != size_y:
-            raise ValueError(
-                "Inputs must be square tensors of shape (n_samples, n_samples)."
-            )
-
-        # Validate group_sizes attribute
-        n_samples = sum(self.group_sizes)
-        if size_x != n_samples:
-            raise ValueError(
-                f"Inputs have {n_samples} samples but `group_sizes` implies a total "
-                f"of {n_samples} samples."
+            for s, fm in zip(self.group_sizes, fixed_pairings):
+                if not fm:
+                    continue
+                if any([len(p) != 2 for p in fm]):
+                    raise ValueError(
+                        "All fixed pairings must be pairs of indices (i, j)."
+                    )
+                if any(min(i, j) < 0 or max(i, j) >= s for i, j in fm):
+                    raise ValueError(
+                        "All fixed pairings must be within the range of the corresponding "
+                        "group size."
+                    )
+            self._effective_number_fixed_pairings = []
+            self._effective_fixed_pairings_zip = []
+            for idx, (s, fm) in enumerate(zip(self.group_sizes, fixed_pairings)):
+                if fm:
+                    num_fm = len(fm)
+                    fm_zip = list(zip(*fm))
+                else:
+                    num_fm = 0
+                    fm_zip = [(), ()]
+                complement = s - num_fm  # Effectively fully fixed when complement <= 1
+                is_fully_fixed = complement <= 1
+                num_efm = s - (s - num_fm) * (not is_fully_fixed)
+                self._effective_number_fixed_pairings.append(num_efm)
+                if is_fully_fixed:
+                    mask = torch.zeros(s, s, dtype=torch.bool)
+                    if complement:
+                        possible_idxs = set(range(s))
+                        fm_zip[0] += tuple((possible_idxs - set(fm_zip[0])))
+                        fm_zip[1] += tuple((possible_idxs - set(fm_zip[1])))
+                else:
+                    mask = torch.ones(s, s, dtype=torch.bool)
+                    for i, j in fm:
+                        mask[..., j, :] = False
+                        mask[..., :, i] = False
+                self.register_buffer(f"_not_fixed_masks_{idx}", mask)
+                self._effective_fixed_pairings_zip.append(fm_zip)
+            self._total_number_fixed_pairings = sum(
+                self._effective_number_fixed_pairings
             )
+        else:
+            self._effective_fixed_pairings_zip = [[(), ()] for _ in self.group_sizes]
+            self._effective_number_fixed_pairings = [0] * len(self.group_sizes)
+            self._total_number_fixed_pairings = 0
+
+    @property
+    def _not_fixed_masks(self) -> list[torch.Tensor]:
+        return [
+            getattr(self, f"_not_fixed_masks_{idx}")
+            for idx in range(len(self.group_sizes))
+        ]
 
-    def create_optimizer(
-        self,
-        optimizer_name: Optional[str] = single_fit_default_cfg["optimizer_name"],
-        optimizer_kwargs: Optional[dict[str, Any]] = single_fit_default_cfg[
-            "optimizer_kwargs"
-        ],
-    ) -> torch.optim.Optimizer:
-        optimizer_cls = getattr(torch.optim, optimizer_name)
-        optimizer_kwargs = (
-            {"lr": 1e-1} if optimizer_kwargs is None else deepcopy(optimizer_kwargs)
+    @property
+    def mode(self) -> str:
+        return self._mode
+
+    @mode.setter
+    def mode(self, value) -> None:
+        value = value.lower()
+        if value not in ["soft", "hard"]:
+            raise ValueError("mode must be either 'soft' or 'hard'.")
+        self._mode = value.lower()
+        _mats_fn_no_fixed = getattr(self, f"_{self._mode}_mats")
+        self._mats_fn = (
+            _mats_fn_no_fixed
+            if not self.fixed_pairings
+            else self._impl_fixed_pairings(_mats_fn_no_fixed)
         )
-        optimizer = optimizer_cls(self.parameters(), **optimizer_kwargs)
-        optimizer.zero_grad()
-
-        return optimizer
 
     def soft_(self) -> None:
-        # Iterate through all child modules and call their soft_ method
-        for module in self.children():
-            if hasattr(module, "soft_"):
-                module.soft_()
+        self.mode = "soft"
 
     def hard_(self) -> None:
-        # Iterate through all child modules and call their hard_ method
-        for module in self.children():
-            if hasattr(module, "hard_"):
-                module.hard_()
+        self.mode = "hard"
 
-    def _hard_pass(
-        self, x: torch.Tensor, y: Optional[torch.Tensor], *, results: DiffPaSSResults
-    ) -> None:
-        self.hard_()
-        with torch.no_grad():
-            out = self(x, y)
-            perms = out["perms"]
-            loss = out["loss"]
-            results.hard_perms.append(
-                [
-                    dccn(perms_this_group).argmax(axis=-1).astype(INGROUP_IDX_DTYPE)
-                    for perms_this_group in perms
-                ]
+    def _impl_fixed_pairings(self, func: callable) -> callable:
+        """Include fixed matchings in the Gumbel-Sinkhorn or Gumbel-matching operators."""
+
+        def wrapper(gen: Iterator[torch.Tensor]) -> Iterator[torch.Tensor]:
+            for s, mat, (row_group, col_group), mask in zip(
+                self.group_sizes,
+                gen,
+                self._effective_fixed_pairings_zip,
+                self._not_fixed_masks,
+            ):
+                mat_all = torch.zeros(
+                    s,
+                    s,
+                    dtype=mat.dtype,
+                    layout=mat.layout,
+                    device=mat.device,
+                )
+                # mat_all[j, i] = 1 means that row i becomes row j under a permutation,
+                # using our conventions
+                mat_all[..., col_group, row_group] = 1
+                mat_all.masked_scatter_(mask.to(torch.bool), mat)
+                yield mat_all
+
+        return lambda: wrapper(func())
+
+    def _soft_mats(self) -> Iterator[torch.Tensor]:
+        """Evaluate the Gumbel-Sinkhorn operator on the current `log_alpha` parameters."""
+        return (
+            gumbel_sinkhorn(
+                log_alpha,
+                tau=self.tau,
+                n_iter=self.n_iter,
+                noise=self.noise,
+                noise_factor=self.noise_factor,
+                noise_std=self.noise_std,
+            )
+            for log_alpha in self.log_alphas
+        )
+
+    def _hard_mats(self) -> Iterator[torch.Tensor]:
+        """Evaluate the Gumbel-matching operator on the current `log_alpha` parameters."""
+        return (
+            gumbel_matching(
+                log_alpha,
+                noise=self.noise,
+                noise_factor=self.noise_factor,
+                noise_std=self.noise_std,
+                unbias_lsa=True,
             )
-            results.hard_losses.append(dccn(loss))
+            for log_alpha in self.log_alphas
+        )
+
+    def forward(self) -> list[torch.Tensor]:
+        """Compute the soft/hard permutations according to ``self._mats_fn.``"""
+        mats = self._mats_fn()
+
+        return list(mats)
+
+
+class MatrixApply(Module):
+    """Apply matrices to chunks of a tensor of shape (n_samples, length, alphabet_size)
+    and collate the results."""
+
+    def __init__(self, group_sizes: Iterable[int]) -> None:
+        super().__init__()
+        self.group_sizes = tuple(s for s in group_sizes)
+        self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
+
+    def forward(self, x: torch.Tensor, *, mats: Sequence[torch.Tensor]) -> torch.Tensor:
+        out = torch.full_like(x, torch.nan)
+        for mats_this_group, sl in zip(mats, self._group_slices):
+            out[..., sl, :, :].copy_(
+                torch.tensordot(mats_this_group, x[sl, :, :], dims=1)
+            )
+
+        return out
+
+
+class PermutationConjugate(Module):
+    """Conjugate blocks of a square 2D tensor of shape (n_samples, n_samples) by
+    permutation matrices."""
+
+    def __init__(self, group_sizes: Iterable[int]) -> None:
+        super().__init__()
+        self.group_sizes = tuple(s for s in group_sizes)
+        self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
+
+    def forward(self, x: torch.Tensor, *, mats: Sequence[torch.Tensor]) -> torch.Tensor:
+        out1 = torch.full_like(x, torch.nan)
+        out2 = torch.full_like(x, torch.nan)
+        # (P * A) * P.T
+        for mats_this_group, sl in zip(mats, self._group_slices):
+            out1[..., sl, :].copy_(torch.tensordot(mats_this_group, x[sl, :], dims=1))
+        for mats_this_group, sl in zip(mats, self._group_slices):
+            out2[..., :, sl].copy_(
+                torch.tensordot(
+                    out1[..., :, sl], mats_this_group.permute((-1, -2)), dims=1
+                )
+            )
+
+        return out2
+
+
+def global_argmax_from_group_argmaxes(mats: Iterable[torch.Tensor]) -> torch.Tensor:
+    global_argmax = []
+    start_idx = 0
+    for mats_this_group in mats:
+        global_argmax.append(mats_this_group.argmax(-1) + start_idx)
+        start_idx += mats_this_group.shape[-1]
+
+    return torch.cat(global_argmax, dim=-1)
+
+
+def apply_hard_permutation_batch_to_similarity(
+    *, x: torch.Tensor, perms: list[torch.Tensor]
+) -> torch.Tensor:
+    """
+    Conjugate a single similarity matrix by a batch of hard permutations.
+
+    Args:
+        perms: List of batches of permutation matrices of shape (..., D, D).
+        x: Similarity matrix of shape (D, D).
+
+    Returns:
+        Batch of conjugated matrices of shape (..., D, D).
+    """
+    global_argmax = global_argmax_from_group_argmaxes(perms)
+    x_permuted_rows = x[global_argmax]
+
+    # Permuting columns is more involved
+    index = global_argmax.view(*global_argmax.shape[:-1], 1, -1).expand(
+        *global_argmax.shape, global_argmax.shape[-1]
+    )
+    # Example of gather with 4D tensor and dim=-1:
+    # out[i][j][k][l] = input[i][j][k][index[i][j][k][l]]
+
+    return torch.gather(x_permuted_rows, -1, index)
+
+# %% ../nbs/model.ipynb 12
+class TwoBodyEntropyLoss(Module):
+    """Differentiable extension of the mean of estimated two-body entropies between
+    all pairs of columns from two one-hot encoded tensors."""
+
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        return smooth_mean_two_body_entropy(x, y)
+
+
+class MILoss(Module):
+    """Differentiable extension of minus the mean of estimated mutual informations
+    between all pairs of columns from two one-hot encoded tensors."""
+
+    def __init__(self):
+        super().__init__()
 
-    def _soft_pass(
+    def forward(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        return smooth_mean_two_body_entropy(x, y) - smooth_mean_one_body_entropy(x)
+
+# %% ../nbs/model.ipynb 17
+class HammingSimilarities(Module):
+    """Compute Hamming similarities between sequences using differentiable
+    operations.
+
+    Optionally, if the sequences are arranged in groups, the computation of
+    similarities can be restricted to within groups.
+    Differentiable operations are used to compute the similarities, which can be
+    either dot products or an L^p distance function."""
+
+    def __init__(
         self,
-        x: torch.Tensor,
-        y: torch.Tensor,
         *,
-        results: DiffPaSSResults,
-        record_soft_perms: bool = False,
-        record_soft_losses: bool = False,
-    ) -> torch.Tensor:
-        self.soft_()
-        out = self(x, y)
-        perms = out["perms"]
-        loss = out["loss"]
-        if record_soft_perms:
-            results.soft_perms.append(
-                [dccn(perms_this_group) for perms_this_group in perms]
+        group_sizes: Optional[Iterable[int]] = None,
+        use_dot: bool = True,
+        p: Optional[float] = None,
+    ) -> None:
+        super().__init__()
+        self.group_sizes = (
+            tuple(s for s in group_sizes) if group_sizes is not None else None
+        )
+        self.use_dot = use_dot
+        self.p = p
+
+        if self.use_dot:
+            if self.p is not None:
+                warn("Since a `p` was provided, `use_dot` will be ignored.")
+            self._similarities_fn = smooth_hamming_similarities_dot
+            self._similarities_fn_kwargs = {}
+        else:
+            if self.p is None:
+                raise ValueError("If `use_dot` is False, `p` must be provided.")
+            self._similarities_fn = smooth_hamming_similarities_cdist
+            self._similarities_fn_kwargs = {"p": self.p}
+
+        self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        size = x.shape[:-3] + (x.shape[-3],) * 2
+        out = torch.full(
+            size, torch.nan, dtype=x.dtype, layout=x.layout, device=x.device
+        )
+        for sl in self._group_slices:
+            out[..., sl, sl].copy_(
+                self._similarities_fn(x[..., sl, :, :], **self._similarities_fn_kwargs)
             )
-        if record_soft_losses:
-            results.soft_losses.append(dccn(loss))
 
-        # Compute total loss
-        loss = loss.sum()
+        return out
 
-        return loss
 
-    def _record_current_log_alphas(self, results: DiffPaSSResults) -> None:
-        results.log_alphas.append(
-            [dccn(log_alpha) for log_alpha in self.permutation.log_alphas]
+class Blosum62Similarities(Module):
+    """Compute Blosum62-based similarities between sequences using differentiable
+    operations.
+
+    Optionally, if the sequences are arranged in groups, the computation of
+    similarities can be restricted to within groups.
+    Differentiable operations are used to compute the similarities, which can be
+    either dot products or an L^p distance function."""
+
+    def __init__(
+        self,
+        *,
+        group_sizes: Optional[Iterable[int]] = None,
+        use_dot: bool = True,
+        p: Optional[float] = None,
+        use_scoredist: bool = False,
+        aa_to_int: Optional[dict[str, int]] = None,
+        gaps_as_stars: bool = True,
+    ) -> None:
+        super().__init__()
+        self.group_sizes = (
+            tuple(s for s in group_sizes) if group_sizes is not None else None
+        )
+        self.use_dot = use_dot
+        self.p = p
+        self.use_scoredist = use_scoredist
+        self.aa_to_int = aa_to_int
+        self.gaps_as_stars = gaps_as_stars
+
+        blosum62_data = get_blosum62_data(
+            aa_to_int=self.aa_to_int, gaps_as_stars=self.gaps_as_stars
         )
+        self.register_buffer("subs_mat", blosum62_data.mat)
+        self.expected_value = blosum62_data.expected_value
 
-    @staticmethod
-    def _init_results(
+        self._similarities_fn_kwargs = {"subs_mat": self.subs_mat}
+        if self.use_dot:
+            if self.p is not None:
+                warn("Since a `p` was provided, `use_dot` will be ignored.")
+            self._similarities_fn = smooth_substitution_matrix_similarities_dot
+            self._similarities_fn_kwargs = {
+                "use_scoredist": self.use_scoredist,
+                "expected_value": self.expected_value,
+            }
+        else:
+            if self.p is None:
+                raise ValueError("If `use_dot` is False, `p` must be provided.")
+            self._similarities_fn = smooth_substitution_matrix_similarities_cdist
+            self._similarities_fn_kwargs = {"p": self.p}
+
+        self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        size = x.shape[:-3] + (x.shape[-3],) * 2
+        out = torch.full(
+            size, torch.nan, dtype=x.dtype, layout=x.layout, device=x.device
+        )
+        for sl in self._group_slices:
+            out[..., sl, sl].copy_(
+                self._similarities_fn(
+                    x[..., sl, :, :],
+                    subs_mat=self.subs_mat,
+                    **self._similarities_fn_kwargs,
+                )
+            )
+
+        return out
+
+# %% ../nbs/model.ipynb 22
+class BestHits(Module):
+    """Compute (reciprocal) best hits within and between groups of sequences,
+    starting from a similarity matrix.
+
+    Best hits can be either 'hard', in which cases they are computed using the
+    argmax, or 'soft', in which case they are computed using the softmax with a
+    temperature parameter `tau`. In both cases, the main diagonal in the similarity
+    matrix is excluded by setting its entries to minus infinity."""
+
+    def __init__(
+        self,
         *,
-        record_log_alphas: bool = single_fit_default_cfg["record_log_alphas"],
-        record_soft_perms: bool = single_fit_default_cfg["record_soft_perms"],
-        record_soft_losses: bool = single_fit_default_cfg["record_soft_losses"],
-    ) -> DiffPaSSResults:
-        """Initialize DiffPaSSResults object."""
-        results = DiffPaSSResults(
-            log_alphas=[] if record_log_alphas else None,
-            soft_perms=[] if record_soft_perms else None,
-            hard_perms=[],
-            soft_losses=[] if record_soft_losses else None,
-            hard_losses=[],
-        )
-
-        return results
-
-    def check_can_optimize(self) -> bool:
-        n_samples = sum(self.group_sizes)
-        n_effectively_fixed = self.permutation._total_number_fixed_pairings
-
-        return n_effectively_fixed < n_samples
-
-    def mean_center_log_alphas(self) -> None:
-        with torch.no_grad():
-            for log_alpha in self.permutation.log_alphas:
-                log_alpha[...] -= log_alpha.mean(dim=(-1, -2), keepdim=True)
+        reciprocal: bool = True,
+        group_sizes: Optional[Iterable[int]],
+        tau: float = 0.1,
+        mode: Literal["soft", "hard"] = "soft",
+    ) -> None:
+        super().__init__()
+        self.reciprocal = reciprocal
+        self.group_sizes = (
+            tuple(s for s in group_sizes) if group_sizes is not None else None
+        )
+        self._group_slices = _consecutive_slices_from_sizes(self.group_sizes)
+        self.tau = tau
+        self.mode = mode
+
+    @property
+    def mode(self) -> str:
+        return self._mode
+
+    @mode.setter
+    def mode(self, value) -> None:
+        value = value.lower()
+        if value not in ["soft", "hard"]:
+            raise ValueError("`mode` must be either 'soft' or 'hard'.")
+        self._mode = value.lower()
+        self._bh_fn = getattr(self, f"_{self._mode}_bh_fn")
+
+    def soft_(self) -> None:
+        self.mode = "soft"
+
+    def hard_(self) -> None:
+        self.mode = "hard"
 
-    def _fit(
+    def _soft_bh_fn(self, similarities: torch.Tensor) -> torch.Tensor:
+        """Compute soft best hits."""
+        return soft_best_hits(
+            similarities,
+            reciprocal=self.reciprocal,
+            group_slices=self._group_slices,
+            tau=self.tau,
+        )
+
+    def _hard_bh_fn(self, similarities: torch.Tensor) -> torch.Tensor:
+        """Compute hard best hits."""
+        return hard_best_hits(
+            similarities,
+            reciprocal=self.reciprocal,
+            group_slices=self._group_slices,
+        )
+
+    def forward(self, similarities: torch.Tensor) -> torch.Tensor:
+        return self._bh_fn(similarities)
+
+# %% ../nbs/model.ipynb 25
+class InterGroupSimilarityLoss(Module):
+    """Compute a loss that compares similarity matrices restricted to inter-group
+    relationships.
+
+    Similarity matrices are expected to be square and symmetric. The loss is computed
+    by comparing the (unrolled and concatenated) upper triangular blocks containing
+    inter-group similarities."""
+
+    def __init__(
         self,
-        x: torch.Tensor,
-        y: torch.Tensor,
         *,
-        results: DiffPaSSResults,
-        epochs: int = single_fit_default_cfg["epochs"],
-        optimizer_name: Optional[str] = single_fit_default_cfg["optimizer_name"],
-        optimizer_kwargs: Optional[dict[str, Any]] = single_fit_default_cfg[
-            "optimizer_kwargs"
-        ],
-        mean_centering: bool = single_fit_default_cfg["mean_centering"],
-        show_pbar: bool = single_fit_default_cfg["show_pbar"],
-        compute_final_soft: bool = single_fit_default_cfg["compute_final_soft"],
-        record_log_alphas: bool = single_fit_default_cfg["record_log_alphas"],
-        record_soft_perms: bool = single_fit_default_cfg["record_soft_perms"],
-        record_soft_losses: bool = single_fit_default_cfg["record_soft_losses"],
-    ) -> bool:
-        can_optimize = self.check_can_optimize()
-        if can_optimize:
-            # Initialize optimizer
-            optimizer = self.create_optimizer(optimizer_name, optimizer_kwargs)
-
-            # ------------------------------------------------------------------------------------------
-            ## Gradient descent
-            # ------------------------------------------------------------------------------------------
-            pbar = make_pbar(epochs, show_pbar)
-            for i in pbar:
-                # Record current log_alphas
-                if record_log_alphas:
-                    self._record_current_log_alphas(results)
-
-                # Hard pass
-                self._hard_pass(x, y, results=results)
-
-                # Soft pass and backward step
-                if i < epochs:
-                    loss = self._soft_pass(
-                        x,
-                        y,
-                        results=results,
-                        record_soft_perms=record_soft_perms,
-                        record_soft_losses=record_soft_losses,
-                    )
-                    loss.backward()
-                    optimizer.step()
-                    optimizer.zero_grad()
-                    if mean_centering:
-                        self.mean_center_log_alphas()
-                elif compute_final_soft:
-                    with torch.no_grad():
-                        self._soft_pass(
-                            x,
-                            y,
-                            results=results,
-                            record_soft_perms=record_soft_perms,
-                            record_soft_losses=record_soft_losses,
-                        )
-        else:
-            # Just optionally record current log_alphas and do a single hard pass
-            if record_log_alphas:
-                self._record_current_log_alphas(results)
-            self._hard_pass(x, y, results=results)
+        group_sizes: Iterable[int],
+        score_fn: Union[callable, None] = None,
+    ) -> None:
+        super().__init__()
+        self.group_sizes = tuple(s for s in group_sizes)
+        self.score_fn = (
+            partial(torch.tensordot, dims=1) if score_fn is None else score_fn
+        )
 
-        return can_optimize
+        diag_blocks_mask = torch.block_diag(
+            *[torch.ones((s, s), dtype=torch.bool) for s in self.group_sizes]
+        )
+        self.register_buffer(
+            "_upper_no_diag_blocks_mask", torch.triu(~diag_blocks_mask)
+        )
 
-    def fit(
+    def forward(
         self,
-        x: torch.Tensor,
-        y: torch.Tensor,
+        similarities_x: torch.Tensor,
+        similarities_y: torch.Tensor,
         *,
-        epochs: int = single_fit_default_cfg["epochs"],
-        optimizer_name: Optional[str] = single_fit_default_cfg["optimizer_name"],
-        optimizer_kwargs: Optional[dict[str, Any]] = single_fit_default_cfg[
-            "optimizer_kwargs"
-        ],
-        mean_centering: bool = single_fit_default_cfg["mean_centering"],
-        show_pbar: bool = single_fit_default_cfg["show_pbar"],
-        compute_final_soft: bool = single_fit_default_cfg["compute_final_soft"],
-        record_log_alphas: bool = single_fit_default_cfg["record_log_alphas"],
-        record_soft_perms: bool = single_fit_default_cfg["record_soft_perms"],
-        record_soft_losses: bool = single_fit_default_cfg["record_soft_losses"],
-    ) -> DiffPaSSResults:
-        self.prepare_fit(x, y)
-
-        # Initialize DiffPaSSResults object
-        results = self._init_results(
-            record_log_alphas=record_log_alphas,
-            record_soft_perms=record_soft_perms,
-            record_soft_losses=record_soft_losses,
-        )
-
-        self._fit(
-            x,
-            y,
-            results=results,
-            epochs=epochs,
-            optimizer_name=optimizer_name,
-            optimizer_kwargs=optimizer_kwargs,
-            mean_centering=mean_centering,
-            show_pbar=show_pbar,
-            compute_final_soft=compute_final_soft,
-            record_log_alphas=record_log_alphas,
-            record_soft_perms=record_soft_perms,
-            record_soft_losses=record_soft_losses,
+        mats: Optional[Sequence[torch.Tensor]] = None,
+    ) -> torch.Tensor:
+        # Input validation
+        assert similarities_x.ndim >= 2 and similarities_y.ndim >= 2
+
+        scores = self.score_fn(
+            similarities_x[..., self._upper_no_diag_blocks_mask],
+            similarities_y[..., self._upper_no_diag_blocks_mask],
         )
+        loss = -scores
+
+        return loss
 
-        return results
 
-    def fit_bootstrap(
+class IntraGroupSimilarityLoss(Module):
+    """Compute a loss that compares similarity matrices restricted to intra-group
+    relationships.
+
+    Similarity matrices are expected to be square and symmetric. Their diagonal
+    elements are ignored.
+    If `group_sizes` is provided, the loss is computed by comparing the (unrolled
+    and concatenated) upper triangular blocks containing intra-group similarities.
+    Otherwise, the loss is computed by comparing the upper triangular part of the
+    full similarity matrices, excluding the main diagonal."""
+
+    def __init__(
         self,
-        x: torch.Tensor,
-        y: torch.Tensor,
         *,
-        n_start: int = 1,
-        n_end: Optional[int] = None,
-        step_size: int = 1,
-        show_pbar: bool = True,
-        single_fit_cfg: Optional[dict] = None,
-    ) -> DiffPaSSResults:
-        self.prepare_fit(x, y)
-        if self.fixed_pairings is None:
-            initial_fixed_pairings = [[] for _ in self.group_sizes]
+        group_sizes: Optional[Iterable[int]] = None,
+        score_fn: Union[callable, None] = None,
+    ) -> None:
+        super().__init__()
+        self.group_sizes = (
+            tuple(s for s in group_sizes) if group_sizes is not None else None
+        )
+        self.score_fn = (
+            partial(torch.tensordot, dims=1) if score_fn is None else score_fn
+        )
+
+        if self.group_sizes is not None:
+            # Boolean mask for the main diagonal blocks corresponding to groups
+            diag_blocks_mask = torch.block_diag(
+                *[torch.ones((s, s), dtype=torch.bool) for s in self.group_sizes]
+            )
+            # Extract the upper triangular part, excluding the main diagonal
+            self.register_buffer(
+                "_upper_diag_blocks_mask", torch.triu(diag_blocks_mask, diagonal=1)
+            )
         else:
-            initial_fixed_pairings = [list(fm) for fm in self.fixed_pairings]
+            self._upper_diag_blocks_mask = None
 
-        _single_fit_cfg = deepcopy(self.single_fit_default_cfg)
-        if single_fit_cfg is not None:
-            _single_fit_cfg.update(single_fit_cfg)
-        single_fit_cfg = _single_fit_cfg
-
-        # Initialize DiffPaSSResults object
-        results = self._init_results(
-            record_log_alphas=single_fit_cfg["record_log_alphas"],
-            record_soft_perms=single_fit_cfg["record_soft_perms"],
-            record_soft_losses=single_fit_cfg["record_soft_losses"],
-        )
-        available_fields = [
-            field.name
-            for field in fields(results)
-            if getattr(results, field.name) is not None
-        ]
-        field_to_length_so_far = {field_name: 0 for field_name in available_fields}
+    def forward(
+        self,
+        similarities_x: torch.Tensor,
+        similarities_y: torch.Tensor,
+        *,
+        mats: Optional[Sequence[torch.Tensor]] = None,
+    ) -> torch.Tensor:
+        assert similarities_x.ndim >= 2 and similarities_y.ndim >= 2
+        assert similarities_x.shape[-2:] == similarities_x.shape[-2:]
 
-        n_samples = len(x)
-        n_groups = len(self.group_sizes)
-        cumsum_group_sizes = np.cumsum([0] + list(self.group_sizes))
-        offsets = np.repeat(cumsum_group_sizes[:-1], repeats=self.group_sizes)
-        group_idxs = np.repeat(np.arange(n_groups), repeats=self.group_sizes)
-
-        # First fit with initial fixed matchings
-        can_optimize = self._fit(x, y, results=results, **single_fit_cfg)
-
-        # Find effective initial fixed matchings
-        effective_initial_fixed_idxs = []
-        for s, efmz in zip(
-            cumsum_group_sizes, self.permutation._effective_fixed_pairings_zip
-        ):
-            if efmz:
-                effective_initial_fixed_idxs += [
-                    (s + efmz_fixed) for efmz_fixed in efmz[1]
-                ]
-        effective_initial_fixed_idxs = np.asarray(effective_initial_fixed_idxs)
-        nonfixed_idxs = np.setdiff1d(np.arange(n_samples), effective_initial_fixed_idxs)
-        n_effective_initial_fixed_pairings = len(effective_initial_fixed_idxs)
-
-        if n_end is None:
-            n_end = n_samples - n_effective_initial_fixed_pairings - 1
-
-        # Subsequent fits: at a given iteration we use fixed matchings chosen uniformly at
-        # random from the results of the previous iteration (excluding the effective initial
-        # fixed matchings)
-        pbar = list(range(n_start, n_end, step_size))
-        pbar = tqdm(pbar) if show_pbar else pbar
-        n_iters_with_optimization = int(can_optimize)
-        for N in pbar:
-            latest_hard_perms = results.hard_perms[-1]
-            mapped_idxs = offsets + np.concatenate(latest_hard_perms)
-            rand_fixed_idxs = np.random.permutation(nonfixed_idxs)[:N]
-            rand_fixed_idxs = np.sort(rand_fixed_idxs)
-            rand_mapped_idxs = mapped_idxs[rand_fixed_idxs]
-            rand_group_idxs = group_idxs[rand_fixed_idxs]
-            rand_fixed_rel_idxs = rand_fixed_idxs - offsets[rand_fixed_idxs]
-            rand_mapped_rel_idxs = rand_mapped_idxs - offsets[rand_mapped_idxs]
-
-            # Update fixed matchings
-            fixed_pairings = [[] for _ in range(n_groups)]
-            for rand_group_idx, mapped_rel_idx, fixed_rel_idx in zip(
-                rand_group_idxs, rand_mapped_rel_idxs, rand_fixed_rel_idxs
-            ):
-                pair = (mapped_rel_idx, fixed_rel_idx)
-                fixed_pairings[rand_group_idx].append(pair)
-            fixed_pairings = [
-                initial_fixed_pairings[k] + fixed_pairings[k] for k in range(n_groups)
-            ]
-            self.permutation.init_fixed_pairings_and_log_alphas(
-                fixed_pairings, device=x.device
+        if self._upper_diag_blocks_mask is None:
+            mask = torch.triu(
+                torch.ones(
+                    similarities_x.shape[-2:],
+                    dtype=torch.bool,
+                    layout=similarities_x.layout,
+                    device=similarities_x.device,
+                ),
+                diagonal=1,
             )
+        else:
+            mask = self._upper_diag_blocks_mask
 
-            field_to_length_so_far = {
-                field_name: len(getattr(results, field_name))
-                for field_name in available_fields
-            }
-            can_optimize = self._fit(x, y, results=results, **single_fit_cfg)
-            if can_optimize:
-                n_iters_with_optimization += 1
-            else:
-                break
-
-        # Reshape results according to number of iterations performed
-        for field_name in available_fields:
-            results_this_field = getattr(results, field_name)
-            n_optimized_results_this_field = (
-                len(results_this_field)
-                if can_optimize
-                else field_to_length_so_far[field_name]
-            )
-
-            assert not n_optimized_results_this_field % n_iters_with_optimization
-            n_in_each_optimized_iter = (
-                n_optimized_results_this_field // n_iters_with_optimization
-            )
-            setattr(
-                results,
-                field_name,
-                [
-                    results_this_field[
-                        j
-                        * n_in_each_optimized_iter : (j + 1)
-                        * n_in_each_optimized_iter
-                    ]
-                    for j in range(n_iters_with_optimization)
-                ]
-                + [results_this_field[n_optimized_results_this_field:]],
-            )
+        scores = self.score_fn(similarities_x[..., mask], similarities_y[..., mask])
+        loss = -scores
 
-        return results
+        return loss
```

### Comparing `diffpass-0.0.1/diffpass/constants.py` & `diffpass-0.1.0/diffpass/constants.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass/data_utils.py` & `diffpass-0.1.0/diffpass/data_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,70 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/data_utils.ipynb.
 
 # %% auto 0
-__all__ = ['SeqRecord', 'SeqRecords', 'GroupwiseSeqRecords', 'create_groupwise_seq_records', 'pad_msas_with_dummy_sequences',
-           'get_single_and_paired_seqs', 'one_hot_encode_msa', 'compute_num_correct_pairings',
-           'compute_comparable_group_idxs']
+__all__ = ['SeqRecord', 'SeqRecords', 'GroupwiseSeqRecords', 'create_groupwise_seq_records', 'remove_groups_not_in_both',
+           'pad_msas_with_dummy_sequences', 'get_single_and_paired_seqs', 'one_hot_encode_msa',
+           'compute_num_correct_pairings', 'compute_comparable_group_idxs']
 
 # %% ../nbs/data_utils.ipynb 4
 from collections import defaultdict
 from collections.abc import Sequence
 from typing import Optional, Union
 from copy import deepcopy
 
 import numpy as np
 
 import torch
 
 from .constants import DEFAULT_AA_TO_INT
 
-
+# Type aliases
 SeqRecord = tuple[str, str]
 SeqRecords = list[SeqRecord]
 GroupwiseSeqRecords = dict[str, SeqRecords]
 
-# %% ../nbs/data_utils.ipynb 5
+# %% ../nbs/data_utils.ipynb 6
 def create_groupwise_seq_records(
-    seq_records: dict[str, SeqRecords],
+    seq_records: SeqRecords,
     group_name_func: callable,
     *,
     remove_groups_with_one_seq: bool = True,
 ) -> GroupwiseSeqRecords:
+    """Group records of the form ``(header, sequence)`` in a collection by group name
+    (e.g. species name), extracted from header information using `group_name_func`."""
     data_group_by_group = defaultdict(SeqRecords)
     for rec in seq_records:
         group_name = group_name_func(rec[0])
         data_group_by_group[group_name].append(rec)
 
     if remove_groups_with_one_seq:
         for group_name in list(data_group_by_group.keys()):
             if len(data_group_by_group[group_name]) < 2:
                 data_group_by_group.pop(group_name)
 
     return data_group_by_group
 
 
+def remove_groups_not_in_both(
+    data_group_by_group_x: GroupwiseSeqRecords,
+    data_group_by_group_y: GroupwiseSeqRecords,
+) -> tuple[GroupwiseSeqRecords, GroupwiseSeqRecords]:
+    """Remove groups that are not present in both input collections."""
+    group_names = set(data_group_by_group_x.keys()) & set(data_group_by_group_y.keys())
+
+    data_group_by_group_x_common = {
+        group_name: data_group_by_group_x[group_name] for group_name in group_names
+    }
+    data_group_by_group_y_common = {
+        group_name: data_group_by_group_y[group_name] for group_name in group_names
+    }
+
+    return data_group_by_group_x_common, data_group_by_group_y_common
+
+
 def pad_msas_with_dummy_sequences(
     data_group_by_group_x: GroupwiseSeqRecords,
     data_group_by_group_y: GroupwiseSeqRecords,
     *,
     dummy_symbol: str = "-",
 ) -> tuple[GroupwiseSeqRecords, GroupwiseSeqRecords]:
     """Pad MSAs with dummy sequences so that all groups/species contain the same
@@ -136,15 +155,15 @@
 
     return {
         "x_seqs_by_group": x_seqs_by_group,
         "y_seqs_by_group": y_seqs_by_group,
         "xy_seqs_to_counts_by_group": xy_seqs_to_counts_by_group,
     }
 
-# %% ../nbs/data_utils.ipynb 6
+# %% ../nbs/data_utils.ipynb 10
 def one_hot_encode_msa(
     seq_records: SeqRecords,
     aa_to_int: Optional[dict[str, int]] = None,
     device: Optional[torch.device] = None,
 ) -> torch.Tensor:
     """
     Given a list of records of the form (header, sequence), assumed to be a parsed MSA,
@@ -161,15 +180,15 @@
 
     tokenized_records_oh = torch.nn.functional.one_hot(tokenized_records).to(
         torch.get_default_dtype()
     )
 
     return tokenized_records_oh
 
-# %% ../nbs/data_utils.ipynb 8
+# %% ../nbs/data_utils.ipynb 12
 def compute_num_correct_pairings(
     hard_perms_by_group: list[np.ndarray],
     *,
     compare_to_identity_permutation: bool,
     single_and_paired_seqs: Optional[dict[str, list]] = None,
 ) -> int:
     """Compute the total number of correct pairings.
@@ -209,15 +228,15 @@
                 xy_key = f"{x_seq}:{y_seq}"
                 if _xy_seqs_to_counts_this_group.get(xy_key, 0) > 0:
                     _xy_seqs_to_counts_this_group[xy_key] -= 1
                     correct += 1
 
     return correct
 
-# %% ../nbs/data_utils.ipynb 10
+# %% ../nbs/data_utils.ipynb 14
 def compute_comparable_group_idxs(
     group_sizes_arr: np.ndarray, *, max_size_ratio: int, max_group_size: int
 ) -> np.ndarray:
     # 1) Groups which have non-zero count for both families but where not both counts are equal to 1
     # NOTE: In AlphaFold this excludes the query (dummy group of size 1)
     mask_not_zero_in_one = (group_sizes_arr[:, 0] * group_sizes_arr[:, 1] != 0) * (
         group_sizes_arr[:, 0] * group_sizes_arr[:, 1] != 1
```

### Comparing `diffpass-0.0.1/diffpass/entropy_ops.py` & `diffpass-0.1.0/diffpass/entropy_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass/gumbel_sinkhorn_ops.py` & `diffpass-0.1.0/diffpass/gumbel_sinkhorn_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass/msa_parsing.py` & `diffpass-0.1.0/diffpass/msa_parsing.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass/sequence_similarity_ops.py` & `diffpass-0.1.0/diffpass/sequence_similarity_ops.py`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/diffpass.egg-info/SOURCES.txt` & `diffpass-0.1.0/diffpass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffpass-0.0.1/settings.ini` & `diffpass-0.1.0/settings.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = DiffPaSS
 lib_name = diffpass
-version = 0.0.1
+version = 0.1.0
 min_python = 3.7
 license = apache2
 black_formatting = True
-
-### nbdev ###
 doc_path = _docs
-lib_path = %(lib_name)s
+lib_path = diffpass
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://Bitbol-Lab.github.io
+doc_baseurl = /DiffPaSS
+git_url = https://github.com/Bitbol-Lab/DiffPaSS
+title = diffpass
 audience = Developers
 author = Umberto Lupo and Damiano Sgarbossa
 author_email = umberto.lupo@epfl.ch, damiano.sgarbossa@epfl.ch
-copyright = 2024 onwards, %(author)s
+copyright = 2024 onwards, Umberto Lupo and Damiano Sgarbossa
 description = Differentiable Pairing using Soft Scores
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
-user = ulupo
-
-### Optional ###
+user = lupo
 requirements = torch numpy scipy matplotlib biopython tqdm pandas
 conda_requirements = pytorch
 dev_requirements = nbdev black jupyter pre-commit
-# console_scripts =
+readme_nb = index.ipynb
+allowed_metadata_keys =
+allowed_cell_metadata_keys =
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
```

### Comparing `diffpass-0.0.1/setup.py` & `diffpass-0.1.0/setup.py`

 * *Files identical despite different names*

