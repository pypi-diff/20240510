# Comparing `tmp/xtrain-0.3.1.tar.gz` & `tmp/xtrain-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.3.1.tar", max compression
+gzip compressed data, was "xtrain-0.3.2.tar", max compression
```

## Comparing `xtrain-0.3.1.tar` & `xtrain-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-05-05 16:05:49.418701 xtrain-0.3.1/LICENSE
--rw-r--r--   0        0        0     1231 2024-05-05 16:05:49.418701 xtrain-0.3.1/README.md
--rw-r--r--   0        0        0      833 2024-05-05 16:06:05.574922 xtrain-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      203 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/__init__.py
--rw-r--r--   0        0        0    12105 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/base_trainer.py
--rw-r--r--   0        0        0     3977 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/closure.py
--rw-r--r--   0        0        0     1631 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/loss.py
--rw-r--r--   0        0        0     4901 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/strategy.py
--rw-r--r--   0        0        0     6490 2024-05-05 16:05:49.422701 xtrain-0.3.1/xtrain/utils.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-10 19:15:25.469526 xtrain-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1832 2024-05-10 19:15:25.469526 xtrain-0.3.2/README.md
+-rw-r--r--   0        0        0      833 2024-05-10 19:15:42.133483 xtrain-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/__init__.py
+-rw-r--r--   0        0        0    13430 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     3968 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/closure.py
+-rw-r--r--   0        0        0     1631 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/loss.py
+-rw-r--r--   0        0        0     4215 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/strategy.py
+-rw-r--r--   0        0        0     7892 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/utils.py
+-rw-r--r--   0        0        0     2165 1970-01-01 00:00:00.000000 xtrain-0.3.2/PKG-INFO
```

### Comparing `xtrain-0.3.1/LICENSE` & `xtrain-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.1/README.md` & `xtrain-0.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     loss = ....
     return loss
 ```
 
 #### Step 3: create an iterator that supplies training data
 
 ```
-my_data = itertools.cycle(
-    zip(sequence_of_inputs, sequence_of_labels)
-)
+my_data = zip(sequence_of_inputs, sequence_of_labels)
 ```
 
 #### Step 4: train
 
 ```
 # create and initialize a Trainer object
 trainer = xtrain.Trainer(
@@ -43,18 +41,47 @@
   losses = my_loss_func,
   optimizer = optax.adam(1e-4),
 )
 
 train_iter = trainer.train(my_data) # returns a iterable object
 
 # iterate the train_iter trains the model
-for step in range(train_steps):
-    model_out = next(train_iter)
-    if step // 1000 == 0:
-        print(train_iter.loss_logs)
-        train_iter.reset_loss_logs()
+for epoch in range(3):
+  for model_out in train_iter:
+    pass
+  print(train_iter.loss_logs)
+  train_iter.reset_loss_logs()
+```
+
+### Training data format
+
+- tensowflow Dataset
+- torch dataloader
+- generator function
+- other python iterable that produce numpy data
+
+### Checkpointing
+
+train_iter is orbax compatible.
+
+```
+import orbax.checkpoint as ocp
+ocp.StandardCheckpointer().save(cp_path, args=ocp.args.StandardSave(train_iter))
+```
+
+### Freeze submodule
+```
+train_iter.freeze("submodule/Dense_0/kernel")
+```
+
+### Simple batch parallelism on multiple device
+```
+# Add a new batch dim to you dataset
+ds = ds.batch(8)
+# create trainer with the Distributed strategy
+trainer_iter = xtrain.Trainer(model, losses, optimizer, strategy=xtrain.Distributed).train(ds)
 ```
 
-### Full documentation
+### API documentation
 
 https://jiyuuchc.github.io/xtrain/
```

### Comparing `xtrain-0.3.1/pyproject.toml` & `xtrain-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.3.1"
+version = "0.3.2"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flax = "^0.8"
```

### Comparing `xtrain-0.3.1/xtrain/base_trainer.py` & `xtrain-0.3.2/xtrain/base_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,20 @@
     def loss(self):
         return self._compute_loss_log()
 
     @property
     def has_aux(self):
         return self.ctx.mutable or self.ctx.capture_intermediates
 
+    @property
+    def vars_and_params(self):
+        v = self.variables.copy()
+        v["params"] = self.train_state["params"]
+        return v
+
     def __iter__(self):
         self.data = Peekable(iter(self.ctx.dataset))
         return self
 
     def _compute_loss_log(self) -> dict:
         return {
             _get_name(loss_log.loss_fn): loss_log.compute()
@@ -327,14 +333,15 @@
 
     def test(
         self,
         dataset: Iterable,
         metrics: METRICS,
         variables: dict,
         strategy: type | None = None,
+        method: Union[Callable[..., Any], str, None] = None,
         **kwargs,
     ) -> Iterator:
         """Create test/validation iterator.
 
         Args:
             dataset: An iterator or iterable to supply the testing data.
                 The iterator should yield a tupple of (inputs, labels).
@@ -358,15 +365,21 @@
             metrics = [metrics]
         try:
             iter(metrics)
         except TypeError:
             metrics = [metrics]
         metrics = [m if isinstance(m, Metric) else LossLog(m) for m in metrics]
 
-        apply_fn = _cached_partial(self.model.apply, **kwargs)
+        apply_fn=_cached_partial(
+            self.model.apply,
+            mutable=self.mutable,
+            capture_intermediates=self.capture_intermediates,
+            method=method,
+            **kwargs,
+        )
 
         predict_fn = strategy.predict
 
         for data in dataset:
             inputs, _, _ = unpack_x_y_sample_weight(data)
             preds = predict_fn(apply_fn, variables, inputs)
             kwargs = dict(
@@ -383,7 +396,35 @@
 
         Returns:
             A metric dict. Keys are metric names.
         """
         for metrics in self.test(*args, **kwargs):
             pass
         return {_get_name(m): m.compute() for m in metrics}
+
+    def predict(self, dataset: Iterable, variables: dict, strategy: type | None = None, method: Union[Callable[..., Any], str, None] = None, **kwargs):
+        """Create predictor iterator.
+
+        Args:
+            dataset: An iterator or iterable to supply the input data.
+            variables: Model weights etc. typically get from TrainIterator
+            strategy: Optionally override the default backend.
+
+        Returns:
+            An iterator. Stepping through it will produce model predictions
+        """
+        if strategy is None:
+            strategy = self.strategy
+
+        apply_fn=_cached_partial(
+            self.model.apply,
+            mutable=self.mutable,
+            capture_intermediates=self.capture_intermediates,
+            method=method,
+            **kwargs,
+        )
+
+        predict_fn = strategy.predict
+
+        for inputs in dataset:
+            preds = predict_fn(apply_fn, variables, inputs)
+            yield preds
```

### Comparing `xtrain-0.3.1/xtrain/closure.py` & `xtrain-0.3.2/xtrain/closure.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,48 +78,47 @@
     training.
 """
 
 class Adversal(nn.Module):
     main_module: nn.Module
     discriminator: nn.Module
     collection_name: str|None = None
-    loss_reduction_fn: Callable|None = jnp.mean
     output_key: str = "output"
+    loss_reduction_fn: Callable|None = jnp.mean
 
-    def __call__(self, inputs, ref_inputs, *args, **kwargs):
-
-        inputs_obj = Inputs.from_value(inputs)
+    def __call__(self, inputs, ref_inputs=None, *args, **kwargs):
+        reduction_fn = self.loss_reduction_fn or (lambda x: x)
 
-        main_out = self.main_module(*inputs_obj.args, *args, **inputs_obj.kwargs, **kwargs)
+        main_out = Inputs.apply(self.main_module, *args, **kwargs)(inputs)
 
         if self.collection_name is None:
             collections = main_out
         else:  
             collections = self.main_module.variables[self.collection_name]
 
         collections = gradient_reversal(collections)
 
         discriminator = Inputs.apply(self.discriminator)
-        dsc_main = discriminator(collections)
-        dsc_ref = discriminator(ref_inputs)
-
-        reduction_fn = self.loss_reduction_fn or (lambda x: x)
         dsc_loss_main = jax.tree_util.tree_map(
             lambda x: reduction_fn(
                 optax.sigmoid_binary_cross_entropy(x, jnp.ones_like(x))
             ),
-            dsc_main,
-        )
-        dsc_loss_ref = jax.tree_util.tree_map(
-            lambda x: reduction_fn(
-                optax.sigmoid_binary_cross_entropy(x, jnp.zeros_like(x))
-            ),
-            dsc_ref,
+            discriminator(collections),
         )
 
+        if ref_inputs is not None:
+            dsc_loss_ref = jax.tree_util.tree_map(
+                lambda x: reduction_fn(
+                    optax.sigmoid_binary_cross_entropy(x, jnp.zeros_like(x))
+                ),
+                discriminator(ref_inputs),
+            )
+        else:
+            dsc_loss_ref = None
+
         output = dict(
             dsc_loss_main = dsc_loss_main,
             dsc_loss_ref = dsc_loss_ref,
         )
         output[self.output_key] = main_out
 
         return output
```

### Comparing `xtrain-0.3.1/xtrain/loss.py` & `xtrain-0.3.2/xtrain/loss.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.1/xtrain/strategy.py` & `xtrain-0.3.2/xtrain/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,34 +6,27 @@
 import jax
 from flax.training.train_state import TrainState
 
 from . import base_trainer
 from .loss import LossLog
 from .utils import Inputs, unpack_prediction_and_state, unpack_x_y_sample_weight
 
-
 class Eager:
     @classmethod
     def loss_fn(cls, params, train_obj, batch):
         inputs, _, _ = unpack_x_y_sample_weight(batch)
 
         step = train_obj.train_state.step
         rngs = {
             name: jax.random.fold_in(rng, step) for name, rng in train_obj.rngs.items()
         }
-        inputs_obj = Inputs.from_value(inputs)
         variables = train_obj.variables
         variables["params"] = params
 
-        model_out = train_obj.train_state.apply_fn(
-            variables,
-            *inputs_obj.args,
-            **inputs_obj.kwargs,
-            rngs=rngs,
-        )
+        model_out = Inputs.apply(train_obj.train_state.apply_fn, variables, rngs=rngs)(inputs)
 
         prediction, _ = unpack_prediction_and_state(model_out, train_obj.has_aux)
 
         args = dict(
             batch=batch,
             prediction=prediction,
         )
@@ -50,40 +43,60 @@
         inputs_obj = Inputs.from_value(inputs)
 
         state = model.init(key, *inputs_obj.args, **inputs_obj.kwargs)
 
         return state
 
     @classmethod
-    def predict(cls, apply_fn, variables, inputs):  # only if model is immutable
+    def predict(cls, apply_fn, variables, inputs):
         # print("JIT Predict")
         inputs_obj = Inputs.from_value(inputs)
         preds = apply_fn(variables, *inputs_obj.args, **inputs_obj.kwargs)
         return preds
 
     @classmethod
     def train_step(
         cls,
         train_obj: base_trainer.TrainIterator,
         batch: tp.Any,
     ) -> tuple[TrainState, tuple[LossLog], tp.Any]:
-        # print('JIT train_step')
+        try:
+            axis_index = jax.lax.axis_index("mapped")
+            train_obj = train_obj.replace(
+                rngs={
+                    name: jax.random.fold_in(key, axis_index)
+                    for name, key in train_obj.rngs.items()
+                }
+            )
+        except NameError:
+            axis_index = -1
+
         grads, (loss_logs, preds) = jax.grad(cls.loss_fn, has_aux=True)(
             train_obj.train_state.params,
             train_obj,
             batch,
         )
 
+        try:
+            grads = jax.lax.pmean(grads, axis_name="mapped")
+            # aggregate logs
+            loss_logs = jax.tree_map(partial(jax.lax.pmean, axis_name="mapped"), loss_logs)
+        except NameError:
+            pass
+        
         grads = jax.tree_util.tree_map(
             lambda x, freeze: jax.numpy.zeros_like(x) if freeze else x,
             grads, train_obj.frozen,
         )
-
+        
         state = train_obj.train_state.apply_gradients(grads=grads)
 
+        #         # sync batch statistics
+        #         model.map(partial(jax.lax.pmean, axis_name="mapped"), tx.BatchStat, inplace=True)
+
         return state, loss_logs, preds
 
 
 class Core(Eager):
     predict = jax.jit(Eager.predict, static_argnames="apply_fn")
 
     @classmethod
@@ -97,60 +110,22 @@
 
 class JIT(Core):
     train_step = jax.jit(Core.train_step)
 
 
 class _Distributed(Eager):
     @classmethod
-    def _train_step(
-        cls,
-        train_obj: base_trainer.TrainIterator,
-        batch: tp.Any,
-    ) -> tuple[TrainState, tp.Sequence[LossLog], tp.Any]:
-        # print("JITTTTING")
-        axis_index = jax.lax.axis_index("mapped")
-        train_obj = train_obj.replace(
-            rngs={
-                name: jax.random.fold_in(key, axis_index)
-                for name, key in train_obj.rngs.items()
-            }
-        )
-
-        grads, (loss_logs, preds) = jax.grad(cls.loss_fn, has_aux=True)(
-            train_obj.train_state.params,
-            train_obj,
-            batch,
-        )
-
-        grads = jax.lax.pmean(grads, axis_name="mapped")
-        
-        grads = jax.tree_util.tree_map(
-            lambda x, freeze: jax.numpy.zeros_like(x) if freeze else x,
-            grads, train_obj.frozen,
-        )
-        
-        state = train_obj.train_state.apply_gradients(grads=grads)
-
-        # aggregate logs
-        loss_logs = jax.tree_map(partial(jax.lax.pmean, axis_name="mapped"), loss_logs)
-
-        #         # sync batch statistics
-        #         model.map(partial(jax.lax.pmean, axis_name="mapped"), tx.BatchStat, inplace=True)
-
-        return state, loss_logs, preds
-
-    @classmethod
     def init_fn(cls, key, model, inputs):
         inputs = jax.tree_map(lambda v: v[0], inputs)
         return Eager.init_fn(key, model, inputs)
 
 
 class Distributed(_Distributed):
     train_step = jax.pmap(
-        _Distributed._train_step,
+        Eager.train_step,
         axis_name="mapped",
         in_axes=(None, 0),
         out_axes=(None, None, 0),
     )
 
     predict = jax.pmap(
         Eager.predict,
@@ -159,15 +134,15 @@
         static_broadcasted_argnums=0,
     )
 
 
 class VMapped(_Distributed):
     train_step = jax.jit(
         jax.vmap(
-            _Distributed._train_step,
+            Eager.train_step,
             axis_name="mapped",
             in_axes=(None, 0),
             out_axes=(None, None, 0),
         ),
     )
 
     predict = jax.jit(
```

### Comparing `xtrain-0.3.1/xtrain/utils.py` & `xtrain-0.3.2/xtrain/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import functools
 import dataclasses
 import re
+import multiprocessing
+import queue
 from collections import deque
 from typing import Any, Dict, Iterable, Optional, Set, Tuple
 
 import jax
 from flax import struct
 
 InputLike = Any
@@ -114,14 +116,70 @@
             return pred, {}
     if isinstance(pred, tuple):
         return pred[0], pred[1]
     else:
         return pred[0], {}
 
 
+class Peekable:
+    def __init__(self, iterator):
+        self.iterator = iterator
+        self.peeked = deque()
+
+    def __iter__(self):
+        return self.iterator
+
+    def __next__(self):
+        if self.peeked:
+            return self.peeked.popleft()
+        return next(self.iterator)
+
+    def peek(self, ahead=0):
+        while len(self.peeked) <= ahead:
+            self.peeked.append(next(self.iterator))
+        return self.peeked[ahead]
+
+
+class PrefetchIterator:
+    def __init__(self, iterator, buffer_size=1):
+        self.iterator = iterator
+        self.buffer_size = buffer_size
+        self.buffer = multiprocessing.Queue(maxsize=buffer_size)
+        self.process = multiprocessing.Process(target=self._prefetch)
+        self.process.daemon = True
+        self.process.start()
+    
+    def _prefetch(self):
+        try:
+            for item in self.iterator:
+                self.buffer.put(item)
+        except Exception as e:
+            self.buffer.put(e)  # Put exception into the buffer
+        finally:
+            self.buffer.put(StopIteration())  # Indicate end of iteration or exception
+    
+    def __iter__(self):
+        return self
+    
+    def __next__(self):
+        item = self.buffer.get()
+
+        # Raise exception if encountered in subprocess
+        if isinstance(item, Exception):
+            # only wait for termination if the exception is StopIteration
+            self.close(joining = isinstance(item, StopIteration))
+            raise item  
+        return item
+    
+    def close(self, joining=False):
+        self.process.terminate()
+        if joining:
+            self.process.join()
+
+
 class Inputs(struct.PyTreeNode):
     args: Tuple[Any, ...] = ()
     kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
     def update(self, *args, **kwargs):
         tmp = self.kwargs.copy()
         tmp.update(kwargs)
@@ -210,19 +268,23 @@
             return isinstance(data, Dataset)
 
 except ImportError:
     TFDatasetAdapter = None
 
 
 class GeneratorAdapter:
-    def __init__(self, g):
+    def __init__(self, g, *, prefetch=0):
         self._generator = g
+        self._prefetch = prefetch
 
     def __iter__(self):
-        return self._generator()
+        if self._prefetch <= 0:
+            return self._generator()
+        else:
+            return PrefetchIterator(self._generator(), buffer_size=self._prefetch)
 
     @classmethod
     def is_adaptor_for(cls, data):
         # treat any callable as potentially a generator func
         return callable(data)
 
 def wrap_data_stream(ds):
@@ -234,25 +296,7 @@
 
     try:
         iter(ds)
     except:
         raise ValueError(f"Unrecognized datasource {ds}")
 
     return ds
-
-class Peekable:
-    def __init__(self, iterator):
-        self.iterator = iterator
-        self.peeked = deque()
-
-    def __iter__(self):
-        return self.iterator
-
-    def __next__(self):
-        if self.peeked:
-            return self.peeked.popleft()
-        return next(self.iterator)
-
-    def peek(self, ahead=0):
-        while len(self.peeked) <= ahead:
-            self.peeked.append(next(self.iterator))
-        return self.peeked[ahead]
```

### Comparing `xtrain-0.3.1/PKG-INFO` & `xtrain-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -39,17 +39,15 @@
     loss = ....
     return loss
 ```
 
 #### Step 3: create an iterator that supplies training data
 
 ```
-my_data = itertools.cycle(
-    zip(sequence_of_inputs, sequence_of_labels)
-)
+my_data = zip(sequence_of_inputs, sequence_of_labels)
 ```
 
 #### Step 4: train
 
 ```
 # create and initialize a Trainer object
 trainer = xtrain.Trainer(
@@ -57,19 +55,48 @@
   losses = my_loss_func,
   optimizer = optax.adam(1e-4),
 )
 
 train_iter = trainer.train(my_data) # returns a iterable object
 
 # iterate the train_iter trains the model
-for step in range(train_steps):
-    model_out = next(train_iter)
-    if step // 1000 == 0:
-        print(train_iter.loss_logs)
-        train_iter.reset_loss_logs()
+for epoch in range(3):
+  for model_out in train_iter:
+    pass
+  print(train_iter.loss_logs)
+  train_iter.reset_loss_logs()
+```
+
+### Training data format
+
+- tensowflow Dataset
+- torch dataloader
+- generator function
+- other python iterable that produce numpy data
+
+### Checkpointing
+
+train_iter is orbax compatible.
+
+```
+import orbax.checkpoint as ocp
+ocp.StandardCheckpointer().save(cp_path, args=ocp.args.StandardSave(train_iter))
+```
+
+### Freeze submodule
+```
+train_iter.freeze("submodule/Dense_0/kernel")
+```
+
+### Simple batch parallelism on multiple device
+```
+# Add a new batch dim to you dataset
+ds = ds.batch(8)
+# create trainer with the Distributed strategy
+trainer_iter = xtrain.Trainer(model, losses, optimizer, strategy=xtrain.Distributed).train(ds)
 ```
 
-### Full documentation
+### API documentation
 
 https://jiyuuchc.github.io/xtrain/
```

