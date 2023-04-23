# Comparing `tmp/high_order_layers_torch-1.3.3.tar.gz` & `tmp/high_order_layers_torch-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "high_order_layers_torch-1.3.3.tar", max compression
+gzip compressed data, was "high_order_layers_torch-1.3.4.tar", max compression
```

## Comparing `high_order_layers_torch-1.3.3.tar` & `high_order_layers_torch-1.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-1.3.3/LICENSE
--rw-r--r--   0        0        0    10636 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/README.md
--rw-r--r--   0        0        0    14898 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/Basis.py
--rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolution.py
--rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolutionTranspose.py
--rw-r--r--   0        0        0     3688 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/LagrangePolynomial.py
--rw-r--r--   0        0        0    22480 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.3/high_order_layers_torch/PolynomialLayers.py
--rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/ProductLayer.py
--rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-1.3.3/high_order_layers_torch/__init__.py
--rw-r--r--   0        0        0    22990 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/high_order_layers_torch/attentions.py
--rw-r--r--   0        0        0     8098 2023-04-22 03:25:58.265287 high_order_layers_torch-1.3.3/high_order_layers_torch/layers.py
--rw-r--r--   0        0        0     7239 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.3/high_order_layers_torch/modules.py
--rw-r--r--   0        0        0    33107 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.3/high_order_layers_torch/networks.py
--rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.3/high_order_layers_torch/positional_embeddings.py
--rw-r--r--   0        0        0     3282 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/high_order_layers_torch/utils.py
--rw-r--r--   0        0        0      731 2023-04-22 03:28:57.406819 high_order_layers_torch-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.3/setup.py
--rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-12-25 19:50:48.693271 high_order_layers_torch-1.3.4/LICENSE
+-rw-r--r--   0        0        0    10636 2023-04-23 14:16:04.430547 high_order_layers_torch-1.3.4/README.md
+-rw-r--r--   0        0        0    14898 2022-11-13 17:24:03.303398 high_order_layers_torch-1.3.4/high_order_layers_torch/Basis.py
+-rw-r--r--   0        0        0    17551 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/FunctionalConvolution.py
+-rw-r--r--   0        0        0     5189 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/FunctionalConvolutionTranspose.py
+-rw-r--r--   0        0        0     3688 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/LagrangePolynomial.py
+-rw-r--r--   0        0        0    23038 2023-04-23 15:26:21.447885 high_order_layers_torch-1.3.4/high_order_layers_torch/PolynomialLayers.py
+-rw-r--r--   0        0        0     1656 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/ProductLayer.py
+-rw-r--r--   0        0        0        0 2020-12-25 19:50:53.940493 high_order_layers_torch-1.3.4/high_order_layers_torch/__init__.py
+-rw-r--r--   0        0        0    22990 2023-04-23 14:16:04.430547 high_order_layers_torch-1.3.4/high_order_layers_torch/attentions.py
+-rw-r--r--   0        0        0     9207 2023-04-23 15:29:24.406308 high_order_layers_torch-1.3.4/high_order_layers_torch/layers.py
+-rw-r--r--   0        0        0     7239 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/modules.py
+-rw-r--r--   0        0        0    33357 2023-04-23 15:32:34.752889 high_order_layers_torch-1.3.4/high_order_layers_torch/networks.py
+-rw-r--r--   0        0        0     2488 2022-11-13 17:24:03.307398 high_order_layers_torch-1.3.4/high_order_layers_torch/positional_embeddings.py
+-rw-r--r--   0        0        0     3282 2023-04-23 14:16:04.430547 high_order_layers_torch-1.3.4/high_order_layers_torch/utils.py
+-rw-r--r--   0        0        0      731 2023-04-23 15:38:15.796514 high_order_layers_torch-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.4/setup.py
+-rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.4/PKG-INFO
```

### Comparing `high_order_layers_torch-1.3.3/LICENSE` & `high_order_layers_torch-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/README.md` & `high_order_layers_torch-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/Basis.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/Basis.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolution.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/FunctionalConvolution.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolutionTranspose.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/FunctionalConvolutionTranspose.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/LagrangePolynomial.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/LagrangePolynomial.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/PolynomialLayers.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/PolynomialLayers.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         x_min = self._eta(index)
         x_max = self._eta(index + 1)
 
         x_global = ((x_local + self._half) / self._length) * (x_max - x_min) + x_min
         return x_global
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-
         periodicity = self.periodicity
         if periodicity is not None:
             x = make_periodic(x, periodicity)
 
         # get the segment index
         id_min = (((x + self._half) / self._length) * self._segments).long()
         device = id_min.device
@@ -207,14 +206,26 @@
         """
         Arg:
             - index is the segment index
         """
         eta = index / float(self._segments)
         return eta * 2 - 1
 
+    def interpolate(
+        self,
+        layer_out: "Piecewise",
+    ) -> None:
+        interpolate_polynomial_layer(self, layer_out)
+
+    def refine(
+        self,
+        layer_out: "Piecewise",
+    ) -> None:
+        refine_polynomial_layer(layer_in=self, layer_out=layer_out)
+
 
 class PiecewisePolynomial(Piecewise):
     def __init__(
         self,
         n: int,
         in_features: int,
         out_features: int,
@@ -392,14 +403,20 @@
         x_global = ((x_local + self._half) / self._length) * (x_max - x_min) + x_min
         return x_global
 
     def _eta(self, index: int):
         eta = index / float(self._segments)
         return eta * 2 - 1
 
+    def interpolate(self, layer_out: "PiecewiseDiscontinuous"):
+        interpolate_polynomial_layer(layer_in=self, layer_out=layer_out)
+
+    def refine(self, layer_out: "PiecewiseDiscontinuous"):
+        refine_discontinuous_polynomial_layer(layer_in=self, layer_out=layer_out)
+
 
 class PiecewiseDiscontinuousPolynomial(PiecewiseDiscontinuous):
     def __init__(
         self,
         n: int,
         in_features: int,
         out_features: int,
@@ -534,15 +551,14 @@
     n_in = poly_in.basis.n
     n_out = poly_out.basis.n
 
     # Compute the weights on polynomial b from a
     with torch.no_grad():  # No grad so we can assign leaf variable in place
         for inputs in range(w_in.shape[0]):
             for outputs in range(w_in.shape[1]):
-
                 # TODO: I could probably do this as a single matrix operation,
                 # but this was easier for me to debug.  Also, it's not performance
                 # critical.
 
                 # loop through the out segments
                 for j in range(segments_out):
                     # compute x in the global space
@@ -600,15 +616,14 @@
     n_in = poly_in.basis.n
     n_out = poly_out.basis.n
 
     # Compute the weights on polynomial b from a
     with torch.no_grad():  # No grad so we can assign leaf variable in place
         for inputs in range(w_in.shape[0]):
             for outputs in range(w_in.shape[1]):
-
                 # TODO: I could probably do this as a single matrix operation,
                 # but this was easier for me to debug.  Also, it's not performance
                 # critical.
 
                 # loop through the out segments
                 for j in range(segments_out):
                     # compute x in the global space
@@ -683,20 +698,18 @@
     elif isinstance(layer_in, PiecewiseDiscontinuous):
         nodes_per_segment = n_in
         upper_limit = 0
 
     with torch.no_grad():  # No grad so we can assign leaf variable in place
         for inputs in range(w_in.shape[0]):
             for outputs in range(w_in.shape[1]):
-
                 a = max_slope * (random.random() * 2 - 1.0)
                 b = max_offset * (random.random() * 2 - 1.0)
 
                 for j in range(segments_in):
-
                     # compute x in the global space
                     x_global = layer_in.x_global(x_in, j)
 
                     y_global = a * x_global + b
 
                     w_in[
                         inputs,
```

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/ProductLayer.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/ProductLayer.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/attentions.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/attentions.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/layers.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -105,63 +105,100 @@
     one of the layers can turn of features of the other.
     """
 
     def __init__(
         self,
         layer_type: str,
         n: str,
-        in_width: int,
-        out_width: int,
+        in_features: int,
+        out_features: int,
         scale: float = 2.0,
         segments: int = None,
         normalization: Callable[[Any], Any] = None,
         num_input_layers: int = 2,
+        **kwargs,
     ) -> None:
         super().__init__()
-
+        self._in_features = in_features
+        self._out_features = out_features
         self._layers = [
             high_order_fc_layers(
                 layer_type=layer_type,
                 n=n,
-                in_features=in_width,
-                out_features=out_width,
+                in_features=in_features,
+                out_features=out_features,
                 segments=segments,
                 rescale_output=False,
                 scale=scale,
                 periodicity=None,
             )
             for _ in range(num_input_layers)
         ]
 
         self._normalization = normalization
 
+    @property
+    def in_features(self):
+        return self._in_features
+
+    @property
+    def out_features(self):
+        return self._out_features
+
     def forward(self, x) -> Tensor:
         outputs = [layer(x) for layer in self._layers]
 
         final = outputs[0]
         for i in range(1, len(outputs)):
             final *= outputs[i]
 
         if self._normalization is not None:
             final = self._normalization(final)
-        
+
         return final
 
+    def initialize(self, max_slope: int, max_offset: int):
+        for layer in self._layers:
+            initialize_polynomial_layer(
+                layer_in=layer, max_slope=max_slope, max_offset=max_offset
+            )
+
+    def interpolate(
+        self,
+        layer_out: "SwitchLayer",
+    ) -> None:
+        for layer1, layer2 in zip(self._layers, layer_out._layers):
+            layer1.interpolate(layer2)
+
+    def refine(self, layer_out: "SwitchLayer"):
+        for layer1, layer2 in zip(self._layers, layer_out._layers):
+            layer1.refine(layer2)
+
+
+def switch_continuous(**kwargs):
+    return SwitchLayer(layer_type="continuous", **kwargs)
+
+
+def switch_discontinuous(**kwargs):
+    return SwitchLayer(layer_type="discontinuous", **kwargs)
+
 
 fc_layers = {
     "baseline_relu": LinearReluAdapter,  # Linear layer folowed by relu
     "baseline": LinearAdapter,  # Standard linear layer
     "continuous": PiecewisePolynomial,
     "continuous_prod": PiecewisePolynomialProd,
     "discontinuous": PiecewiseDiscontinuousPolynomial,
     "discontinuous_prod": PiecewiseDiscontinuousPolynomialProd,
     "polynomial": Polynomial,
     "polynomial_prod": PolynomialProd,
     "product": Product,
     "fourier": FourierSeries,
+    "switch_continuous": switch_continuous,
+    "switch_discontinuous": switch_discontinuous,
 }
 
 convolutional_layers = {
     "continuous2d": PiecewisePolynomialConvolution2d,
     "continuous1d": PiecewisePolynomialConvolution1d,
     "continuous_prod2d": None,  # PiecewisePolynomialProd,
     "discontinuous2d": PiecewiseDiscontinuousPolynomialConvolution2d,
```

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/modules.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/modules.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/networks.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import torch.nn.functional as F
 from pytorch_lightning import LightningModule
 from torch import Tensor
 from torch.nn import Linear
 
 from high_order_layers_torch.layers import (
     SumLayer,
+    SwitchLayer,
     fixed_rotation_layer,
     high_order_convolution_layers,
     high_order_convolution_transpose_layers,
     high_order_fc_layers,
 )
 from high_order_layers_torch.PolynomialLayers import (
     PiecewiseDiscontinuous,
@@ -570,29 +571,27 @@
                 layer_name = f"normal_{i}"
 
                 setattr(self, layer_name, layer)
                 self.layer_dict[layer_name] = layer
                 self.layer_list.append(layer_name)
 
     def compute_sizes(self, input_size: int):
-
         widths = [input_size]
         for i, val in enumerate(self.kernel_size):
             nw = math.ceil((widths[i] - self.kernel_size[i] + 1) / self.stride[i])
             widths.append(nw)
 
         output_sizes = [
             self.channels[i] * focus
             for i, focus in enumerate(self.focus + [widths[-1]])
         ]
 
         return widths, output_sizes
 
     def forward(self, x: Tensor) -> Tensor:
-
         early = [x[:, :, -self.focus[0] :].flatten(1)]
         count = 1
         for name in self.layer_list:
             x = self.layer_dict[name](x)  # Assuming it only does this move once!
             if "normal" in name and count < len(self.focus):
                 tail = x[:, :, -self.focus[count] :].flatten(1)
                 early.append(tail)
@@ -766,15 +765,14 @@
     hidden_layers: int,
     rotations: int,
     scale: float = 2.0,
     periodicity: float = 2.0,
     normalization: Optional[torch.nn.Module] = None,
     resnet: bool = False,
 ) -> torch.nn.Module:
-
     fixed_input, fixed_output_width = fixed_rotation_layer(
         n=in_width, rotations=rotations
     )
 
     mlp = HighOrderMLP(
         layer_type=layer_type,
         n=n,
@@ -803,15 +801,14 @@
     hidden_width: int,
     out_width: int,
     hidden_layers: int,
     non_linearity: None,
     normalization: torch.nn.Module,
     rotations: int,
 ) -> torch.nn.Module:
-
     fixed_input, fixed_output_width = fixed_rotation_layer(
         n=in_width, rotations=rotations
     )
 
     mlp = LowOrderMLP(
         in_width=fixed_output_width,
         out_width=out_width,
@@ -845,14 +842,15 @@
                         1/input_size is bad for deep networks.
                         scale_slope=lambda input_size : 1/input_size
                         scale_slope=lambda input_size : 1/sqrt(input_size)
                         scale_slope=lambda input_size : 1
     Returns :
         Nothing, updates network in place.
     """
+
     layers = [
         module
         for module in network.model.modules()
         if not isinstance(module, nn.Sequential)
     ]
 
     for layer in layers:
@@ -861,14 +859,19 @@
 
             # In the worst case all the inputs have the same slope, so we normalize by number
             # of inputs.  Would still approach 0 avg slope for infinite width so maybe should
             # using kaiming init...
             initialize_polynomial_layer(
                 layer, max_slope=max_slope * scale_slope(inputs), max_offset=max_offset
             )
+        if isinstance(layer, SwitchLayer):
+            inputs = layer.in_features
+            layer.initialize(
+                max_slope=max_slope * scale_slope(inputs), max_offset=max_offset
+            )
 
 
 def interpolate_high_order_mlp(
     network_in: HighOrderMLP, network_out: HighOrderMLP
 ) -> None:
     """
     Create a new network with weights interpolated from network_in.  If network_out has higher
@@ -892,16 +895,16 @@
         for module in network_out.model.modules()
         if not isinstance(module, nn.Sequential)
     ]
 
     layer_pairs = zip(layers_in, layers_out)
 
     for l_in, l_out in layer_pairs:
-        if isinstance(l_in, (PiecewisePolynomial, PiecewiseDiscontinuousPolynomial)):
-            interpolate_polynomial_layer(l_in, l_out)
+        if hasattr(l_in, "interpolate"):
+            l_in.interpolate(l_out)
 
 
 def hp_refine_high_order_mlp(
     network_in: HighOrderMLP, network_out: HighOrderMLP
 ) -> None:
     """
     Create a new network with weights interpolated from network_in.  The user can change both the polynomial
@@ -923,22 +926,27 @@
         for module in network_out.model.modules()
         if not isinstance(module, nn.Sequential)
     ]
 
     layer_pairs = zip(layers_in, layers_out)
 
     for l_in, l_out in layer_pairs:
+        if hasattr(l_in, "refine"):
+            l_in.refine(l_out)
+
+        """
         if isinstance(l_in, PiecewisePolynomial) and isinstance(
             l_out, PiecewisePolynomial
         ):
             refine_polynomial_layer(l_in, l_out)
         elif isinstance(l_in, PiecewiseDiscontinuous) and isinstance(
             l_out, PiecewiseDiscontinuous
         ):
             refine_discontinuous_polynomial_layer(l_in, l_out)
+        """
 
 
 def smooth_discontinuous_network(network_in: torch.nn.Module, factor: float) -> None:
     layers = [
         module
         for module in network_in.model.modules()
         if isinstance(module, PiecewiseDiscontinuous)
```

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/positional_embeddings.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/positional_embeddings.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/high_order_layers_torch/utils.py` & `high_order_layers_torch-1.3.4/high_order_layers_torch/utils.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.3/pyproject.toml` & `high_order_layers_torch-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "high-order-layers-torch"
-version = "1.3.3"
+version = "1.3.4"
 description = "High order layers in pytorch"
 authors = ["jloverich <john.loverich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `high_order_layers_torch-1.3.3/setup.py` & `high_order_layers_torch-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'torch-optimizer>=0.3.0,<0.4.0',
  'torch>=2.0.0,<3.0.0',
  'torchmetrics>=0.10.2,<0.11.0',
  'torchvision>=0.15.1,<0.16.0']
 
 setup_kwargs = {
     'name': 'high-order-layers-torch',
-    'version': '1.3.3',
+    'version': '1.3.4',
     'description': 'High order layers in pytorch',
     'long_description': '![Build Status](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)\n\n# Piecewise Polynomial and Fourier Layers in PyTorch\n\nThis is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.\n\nLagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant.  Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models.  This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.\n\n## Idea\n\nThe idea is extremely simple - instead of a single weight at the synapse, use n-weights.  The n-weights describe a piecewise polynomial (or other complex function) and each of the n-weights can be updated independently.  A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well.  This can be implemented as construction of a polynomial or Fourier kernel followed by a standard pytorch layer where a linear activation is used.\n\nIn the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.\n\n<img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">\n\n## Why\n\nUsing higher order polynomial representations might allow networks with much fewer total weights.\n\n\n## Fully Connected Layer Types\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n\nA helper function is provided in selecting and switching between these layers\n\n```python\nfrom high_order_layers_torch.layers import *\nlayer1 = high_order_fc_layers(\n    layer_type=layer_type,\n    n=n,\n    in_features=784,\n    out_features=100,\n    segments=segments,\n    alpha=linear_part\n)\n```\n\nwhere `layer_type` is one of\n| layer_type          | representation\n|--------------------|-------------------------|\n|continuous         |  piecewise polynomial using sum at the neuron |\n|continuous_prod    |  piecewise polynomial using products at the neuron |\n|discontinuous      |  discontinuous piecewise polynomial with sum at the neuron|\n|discontinuous_prod | discontinous piecewise polynomial with product at the neuron|\n|polynomial | single polynomial (non piecewise) with sum at the neuron|\n|polynomial_prod | single polynomial (non piecewise) with product at the neuron|\n|product | Product |\n|fourier | fourier series with sum at the neuron |\n\n\n\n`n` is the number of interpolation points per segment for polynomials or the number of frequencies for fourier series, `segments` is the number of segments for piecewise polynomials, `alpha` is used in product layers and when set to 1 keeps the linear part of the product, when set to 0 it subtracts the linear part from the product.\n\n## Convolutional Layer Types\n\n```python\nconv_layer = high_order_convolution_layers(layer_type=layer_type, n=n, in_channels=3, out_channels=6, kernel_size=5, segments=segments, rescale_output=rescale_output, periodicity=periodicity)\n```\n\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n| layer_type   | representation       |\n|--------------|----------------------|\n|continuous(1d,2d)   | piecewise continuous polynomial\n|discontinuous(1d,2d) | piecewise discontinuous polynomial\n|polynomial(1d,2d) | single polynomial\n|fourier(1d,2d) | fourier series convolution\n\n## h and p refinement\np refinement is taking an existing network and increasing the polynomial order of that network without changing the network output.  This allow the user to train a network at low polynomial order and then use that same network to initialize a network with higher polynomial order.  This is particularly useful since a high order polynomial network will often converge poorly without the right initialization, the lower order network provides a good initial solution.  The function for changing the order of a network is\n```\nfrom high_order_layers_torch.networks import interpolate_high_order_mlp\ninterpolate_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n```\ncurrent implementation only works with high order MLPs, not with convnets.  A similar function exists for h refinement.  h refinement is\nrefining the number of segments in a layer, and is used for similar reasoning.  Layers with lots of segments may be slow to converge\nso the user starts with a small number of segments (1 or 2) and then increases the number of segments (h) using the lower initialization.  The following function currently only works for high order MLPs, not with convnets\n```\nfrom high_order_layers_torch.network import hp_refine_high_order_mlp\nhp_refine_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n)\n```\n# Installing\n\n## Installing locally\n\nThis repo uses poetry, so run\n\n```\npoetry install\n```\n\nand then\n\n```\npoetry shell\n```\n\n## Installing from pypi\n\n```bash\npip install high-order-layers-torch\n```\n\nor\n\n```\npoetry add high-order-layers-torch\n```\n# Examples\n\n## Simple function approximation\n\nApproximating a simple function using a single input and single output (single layer) with no hidden layers\nto approximate a function using continuous and discontinuous piecewise polynomials (with 5 pieces) and simple\npolynomials and fourier series.  The standard approach using ReLU is non competitive.  To see more complex see\nthe implicit representation page [here](https://github.com/jloveric/high-order-implicit-representation).\n\n![piecewise continuous polynomial](plots/piecewise_continuous.png)\n![piecewise discontinuous polynomial](plots/piecewise_discontinuous.png)\n![polynomial](plots/polynomial.png)\n![fourier series](plots/fourier_series.png)\n\n```python\npython examples/function_example.py\n```\n\n## XOR : 0.5 for x*y > 0 else -0.5\nSimple XOR problem using the standard network structure (2 inputs 2 hidden 1 output) this will also work with no hidden layers. The function is discontinuous along the axis and we try and fit that function. Using piecewise discontinuous layers the model can match the function exactly.\n![piecewise discontinuous polynomial](plots/xor_discontinuous.png)\nWith piecewise continuous it doesn\'t work quite as well.\n![piecewise continuous polynomial](plots/xor_continuous.png)\nPolynomial doesn\'t work well at all (expected).\n![polynomial](plots/xor_polynomial.png)\n\n## MNIST (convolutional)\n\n```python\npython examples/mnist.py max_epochs=1 train_fraction=0.1 layer_type=continuous2d n=4 segments=2\n```\n\n## CIFAR100 (convolutional)\n\n```\npython examples/cifar100.py -m max_epochs=20 train_fraction=1.0 layer_type=polynomial segments=2 n=7 nonlinearity=False rescale_output=False periodicity=2.0 lr=0.001 linear_output=False\n```\n\n## Variational Autoencoder\nStill a WIP.  Does work, but needs improvement.\n```\npython examples/variational_autoencoder.py -m max_epochs=300 train_fraction=1.0\n```\nrun with nevergrad for parameter tuning\n```\npython examples/variational_autoencoder.py -m\n```\n## Invariant MNIST (fully connected)\nWithout polynomial refinement\n```python\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 mlp.layer_type=continuous mlp.n=5 mlp.p_refine=False mlp.hidden.layers=4\n```\nwith polynomial refinement (p-refinement)\n```\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 layer_type=mlp.continuous mlp.n=2 mlp.target_n=5 mlp.p_refine=True\n```\nI\'ve also added hp refinement, but it needs a lot of testing.\n## Implicit Representation\n\nAn example of implicit representation for image compression, language generation can be found [here](https://github.com/jloveric/high-order-implicit-representation).  I intend to explore generative models in natural language further [here](https://github.com/jloveric/language-interpolation)\n\n## PDEs in Fluid Dynamics\n\nAn example using implicit representation to solve hyperbolic (nonlinear) wave equations can be found [here](https://github.com/jloveric/neural-network-pdes)\n\n## Natural Language Generation\n\nExamples using these networks for natural language generation can be found\n[here](https://github.com/jloveric/language-interpolation)\n\n## Generative music\n\nWork in progress\n[here](https://github.com/jloveric/high-order-generative-music)\n\n\n## Test and Coverage\nAfter installing and running\n```\npoetry shell\n```\nrun\n```\npytest\n```\nfor coverage, run\n```\ncoverage run -m pytest\n```\nand then\n```\ncoverage report\n```\n## A note on the unit\nThe layers used here do not require additional activation functions and use a simple sum or product in place of the activation.\nI almost always use sum units, but product units are performed in this manner\n\n$$ product=-1+\\prod_{i}(1 + f_{i})+(1-\\alpha)\\sum_{i}f_{i} $$\n\nThe 1 is added to each function output to as each of the sub products is also computed.  The linear part is controlled by\nthe alpha parameter.\n\n## Notes on normalization\nAlthough you can use batchnorm, layernorm etc... I\'ve found that you can actually just use the infinity norm ("max_abs" norm) which has no parameters\nfor this formulation (same approach seems not to work very well for standard relu networks - but need to investigate this further).\nThe max_abs normalization is defined this way\n```\nnormalized_x = x/(max(abs(x))+eps)\n```\nwhere the normalization is done per sample (as opposed to per batch).  The way the layers are formulated, we don\'t want the neuron\nvalues to extend beyond [-1, 1] as the polynomial values grow rapidly beyond that range.  I also use mirror periodicity to keep the\nvalues within from growing rapidly. We want the values to cover the entire range [-1, 1] of the polynomials as the weights\nare packed towards the edges of each segment. Normalizing by the sample L2 norm pushes most of the values towards\nzero, which I don\'t want.\n\n\n## Reference\n```\n@misc{Loverich2020,\n  author = {Loverich, John},\n  title = {High Order Layers Torch},\n  year = {2020},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/jloveric/high-order-layers-torch}},\n}\n```\n',
     'author': 'jloverich',
     'author_email': 'john.loverich@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `high_order_layers_torch-1.3.3/PKG-INFO` & `high_order_layers_torch-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: high-order-layers-torch
-Version: 1.3.3
+Version: 1.3.4
 Summary: High order layers in pytorch
 License: MIT
 Author: jloverich
 Author-email: john.loverich@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

