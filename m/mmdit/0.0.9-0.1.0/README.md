# Comparing `tmp/mmdit-0.0.9.tar.gz` & `tmp/mmdit-0.1.0.tar.gz`

## Comparing `mmdit-0.0.9.tar` & `mmdit-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/__init__.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/mmdit_generalized_pytorch.py
--rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.9/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.9/LICENSE
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.9/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.1.0/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.1.0/mmdit/__init__.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 mmdit-0.1.0/mmdit/adaptive_attention.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 mmdit-0.1.0/mmdit/mmdit_generalized_pytorch.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 mmdit-0.1.0/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 mmdit-0.1.0/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 mmdit-0.1.0/PKG-INFO
```

### Comparing `mmdit-0.0.9/mmdit.png` & `mmdit-0.1.0/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.9/.github/workflows/python-publish.yml` & `mmdit-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.9/mmdit/mmdit_generalized_pytorch.py` & `mmdit-0.1.0/mmdit/mmdit_generalized_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from torch import Tensor
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
 from einops import rearrange, pack, unpack
 from einops.layers.torch import Rearrange
 
-from x_transformers import FeedForward
+from x_transformers import (
+    RMSNorm,
+    FeedForward
+)
 
 from mmdit.mmdit_pytorch import (
     JointAttention
 )
 
 # helpers
 
@@ -186,28 +189,35 @@
 # mm dit transformer - simply many blocks
 
 class MMDiT(Module):
     def __init__(
         self,
         *,
         depth,
+        dim_modalities,
+        final_norms = True,
         **block_kwargs
     ):
         super().__init__()
-        blocks = [MMDiTBlock(**block_kwargs) for _ in range(depth)]
+        blocks = [MMDiTBlock(dim_modalities = dim_modalities, **block_kwargs) for _ in range(depth)]
         self.blocks = ModuleList(blocks)
 
+        norms = [RMSNorm(dim) for dim in dim_modalities]
+        self.norms = ModuleList(norms)
+
     def forward(
         self,
         *,
         modality_tokens: Tuple[Tensor, ...],
         modality_masks: Tuple[Tensor | None, ...] | None = None,
         time_cond = None
     ):
         for block in self.blocks:
             modality_tokens = block(
                 time_cond = time_cond,
                 modality_tokens = modality_tokens,
                 modality_masks = modality_masks
             )
 
-        return modality_tokens
+        modality_tokens = [norm(tokens) for tokens, norm in zip(modality_tokens, self.norms)]
+
+        return tuple(modality_tokens)
```

### Comparing `mmdit-0.0.9/mmdit/mmdit_pytorch.py` & `mmdit-0.1.0/mmdit/mmdit_pytorch.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 
 import torch
 from torch import nn
 from torch import Tensor
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
-from einops import rearrange, pack, unpack
+from einops import rearrange, repeat, pack, unpack
 from einops.layers.torch import Rearrange
 
 from x_transformers.attend import Attend
-from x_transformers import FeedForward
+from x_transformers import (
+    RMSNorm,
+    FeedForward
+)
 
 # helpers
 
 def exists(v):
     return v is not None
 
 def default(v, d):
@@ -325,37 +328,61 @@
 # mm dit transformer - simply many blocks
 
 class MMDiT(Module):
     def __init__(
         self,
         *,
         depth,
+        dim_image,
+        num_register_tokens = 0,
+        final_norm = True,
         **block_kwargs
     ):
         super().__init__()
+
+        self.has_register_tokens = num_register_tokens > 0
+        self.register_tokens = nn.Parameter(torch.zeros(num_register_tokens, dim_image))
+        nn.init.normal_(self.register_tokens, std = 0.02)
+
         self.blocks = ModuleList([])
 
         for _ in range(depth):
-            block = MMDiTBlock(**block_kwargs)
+            block = MMDiTBlock(
+                dim_image = dim_image,
+                **block_kwargs
+            )
+
             self.blocks.append(block)
 
+        self.norm = RMSNorm(dim_image) if final_norm else nn.Identity()
+
     def forward(
         self,
         *,
         text_tokens,
         image_tokens,
         text_mask = None,
         time_cond = None,
         should_skip_last_feedforward = True
     ):
+
+        if self.has_register_tokens:
+            register_tokens = repeat(self.register_tokens, 'n d -> b n d', b = image_tokens.shape[0])
+            image_tokens, packed_shape = pack([register_tokens, image_tokens], 'b * d')
+
         for ind, block in enumerate(self.blocks):
             is_last = ind == (len(self.blocks) - 1)
 
             text_tokens, image_tokens = block(
                 time_cond = time_cond,
                 text_tokens = text_tokens,
                 image_tokens = image_tokens,
                 text_mask = text_mask,
                 skip_feedforward_text_tokens = is_last and should_skip_last_feedforward
             )
 
+        if self.has_register_tokens:
+            _, image_tokens = unpack(image_tokens, packed_shape, 'b * d')
+
+        image_tokens = self.norm(image_tokens)
+
         return text_tokens, image_tokens
```

### Comparing `mmdit-0.0.9/.gitignore` & `mmdit-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.9/LICENSE` & `mmdit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.9/README.md` & `mmdit-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="./mmdit.png" width="300px"></img>
 
-## MMDiT (wip)
+## MMDiT
 
-Implementation of a single layer of the MMDiT, proposed by Esser et al. in <a href="https://arxiv.org/abs/2403.03206">Stable Diffusion 3</a>, in Pytorch and Jax
+Implementation of a single layer of the MMDiT, proposed by Esser et al. in <a href="https://arxiv.org/abs/2403.03206">Stable Diffusion 3</a>, in Pytorch
 
 Besides a straight reproduction, will also generalize to > 2 modalities, as I can envision an MMDiT for images, audio, and text.
 
 Will also offer an improvised variant of the attention that adaptively selects the weights to use through learned gating.
 
 ## Install
 
@@ -91,7 +91,16 @@
     author  = {Patrick Esser and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and Robin Rombach},
     journal = {ArXiv},
     year    = {2024},
     volume  = {abs/2403.03206},
     url     = {https://api.semanticscholar.org/CorpusID:268247980}
 }
 ```
+
+```bibtex
+@inproceedings{Darcet2023VisionTN,
+    title   = {Vision Transformers Need Registers},
+    author  = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal and Piotr Bojanowski},
+    year    = {2023},
+    url     = {https://api.semanticscholar.org/CorpusID:263134283}
+}
+```
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
-[./mmdit.png]## MMDiT (wip) Implementation of a single layer of the MMDiT,
-proposed by Esser et al. in _S_t_a_b_l_e_ _D_i_f_f_u_s_i_o_n_ _3, in Pytorch and Jax Besides a
-straight reproduction, will also generalize to > 2 modalities, as I can
-envision an MMDiT for images, audio, and text. Will also offer an improvised
-variant of the attention that adaptively selects the weights to use through
-learned gating. ## Install ```bash $ pip install mmdit ``` ## Usage ```python
-import torch from mmdit import MMDiTBlock # define mm dit block block =
-MMDiTBlock( dim_joint_attn = 512, dim_cond = 256, dim_text = 768, dim_image =
-512, qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256)
-text_tokens = torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool()
-image_tokens = torch.randn(1, 1024, 512) # single block forward
-text_tokens_next, image_tokens_next = block( time_cond = time_cond, text_tokens
-= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` A
-generalized version can be used as so ```python import torch from
-mmdit.mmdit_generalized_pytorch import MMDiT mmdit = MMDiT( depth = 2,
-dim_modalities = (768, 512, 384), dim_joint_attn = 512, dim_cond = 256,
+[./mmdit.png]## MMDiT Implementation of a single layer of the MMDiT, proposed
+by Esser et al. in _S_t_a_b_l_e_ _D_i_f_f_u_s_i_o_n_ _3, in Pytorch Besides a straight
+reproduction, will also generalize to > 2 modalities, as I can envision an
+MMDiT for images, audio, and text. Will also offer an improvised variant of the
+attention that adaptively selects the weights to use through learned gating. ##
+Install ```bash $ pip install mmdit ``` ## Usage ```python import torch from
+mmdit import MMDiTBlock # define mm dit block block = MMDiTBlock
+( dim_joint_attn = 512, dim_cond = 256, dim_text = 768, dim_image = 512,
 qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256) text_tokens =
-torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool() video_tokens =
-torch.randn(1, 1024, 512) audio_tokens = torch.randn(1, 256, 384) # forward
-text_tokens, video_tokens, audio_tokens = mmdit( modality_tokens =
-(text_tokens, video_tokens, audio_tokens), modality_masks = (text_mask, None,
-None), time_cond = time_cond, ) ``` ## Citations ```bibtex @article
+torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool() image_tokens =
+torch.randn(1, 1024, 512) # single block forward text_tokens_next,
+image_tokens_next = block( time_cond = time_cond, text_tokens = text_tokens,
+text_mask = text_mask, image_tokens = image_tokens ) ``` A generalized version
+can be used as so ```python import torch from mmdit.mmdit_generalized_pytorch
+import MMDiT mmdit = MMDiT( depth = 2, dim_modalities = (768, 512, 384),
+dim_joint_attn = 512, dim_cond = 256, qk_rmsnorm = True ) # mock inputs
+time_cond = torch.randn(1, 256) text_tokens = torch.randn(1, 512, 768)
+text_mask = torch.ones((1, 512)).bool() video_tokens = torch.randn(1, 1024,
+512) audio_tokens = torch.randn(1, 256, 384) # forward text_tokens,
+video_tokens, audio_tokens = mmdit( modality_tokens = (text_tokens,
+video_tokens, audio_tokens), modality_masks = (text_mask, None, None),
+time_cond = time_cond, ) ``` ## Citations ```bibtex @article
 {Esser2024ScalingRF, title = {Scaling Rectified Flow Transformers for High-
 Resolution Image Synthesis}, author = {Patrick Esser and Sumith Kulal and A.
 Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and
 Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim
 Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and
 Robin Rombach}, journal = {ArXiv}, year = {2024}, volume = {abs/2403.03206},
-url = {https://api.semanticscholar.org/CorpusID:268247980} } ```
+url = {https://api.semanticscholar.org/CorpusID:268247980} } ``` ```bibtex
+@inproceedings{Darcet2023VisionTN, title = {Vision Transformers Need
+Registers}, author = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal and
+Piotr Bojanowski}, year = {2023}, url = {https://api.semanticscholar.org/
+CorpusID:263134283} } ```
```

### Comparing `mmdit-0.0.9/pyproject.toml` & `mmdit-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.9"
+version = "0.1.0"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.9/PKG-INFO` & `mmdit-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.9
+Version: 0.1.0
 Summary: MMDiT
 Project-URL: Homepage, https://pypi.org/project/mmdit/
 Project-URL: Repository, https://github.com/lucidrains/mmdit
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -38,17 +38,17 @@
 Requires-Dist: torch>=2.0
 Requires-Dist: x-transformers>=1.28.5
 Provides-Extra: examples
 Description-Content-Type: text/markdown
 
 <img src="./mmdit.png" width="300px"></img>
 
-## MMDiT (wip)
+## MMDiT
 
-Implementation of a single layer of the MMDiT, proposed by Esser et al. in <a href="https://arxiv.org/abs/2403.03206">Stable Diffusion 3</a>, in Pytorch and Jax
+Implementation of a single layer of the MMDiT, proposed by Esser et al. in <a href="https://arxiv.org/abs/2403.03206">Stable Diffusion 3</a>, in Pytorch
 
 Besides a straight reproduction, will also generalize to > 2 modalities, as I can envision an MMDiT for images, audio, and text.
 
 Will also offer an improvised variant of the attention that adaptively selects the weights to use through learned gating.
 
 ## Install
 
@@ -133,7 +133,16 @@
     author  = {Patrick Esser and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and Robin Rombach},
     journal = {ArXiv},
     year    = {2024},
     volume  = {abs/2403.03206},
     url     = {https://api.semanticscholar.org/CorpusID:268247980}
 }
 ```
+
+```bibtex
+@inproceedings{Darcet2023VisionTN,
+    title   = {Vision Transformers Need Registers},
+    author  = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal and Piotr Bojanowski},
+    year    = {2023},
+    url     = {https://api.semanticscholar.org/CorpusID:263134283}
+}
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.9 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.1.0 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -19,36 +19,39 @@
 intelligence,attention mechanism,deep learning,multi-modal transformer
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.9 Requires-Dist:
 einops>=0.8.0 Requires-Dist: torch>=2.0 Requires-Dist: x-transformers>=1.28.5
 Provides-Extra: examples Description-Content-Type: text/markdown [./
-mmdit.png]## MMDiT (wip) Implementation of a single layer of the MMDiT,
-proposed by Esser et al. in _S_t_a_b_l_e_ _D_i_f_f_u_s_i_o_n_ _3, in Pytorch and Jax Besides a
-straight reproduction, will also generalize to > 2 modalities, as I can
-envision an MMDiT for images, audio, and text. Will also offer an improvised
-variant of the attention that adaptively selects the weights to use through
-learned gating. ## Install ```bash $ pip install mmdit ``` ## Usage ```python
-import torch from mmdit import MMDiTBlock # define mm dit block block =
-MMDiTBlock( dim_joint_attn = 512, dim_cond = 256, dim_text = 768, dim_image =
-512, qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256)
-text_tokens = torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool()
-image_tokens = torch.randn(1, 1024, 512) # single block forward
-text_tokens_next, image_tokens_next = block( time_cond = time_cond, text_tokens
-= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` A
-generalized version can be used as so ```python import torch from
-mmdit.mmdit_generalized_pytorch import MMDiT mmdit = MMDiT( depth = 2,
-dim_modalities = (768, 512, 384), dim_joint_attn = 512, dim_cond = 256,
-qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256) text_tokens =
-torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool() video_tokens =
-torch.randn(1, 1024, 512) audio_tokens = torch.randn(1, 256, 384) # forward
-text_tokens, video_tokens, audio_tokens = mmdit( modality_tokens =
-(text_tokens, video_tokens, audio_tokens), modality_masks = (text_mask, None,
-None), time_cond = time_cond, ) ``` ## Citations ```bibtex @article
-{Esser2024ScalingRF, title = {Scaling Rectified Flow Transformers for High-
-Resolution Image Synthesis}, author = {Patrick Esser and Sumith Kulal and A.
-Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and
-Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim
-Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and
-Robin Rombach}, journal = {ArXiv}, year = {2024}, volume = {abs/2403.03206},
-url = {https://api.semanticscholar.org/CorpusID:268247980} } ```
+mmdit.png]## MMDiT Implementation of a single layer of the MMDiT, proposed by
+Esser et al. in _S_t_a_b_l_e_ _D_i_f_f_u_s_i_o_n_ _3, in Pytorch Besides a straight reproduction,
+will also generalize to > 2 modalities, as I can envision an MMDiT for images,
+audio, and text. Will also offer an improvised variant of the attention that
+adaptively selects the weights to use through learned gating. ## Install
+```bash $ pip install mmdit ``` ## Usage ```python import torch from mmdit
+import MMDiTBlock # define mm dit block block = MMDiTBlock( dim_joint_attn =
+512, dim_cond = 256, dim_text = 768, dim_image = 512, qk_rmsnorm = True ) #
+mock inputs time_cond = torch.randn(1, 256) text_tokens = torch.randn(1, 512,
+768) text_mask = torch.ones((1, 512)).bool() image_tokens = torch.randn(1,
+1024, 512) # single block forward text_tokens_next, image_tokens_next = block
+( time_cond = time_cond, text_tokens = text_tokens, text_mask = text_mask,
+image_tokens = image_tokens ) ``` A generalized version can be used as so
+```python import torch from mmdit.mmdit_generalized_pytorch import MMDiT mmdit
+= MMDiT( depth = 2, dim_modalities = (768, 512, 384), dim_joint_attn = 512,
+dim_cond = 256, qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1,
+256) text_tokens = torch.randn(1, 512, 768) text_mask = torch.ones((1,
+512)).bool() video_tokens = torch.randn(1, 1024, 512) audio_tokens =
+torch.randn(1, 256, 384) # forward text_tokens, video_tokens, audio_tokens =
+mmdit( modality_tokens = (text_tokens, video_tokens, audio_tokens),
+modality_masks = (text_mask, None, None), time_cond = time_cond, ) ``` ##
+Citations ```bibtex @article{Esser2024ScalingRF, title = {Scaling Rectified
+Flow Transformers for High-Resolution Image Synthesis}, author = {Patrick Esser
+and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry
+Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and
+Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin
+and Yannik Marek and Robin Rombach}, journal = {ArXiv}, year = {2024}, volume =
+{abs/2403.03206}, url = {https://api.semanticscholar.org/CorpusID:268247980} }
+``` ```bibtex @inproceedings{Darcet2023VisionTN, title = {Vision Transformers
+Need Registers}, author = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal
+and Piotr Bojanowski}, year = {2023}, url = {https://api.semanticscholar.org/
+CorpusID:263134283} } ```
```

