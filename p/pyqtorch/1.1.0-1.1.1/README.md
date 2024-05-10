# Comparing `tmp/pyqtorch-1.1.0.tar.gz` & `tmp/pyqtorch-1.1.1.tar.gz`

## Comparing `pyqtorch-1.1.0.tar` & `pyqtorch-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/README.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/mkdocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/setup.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/docs/index.md
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/__init__.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/adjoint.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/analog.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/apply.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/circuit.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/matrices.py
--rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/parametric.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/primitive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/py.typed
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyqtorch/utils.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/tests/test_analog.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/tests/test_circuit.py
--rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/tests/test_digital.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/LICENSE
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pyqtorch-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/README.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/mkdocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/setup.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/index.md
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/adjoint.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/analog.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/apply.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/circuit.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     8620 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/parametric.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/primitive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/py.typed
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_analog.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_circuit.py
+-rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_digital.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/PKG-INFO
```

### Comparing `pyqtorch-1.1.0/.pre-commit-config.yaml` & `pyqtorch-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/README.md` & `pyqtorch-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/mkdocs.yml` & `pyqtorch-1.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-1.1.1/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/docs/CODE_OF_CONDUCT.md` & `pyqtorch-1.1.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/docs/CONTRIBUTING.md` & `pyqtorch-1.1.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/docs/index.md` & `pyqtorch-1.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/pyqtorch/__init__.py` & `pyqtorch-1.1.1/pyqtorch/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # # See the License for the specific language governing permissions and
 # # limitations under the License.
 from __future__ import annotations
 
 from .analog import HamiltonianEvolution
 from .apply import apply_operator
-from .circuit import QuantumCircuit, expectation
+from .circuit import Add, Merge, QuantumCircuit, Scale, Sequence, expectation
 from .parametric import CPHASE, CRX, CRY, CRZ, PHASE, RX, RY, RZ, U
 from .primitive import (
     CNOT,
     CSWAP,
     CY,
     CZ,
     SWAP,
```

### Comparing `pyqtorch-1.1.0/pyqtorch/adjoint.py` & `pyqtorch-1.1.1/pyqtorch/adjoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,23 +32,25 @@
         return inner_prod(ctx.out_state, ctx.projected_state).real
 
     @staticmethod
     @no_grad()
     def backward(ctx: Any, grad_out: Tensor) -> tuple:
         param_values = ctx.saved_tensors
         values = param_dict(ctx.param_names, param_values)
-        grads_dict = values.copy()
-        for op in ctx.circuit.reverse():
+        grads_dict = {k: None for k in values.keys()}
+        for op in ctx.circuit.operations[::-1]:
             ctx.out_state = apply_operator(ctx.out_state, op.dagger(values), op.qubit_support)
             if isinstance(op, Parametric):
                 if values[op.param_name].requires_grad:
                     mu = apply_operator(ctx.out_state, op.jacobian(values), op.qubit_support)
                     grad = grad_out * 2 * inner_prod(ctx.projected_state, mu).real
                 else:
                     grad = zeros(1)
-
-                grads_dict[op.param_name] = grad
+                if grads_dict[op.param_name] is not None:
+                    grads_dict[op.param_name] += grad
+                else:
+                    grads_dict[op.param_name] = grad
 
             ctx.projected_state = apply_operator(
                 ctx.projected_state, op.dagger(values), op.qubit_support
             )
         return (None, None, None, None, *grads_dict.values())
```

### Comparing `pyqtorch-1.1.0/pyqtorch/analog.py` & `pyqtorch-1.1.1/pyqtorch/analog.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/pyqtorch/apply.py` & `pyqtorch-1.1.1/pyqtorch/apply.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from string import ascii_letters as ABC
-from typing import Tuple
 
-from numpy import array
+import torch
+from numpy import array, log2
 from numpy.typing import NDArray
-from torch import einsum
+from torch import Tensor, einsum
 
-from pyqtorch.utils import Operator, State
+from pyqtorch.utils import batch_first, batch_last, promote_operator
 
 ABC_ARRAY: NDArray = array(list(ABC))
 
 
 def apply_operator(
-    state: State,
-    operator: Operator,
-    qubits: Tuple[int, ...] | list[int],
+    state: Tensor,
+    operator: Tensor,
+    qubits: tuple[int, ...] | list[int],
     n_qubits: int = None,
     batch_size: int = None,
-) -> State:
+) -> Tensor:
     """Applies an operator, i.e. a single tensor of shape [2, 2, ...], on a given state
        of shape [2 for _ in range(n_qubits)] for a given set of (target and control) qubits.
 
        Since dimension 'i' in 'state' corresponds to all amplitudes where qubit 'i' is 1,
        target and control qubits represent the dimensions over which to contract the 'operator'.
        Contraction means applying the 'dot' operation between the operator array and dimension 'i'
        of 'state, resulting in a new state where the result of the 'dot' operation has been moved to
@@ -53,7 +53,36 @@
     operator_dims[-1] = in_state_dims[-1]
     out_state_dims = in_state_dims.copy()
     out_state_dims[qubits] = operator_dims[0:n_support]
     operator_dims, in_state_dims, out_state_dims = list(
         map(lambda e: "".join(list(e)), [operator_dims, in_state_dims, out_state_dims])
     )
     return einsum(f"{operator_dims},{in_state_dims}->{out_state_dims}", operator, state)
+
+
+def operator_product(op1: Tensor, op2: Tensor, target: int) -> Tensor:
+    """
+    Compute the product of two operators.
+
+    Args:
+        op1 (Tensor): The first operator.
+        op2 (Tensor): The second operator.
+        target (int): The target qubit index.
+
+    Returns:
+        Tensor: The product of the two operators.
+    """
+
+    n_qubits_1 = int(log2(op1.size(1)))
+    n_qubits_2 = int(log2(op2.size(1)))
+    batch_size_1 = op1.size(-1)
+    batch_size_2 = op2.size(-1)
+    if n_qubits_1 > n_qubits_2:
+        op2 = promote_operator(op2, target, n_qubits_1)
+    elif n_qubits_1 < n_qubits_2:
+        op1 = promote_operator(op1, target, n_qubits_2)
+    if batch_size_1 > batch_size_2:
+        op2 = op2.repeat(1, 1, batch_size_1)[:, :, :batch_size_1]
+    elif batch_size_2 > batch_size_1:
+        op1 = op1.repeat(1, 1, batch_size_2)[:, :, :batch_size_2]
+
+    return batch_last(torch.bmm(batch_first(op1), batch_first(op2)))
```

### Comparing `pyqtorch-1.1.0/pyqtorch/matrices.py` & `pyqtorch-1.1.1/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/pyqtorch/parametric.py` & `pyqtorch-1.1.1/pyqtorch/parametric.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
             return Parametric._expand_values(values[self.param_name])
 
         def parse_tensor(values: dict[str, torch.Tensor] | torch.Tensor = {}) -> torch.Tensor:
             return Parametric._expand_values(values)
 
         self.parse_values = parse_tensor if param_name == "" else parse_values
 
+    def __hash__(self) -> int:
+        return hash(self.qubit_support) + hash(self.param_name)
+
     @staticmethod
     def _expand_values(values: torch.Tensor) -> torch.Tensor:
         return values.unsqueeze(0) if len(values.size()) == 0 else values
 
     def unitary(self, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> Operator:
         thetas = self.parse_values(values)
         batch_size = len(thetas)
```

### Comparing `pyqtorch-1.1.0/pyqtorch/primitive.py` & `pyqtorch-1.1.1/pyqtorch/primitive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 from math import log2
-from typing import Any, Tuple
+from typing import Any
 
 import torch
+from torch import Tensor
 
 from pyqtorch.apply import apply_operator
 from pyqtorch.matrices import OPERATIONS_DICT, _controlled, _dagger
-from pyqtorch.utils import Operator, State, product_state
+from pyqtorch.utils import product_state
 
 
 class Primitive(torch.nn.Module):
-    def __init__(self, pauli: torch.Tensor, target: int) -> None:
+    def __init__(self, pauli: Tensor, target: int) -> None:
         super().__init__()
         self.target: int = target
-        self.qubit_support: Tuple[int, ...] = (target,)
+        self.qubit_support: tuple[int, ...] = (target,)
         self.n_qubits: int = max(self.qubit_support)
         self.register_buffer("pauli", pauli)
         self._param_type = None
         self._device = self.pauli.device
         self._dtype = self.pauli.dtype
 
     def __key(self) -> tuple:
@@ -36,23 +37,23 @@
     def extra_repr(self) -> str:
         return f"qubit_support={self.qubit_support}"
 
     @property
     def param_type(self) -> None:
         return self._param_type
 
-    def unitary(self, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> Operator:
+    def unitary(self, values: dict[str, Tensor] | Tensor = dict()) -> Tensor:
         return self.pauli.unsqueeze(2)
 
-    def forward(self, state: State, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> State:
+    def forward(self, state: Tensor, values: dict[str, Tensor] | Tensor = dict()) -> Tensor:
         return apply_operator(
             state, self.unitary(values), self.qubit_support, len(state.size()) - 1
         )
 
-    def dagger(self, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> Operator:
+    def dagger(self, values: dict[str, Tensor] | Tensor = dict()) -> Tensor:
         return _dagger(self.unitary(values))
 
     @property
     def device(self) -> torch.device:
         return self._device
 
     @property
@@ -81,15 +82,15 @@
         super().__init__(OPERATIONS_DICT["Z"], target)
 
 
 class I(Primitive):  # noqa: E742
     def __init__(self, target: int):
         super().__init__(OPERATIONS_DICT["I"], target)
 
-    def forward(self, state: State, values: dict[str, torch.Tensor] = None) -> State:
+    def forward(self, state: Tensor, values: dict[str, Tensor] = None) -> Tensor:
         return state
 
 
 class H(Primitive):
     def __init__(self, target: int):
         super().__init__(OPERATIONS_DICT["H"], target)
 
@@ -131,50 +132,50 @@
         super().__init__(OPERATIONS_DICT["SWAP"], target)
         self.control = (control,) if isinstance(control, int) else control
         self.qubit_support = self.control + (target,)
         self.n_qubits = max(self.qubit_support)
 
 
 class CSWAP(Primitive):
-    def __init__(self, control: int | Tuple[int, ...], target: int):
+    def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__(OPERATIONS_DICT["CSWAP"], target)
         self.control = (control,) if isinstance(control, int) else control
         self.target = target
         self.qubit_support = self.control + (target,)
         self.n_qubits = max(self.qubit_support)
 
 
 class ControlledOperationGate(Primitive):
-    def __init__(self, gate: str, control: int | Tuple[int, ...], target: int):
+    def __init__(self, gate: str, control: int | tuple[int, ...], target: int):
         self.control = (control,) if isinstance(control, int) else control
         mat = OPERATIONS_DICT[gate]
         mat = _controlled(
             unitary=mat.unsqueeze(2),
             batch_size=1,
             n_control_qubits=len(self.control) - (int)(log2(mat.shape[0])) + 1,
         ).squeeze(2)
         super().__init__(mat, target)
         self.qubit_support = self.control + (target,)
         self.n_qubits = max(self.qubit_support)
 
 
 class CNOT(ControlledOperationGate):
-    def __init__(self, control: int | Tuple[int, ...], target: int):
+    def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__("X", control, target)
 
 
 CX = CNOT
 
 
 class CY(ControlledOperationGate):
-    def __init__(self, control: int | Tuple[int, ...], target: int):
+    def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__("Y", control, target)
 
 
 class CZ(ControlledOperationGate):
-    def __init__(self, control: int | Tuple[int, ...], target: int):
+    def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__("Z", control, target)
 
 
 class Toffoli(ControlledOperationGate):
-    def __init__(self, control: int | Tuple[int, ...], target: int):
+    def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__("X", control, target)
```

### Comparing `pyqtorch-1.1.0/tests/test_analog.py` & `pyqtorch-1.1.1/tests/test_analog.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/tests/test_digital.py` & `pyqtorch-1.1.1/tests/test_digital.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 import random
 from math import log2
 from typing import Callable, Tuple
 
 import pytest
 import torch
+from torch import Tensor
 
 import pyqtorch as pyq
-from pyqtorch.apply import apply_operator
-from pyqtorch.matrices import DEFAULT_MATRIX_DTYPE, IMAT, ZMAT
+from pyqtorch.apply import apply_operator, operator_product
+from pyqtorch.matrices import DEFAULT_MATRIX_DTYPE, IMAT, ZMAT, _dagger
 from pyqtorch.parametric import Parametric
-from pyqtorch.utils import ATOL, product_state
+from pyqtorch.primitive import Primitive
+from pyqtorch.utils import ATOL, density_mat, product_state, promote_operator, random_state
 
 state_000 = product_state("000")
 state_001 = product_state("001")
 state_100 = product_state("100")
 state_101 = product_state("101")
 state_110 = product_state("110")
 state_111 = product_state("111")
@@ -108,63 +110,63 @@
     )
     assert torch.allclose(
         pyq.Projector((0, 1, 2), ket="111", bra="111")(product_state("111")), t111
     )
 
 
 def test_CNOT_state00_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CNOT(0, 1)(product_state("00"), None)
+    result: Tensor = pyq.CNOT(0, 1)(product_state("00"), None)
     assert torch.equal(product_state("00"), result)
 
 
 def test_CNOT_state10_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CNOT(0, 1)(product_state("10"), None)
+    result: Tensor = pyq.CNOT(0, 1)(product_state("10"), None)
     assert torch.allclose(product_state("11"), result)
 
 
 def test_CNOT_state11_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CNOT(0, 1)(product_state("11"), None)
+    result: Tensor = pyq.CNOT(0, 1)(product_state("11"), None)
     assert torch.allclose(product_state("10"), result)
 
 
 def test_CRY_state10_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CRY(0, 1, "theta")(
+    result: Tensor = pyq.CRY(0, 1, "theta")(
         product_state("10"), {"theta": torch.tensor([torch.pi])}
     )
     assert torch.allclose(product_state("11"), result, atol=ATOL)
 
 
 def test_CRY_state01_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CRY(1, 0, "theta")(
+    result: Tensor = pyq.CRY(1, 0, "theta")(
         product_state("01"), {"theta": torch.tensor([torch.pi])}
     )
     assert torch.allclose(product_state("11"), result, atol=ATOL)
 
 
 def test_CSWAP_state101_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CSWAP((0, 1), 2)(product_state("101"), None)
+    result: Tensor = pyq.CSWAP((0, 1), 2)(product_state("101"), None)
     assert torch.allclose(product_state("110"), result)
 
 
 def test_CSWAP_state110_controlqubit_0() -> None:
-    result: torch.Tensor = pyq.CSWAP((0, 1), 2)(product_state("101"), None)
+    result: Tensor = pyq.CSWAP((0, 1), 2)(product_state("101"), None)
     assert torch.allclose(product_state("110"), result)
 
 
 @pytest.mark.parametrize(
     "initial_state,expected_state",
     [
         (state_000, state_000),
         (state_001, state_001),
         (state_100, state_100),
         (state_101, state_110),
         (state_110, state_101),
     ],
 )
-def test_CSWAP_controlqubits0(initial_state: torch.Tensor, expected_state: torch.Tensor) -> None:
+def test_CSWAP_controlqubits0(initial_state: Tensor, expected_state: Tensor) -> None:
     cswap = pyq.CSWAP((0, 1), 2)
     assert torch.allclose(cswap(initial_state, None), expected_state)
 
 
 @pytest.mark.parametrize(
     "initial_state,expected_state",
     [
@@ -172,15 +174,15 @@
         (state_001, state_001),
         (state_100, state_100),
         (state_101, state_101),
         (state_110, state_111),
         (state_1110, state_1111),
     ],
 )
-def test_Toffoli_controlqubits0(initial_state: torch.Tensor, expected_state: torch.Tensor) -> None:
+def test_Toffoli_controlqubits0(initial_state: Tensor, expected_state: Tensor) -> None:
     n_qubits = int(log2(torch.numel(initial_state)))
     qubits = tuple([i for i in range(n_qubits)])
     toffoli = pyq.Toffoli(qubits[:-1], qubits[-1])
     assert torch.allclose(toffoli(initial_state, None), expected_state)
 
 
 @pytest.mark.parametrize(
@@ -193,15 +195,15 @@
         (state_110, True),
         (state_1110, True),
     ],
 )
 @pytest.mark.parametrize("gate", ["RX", "RY", "RZ", "PHASE"])
 @pytest.mark.parametrize("batch_size", [1, 2])
 def test_multi_controlled_gates(
-    initial_state: torch.Tensor, expects_rotation: bool, batch_size: int, gate: str
+    initial_state: Tensor, expects_rotation: bool, batch_size: int, gate: str
 ) -> None:
     phi = "phi"
     rot_gate = getattr(pyq, gate)
     controlled_rot_gate = getattr(pyq, "C" + gate)
     phi = torch.rand(batch_size)
     n_qubits = int(log2(torch.numel(initial_state)))
     qubits = tuple([i for i in range(n_qubits)])
@@ -284,7 +286,59 @@
     params = ["phi", "theta", "omega"]
     u = pyq.U(target, *params)
     values = {param: torch.rand(1) for param in params}
     state = pyq.random_state(n_qubits)
     assert torch.allclose(
         u(state, values), pyq.QuantumCircuit(n_qubits, u.digital_decomposition())(state, values)
     )
+
+
+@pytest.mark.parametrize("n_qubits,batch_size", torch.randint(1, 6, (8, 2)))
+def test_dm(n_qubits: Tensor, batch_size: Tensor) -> None:
+    state = random_state(n_qubits)
+    projector = torch.outer(state.flatten(), state.conj().flatten()).view(
+        2**n_qubits, 2**n_qubits, 1
+    )
+    dm = density_mat(state)
+    assert dm.size() == torch.Size([2**n_qubits, 2**n_qubits, 1])
+    assert torch.allclose(dm, projector)
+    states = []
+    projectors = []
+    for batch in range(batch_size):
+        state = random_state(n_qubits)
+        states.append(state)
+        projector = torch.outer(state.flatten(), state.conj().flatten()).view(
+            2**n_qubits, 2**n_qubits, 1
+        )
+        projectors.append(projector)
+    dm_proj = torch.cat(projectors, dim=2)
+    state_cat = torch.cat(states, dim=n_qubits)
+    dm = density_mat(state_cat)
+    assert dm.size() == torch.Size([2**n_qubits, 2**n_qubits, batch_size])
+    assert torch.allclose(dm, dm_proj)
+
+
+def test_promote(gate: Primitive) -> None:
+    n_qubits = torch.randint(low=1, high=8, size=(1,)).item()
+    target = random.choice([i for i in range(n_qubits)])
+    op_prom = promote_operator(gate(target).unitary(), target, n_qubits)
+    assert op_prom.size() == torch.Size([2**n_qubits, 2**n_qubits, 1])
+    assert torch.allclose(
+        operator_product(op_prom, _dagger(op_prom), target),
+        torch.eye(2**n_qubits, dtype=torch.cdouble).unsqueeze(2),
+    )
+
+
+def test_operator_product(gate: Primitive) -> None:
+    n_qubits = torch.randint(low=1, high=8, size=(1,)).item()
+    target = random.choice([i for i in range(n_qubits)])
+    batch_size_1 = torch.randint(low=1, high=5, size=(1,)).item()
+    batch_size_2 = torch.randint(low=1, high=5, size=(1,)).item()
+    max_batch = max(batch_size_2, batch_size_1)
+    op_prom = promote_operator(gate(target).unitary(), target, n_qubits).repeat(1, 1, batch_size_1)
+    op_mul = operator_product(
+        gate(target).unitary().repeat(1, 1, batch_size_2), _dagger(op_prom), target
+    )
+    assert op_mul.size() == torch.Size([2**n_qubits, 2**n_qubits, max_batch])
+    assert torch.allclose(
+        op_mul, torch.eye(2**n_qubits, dtype=torch.cdouble).unsqueeze(2).repeat(1, 1, max_batch)
+    )
```

### Comparing `pyqtorch-1.1.0/.gitignore` & `pyqtorch-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/LICENSE` & `pyqtorch-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.0/pyproject.toml` & `pyqtorch-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
     { name = "Roland Guichard", email = "roland.guichard@pasqal.com" },
     { name = "Joao P. Moutinho", email = "joao.moutinho@pasqal.com"},
 ]
 requires-python = ">=3.8,<3.13"
 license = {text = "Apache 2.0"}
-version = "1.1.0"
+version = "1.1.1"
 classifiers=[
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-1.1.0/PKG-INFO` & `pyqtorch-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyqtorch
-Version: 1.1.0
+Version: 1.1.1
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

