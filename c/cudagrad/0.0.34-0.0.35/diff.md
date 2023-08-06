# Comparing `tmp/cudagrad-0.0.34.tar.gz` & `tmp/cudagrad-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.34.tar", last modified: Mon Jul 31 02:04:30 2023, max compression
+gzip compressed data, was "cudagrad-0.0.35.tar", last modified: Sun Aug  6 15:12:42 2023, max compression
```

## Comparing `cudagrad-0.0.34.tar` & `cudagrad-0.0.35.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.017207 cudagrad-0.0.34/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-29 19:31:23.000000 cudagrad-0.0.34/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3662 2023-07-31 02:04:30.017089 cudagrad-0.0.34/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3159 2023-07-29 20:12:25.000000 cudagrad-0.0.34/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.014887 cudagrad-0.0.34/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)      131 2023-07-31 02:04:13.000000 cudagrad-0.0.34/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5852 2023-07-31 02:00:43.000000 cudagrad-0.0.34/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.015724 cudagrad-0.0.34/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3662 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.34/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-31 02:04:13.000000 cudagrad-0.0.34/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-31 02:04:30.017250 cudagrad-0.0.34/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.34/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.016532 cudagrad-0.0.34/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.34/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.34/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.34/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.016807 cudagrad-0.0.34/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.34/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.031106 cudagrad-0.0.35/
+-rw-r--r--   0 ryan       (501) staff       (20)     1112 2023-08-02 22:59:21.000000 cudagrad-0.0.35/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)       42 2023-08-06 01:04:30.000000 cudagrad-0.0.35/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3692 2023-08-06 15:12:42.030980 cudagrad-0.0.35/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3167 2023-08-05 23:00:08.000000 cudagrad-0.0.35/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.028390 cudagrad-0.0.35/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      120 2023-08-06 06:30:25.000000 cudagrad-0.0.35/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5678 2023-08-06 06:30:27.000000 cudagrad-0.0.35/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.029345 cudagrad-0.0.35/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3692 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      337 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.35/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-08-06 15:12:41.000000 cudagrad-0.0.35/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      984 2023-08-06 06:32:56.000000 cudagrad-0.0.35/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-08-06 15:12:42.031147 cudagrad-0.0.35/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1648 2023-08-06 06:30:00.000000 cudagrad-0.0.35/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.030147 cudagrad-0.0.35/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2888 2023-08-06 06:29:45.000000 cudagrad-0.0.35/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.35/src/ops.cu
+-rw-r--r--   0 ryan       (501) staff       (20)    20914 2023-08-05 23:40:01.000000 cudagrad-0.0.35/src/tensor.hpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-08-06 15:12:42.030630 cudagrad-0.0.35/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-08-05 19:26:40.000000 cudagrad-0.0.35/tests/test.py
```

### Comparing `cudagrad-0.0.34/PKG-INFO` & `cudagrad-0.0.35/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.34
+Version: 0.0.35
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
 # cudagrad
 
 A small autograd engine
 
 Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
-#include "cudagrad.hpp"
+#include "tensor.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
@@ -40,15 +41,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; python ./examples/example.py
+# python -m pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.34/README.md` & `cudagrad-0.0.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
-#include "cudagrad.hpp"
+#include "tensor.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
@@ -25,15 +25,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; python ./examples/example.py
+# python -m pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.34/cudagrad/mlp.py` & `cudagrad-0.0.35/cudagrad/mlp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,188 +1,189 @@
 # type: ignore
+#
+# Copyright 2023 Ryan Moore
+#
+# So the magic is that there's this relatively simple algorithm called
+# backpropagation that takes the error in the output and sends that
+# error backwards through the network and computes through all the
+# connections how you should change them to improve the behavior, and
+# then you change them all a tiny bit and you just keep going with
+# another example. And surprisingly that actually works. For many years
+# people thought that would just get jammed up — it would get stuck
+# somewhere — but no it doesn't, it actually works very well.
+#
+# Geoffrey Hinton
+
 # %%
 import random
 from typing import *  # type: ignore
 
-from .cudagrad_bindings import *  # type: ignore
-
-# %matplotlib inline
+from .tensor import *  # type: ignore
 
+# wait, can cudagrad use python's global seed randomness?
+# probably hard/impossible to comunicate back to c++
+# horrible, good idea!
 random.seed(1337)
 
-from micrograd.engine import Value
-from micrograd.nn import MLP, Layer, Neuron
 
-# %%
-if __name__ == "__main__":
-    # %%
-    n = MLP(3, [1, 1])
-    m = MLP(3, [2, 1])
-    n, m
+class Module:
+    def zero_grad(self):
+        for p in self.parameters():
+            p.grad = 0
+
+    def parameters(self):
+        return []
+
+
+class Neuron(Module):
+    def __init__(self, nin, nonlin=True):
+        self.w = [tensor([1], [random.uniform(-1, 1)]) for _ in range(nin)]
+        self.b = tensor([1], [0])
+        self.nonlin = nonlin
+
+    def __call__(self, x):
+        ans = tensor([1], [0])
+        for elem_x in x:
+            for elem_w in self.w:
+                if type(elem_x) != Tensor:
+                    elem_x = tensor([1], [elem_x])
+                ans = ans + (elem_w * elem_x)
+        ans = ans + self.b
+        return ans
+        # act = sum((wi*xi for wi,xi in zip(self.w, x)), self.b)
+        # return act.relu() if self.nonlin else act
+
+    def parameters(self):
+        return self.w + [self.b]
+
+    def zero_grad(self):
+        for tensor in self.w + [self.b]:
+            tensor.zero_grad()
+
+    def train(self, rate: float):
+        for tensor in self.w + [self.b]:
+            assert tensor.size == [1]
+            # FIXME this is a must fix, I must be able to assign to data!
+            # >>> cg
+            # <module 'cudagrad' from '/Users/ryan/cudagrad/cudagrad/__init__.py'>
+            # >>> x = cg.tensor([1], [42])
+            # >>> x
+            # [42]
+            # [0]
+            # >>> x.data
+            # [42.0]
+            # >>> x.data = [1]
+            # Traceback (most recent call last):
+            # File "<stdin>", line 1, in <module>
+            # AttributeError: can't set attribute
+            # >>> x.data[0]
+            # 42.0
+            # >>> x.data[0] = 1
+            # >>> x
+            # [42]
+            # [0]
+            before = tensor.data[0]
+            update_value = tensor.data[0] + rate * tensor.grad[0]
+            tensor.data[0] = tensor.data[0] + rate * tensor.grad[0]
+            print(before, "->", tensor.data[0])
+            # print(tensor.data[0])
+            # print('after', tensor.data[0])
+
+    def __repr__(self):
+        return f"{'ReLU' if self.nonlin else 'Linear'}Neuron({len(self.w)})"
+
+
+class Layer(Module):
+    def __init__(self, nin, nout, **kwargs):
+        self.neurons = [Neuron(nin, **kwargs) for _ in range(nout)]
+
+    def __call__(self, x):
+        out = [n(x) for n in self.neurons]
+        return out[0] if len(out) == 1 else out
+
+    def parameters(self):
+        return [p for n in self.neurons for p in n.parameters()]
+
+    def zero_grad(self):
+        for neuron in self.neurons:
+            neuron.zero_grad()
+
+    def train(self, rate: float):
+        for neuron in self.neurons:
+            neuron.train(rate)
+
+    def __repr__(self):
+        return f"Layer of [{', '.join(str(n) for n in self.neurons)}]"
+
+
+class MLP(Module):
+    def __init__(self, nin, nouts):
+        sz = [nin] + nouts
+        self.layers = [
+            Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
+            for i in range(len(nouts))
+        ]
+
+    def __call__(self, x):
+        for layer in self.layers:
+            x = layer(x)
+        return x
+
+    def parameters(self):
+        return [p for layer in self.layers for p in layer.parameters()]
+
+    def zero_grad(self):
+        for layer in self.layers:
+            layer.zero_grad()
+
+    def train(self, rate: float):
+        for layer in self.layers:
+            layer.train(rate)
 
-    # %%
-    class _:  # MLP
-        from typing import List
+    def __repr__(self):
+        return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
 
-        def __init__(self, nin: int, nouts: List[int]):
-            sz = [nin] + nouts
-            self.layers = [
-                Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
-                for i in range(len(nouts))
-            ]
-
-    # MLP CONSTRUCTOR
-    # this is straightforward right, we make layers of
-    # cin, cout combos but we only make #cout of them
-    # each layers takes nin starting with nin, but then
-    # all other layers take the nouts[i] of the previous
-
-    # LINEAR OUTPUT
-    # the last layers is linear so we can predict any number not just [0,int)
-
-    # RELU LAYERS
-    # ReLU (Rectified Linear Unit) introduces non-linearity into neural networks
-    # due to its non-linear nature. The ReLU function is defined as:
-    #
-    # f(x) = max(0, x)
-    #
-    # without relus (or any non linear activation) nn's would be linear funtions
-
-    #  By definition, the ReLU is 𝑚𝑎𝑥(0,𝑥). Therefore, if we split the domain from
-    # (−∞,0] or [0,∞), then the function is linear. However, it's easy to see
-    # that 𝑓(−1)+𝑓(1)≠𝑓(0). Hence, by definition, ReLU is not linear.
-    # https://datascience.stackexchange.com/a/26481
-    # %%
-    def internals(n: MLP) -> None:
-        for layer in n.layers:
-            print(layer, "---")
-            for neuron in layer.neurons:
-                print(neuron, "*")
-                for value in neuron.parameters():  # .w and [.b]
-                    print(value, ".")
 
-    # %%
-
-    internals(n)
-    # MLP Diagram:
-    #
-    #   Input (3 features)
-    #       ↓
-    # Layer 1 (ReLUNeuron) # w: [0.2, 0.1, 0.3], b: 0.0
-    #       ↓
-    # Layer 2 (LinearNeuron) # w: [0.2], b: 0.0
-    #       ↓
-    #  Output (1 output)
+if __name__ == "__main__":
+    #%%
+    print(Neuron(2)([0.5, 0.2]).data)
+    print(Neuron(2)([tensor([1], [0.5]), tensor([1], [0.2])]).data)
+    l = Layer(3, 2)
 
-    # %%
-    internals(m)
-    # here's why this makes sense
-    # you take three inputs, every neuron needs 3 weights plus a bias
-    # but the number outputs of the first layer is two
-    # so you need two neurons in the first layer
-    # the linear layer gives two inputs and thus has two weights
+    # Layer(1, 2)
+    # MLP(2, [2, 1])
     # %%
 
+    # TODO make commented out part work make it a test
+
     xs = [[2.0, 3.0, -1.0], [3.0, -1.0, 0.5], [0.5, 1.0, 1.0], [1.0, 1.0, -1.0]]
     ys = [1.0, -1.0, -1.0, 1.0]
     # %%
 
+    # TODO make Mean Squared Error loss function some python function
+    #      redoing this is annoying how does pytorch store loss functions?
+
     nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
     for _ in range(50):
-        ypred = [nn(x) for x in xs]
-        loss = sum((a - b) ** 2 for a, b in zip(ypred, ys))
-        for p in nn.parameters():
-            p.grad = 0.0
-        loss.backward()
-        for p in nn.parameters():
-            p.data += -0.05 * p.grad
-        print(_ + 1, loss.data, [f"{x.data:1.2f}" for x in ypred])
-    # %%
-
-    import random
-
-    # import cudagrad
-    # from cudagrad import Tensor, tensor
-
-    class Module:
-        def zero_grad(self):
-            for p in self.parameters():
-                p.grad = 0
-
-        def parameters(self):
-            return []
-
-    class Neuron(Module):
-        def __init__(self, nin, nonlin=True):
-            self.w = [tensor([1], [random.uniform(-1, 1)]) for _ in range(nin)]
-            self.b = tensor([1], [0])
-            self.nonlin = nonlin
-
-        def __call__(self, x):
-            ans = tensor([1], [0])
-            for elem_x in x:
-                for elem_w in self.w:
-                    if type(elem_x) != Tensor:
-                        elem_x = tensor([1], [elem_x])
-                    ans = ans + (elem_w * elem_x)
-            ans = ans + self.b
-            return ans
-            # act = sum((wi*xi for wi,xi in zip(self.w, x)), self.b)
-            # return act.relu() if self.nonlin else act
 
-        def parameters(self):
-            return self.w + [self.b]
+        ypred = [nn(x) for x in xs]
+        # print(ypred, ys)
+        # print(list(zip(ypred, ys)))
 
-        def __repr__(self):
-            return f"{'ReLU' if self.nonlin else 'Linear'}Neuron({len(self.w)})"
+        # TODO ** POW would be nice here
+        # TODO no idea why sum() doesnt work
+        tensor_ys = [tensor([1], [float(y)]) for y in ys]
+        loss = tensor([1], [0.0])
+        for x in [(a - b) * (a - b) for a, b in zip(ypred, tensor_ys)]:
+            loss = loss + x
+        # loss = sum((a - b) * (a - b) for a, b in zip(ypred, tensor_ys))
+
+        nn.zero_grad()
+        # for p in nn.parameters():
+        #     p.grad = 0.0
 
-    # %%
-    print(Neuron(2)([0.5, 0.2]).data)
-    print(Neuron(2)([tensor([1], [0.5]), tensor([1], [0.2])]).data)
-    # Layer(1, 2)
-    # MLP(2, [2, 1])
+        loss.backward()
+        nn.train(-0.05)
+        # for p in nn.parameters():
+        #     p.data += -0.05 * p.grad
 
-    # # %%
-    # class Layer(Module):
-    #     def __init__(self, nin, nout, **kwargs):
-    #         self.neurons = [Neuron(nin, **kwargs) for _ in range(nout)]
-
-    #     def __call__(self, x):
-    #         out = [n(x) for n in self.neurons]
-    #         return out[0] if len(out) == 1 else out
-
-    #     def parameters(self):
-    #         return [p for n in self.neurons for p in n.parameters()]
-
-    #     def __repr__(self):
-    #         return f"Layer of [{', '.join(str(n) for n in self.neurons)}]"
-
-    # class MLP(Module):
-    #     def __init__(self, nin, nouts):
-    #         sz = [nin] + nouts
-    #         self.layers = [
-    #             Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
-    #             for i in range(len(nouts))
-    #         ]
-
-    #     def __call__(self, x):
-    #         for layer in self.layers:
-    #             x = layer(x)
-    #         return x
-
-    #     def parameters(self):
-    #         return [p for layer in self.layers for p in layer.parameters()]
-
-    #     def __repr__(self):
-    #         return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
-
-    # # %%
-    # # nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
-    # # for _ in range(50):
-    # #     ypred = [nn(x) for x in xs]
-    # #     loss = sum((a - b) ** 2 for a, b in zip(ypred, ys))
-    # #     for p in nn.parameters():
-    # #         p.grad = 0.0
-    # #     loss.backward()
-    # #     for p in nn.parameters():
-    # #         p.data += -0.05 * p.grad
-    # #     print(_ + 1, loss.data, [f"{x.data:1.2f}" for x in ypred])
+        # print(_ + 1, loss.data[0], [f"{y.data[0]:1.2f}" for y in ypred])
```

### Comparing `cudagrad-0.0.34/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.35/cudagrad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.34
+Version: 0.0.35
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
 # cudagrad
 
 A small autograd engine
 
 Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
-#include "cudagrad.hpp"
+#include "tensor.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
@@ -40,15 +41,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; python ./examples/example.py
+# python -m pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.34/pyproject.toml` & `cudagrad-0.0.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.34"
+version = "0.0.35"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 # TEMP while we implement mlp
 dependencies = [ "micrograd",]
 [[project.authors]]
```

### Comparing `cudagrad-0.0.34/setup.py` & `cudagrad-0.0.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/cudagrad/pull/53)
 
 ext_modules = [
     Pybind11Extension(
-        "cudagrad.cudagrad_bindings",
+        "cudagrad.tensor",
         ["src/bindings.cpp"],
         # Example: passing in the version to the compiled code
         define_macros=[("VERSION_INFO", __version__)],
     ),
 ]
 
 setup(
```

### Comparing `cudagrad-0.0.34/src/bindings.cpp` & `cudagrad-0.0.35/src/bindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 // Copyright 2023 Ryan Moore
 //
 // If the implementation is easy to explain, it may be a good idea.
 //
 // Tim Peters
 
 #include <sstream>
-#include "cudagrad.hpp"
+#include "tensor.hpp"
 
 #include <pybind11/stl.h>
 #include <pybind11/pybind11.h>
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 namespace py = pybind11;
 
-PYBIND11_MODULE(cudagrad_bindings, m) {
+PYBIND11_MODULE(tensor, m) {
     m.doc() = R"pbdoc(
         Pybind11 example plugin
         -----------------------
 
         .. currentmodule:: cudagrad
 
         .. autosummary::
@@ -47,14 +47,15 @@
     //              override str when no str present?
     py::class_<cg::Tensor, std::shared_ptr<cg::Tensor>>(m, "Tensor")
         .def(py::init<std::vector<int>, std::vector<float>>())
         .def("get_shared", &cg::Tensor::get_shared)
         .def("backward", &cg::Tensor::backward)
         .def("zero_grad", &cg::Tensor::zero_grad)
         .def("sum", &cg::Tensor::sum)
+        .def("relu", &cg::Tensor::relu)
         .def_property_readonly("size", &cg::Tensor::get_size)
         .def_property_readonly("data", &cg::Tensor::get_data)
         .def_property_readonly("grad", &cg::Tensor::get_grad)
         .def("graph", &cg::Tensor::graph)
         .def_static("ones", &cg::Tensor::ones)
         .def_static("zeros", &cg::Tensor::zeros)
         .def_static("explode", &cg::Tensor::explode)
@@ -66,17 +67,15 @@
         .def("__matmul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a.get()->matmul(b); })
         .def("__str__", [](std::shared_ptr<cg::Tensor> t) {
             std::ostringstream os;
             os << t;
             return os.str();
         })
         .def("__repr__", [](std::shared_ptr<cg::Tensor> t) {
-            std::ostringstream os;
-            os << t;
-            return os.str();
+            return t.get()->repr();
         });
 
 #ifdef VERSION_INFO
     m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
 #else
     m.attr("__version__") = "dev";
 #endif
```

### Comparing `cudagrad-0.0.34/src/cudagrad.hpp` & `cudagrad-0.0.35/src/tensor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 // pieces of advice. The first piece of advice is whenever you can, use vector.
 // The second piece of advice is if you cannot, find a way how you can. This is
 // to avoid any data structures except arrays... Vector is an array, right. Sort
 // of, you say, 'Well... Aren't there exceptions?' – Yes, not for you!
 //
 // Alexander Stepanov
 
-#ifndef SRC_CUDAGRAD_HPP_
-#define SRC_CUDAGRAD_HPP_
+#ifndef SRC_TENSOR_HPP_
+#define SRC_TENSOR_HPP_
 
 #include <algorithm>
 #include <cassert>
 #include <functional>
 #include <iostream>
 #include <memory>
 #include <numeric>
 #include <random>
+#include <sstream>
 #include <stdexcept>
 #include <string>
 #include <utility>
 #include <vector>
 
 namespace cg {
 
@@ -118,16 +119,35 @@
         strides_(std::move(other.strides_)) {}
 
   std::shared_ptr<Tensor> get_shared() { return this->shared_from_this(); }
 
   void backward();
   void zero_grad();
   std::shared_ptr<Tensor> sum();
+  std::shared_ptr<Tensor> relu();
   std::shared_ptr<Tensor> matmul(std::shared_ptr<Tensor> other);
 
+  std::string repr() {
+    std::ostringstream oss_s;
+    for (const auto& s : size_) {
+      oss_s << s << ", ";
+    }
+    std::string s_str = oss_s.str();
+    s_str = s_str.substr(0, s_str.length() - 2);
+
+    std::ostringstream oss_d;
+    for (const auto& d : data_) {
+      oss_d << d << ", ";
+    }
+    std::string d_str = oss_d.str();
+    d_str = d_str.substr(0, d_str.length() - 2);
+
+    return std::string("tensor([") + s_str + std::string("], [") + d_str + std::string("])");
+  }
+
   void size() {
     for (auto x : size_) std::cout << x << std::endl;
   }
   void data() {
     for (auto x : data_) std::cout << x << std::endl;
   }
   void grad() {
@@ -341,22 +361,22 @@
   }
   return std::make_shared<Tensor>(
       std::vector<int>{1}, std::vector<float>{total},
       std::vector<std::shared_ptr<Tensor>>{get_shared()},
       std::make_shared<SumBackward>(), 's');
 }
 
-std::shared_ptr<Tensor> relu(std::shared_ptr<Tensor> input) {
-  std::vector<float> result_data(input.get()->data_.size());
-  for (int i = 0; i < input.get()->data_.size(); ++i) {
-    result_data[i] = std::max(0.0f, input.get()->data_[i]);
+std::shared_ptr<Tensor> Tensor::relu() {
+  std::vector<float> result_data(data_.size());
+  for (int i = 0; i < data_.size(); ++i) {
+    result_data[i] = std::max(0.0f, data_[i]);
   }
   return std::make_shared<Tensor>(
-      input.get()->size_, result_data,
-      std::vector<std::shared_ptr<Tensor>>{input.get()->get_shared()},
+      size_, result_data,
+      std::vector<std::shared_ptr<Tensor>>{get_shared()},
       std::make_shared<ReluBackward>(), 'r');
 }
 
 std::shared_ptr<Tensor> tensor(std::initializer_list<int> size,
                                std::initializer_list<float> data) {
   return std::make_shared<Tensor>(size, data);
 }
@@ -630,15 +650,15 @@
       if (ans == nullptr) {
         ans = (weights_[i] * inputs[i]);
       } else {
         ans = ans + (weights_[i] * inputs[i]);
       }
     }
     ans = ans + bias_;
-    return relu(ans);
+    return ans.get()->relu();
   }
 
   void train() {
     for (int i = 0; i < weights_.size(); ++i) {
       // std::cout << "weight before: " << weights_[i].get()->data_[0] <<
       // std::endl;
       weights_[i].get()->data_[0] = weights_[i].get()->data_[0] +
@@ -654,8 +674,8 @@
   // TODO(yrom1) parameters, how do i make this like std iterator?
 };
 
 }  // namespace nn
 
 }  // namespace cg
 
-#endif  // SRC_CUDAGRAD_HPP_
+#endif  // SRC_TENSOR_HPP_
```

### Comparing `cudagrad-0.0.34/tests/test.py` & `cudagrad-0.0.35/tests/test.py`

 * *Files identical despite different names*

