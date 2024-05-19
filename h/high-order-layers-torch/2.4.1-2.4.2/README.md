# Comparing `tmp/high_order_layers_torch-2.4.1.tar.gz` & `tmp/high_order_layers_torch-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "high_order_layers_torch-2.4.1.tar", max compression
+gzip compressed data, was "high_order_layers_torch-2.4.2.tar", max compression
```

## Comparing `high_order_layers_torch-2.4.1.tar` & `high_order_layers_torch-2.4.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1065 2020-12-25 19:50:48.693271 high_order_layers_torch-2.4.1/LICENSE
--rw-r--r--   0        0        0    11028 2023-12-21 14:44:07.294423 high_order_layers_torch-2.4.1/README.md
--rw-r--r--   0        0        0    15011 2023-12-19 12:04:21.593470 high_order_layers_torch-2.4.1/high_order_layers_torch/Basis.py
--rw-r--r--   0        0        0    17551 2022-11-13 17:24:03.307398 high_order_layers_torch-2.4.1/high_order_layers_torch/FunctionalConvolution.py
--rw-r--r--   0        0        0     5189 2022-11-13 17:24:03.307398 high_order_layers_torch-2.4.1/high_order_layers_torch/FunctionalConvolutionTranspose.py
--rw-r--r--   0        0        0     4353 2023-12-21 15:52:38.612483 high_order_layers_torch-2.4.1/high_order_layers_torch/LagrangePolynomial.py
--rw-r--r--   0        0        0    23810 2023-04-24 00:49:21.281123 high_order_layers_torch-2.4.1/high_order_layers_torch/PolynomialLayers.py
--rw-r--r--   0        0        0     1656 2022-11-13 17:24:03.307398 high_order_layers_torch-2.4.1/high_order_layers_torch/ProductLayer.py
--rw-r--r--   0        0        0        0 2020-12-25 19:50:53.940493 high_order_layers_torch-2.4.1/high_order_layers_torch/__init__.py
--rw-r--r--   0        0        0    22990 2023-04-23 14:16:04.430547 high_order_layers_torch-2.4.1/high_order_layers_torch/attentions.py
--rw-r--r--   0        0        0    10014 2023-12-23 20:38:46.514604 high_order_layers_torch-2.4.1/high_order_layers_torch/layers.py
--rw-r--r--   0        0        0     7417 2023-12-21 14:44:07.298423 high_order_layers_torch-2.4.1/high_order_layers_torch/modules.py
--rw-r--r--   0        0        0    33647 2023-12-21 14:46:25.817632 high_order_layers_torch-2.4.1/high_order_layers_torch/networks.py
--rw-r--r--   0        0        0     2488 2022-11-13 17:24:03.307398 high_order_layers_torch-2.4.1/high_order_layers_torch/positional_embeddings.py
--rw-r--r--   0        0        0       36 2023-12-22 15:04:00.247529 high_order_layers_torch-2.4.1/high_order_layers_torch/sparse_optimizers/__init__.py
--rw-r--r--   0        0        0     2708 2023-12-22 18:08:58.147121 high_order_layers_torch-2.4.1/high_order_layers_torch/sparse_optimizers/sparse_lion.py
--rw-r--r--   0        0        0     3782 2023-12-23 20:36:57.132806 high_order_layers_torch-2.4.1/high_order_layers_torch/utils.py
--rw-r--r--   0        0        0      728 2023-12-23 21:07:58.666269 high_order_layers_torch-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    11826 1970-01-01 00:00:00.000000 high_order_layers_torch-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-12-01 04:11:06.990013 high_order_layers_torch-2.4.2/AUTHORS
+-rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-2.4.2/LICENSE
+-rw-r--r--   0        0        0    16862 2024-05-18 17:50:24.922757 high_order_layers_torch-2.4.2/README.md
+-rw-r--r--   0        0        0    15011 2023-12-17 04:34:43.639007 high_order_layers_torch-2.4.2/high_order_layers_torch/Basis.py
+-rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolution.py
+-rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolutionTranspose.py
+-rw-r--r--   0        0        0     4353 2023-12-22 02:16:19.376958 high_order_layers_torch-2.4.2/high_order_layers_torch/LagrangePolynomial.py
+-rw-r--r--   0        0        0    23810 2023-09-09 01:07:24.996672 high_order_layers_torch-2.4.2/high_order_layers_torch/PolynomialLayers.py
+-rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-2.4.2/high_order_layers_torch/ProductLayer.py
+-rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-2.4.2/high_order_layers_torch/__init__.py
+-rw-r--r--   0        0        0    22990 2023-04-21 03:06:49.131515 high_order_layers_torch-2.4.2/high_order_layers_torch/attentions.py
+-rw-r--r--   0        0        0    10014 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/layers.py
+-rw-r--r--   0        0        0     7417 2023-12-19 14:12:35.081663 high_order_layers_torch-2.4.2/high_order_layers_torch/modules.py
+-rw-r--r--   0        0        0    33647 2023-12-22 02:16:19.376958 high_order_layers_torch-2.4.2/high_order_layers_torch/networks.py
+-rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-2.4.2/high_order_layers_torch/positional_embeddings.py
+-rw-r--r--   0        0        0       36 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/__init__.py
+-rw-r--r--   0        0        0     2708 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/sparse_lion.py
+-rw-r--r--   0        0        0     3782 2023-12-30 15:03:34.401299 high_order_layers_torch-2.4.2/high_order_layers_torch/utils.py
+-rw-r--r--   0        0        0      729 2024-05-19 13:39:06.261983 high_order_layers_torch-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0    17703 1970-01-01 00:00:00.000000 high_order_layers_torch-2.4.2/PKG-INFO
```

### Comparing `high_order_layers_torch-2.4.1/LICENSE` & `high_order_layers_torch-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/README.md` & `high_order_layers_torch-2.4.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,84 @@
 
+<!---
+[![CI](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml)
+--->
+
 # Piecewise Polynomial in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
-Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.
+Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [Discontinuous Piecewise Polynomial Neural Networks](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including huge number of extensions including continuous, Fourier series and convolutional neural networks... and many applications with varrying degrees of success.
 
 ## Collab Notebook
 Using simple high order layers
 [Simple function approximation](https://colab.research.google.com/drive/1kew0Kz4v5GB5D59-wP1rHZuCdhYknz4s?usp=sharing)
 
 Using simple high order MLP
 [2d function approximation](https://colab.research.google.com/drive/14wSNzBUFYk-1o6fuqiux_y33aV9VuwkF?usp=sharing)
 
 
 ## Idea
 
-The idea is extremely simple - instead of a single weight at the synapse, use n-weights.  The n-weights describe a piecewise polynomial (or other complex function) and each of the n-weights can be updated independently. A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well.  This can be implemented as construction of a polynomial or Fourier kernel followed by a standard pytorch layer where a linear activation is used.
+The idea is extremely simple, instead of a weight at the synapse we have a function F(x) that can be arbitrarily complex. As a practical matter I implement this by using multiple weights corresponding to each link, these weight are used as parameters of the function, and to make sure there is still some GPU efficiency, these weights are just coefficients of the basis functions.  In most of this work, the n-weights describe the value of a piecewise polynomial on a regular grid (in the case of a piecewise polynomial) each of the n-weights can be updated independently. A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well. Because the non-linearity is applied on the link, the node is simply a summation
 
 In the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.
 
 <img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">
 
+A small layer then looks like this, the values at the nodes are just summed.
+
+<img src="plots/PiecewisePolynomialLayer.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+A single neuron input output pair with a piecewise function is shown below. In the case where we use polynomials, Lagrange polynomials are being used so the values of the weights are identical to the value of the function at that point. The spacing is determined by chebyshev lobatto points, so there are always weights at the edge of each segment. In the case of discontinuous polynomial, the weights there are 2 weights for each interior segment edge.
+
+<img src="plots/NeuronDrawing.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+The image below shows the function passing through the weights when using lagrange polynomials. Note that there is no derivative continuity at the boundaries.
+
+<img src="plots/NeuronDrawingWeights.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+
 ## Why
 
-Using higher order polynomial representations might allow networks with much fewer total weights.
+Using higher order polynomial representations allow networks with much fewer total weights in certain cases. There is a
+well known phenomena in numerical modeling known as exponential convergence using spectral methods when using hp refinement,
+it's possible something like that can happen in neural networks as well.
+
+## Is this a KAN?
+
+Actually a single layer piecewise polynomial KAN (which is actually 2 layers) is a special case of a 2 layer
+piecewise polynomial network, which is used in this repo. Therefore, a piecewise polynomial layer is actually "Half a KAN" so
+it's actually simpler - Often all you need is a single polynomial layer at the input followed by a standard MLP so
+having the piecewise polynomial layer is important. Other names that have been used in the past Deep FLANN
+(functional link artificial neural network).
+
+Lagrange polynomials are widely used in finite element analysis and have the advantage that the value of the weight
+is actually the value of the function at that point in space. By limiting the weights you are limiting the maximum
+value of the function (the function may be higher than the weights in between the nodes). Also, when you go beyond the
+range of definition [-1,1] the polynomial is still defined using the last (or first) polynomial in the sequence, whether you want it defined that way at high polynomial order is another question. I mention a paper at the bottom where they do a linear
+extension beyond the range [-1,1] so values do not rise too fast - but normalization works as well.
+
+## Issues
+
+What about instabilities due to steep gradients? Seems like you can get around those with various approaches, polynomial
+refinement is one (start with piecewise linear and than increase the polynomial order after it converges), the lion
+optimizer helps a lot as well.
+
+The biggest issues I've experienced though are that it's slower than dense networks and certain operations can
+take up more memory which can cause major issues with models that already push the limits of your gpu. Now that
+KANs are popular, hopefully there will be enough people to address all these issues.
+
+In general, with enough effort, it seems I can make them "work" for any place the classic ReLU network works and
+in certain situations they clearly work much better. They also do a great job of overfitting, which just means,
+I need more data. For problems where your inputs are positional, x and y..., they seem to be far better.
+
+Finally, I believe these methods actually will benefit much more from (approximate) second order optimizers. I used those in
+my original implementation. Although there are plenty of second order optimizers out there, to date, pytorch does
+not have a standard one except LBFGS which has its own issues.
 
 ## Fully Connected Layer Types
 All polynomials are Lagrange polynomials with Chebyshev interpolation points.
 
 A helper function is provided in selecting and switching between these layers
 
 ```python
@@ -50,15 +101,14 @@
 |discontinuous_prod | discontinous piecewise polynomial with product at the neuron|
 |polynomial | single polynomial (non piecewise) with sum at the neuron|
 |polynomial_prod | single polynomial (non piecewise) with product at the neuron|
 |product | Product |
 |fourier | fourier series with sum at the neuron |
 
 
-
 `n` is the number of interpolation points per segment for polynomials or the number of frequencies for fourier series, `segments` is the number of segments for piecewise polynomials, `alpha` is used in product layers and when set to 1 keeps the linear part of the product, when set to 0 it subtracts the linear part from the product.
 
 ## Convolutional Layer Types
 
 ```python
 conv_layer = high_order_convolution_layers(layer_type=layer_type, n=n, in_channels=3, out_channels=6, kernel_size=5, segments=segments, rescale_output=rescale_output, periodicity=periodicity)
 ```
@@ -67,14 +117,25 @@
 | layer_type   | representation       |
 |--------------|----------------------|
 |continuous(1d,2d)   | piecewise continuous polynomial
 |discontinuous(1d,2d) | piecewise discontinuous polynomial
 |polynomial(1d,2d) | single polynomial
 |fourier(1d,2d) | fourier series convolution
 
+## Initializing of layers
+For non convolutional layers I've found that initializing the polynomials to continuous line across all segments, works better then a random wiggly polynomial. I don't have similar functions implemented for convolutional layers. Here is a function that does this initialization (it can be found in [networks.py](https://github.com/jloveric/high-order-layers-torch/blob/master/high_order_layers_torch/networks.py))
+```
+def initialize_network_polynomial_layers(
+    network: nn.Module,
+    max_slope: float,
+    max_offset: float,
+    scale_slope: Callable[[float], float] = lambda input_size: 1,
+)
+```
+
 ## h and p refinement
 p refinement is taking an existing network and increasing the polynomial order of that network without changing the network output.  This allow the user to train a network at low polynomial order and then use that same network to initialize a network with higher polynomial order.  This is particularly useful since a high order polynomial network will often converge poorly without the right initialization, the lower order network provides a good initial solution.  The function for changing the order of a network is
 ```
 from high_order_layers_torch.networks import interpolate_high_order_mlp
 interpolate_high_order_mlp(
     network_in: HighOrderMLP, network_out: HighOrderMLP
 ```
@@ -233,17 +294,36 @@
 where the normalization is done per sample (as opposed to per batch).  The way the layers are formulated, we don't want the neuron
 values to extend beyond [-1, 1] as the polynomial values grow rapidly beyond that range.  You can also use mirror periodicity to keep the
 values within from growing rapidly. We want the values to cover the entire range [-1, 1] of the polynomials as the weights
 are packed towards the edges of each segment (though using even number of segments means you'll have a lot of weights near the origin).
 
 
 ## Reference
+You can refer to this repo here
 ```
 @misc{Loverich2020,
   author = {Loverich, John},
   title = {High Order Layers Torch},
   year = {2020},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/jloveric/high-order-layers-torch}},
 }
 ```
+and there is an old paper which was originally written in c++ and doesn't cover
+nearly as much as this repo and all the dependent repos, which you can also refer
+to
+```
+@article{loverich2015discontinuous,
+  title={Discontinuous Piecewise Polynomial Neural Networks},
+  author={Loverich, John},
+  journal={arXiv preprint arXiv:1505.04211},
+  year={2015}
+}
+```
+## Notes
+
+Recently the paper [KAN: Kolmogorov–Arnold Networks](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
+polynomials.
+
+This paper [Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
+to the values beyond [-1,1] so it might be interesting to implement
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/Basis.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/Basis.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/FunctionalConvolution.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolution.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/FunctionalConvolutionTranspose.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/FunctionalConvolutionTranspose.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/LagrangePolynomial.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/LagrangePolynomial.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/PolynomialLayers.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/PolynomialLayers.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/ProductLayer.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/ProductLayer.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/attentions.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/attentions.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/layers.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/layers.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/modules.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/modules.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/networks.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/networks.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/positional_embeddings.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/positional_embeddings.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/sparse_optimizers/sparse_lion.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/sparse_optimizers/sparse_lion.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/high_order_layers_torch/utils.py` & `high_order_layers_torch-2.4.2/high_order_layers_torch/utils.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-2.4.1/pyproject.toml` & `high_order_layers_torch-2.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "high-order-layers-torch"
-version = "2.4.1"
+version = "2.4.2"
 description = "High order layers in pytorch"
 authors = ["jloverich <john.loverich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 torch-optimizer = "^0.3.0"
 hydra-core = "^1.2.0"
 pytorch-lightning = "^2.0.0"
 torch = ">=2.1.1"
-torchvision = "^0.16.1"
+torchvision = ">=0.18.0"
 lion-pytorch = "^0.1.2"
 torchmetrics = "^1.2.1"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.3"
 black = "^22.3.0"
 pytest = "^7.1.2"
```

### Comparing `high_order_layers_torch-2.4.1/PKG-INFO` & `high_order_layers_torch-2.4.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,107 @@
 Metadata-Version: 2.1
 Name: high-order-layers-torch
-Version: 2.4.1
+Version: 2.4.2
 Summary: High order layers in pytorch
 License: MIT
 Author: jloverich
 Author-email: john.loverich@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hydra-core (>=1.2.0,<2.0.0)
 Requires-Dist: lion-pytorch (>=0.1.2,<0.2.0)
 Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
 Requires-Dist: torch (>=2.1.1)
 Requires-Dist: torch-optimizer (>=0.3.0,<0.4.0)
 Requires-Dist: torchmetrics (>=1.2.1,<2.0.0)
-Requires-Dist: torchvision (>=0.16.1,<0.17.0)
+Requires-Dist: torchvision (>=0.18.0)
 Description-Content-Type: text/markdown
 
 
+<!---
+[![CI](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml)
+--->
+
 # Piecewise Polynomial in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
-Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.
+Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant. Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models. This is a PyTorch implementation of this [Discontinuous Piecewise Polynomial Neural Networks](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including huge number of extensions including continuous, Fourier series and convolutional neural networks... and many applications with varrying degrees of success.
 
 ## Collab Notebook
 Using simple high order layers
 [Simple function approximation](https://colab.research.google.com/drive/1kew0Kz4v5GB5D59-wP1rHZuCdhYknz4s?usp=sharing)
 
 Using simple high order MLP
 [2d function approximation](https://colab.research.google.com/drive/14wSNzBUFYk-1o6fuqiux_y33aV9VuwkF?usp=sharing)
 
 
 ## Idea
 
-The idea is extremely simple - instead of a single weight at the synapse, use n-weights.  The n-weights describe a piecewise polynomial (or other complex function) and each of the n-weights can be updated independently. A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well.  This can be implemented as construction of a polynomial or Fourier kernel followed by a standard pytorch layer where a linear activation is used.
+The idea is extremely simple, instead of a weight at the synapse we have a function F(x) that can be arbitrarily complex. As a practical matter I implement this by using multiple weights corresponding to each link, these weight are used as parameters of the function, and to make sure there is still some GPU efficiency, these weights are just coefficients of the basis functions.  In most of this work, the n-weights describe the value of a piecewise polynomial on a regular grid (in the case of a piecewise polynomial) each of the n-weights can be updated independently. A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well. Because the non-linearity is applied on the link, the node is simply a summation
 
 In the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.
 
 <img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">
 
+A small layer then looks like this, the values at the nodes are just summed.
+
+<img src="plots/PiecewisePolynomialLayer.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+A single neuron input output pair with a piecewise function is shown below. In the case where we use polynomials, Lagrange polynomials are being used so the values of the weights are identical to the value of the function at that point. The spacing is determined by chebyshev lobatto points, so there are always weights at the edge of each segment. In the case of discontinuous polynomial, the weights there are 2 weights for each interior segment edge.
+
+<img src="plots/NeuronDrawing.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+The image below shows the function passing through the weights when using lagrange polynomials. Note that there is no derivative continuity at the boundaries.
+
+<img src="plots/NeuronDrawingWeights.svg" width=50% height=50% style="display: block; margin: 0 auto">
+
+
 ## Why
 
-Using higher order polynomial representations might allow networks with much fewer total weights.
+Using higher order polynomial representations allow networks with much fewer total weights in certain cases. There is a
+well known phenomena in numerical modeling known as exponential convergence using spectral methods when using hp refinement,
+it's possible something like that can happen in neural networks as well.
+
+## Is this a KAN?
+
+Actually a single layer piecewise polynomial KAN (which is actually 2 layers) is a special case of a 2 layer
+piecewise polynomial network, which is used in this repo. Therefore, a piecewise polynomial layer is actually "Half a KAN" so
+it's actually simpler - Often all you need is a single polynomial layer at the input followed by a standard MLP so
+having the piecewise polynomial layer is important. Other names that have been used in the past Deep FLANN
+(functional link artificial neural network).
+
+Lagrange polynomials are widely used in finite element analysis and have the advantage that the value of the weight
+is actually the value of the function at that point in space. By limiting the weights you are limiting the maximum
+value of the function (the function may be higher than the weights in between the nodes). Also, when you go beyond the
+range of definition [-1,1] the polynomial is still defined using the last (or first) polynomial in the sequence, whether you want it defined that way at high polynomial order is another question. I mention a paper at the bottom where they do a linear
+extension beyond the range [-1,1] so values do not rise too fast - but normalization works as well.
+
+## Issues
+
+What about instabilities due to steep gradients? Seems like you can get around those with various approaches, polynomial
+refinement is one (start with piecewise linear and than increase the polynomial order after it converges), the lion
+optimizer helps a lot as well.
+
+The biggest issues I've experienced though are that it's slower than dense networks and certain operations can
+take up more memory which can cause major issues with models that already push the limits of your gpu. Now that
+KANs are popular, hopefully there will be enough people to address all these issues.
+
+In general, with enough effort, it seems I can make them "work" for any place the classic ReLU network works and
+in certain situations they clearly work much better. They also do a great job of overfitting, which just means,
+I need more data. For problems where your inputs are positional, x and y..., they seem to be far better.
+
+Finally, I believe these methods actually will benefit much more from (approximate) second order optimizers. I used those in
+my original implementation. Although there are plenty of second order optimizers out there, to date, pytorch does
+not have a standard one except LBFGS which has its own issues.
 
 ## Fully Connected Layer Types
 All polynomials are Lagrange polynomials with Chebyshev interpolation points.
 
 A helper function is provided in selecting and switching between these layers
 
 ```python
@@ -72,15 +124,14 @@
 |discontinuous_prod | discontinous piecewise polynomial with product at the neuron|
 |polynomial | single polynomial (non piecewise) with sum at the neuron|
 |polynomial_prod | single polynomial (non piecewise) with product at the neuron|
 |product | Product |
 |fourier | fourier series with sum at the neuron |
 
 
-
 `n` is the number of interpolation points per segment for polynomials or the number of frequencies for fourier series, `segments` is the number of segments for piecewise polynomials, `alpha` is used in product layers and when set to 1 keeps the linear part of the product, when set to 0 it subtracts the linear part from the product.
 
 ## Convolutional Layer Types
 
 ```python
 conv_layer = high_order_convolution_layers(layer_type=layer_type, n=n, in_channels=3, out_channels=6, kernel_size=5, segments=segments, rescale_output=rescale_output, periodicity=periodicity)
 ```
@@ -89,14 +140,25 @@
 | layer_type   | representation       |
 |--------------|----------------------|
 |continuous(1d,2d)   | piecewise continuous polynomial
 |discontinuous(1d,2d) | piecewise discontinuous polynomial
 |polynomial(1d,2d) | single polynomial
 |fourier(1d,2d) | fourier series convolution
 
+## Initializing of layers
+For non convolutional layers I've found that initializing the polynomials to continuous line across all segments, works better then a random wiggly polynomial. I don't have similar functions implemented for convolutional layers. Here is a function that does this initialization (it can be found in [networks.py](https://github.com/jloveric/high-order-layers-torch/blob/master/high_order_layers_torch/networks.py))
+```
+def initialize_network_polynomial_layers(
+    network: nn.Module,
+    max_slope: float,
+    max_offset: float,
+    scale_slope: Callable[[float], float] = lambda input_size: 1,
+)
+```
+
 ## h and p refinement
 p refinement is taking an existing network and increasing the polynomial order of that network without changing the network output.  This allow the user to train a network at low polynomial order and then use that same network to initialize a network with higher polynomial order.  This is particularly useful since a high order polynomial network will often converge poorly without the right initialization, the lower order network provides a good initial solution.  The function for changing the order of a network is
 ```
 from high_order_layers_torch.networks import interpolate_high_order_mlp
 interpolate_high_order_mlp(
     network_in: HighOrderMLP, network_out: HighOrderMLP
 ```
@@ -255,18 +317,36 @@
 where the normalization is done per sample (as opposed to per batch).  The way the layers are formulated, we don't want the neuron
 values to extend beyond [-1, 1] as the polynomial values grow rapidly beyond that range.  You can also use mirror periodicity to keep the
 values within from growing rapidly. We want the values to cover the entire range [-1, 1] of the polynomials as the weights
 are packed towards the edges of each segment (though using even number of segments means you'll have a lot of weights near the origin).
 
 
 ## Reference
+You can refer to this repo here
 ```
 @misc{Loverich2020,
   author = {Loverich, John},
   title = {High Order Layers Torch},
   year = {2020},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/jloveric/high-order-layers-torch}},
 }
 ```
+and there is an old paper which was originally written in c++ and doesn't cover
+nearly as much as this repo and all the dependent repos, which you can also refer
+to
+```
+@article{loverich2015discontinuous,
+  title={Discontinuous Piecewise Polynomial Neural Networks},
+  author={Loverich, John},
+  journal={arXiv preprint arXiv:1505.04211},
+  year={2015}
+}
+```
+## Notes
+
+Recently the paper [KAN: Kolmogorov–Arnold Networks](https://arxiv.org/pdf/2404.19756) was published (9 years after the original implementation of the technique in this repo), where B-splines were used on the grid. Looking at that repo, the real difference seems to be B-splines vs lagrange
+polynomials.
 
+This paper [Variations on the Chebyshev-Lagrange Activation Function](https://arxiv.org/abs/1906.10064) implements a linear extension 
+to the values beyond [-1,1] so it might be interesting to implement
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

