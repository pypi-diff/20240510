# Comparing `tmp/meshgpt-pytorch-1.1.1.tar.gz` & `tmp/meshgpt_pytorch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt-pytorch-1.1.1.tar", last modified: Thu Mar 14 02:22:47 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.0.tar", last modified: Fri May 10 17:54:10 2024, max compression
```

## Comparing `meshgpt-pytorch-1.1.1.tar` & `meshgpt_pytorch-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:22:47.851175 meshgpt-pytorch-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-14 02:22:47.851175 meshgpt-pytorch-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:22:47.851175 meshgpt-pytorch-1.1.1/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    49273 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:22:47.851175 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-14 02:22:47.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-14 02:22:47.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:22:47.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-14 02:22:47.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 02:22:47.000000 meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 02:22:47.851175 meshgpt-pytorch-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-14 02:22:40.000000 meshgpt-pytorch-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50365 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 17:54:10.000000 meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:54:10.459637 meshgpt_pytorch-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 17:54:06.000000 meshgpt_pytorch-1.2.0/setup.py
```

### Comparing `meshgpt-pytorch-1.1.1/LICENSE` & `meshgpt_pytorch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt-pytorch-1.1.1/PKG-INFO` & `meshgpt_pytorch-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.1.1
+Version: 1.2.0
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt-pytorch-1.1.1/README.md` & `meshgpt_pytorch-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt-pytorch-1.1.1/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.0/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt-pytorch-1.1.1/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.0/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,28 @@
 
     if remainder <= 0:
         return t
 
     padding = (0, remainder) if right else (remainder, 0)
     return pad_at_dim(t, padding, dim = dim, value = value)
 
+def masked_mean(tensor, mask, dim = -1, eps = 1e-5):
+    if not exists(mask):
+        return tensor.mean(dim = dim)
+
+    mask = rearrange(mask, '... -> ... 1')
+    tensor = tensor.masked_fill(~mask, 0.)
+
+    total_el = mask.sum(dim = dim)
+    num = tensor.sum(dim = dim)
+    den = total_el.float().clamp(min = eps)
+    mean = num / den
+    mean = mean.masked_fill(total_el == 0, 0.)
+    return mean
+
 # continuous embed
 
 def ContinuousEmbed(dim_cont):
     return nn.Sequential(
         Rearrange('... -> ... 1'),
         nn.Linear(1, dim_cont),
         nn.SiLU(),
@@ -1035,17 +1049,22 @@
 
         self.autoencoder = autoencoder
         set_module_requires_grad_(autoencoder, False)
 
         self.codebook_size = autoencoder.codebook_size
         self.num_quantizers = autoencoder.num_quantizers
 
-        self.sos_token = nn.Parameter(torch.randn(dim_fine))
         self.eos_token_id = self.codebook_size
 
+        # the fine transformer sos token
+        # as well as a projection of pooled text embeddings to condition it
+        # (todo) - sos token should be moved to the coarse transformer stage
+
+        self.sos_token = nn.Parameter(torch.randn(dim_fine))
+
         # they use axial positional embeddings
 
         assert divisible_by(max_seq_len, self.num_vertices_per_face * self.num_quantizers), f'max_seq_len ({max_seq_len}) must be divisible by (3 x {self.num_quantizers}) = {3 * self.num_quantizers}' # 3 or 4 vertices per face, with D codes per vertex
 
         self.token_embed = nn.Embedding(self.codebook_size + 1, dim)
 
         self.quantize_level_embed = nn.Parameter(torch.randn(self.num_quantizers, dim))
@@ -1063,15 +1082,19 @@
         cross_attn_dim_context = None
 
         if condition_on_text:
             self.conditioner = TextEmbeddingReturner(
                 model_types = text_condition_model_types,
                 cond_drop_prob = text_condition_cond_drop_prob
             )
-            cross_attn_dim_context = self.conditioner.dim_latent
+
+            dim_text = self.conditioner.dim_latent
+            cross_attn_dim_context = dim_text
+
+            self.to_sos_text_cond = nn.Linear(dim_text, dim_fine)
 
         # for summarizing the vertices of each face
 
         self.to_face_tokens = nn.Sequential(
             nn.Linear(self.num_quantizers * self.num_vertices_per_face * dim, dim),
             nn.LayerNorm(dim)
         )
@@ -1433,18 +1456,32 @@
         else:
             attended_face_codes = cached_attended_face_codes
 
         # maybe project from coarse to fine dimension for hierarchical transformers
 
         attended_face_codes = self.maybe_project_coarse_to_fine(attended_face_codes)
 
-        # auto prepend sos token
+        # repeat sos token across batch
 
         sos = repeat(self.sos_token, 'd -> b d', b = batch)
 
+        # condition sos token if needed
+
+        if self.condition_on_text:
+            pooled_text_embed = masked_mean(
+                maybe_dropped_text_embeds.embed,
+                maybe_dropped_text_embeds.mask,
+                dim = 1
+            )
+
+            sos_cond = self.to_sos_text_cond(pooled_text_embed)
+            sos = sos + sos_cond
+
+        # auto prepend sos token
+
         attended_face_codes_with_sos, _ = pack([sos, attended_face_codes], 'b * d')
 
         grouped_codes = pad_to_length(grouped_codes, attended_face_codes_with_sos.shape[-2], dim = 1)
         fine_vertex_codes, _ = pack([attended_face_codes_with_sos, grouped_codes], 'b n * d')
 
         fine_vertex_codes = fine_vertex_codes[..., :-1, :]
```

### Comparing `meshgpt-pytorch-1.1.1/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.0/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt-pytorch-1.1.1/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.0/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.1.1
+Version: 1.2.0
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt-pytorch-1.1.1/setup.py` & `meshgpt_pytorch-1.2.0/setup.py`

 * *Files identical despite different names*

