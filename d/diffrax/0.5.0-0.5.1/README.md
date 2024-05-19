# Comparing `tmp/diffrax-0.5.0.tar.gz` & `tmp/diffrax-0.5.1.tar.gz`

## Comparing `diffrax-0.5.0.tar` & `diffrax-0.5.1.tar`

### file list

```diff
@@ -1,54 +1,64 @@
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/__init__.py
--rw-r--r--   0        0        0    29405 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_adjoint.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_autocitation.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_custom_types.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_event.py
--rw-r--r--   0        0        0    27718 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_global_interpolation.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_heuristics.py
--rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_integrate.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_local_interpolation.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_misc.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_path.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_saveat.py
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solution.py
--rw-r--r--   0        0        0    21311 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_term.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_brownian/__init__.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_brownian/base.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_brownian/path.py
--rw-r--r--   0        0        0    17054 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_brownian/tree.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_root_finder/__init__.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_root_finder/_verychord.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_root_finder/_with_tols.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/__init__.py
--rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/base.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/bosh3.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/dopri5.py
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/dopri8.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/euler.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/euler_heun.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/heun.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/implicit_euler.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kencarp3.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kencarp4.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kencarp5.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kvaerno3.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kvaerno4.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/kvaerno5.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/leapfrog_midpoint.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/midpoint.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/milstein.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/ralston.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/reversible_heun.py
--rw-r--r--   0        0        0    51990 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/runge_kutta.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/semi_implicit_euler.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/sil3.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_solver/tsit5.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_step_size_controller/__init__.py
--rw-r--r--   0        0        0    30301 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_step_size_controller/adaptive.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_step_size_controller/base.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 diffrax-0.5.0/diffrax/_step_size_controller/constant.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 diffrax-0.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 diffrax-0.5.0/LICENSE
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 diffrax-0.5.0/README.md
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 diffrax-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    17181 2020-02-02 00:00:00.000000 diffrax-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/__init__.py
+-rw-r--r--   0        0        0    29507 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_adjoint.py
+-rw-r--r--   0        0        0    19734 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_autocitation.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_custom_types.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_event.py
+-rw-r--r--   0        0        0    28299 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_global_interpolation.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_heuristics.py
+-rw-r--r--   0        0        0    39435 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_integrate.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_local_interpolation.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_misc.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_path.py
+-rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_progress_meter.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_saveat.py
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solution.py
+-rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_term.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_typing.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/py.typed
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_brownian/__init__.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_brownian/base.py
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_brownian/path.py
+-rw-r--r--   0        0        0    18767 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_brownian/tree.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_root_finder/__init__.py
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_root_finder/_verychord.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_root_finder/_with_tols.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/__init__.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/base.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/bosh3.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/dopri5.py
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/dopri8.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/euler.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/euler_heun.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/heun.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/implicit_euler.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kencarp3.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kencarp4.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kencarp5.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kvaerno3.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kvaerno4.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/kvaerno5.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/leapfrog_midpoint.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/midpoint.py
+-rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/milstein.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/ralston.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/reversible_heun.py
+-rw-r--r--   0        0        0    51952 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/runge_kutta.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/sea.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/semi_implicit_euler.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/shark.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/shark_general.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/sil3.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/slowrk.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/spark.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/sra1.py
+-rw-r--r--   0        0        0    27182 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/srk.py
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_solver/tsit5.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_step_size_controller/__init__.py
+-rw-r--r--   0        0        0    31906 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_step_size_controller/adaptive.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_step_size_controller/base.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 diffrax-0.5.1/diffrax/_step_size_controller/constant.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 diffrax-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 diffrax-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 diffrax-0.5.1/README.md
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 diffrax-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 diffrax-0.5.1/PKG-INFO
```

### Comparing `diffrax-0.5.0/diffrax/__init__.py` & `diffrax-0.5.1/diffrax/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 )
 from ._autocitation import citation as citation, citation_rules as citation_rules
 from ._brownian import (
     AbstractBrownianPath as AbstractBrownianPath,
     UnsafeBrownianPath as UnsafeBrownianPath,
     VirtualBrownianTree as VirtualBrownianTree,
 )
-from ._custom_types import LevyVal as LevyVal
+from ._custom_types import (
+    AbstractBrownianIncrement as AbstractBrownianIncrement,
+    AbstractSpaceTimeLevyArea as AbstractSpaceTimeLevyArea,
+    AbstractSpaceTimeTimeLevyArea as AbstractSpaceTimeTimeLevyArea,
+    BrownianIncrement as BrownianIncrement,
+    SpaceTimeLevyArea as SpaceTimeLevyArea,
+    SpaceTimeTimeLevyArea as SpaceTimeTimeLevyArea,
+)
 from ._event import (
     AbstractDiscreteTerminatingEvent as AbstractDiscreteTerminatingEvent,
     DiscreteTerminatingEvent as DiscreteTerminatingEvent,
     SteadyStateEvent as SteadyStateEvent,
 )
 from ._global_interpolation import (
     AbstractGlobalInterpolation as AbstractGlobalInterpolation,
@@ -33,14 +40,20 @@
     AbstractLocalInterpolation as AbstractLocalInterpolation,
     FourthOrderPolynomialInterpolation as FourthOrderPolynomialInterpolation,
     LocalLinearInterpolation as LocalLinearInterpolation,
     ThirdOrderHermitePolynomialInterpolation as ThirdOrderHermitePolynomialInterpolation,  # noqa: E501
 )
 from ._misc import adjoint_rms_seminorm as adjoint_rms_seminorm
 from ._path import AbstractPath as AbstractPath
+from ._progress_meter import (
+    AbstractProgressMeter as AbstractProgressMeter,
+    NoProgressMeter as NoProgressMeter,
+    TextProgressMeter as TextProgressMeter,
+    TqdmProgressMeter as TqdmProgressMeter,
+)
 from ._root_finder import (
     VeryChord as VeryChord,
     with_stepsize_controller_tols as with_stepsize_controller_tols,
 )
 from ._saveat import SaveAt as SaveAt, SubSaveAt as SubSaveAt
 from ._solution import (
     is_event as is_event,
@@ -55,23 +68,25 @@
     AbstractERK as AbstractERK,
     AbstractESDIRK as AbstractESDIRK,
     AbstractImplicitSolver as AbstractImplicitSolver,
     AbstractItoSolver as AbstractItoSolver,
     AbstractRungeKutta as AbstractRungeKutta,
     AbstractSDIRK as AbstractSDIRK,
     AbstractSolver as AbstractSolver,
+    AbstractSRK as AbstractSRK,
     AbstractStratonovichSolver as AbstractStratonovichSolver,
     AbstractWrappedSolver as AbstractWrappedSolver,
     Bosh3 as Bosh3,
     ButcherTableau as ButcherTableau,
     CalculateJacobian as CalculateJacobian,
     Dopri5 as Dopri5,
     Dopri8 as Dopri8,
     Euler as Euler,
     EulerHeun as EulerHeun,
+    GeneralShARK as GeneralShARK,
     HalfSolver as HalfSolver,
     Heun as Heun,
     ImplicitEuler as ImplicitEuler,
     ItoMilstein as ItoMilstein,
     KenCarp3 as KenCarp3,
     KenCarp4 as KenCarp4,
     KenCarp5 as KenCarp5,
@@ -79,16 +94,22 @@
     Kvaerno4 as Kvaerno4,
     Kvaerno5 as Kvaerno5,
     LeapfrogMidpoint as LeapfrogMidpoint,
     Midpoint as Midpoint,
     MultiButcherTableau as MultiButcherTableau,
     Ralston as Ralston,
     ReversibleHeun as ReversibleHeun,
+    SEA as SEA,
     SemiImplicitEuler as SemiImplicitEuler,
+    ShARK as ShARK,
     Sil3 as Sil3,
+    SlowRK as SlowRK,
+    SPaRK as SPaRK,
+    SRA1 as SRA1,
+    StochasticButcherTableau as StochasticButcherTableau,
     StratonovichMilstein as StratonovichMilstein,
     Tsit5 as Tsit5,
 )
 from ._step_size_controller import (
     AbstractAdaptiveStepSizeController as AbstractAdaptiveStepSizeController,
     AbstractStepSizeController as AbstractStepSizeController,
     ConstantStepSize as ConstantStepSize,
```

### Comparing `diffrax-0.5.0/diffrax/_adjoint.py` & `diffrax-0.5.1/diffrax/_adjoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import functools as ft
 import warnings
-from collections.abc import Iterable
-from typing import Any, Optional, Union
+from collections.abc import Callable, Iterable
+from typing import Any, cast, Optional, Union
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
@@ -16,14 +16,17 @@
 
 from ._heuristics import is_sde, is_unsafe_sde
 from ._saveat import save_y, SaveAt, SubSaveAt
 from ._solver import AbstractItoSolver, AbstractRungeKutta, AbstractStratonovichSolver
 from ._term import AbstractTerm, AdjointTerm
 
 
+ω = cast(Callable, ω)
+
+
 def _is_none(x):
     return x is None
 
 
 def _is_subsaveat(x: Any) -> bool:
     return isinstance(x, SubSaveAt)
 
@@ -124,14 +127,15 @@
         t1,
         dt0,
         max_steps,
         throw,
         init_state,
         passed_solver_state,
         passed_controller_state,
+        progress_meter,
     ) -> Any:
         """Runs the main solve loop. Subclasses can override this to provide custom
         backpropagation behaviour; see for example the implementation of
         [`diffrax.BacksolveAdjoint`][].
         """
 
     # Eurgh, delayed imports to handle circular dependencies.
@@ -555,23 +559,24 @@
     saveat,
     t0,
     t1,
     dt0,
     max_steps,
     throw,
     init_state,
+    progress_meter,
 ):
     assert discrete_terminating_event is None
 
     #
     # Unpack our various arguments. Delete a lot of things just to make sure we're not
     # using them later.
     #
 
-    del perturbed, init_state, t1
+    del perturbed, init_state, t1, progress_meter
     ts, ys = residuals
     del residuals
     grad_final_state, _ = grad_final_state__aux_stats
     # Note that `grad_final_state.save_state` has type `PyTree[SaveState]`; here we are
     # relying on the guard in `BacksolveAdjoint` that it have trivial structure.
     grad_ys = grad_final_state.save_state.ys
     # We take the simple way out and don't try to handle symbolic zeros.
```

### Comparing `diffrax-0.5.0/diffrax/_autocitation.py` & `diffrax-0.5.1/diffrax/_autocitation.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,31 @@
 from ._brownian import AbstractBrownianPath, VirtualBrownianTree
 from ._heuristics import is_cde, is_sde
 from ._integrate import diffeqsolve
 from ._misc import adjoint_rms_seminorm
 from ._saveat import SubSaveAt
 from ._solver import (
     AbstractImplicitSolver,
+    AbstractItoSolver,
+    AbstractSRK,
+    AbstractStratonovichSolver,
     Dopri5,
     Dopri8,
+    GeneralShARK,
     Kvaerno3,
     Kvaerno4,
     Kvaerno5,
     LeapfrogMidpoint,
     ReversibleHeun,
+    SEA,
     SemiImplicitEuler,
+    ShARK,
+    SlowRK,
+    SPaRK,
+    SRA1,
     Tsit5,
 )
 from ._step_size_controller import PIDController
 
 
 def citation(*args, **kwargs):
     """Autogenerate a list of BibTeX references for the numerical methods being used.
@@ -370,15 +379,23 @@
             return r"""
 % You are backpropagating using adjoint seminorms, which was introduced in::
 """ + _parse_reference(adjoint_rms_seminorm)
 
 
 @citation_rules.append
 def _explicit_solver(solver, terms=None):
-    if not isinstance(solver, AbstractImplicitSolver) and not is_sde(terms):
+    if not isinstance(
+        solver,
+        (
+            AbstractImplicitSolver,
+            AbstractSRK,
+            AbstractItoSolver,
+            AbstractStratonovichSolver,
+        ),
+    ) and not is_sde(terms):
         return r"""
 % You are using an explicit solver, and may wish to cite the standard textbook:
 @book{hairer2008solving-i,
   address={Berlin},
   author={Hairer, E. and N{\o}rsett, S.P. and Wanner, G.},
   edition={Second Revised Edition},
   publisher={Springer},
@@ -463,14 +480,20 @@
     if type(solver) in (
         Tsit5,
         Kvaerno3,
         Kvaerno4,
         Kvaerno5,
         ReversibleHeun,
         LeapfrogMidpoint,
+        ShARK,
+        SRA1,
+        SlowRK,
+        GeneralShARK,
+        SPaRK,
+        SEA,
     ):
         return (
             r"""
 % You are using the """
             + solver.__class__.__name__
             + r""" solver, which was introduced in:
 """
```

### Comparing `diffrax-0.5.0/diffrax/_event.py` & `diffrax-0.5.1/diffrax/_event.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_global_interpolation.py` & `diffrax-0.5.1/diffrax/_global_interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import functools as ft
 from collections.abc import Callable
-from typing import Optional, TYPE_CHECKING
+from typing import cast, Optional, TYPE_CHECKING
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 
 
 if TYPE_CHECKING:
     from typing import ClassVar as AbstractVar
 else:
     from equinox import AbstractVar
+
 from equinox.internal import ω
 from jaxtyping import Array, ArrayLike, PyTree, Real, Shaped
 
 from ._custom_types import DenseInfos, IntScalarLike, RealScalarLike, Y
 from ._local_interpolation import AbstractLocalInterpolation
 from ._misc import fill_forward, left_broadcast_to
 from ._path import AbstractPath
 
 
+ω = cast(Callable, ω)
+
+
 class AbstractGlobalInterpolation(AbstractPath):
     ts: AbstractVar[Real[Array, " times"]]
     ts_size: AbstractVar[IntScalarLike]
 
     def __check_init__(self):
         if self.ts.ndim != 1:
             raise ValueError("`ts` must be one dimensional.")
@@ -135,15 +139,18 @@
 
         prev_ys = jtu.tree_map(_index, self.ys)
         next_ys = (self.ys**ω)[index + 1].ω
         prev_t = self.ts[index]
         next_t = self.ts[index + 1]
         diff_t = next_t - prev_t
 
-        return (prev_ys**ω + (next_ys**ω - prev_ys**ω) * (fractional_part / diff_t)).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (
+                prev_ys**ω + (next_ys**ω - prev_ys**ω) * (fractional_part / diff_t)
+            ).ω
 
     @eqx.filter_jit
     def derivative(self, t: RealScalarLike, left: bool = True) -> PyTree[Array]:
         r"""Evaluate the derivative of the linear interpolation. Essentially equivalent
         to `jax.jvp(self.evaluate, (t,), (jnp.ones_like(t),))`.
 
         **Arguments:**
@@ -157,18 +164,19 @@
         The derivative of the interpolation of the data. Suppose $t_j < t < t_{j+1}$,
         where $t_j$ and $t_{j+1}$ are some elements of `ts` passed in `__init__`. Then
         the value returned is $\frac{y_{j+1} - y_j}{t_{j+1} - t_j}$.
         """
 
         index, _ = self._interpret_t(t, left)
 
-        return (
-            (ω(self.ys)[index + 1] - ω(self.ys)[index])
-            / (self.ts[index + 1] - self.ts[index])
-        ).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (
+                (ω(self.ys)[index + 1] - ω(self.ys)[index])
+                / (self.ts[index + 1] - self.ts[index])
+            ).ω
 
 
 LinearInterpolation.__init__.__doc__ = """**Arguments:**
 
 - `ts`: Some increasing collection of times.
 - `ys`: The value of the data at those times.
 
@@ -246,18 +254,19 @@
 
         if t1 is not None:
             return self.evaluate(t1, left=left) - self.evaluate(t0, left=left)
         index, frac = self._interpret_t(t0, left)
 
         d, c, b, a = self.coeffs
 
-        return (
-            ω(a)[index]
-            + frac * (ω(b)[index] + frac * (ω(c)[index] + frac * ω(d)[index]))
-        ).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (
+                ω(a)[index]
+                + frac * (ω(b)[index] + frac * (ω(c)[index] + frac * ω(d)[index]))
+            ).ω
 
     @eqx.filter_jit
     def derivative(
         self, t: RealScalarLike, left: bool = True
     ) -> PyTree[Shaped[Array, "?*shape"], "Y"]:
         r"""Evaluate the derivative of the cubic interpolation. Essentially equivalent
         to `jax.jvp(self.evaluate, (t,), (jnp.ones_like(t),))`.
@@ -275,15 +284,16 @@
         The derivative of the interpolation of the data.
         """
 
         index, frac = self._interpret_t(t, left)
 
         d, c, b, _ = self.coeffs
 
-        return (ω(b)[index] + frac * (2 * ω(c)[index] + frac * 3 * ω(d)[index])).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (ω(b)[index] + frac * (2 * ω(c)[index] + frac * 3 * ω(d)[index])).ω
 
 
 CubicInterpolation.__init__.__doc__ = """**Arguments:**
 
 - `ts`: Some increasing collection of times.
 - `coeffs`: The coefficients at all but the last time.
 
@@ -614,34 +624,37 @@
         Real[Array, " *channels"],
         Shaped[Array, " *channels"],
         Shaped[Array, " *channels"],
     ],
 ]:
     prev_ti, prev_yi, prev_deriv_i = carry
     ti, yi, next_ti, next_yi = value
-    first_deriv_i = (next_yi - yi) / (next_ti - ti)
-    later_deriv_i = (yi - prev_yi) / (ti - prev_ti)
+    with jax.numpy_dtype_promotion("standard"):
+        first_deriv_i = (next_yi - yi) / (next_ti - ti)
+        later_deriv_i = (yi - prev_yi) / (ti - prev_ti)
     deriv_i = jnp.where(jnp.isnan(prev_yi), first_deriv_i, later_deriv_i)
     cond = jnp.isnan(yi)
     carry_ti = jnp.where(cond, prev_ti, ti)
     carry_yi = jnp.where(cond, prev_yi, yi)
     carry_deriv_i = jnp.where(cond, prev_deriv_i, deriv_i)
 
     return (carry_ti, carry_yi, carry_deriv_i), (carry_ti, carry_yi, carry_deriv_i)
 
 
 def _hermite_coeffs(t0, y0, deriv0, t1, y1):
     t_diff = t1 - t0
-    deriv1 = (y1 - y0) / t_diff
-    d_deriv = deriv1 - deriv0
 
-    a = y0
-    b = deriv0
-    c = 2 * d_deriv / t_diff
-    d = -d_deriv / t_diff**2
+    with jax.numpy_dtype_promotion("standard"):
+        deriv1 = (y1 - y0) / t_diff
+        d_deriv = deriv1 - deriv0
+
+        a = y0
+        b = deriv0
+        c = 2 * d_deriv / t_diff
+        d = -d_deriv / (t_diff**2)
 
     return d, c, b, a
 
 
 def _hermite_impl(prev_ti, prev_yi, prev_deriv_i, ti, next_ti, next_yi):
     d, c, b, a = _hermite_coeffs(prev_ti, prev_yi, prev_deriv_i, next_ti, next_yi)
     ts = jnp.stack([prev_ti, next_ti])
@@ -676,15 +689,16 @@
 
     t0 = ts[0]
     if replace_nans_at_start is None:
         y0 = ys[0]
     else:
         y0 = jnp.broadcast_to(replace_nans_at_start, ys[0].shape)
     if deriv0 is None:
-        deriv0 = (next_ys[0] - y0) / (next_ts[0] - t0)
+        with jax.numpy_dtype_promotion("standard"):
+            deriv0 = (next_ys[0] - y0) / (next_ts[0] - t0)
     else:
         deriv0 = jnp.broadcast_to(deriv0, ys[0].shape)
     ts = ts[:-1]
     ys = ys[:-1]
     _, (prev_ts, prev_ys, prev_derivs) = lax.scan(
         _hermite_forward, (t0, y0, deriv0), (ts[1:], ys[1:], next_ts[1:], next_ys[1:])
     )
@@ -754,14 +768,18 @@
     The coefficients of the Hermite cubic spline. If `ts` has length $T$ then the
     coefficients will be of length $T - 1$, covering each of the intervals from `ts[0]`
     to `ts[1]`, and `ts[1]` to `ts[2]` etc.
     """
 
     ts = _check_ts(ts)
     fn = ft.partial(_backward_hermite_coefficients, fill_forward_nans_at_end, ts)
+
+    if len(jtu.tree_leaves(ys)) == 0:
+        return tuple(ys for _ in range(4))
+
     if deriv0 is None:
         if replace_nans_at_start is None:
             coeffs = jtu.tree_map(fn, ys)
         else:
             _fn = lambda ys, replace_nans_at_start: fn(ys, None, replace_nans_at_start)
             coeffs = jtu.tree_map(_fn, ys, replace_nans_at_start)
     else:
```

### Comparing `diffrax-0.5.0/diffrax/_heuristics.py` & `diffrax-0.5.1/diffrax/_heuristics.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_integrate.py` & `diffrax-0.5.1/diffrax/_integrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import functools as ft
 import typing
 import warnings
 from collections.abc import Callable
-from typing import Any, get_args, get_origin, Optional, Tuple, TYPE_CHECKING
+from typing import (
+    Any,
+    get_args,
+    get_origin,
+    Optional,
+    Tuple,
+    TYPE_CHECKING,
+)
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.core
 import jax.numpy as jnp
 import jax.tree_util as jtu
@@ -20,15 +27,19 @@
     FloatScalarLike,
     IntScalarLike,
     RealScalarLike,
 )
 from ._event import AbstractDiscreteTerminatingEvent
 from ._global_interpolation import DenseInterpolation
 from ._heuristics import is_sde, is_unsafe_sde
-from ._misc import static_select
+from ._misc import linear_rescale, static_select
+from ._progress_meter import (
+    AbstractProgressMeter,
+    NoProgressMeter,
+)
 from ._root_finder import use_stepsize_tol
 from ._saveat import SaveAt, SubSaveAt
 from ._solution import is_okay, is_successful, RESULTS, Solution
 from ._solver import (
     AbstractImplicitSolver,
     AbstractItoSolver,
     AbstractSolver,
@@ -41,14 +52,15 @@
 from ._step_size_controller import (
     AbstractAdaptiveStepSizeController,
     AbstractStepSizeController,
     ConstantStepSize,
     StepTo,
 )
 from ._term import AbstractTerm, MultiTerm, ODETerm, WrapTerm
+from ._typing import better_isinstance, get_args_of, get_origin_no_specials
 
 
 class SaveState(eqx.Module):
     saveat_ts_index: IntScalarLike
     ts: eqxi.MaybeBuffer[Real[Array, " times"]]
     ys: PyTree[eqxi.MaybeBuffer[Inexact[Array, "times ..."]]]
     save_index: IntScalarLike
@@ -67,36 +79,88 @@
     num_accepted_steps: IntScalarLike
     num_rejected_steps: IntScalarLike
     # Output that is .at[].set() updated during the solve (and their indices)
     save_state: PyTree[SaveState]
     dense_ts: Optional[eqxi.MaybeBuffer[Float[Array, " times_plus_1"]]]
     dense_infos: Optional[BufferDenseInfos]
     dense_save_index: Optional[IntScalarLike]
+    progress_meter_state: PyTree[Array]
 
 
-def _is_none(x):
+def _is_none(x: Any) -> bool:
     return x is None
 
 
-def _term_compatible(terms, term_structure):
-    def _check(term_cls, term):
-        if get_origin(term_cls) is MultiTerm:
+def _term_compatible(
+    y: PyTree[ArrayLike],
+    args: PyTree[Any],
+    terms: PyTree[AbstractTerm],
+    term_structure: PyTree,
+    contr_kwargs: PyTree[dict],
+) -> bool:
+    error_msg = "term_structure"
+
+    def _check(term_cls, term, term_contr_kwargs, yi):
+        if get_origin_no_specials(term_cls, error_msg) is MultiTerm:
             if isinstance(term, MultiTerm):
                 [_tmp] = get_args(term_cls)
                 assert get_origin(_tmp) in (tuple, Tuple), "Malformed term_structure"
-                if not _term_compatible(term.terms, get_args(_tmp)):
-                    raise ValueError
+                assert len(term.terms) == len(get_args(_tmp))
+                assert type(term_contr_kwargs) is tuple
+                assert len(term.terms) == len(term_contr_kwargs)
+                for term, arg, term_contr_kwarg in zip(
+                    term.terms, get_args(_tmp), term_contr_kwargs
+                ):
+                    if not _term_compatible(yi, args, term, arg, term_contr_kwarg):
+                        raise ValueError
             else:
                 raise ValueError
         else:
-            if not isinstance(term, term_cls):
+            # Check that `term` is an instance of `term_cls` (ignoring any generic
+            # parameterization).
+            origin_cls = get_origin_no_specials(term_cls, error_msg)
+            if origin_cls is None:
+                origin_cls = term_cls
+            if not isinstance(term, origin_cls):
                 raise ValueError
 
+            # Now check the generic parametrization of `term_cls`; can be one of:
+            # -----------------------------------------
+            # `term_cls`                | `term_args`
+            # --------------------------|--------------
+            # AbstractTerm              | ()
+            # AbstractTerm[VF, Control] | (VF, Control)
+            # -----------------------------------------
+            term_args = get_args_of(AbstractTerm, term_cls, error_msg)
+            n_term_args = len(term_args)
+            if n_term_args == 0:
+                pass
+            elif n_term_args == 2:
+                vf_type_expected, control_type_expected = term_args
+                vf_type = eqx.filter_eval_shape(term.vf, 0.0, yi, args)
+                vf_type_compatible = eqx.filter_eval_shape(
+                    better_isinstance, vf_type, vf_type_expected
+                )
+                if not vf_type_compatible:
+                    raise ValueError
+
+                contr = ft.partial(term.contr, **term_contr_kwargs)
+                control_type = jax.eval_shape(contr, 0.0, 0.0)
+                control_type_compatible = eqx.filter_eval_shape(
+                    better_isinstance, control_type, control_type_expected
+                )
+                if not control_type_compatible:
+                    raise ValueError
+            else:
+                assert False, "Malformed term structure"
+            # If we've got to this point then the term is compatible
+
     try:
-        jtu.tree_map(_check, term_structure, terms)
+        with jax.numpy_dtype_promotion("standard"):
+            jtu.tree_map(_check, term_structure, terms, contr_kwargs, y)
     except ValueError:
         # ValueError may also arise from mismatched tree structures
         return False
     return True
 
 
 def _is_subsaveat(x: Any) -> bool:
@@ -185,14 +249,15 @@
     dt0,
     max_steps,
     terms,
     args,
     init_state,
     inner_while_loop,
     outer_while_loop,
+    progress_meter,
 ):
     if saveat.dense:
         dense_ts = init_state.dense_ts
         dense_ts = dense_ts.at[0].set(t0)
         init_state = eqx.tree_at(lambda s: s.dense_ts, init_state, dense_ts)
 
     def save_t0(subsaveat: SubSaveAt, save_state: SaveState) -> SaveState:
@@ -275,14 +340,18 @@
         #
         # Do some book-keeping.
         #
 
         tprev = jnp.minimum(tprev, t1)
         tnext = _clip_to_end(tprev, tnext, t1, keep_step)
 
+        progress_meter_state = progress_meter.step(
+            state.progress_meter_state, linear_rescale(t0, tprev, t1)
+        )
+
         # The other parts of the mutable state are kept/not-kept (based on whether the
         # step was accepted) by the stepsize controller. But it doesn't get access to
         # these parts, so we do them here.
         keep = lambda a, b: jnp.where(keep_step, a, b)
         y = jtu.tree_map(keep, y, state.y)
         solver_state = jtu.tree_map(keep, solver_state, state.solver_state)
         made_jump = static_select(keep_step, made_jump, state.made_jump)
@@ -402,14 +471,15 @@
             num_steps=num_steps,
             num_accepted_steps=num_accepted_steps,
             num_rejected_steps=num_rejected_steps,
             save_state=save_state,
             dense_ts=dense_ts,  # pyright: ignore
             dense_infos=dense_infos,
             dense_save_index=dense_save_index,
+            progress_meter_state=progress_meter_state,
         )
 
         if discrete_terminating_event is not None:
             discrete_terminating_event_occurred = discrete_terminating_event(
                 new_state,
                 solver=solver,
                 stepsize_controller=stepsize_controller,
@@ -506,14 +576,15 @@
     *,
     saveat: SaveAt = SaveAt(t1=True),
     stepsize_controller: AbstractStepSizeController = ConstantStepSize(),
     adjoint: AbstractAdjoint = RecursiveCheckpointAdjoint(),
     discrete_terminating_event: Optional[AbstractDiscreteTerminatingEvent] = None,
     max_steps: Optional[int] = 4096,
     throw: bool = True,
+    progress_meter: AbstractProgressMeter = NoProgressMeter(),
     solver_state: Optional[PyTree[ArrayLike]] = None,
     controller_state: Optional[PyTree[ArrayLike]] = None,
     made_jump: Optional[BoolScalarLike] = None,
 ) -> Solution:
     """Solves a differential equation.
 
     This function is the main entry point for solving all kinds of initial value
@@ -583,14 +654,17 @@
 
             When `jax.vmap`-ing a differential equation solve, then
             `throw=True` means that an exception will be raised if any batch element
             fails. You may prefer to set `throw=False` and inspect the `result` field
             of the returned solution object, to determine which batch elements
             succeeded and which failed.
 
+    - `progress_meter`: A progress meter to indicate how far through the solve has
+        progressed. See [the progress meters page](./progress_meter.md).
+
     - `solver_state`: Some initial state for the solver. Generally obtained by
         `SaveAt(solver_state=True)` from a previous solve.
 
     - `controller_state`: Some initial state for the step size controller. Generally
         obtained by `SaveAt(controller_state=True)` from a previous solve.
 
     - `made_jump`: Whether a jump has just been made at `t0`. Used to update
@@ -631,66 +705,20 @@
         dt0 = eqxi.error_if(jnp.array(dt0), pred, msg)
 
     # Error checking and warning for complex dtypes
     if any(
         eqx.is_array(xi) and jnp.iscomplexobj(xi)
         for xi in jtu.tree_leaves((terms, y0, args))
     ):
-        if isinstance(solver, AbstractImplicitSolver):
-            raise ValueError(
-                "Implicit solvers in conjunction with complex dtypes is currently not "
-                "supported."
-            )
         warnings.warn(
             "Complex dtype support is work in progress, please read "
             "https://github.com/patrick-kidger/diffrax/pull/197 and proceed carefully.",
             stacklevel=2,
         )
 
-    # Backward compatibility
-    if isinstance(
-        solver, (EulerHeun, ItoMilstein, StratonovichMilstein)
-    ) and _term_compatible(terms, (ODETerm, AbstractTerm)):
-        warnings.warn(
-            "Passing `terms=(ODETerm(...), SomeOtherTerm(...))` to "
-            f"{solver.__class__.__name__} is deprecated in favour of "
-            "`terms=MultiTerm(ODETerm(...), SomeOtherTerm(...))`. This means that "
-            "the same terms can now be passed used for both general and SDE-specific "
-            "solvers!",
-            stacklevel=2,
-        )
-        terms = MultiTerm(*terms)
-
-    # Error checking
-    if not _term_compatible(terms, solver.term_structure):
-        raise ValueError(
-            "`terms` must be a PyTree of `AbstractTerms` (such as `ODETerm`), with "
-            f"structure {solver.term_structure}"
-        )
-
-    if is_sde(terms):
-        if not isinstance(solver, (AbstractItoSolver, AbstractStratonovichSolver)):
-            warnings.warn(
-                f"`{type(solver).__name__}` is not marked as converging to either the "
-                "Itô or the Stratonovich solution.",
-                stacklevel=2,
-            )
-        if isinstance(stepsize_controller, AbstractAdaptiveStepSizeController):
-            # Specific check to not work even if using HalfSolver(Euler())
-            if isinstance(solver, Euler):
-                raise ValueError(
-                    "An SDE should not be solved with adaptive step sizes with Euler's "
-                    "method, as it may not converge to the correct solution."
-                )
-    if is_unsafe_sde(terms):
-        if isinstance(stepsize_controller, AbstractAdaptiveStepSizeController):
-            raise ValueError(
-                "`UnsafeBrownianPath` cannot be used with adaptive step sizes."
-            )
-
     # Allow setting e.g. t0 as an int with dt0 as a float.
     timelikes = [t0, t1, dt0] + [
         s.ts for s in jtu.tree_leaves(saveat.subs, is_leaf=_is_subsaveat)
     ]
     timelikes = [x for x in timelikes if x is not None]
     with jax.numpy_dtype_promotion("standard"):
         time_dtype = jnp.result_type(*timelikes)
@@ -726,14 +754,59 @@
         with jax.numpy_dtype_promotion("standard"):
             _dtype = jnp.result_type(yi, time_dtype)  # noqa: F821
         return jnp.asarray(yi, dtype=_dtype)
 
     y0 = jtu.tree_map(_promote, y0)
     del timelikes
 
+    # Backward compatibility
+    if isinstance(
+        solver, (EulerHeun, ItoMilstein, StratonovichMilstein)
+    ) and _term_compatible(
+        y0, args, terms, (ODETerm, AbstractTerm), solver.term_compatible_contr_kwargs
+    ):
+        warnings.warn(
+            "Passing `terms=(ODETerm(...), SomeOtherTerm(...))` to "
+            f"{solver.__class__.__name__} is deprecated in favour of "
+            "`terms=MultiTerm(ODETerm(...), SomeOtherTerm(...))`. This means that "
+            "the same terms can now be passed used for both general and SDE-specific "
+            "solvers!",
+            stacklevel=2,
+        )
+        terms = MultiTerm(*terms)
+
+    # Error checking
+    if not _term_compatible(
+        y0, args, terms, solver.term_structure, solver.term_compatible_contr_kwargs
+    ):
+        raise ValueError(
+            "`terms` must be a PyTree of `AbstractTerms` (such as `ODETerm`), with "
+            f"structure {solver.term_structure}"
+        )
+
+    if is_sde(terms):
+        if not isinstance(solver, (AbstractItoSolver, AbstractStratonovichSolver)):
+            warnings.warn(
+                f"`{type(solver).__name__}` is not marked as converging to either the "
+                "Itô or the Stratonovich solution.",
+                stacklevel=2,
+            )
+        if isinstance(stepsize_controller, AbstractAdaptiveStepSizeController):
+            # Specific check to not work even if using HalfSolver(Euler())
+            if isinstance(solver, Euler):
+                raise ValueError(
+                    "An SDE should not be solved with adaptive step sizes with Euler's "
+                    "method, as it may not converge to the correct solution."
+                )
+    if is_unsafe_sde(terms):
+        if isinstance(stepsize_controller, AbstractAdaptiveStepSizeController):
+            raise ValueError(
+                "`UnsafeBrownianPath` cannot be used with adaptive step sizes."
+            )
+
     # Normalises time: if t0 > t1 then flip things around.
     direction = jnp.where(t0 < t1, 1, -1)
     t0 = t0 * direction
     t1 = t1 * direction
     if dt0 is not None:
         dt0 = dt0 * direction
     saveat = eqx.tree_at(
@@ -887,14 +960,17 @@
         dense_infos = jtu.tree_map(_make_full, dense_info)
         dense_save_index = 0
     else:
         dense_ts = None
         dense_infos = None
         dense_save_index = None
 
+    # Progress meter
+    progress_meter_state = progress_meter.init()
+
     # Initialise state
     init_state = State(
         y=y0,
         tprev=tprev,
         tnext=tnext,
         made_jump=made_jump,
         solver_state=solver_state,
@@ -903,14 +979,15 @@
         num_steps=num_steps,
         num_accepted_steps=num_accepted_steps,
         num_rejected_steps=num_rejected_steps,
         save_state=save_state,
         dense_ts=dense_ts,
         dense_infos=dense_infos,
         dense_save_index=dense_save_index,
+        progress_meter_state=progress_meter_state,
     )
 
     #
     # Main loop
     #
 
     final_state, aux_stats = adjoint.loop(
@@ -924,20 +1001,23 @@
         t1=t1,
         dt0=dt0,
         max_steps=max_steps,
         init_state=init_state,
         throw=throw,
         passed_solver_state=passed_solver_state,
         passed_controller_state=passed_controller_state,
+        progress_meter=progress_meter,
     )
 
     #
     # Finish up
     #
 
+    progress_meter.close(final_state.progress_meter_state)
+
     is_save_state = lambda x: isinstance(x, SaveState)
     ts = jtu.tree_map(
         lambda s: s.ts * direction, final_state.save_state, is_leaf=is_save_state
     )
     ys = jtu.tree_map(lambda s: s.ys, final_state.save_state, is_leaf=is_save_state)
     # It's important that we don't do any further postprocessing on `ys` here, as
     # it is the `final_state` value that is used when backpropagating via
```

### Comparing `diffrax-0.5.0/diffrax/_local_interpolation.py` & `diffrax-0.5.1/diffrax/_local_interpolation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import Optional, TYPE_CHECKING
+from collections.abc import Callable
+from typing import cast, Optional, TYPE_CHECKING
 
+import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 
 
 if TYPE_CHECKING:
     from typing import ClassVar as AbstractVar
@@ -13,34 +15,40 @@
 from jaxtyping import Array, ArrayLike, PyTree, Shaped
 
 from ._custom_types import RealScalarLike, Y
 from ._misc import linear_rescale
 from ._path import AbstractPath
 
 
+ω = cast(Callable, ω)
+
+
 class AbstractLocalInterpolation(AbstractPath):
     pass
 
 
 class LocalLinearInterpolation(AbstractLocalInterpolation):
     t0: RealScalarLike
     t1: RealScalarLike
     y0: Y
     y1: Y
 
     def evaluate(
         self, t0: RealScalarLike, t1: Optional[RealScalarLike] = None, left: bool = True
     ) -> PyTree[Array]:
         del left
-        if t1 is None:
-            coeff = linear_rescale(self.t0, t0, self.t1)
-            return (self.y0**ω + coeff * (self.y1**ω - self.y0**ω)).call(jnp.asarray).ω
-        else:
-            coeff = (t1 - t0) / (self.t1 - self.t0)
-            return (coeff * (self.y1**ω - self.y0**ω)).call(jnp.asarray).ω
+        with jax.numpy_dtype_promotion("standard"):
+            if t1 is None:
+                coeff = linear_rescale(self.t0, t0, self.t1)
+                return (
+                    (self.y0**ω + coeff * (self.y1**ω - self.y0**ω)).call(jnp.asarray).ω
+                )
+            else:
+                coeff = (t1 - t0) / (self.t1 - self.t0)
+                return (coeff * (self.y1**ω - self.y0**ω)).call(jnp.asarray).ω
 
 
 class ThirdOrderHermitePolynomialInterpolation(AbstractLocalInterpolation):
     t0: RealScalarLike
     t1: RealScalarLike
     coeffs: PyTree[Shaped[Array, "4 ?*dims"], "Y"]
 
@@ -74,15 +82,16 @@
         del left
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
 
         t = linear_rescale(self.t0, t0, self.t1)
 
         def _eval(_coeffs):
-            return jnp.polyval(_coeffs, t)
+            with jax.numpy_dtype_promotion("standard"):
+                return jnp.polyval(_coeffs, t)
 
         return jtu.tree_map(_eval, self.coeffs)
 
 
 class FourthOrderPolynomialInterpolation(AbstractLocalInterpolation):
     t0: RealScalarLike
     t1: RealScalarLike
@@ -96,15 +105,16 @@
         t0: RealScalarLike,
         t1: RealScalarLike,
         y0: Y,
         y1: Y,
         k: PyTree[Shaped[Array, "order ?*y"], "Y"],
     ):
         def _calculate(_y0, _y1, _k):
-            _ymid = _y0 + jnp.tensordot(self.c_mid, _k, axes=1)
+            with jax.numpy_dtype_promotion("standard"):
+                _ymid = _y0 + jnp.tensordot(self.c_mid, _k, axes=1)
             _f0 = _k[0]
             _f1 = _k[-1]
             # TODO: rewrite as matrix-vector product?
             _a = 2 * (_f1 - _f0) - 8 * (_y1 + _y0) + 16 * _ymid
             _b = 5 * _f0 - 3 * _f1 + 18 * _y0 + 14 * _y1 - 32 * _ymid
             _c = _f1 - 4 * _f0 - 11 * _y0 - 5 * _y1 + 16 * _ymid
             return jnp.stack([_a, _b, _c, _f0, _y0])
@@ -119,10 +129,11 @@
         del left
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
 
         t = linear_rescale(self.t0, t0, self.t1)
 
         def _eval(_coeffs):
-            return jnp.polyval(_coeffs, t)
+            with jax.numpy_dtype_promotion("standard"):
+                return jnp.polyval(_coeffs, t)
 
         return jtu.tree_map(_eval, self.coeffs)
```

### Comparing `diffrax-0.5.0/diffrax/_misc.py` & `diffrax-0.5.1/diffrax/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     will apply. If `JAX_NUMPY_DTYPE_PROMOTION=strict` then we loosen from prohibiting
     all dtype casting, to still allowing upcasting.
     """
     x_dtype = jnp.result_type(x)
     target_dtype = jnp.result_type(array_for_dtype)
     with jax.numpy_dtype_promotion("standard"):
         promote_dtype = jnp.result_type(x_dtype, target_dtype)
-    config_value = jax.config.jax_numpy_dtype_promotion
+    config_value = jax.config.jax_numpy_dtype_promotion  # pyright: ignore
     if config_value == "strict":
         if target_dtype != promote_dtype:
             raise ValueError(
                 f"When `JAX_NUMPY_DTYPE_PROMOTION=strict`, then {x_name} must have "
                 f"a dtype that can be promoted to the dtype of {dtype_name}. "
                 f"However {x_name} had dtype {x_dtype} and {dtype_name} had dtype "
                 f"{target_dtype}."
```

### Comparing `diffrax-0.5.0/diffrax/_path.py` & `diffrax-0.5.1/diffrax/_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import abc
-from typing import Optional, TYPE_CHECKING
+from typing import Generic, Optional, TYPE_CHECKING, TypeVar
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 
 
 if TYPE_CHECKING:
     from typing import ClassVar as AbstractVar
 else:
     from equinox import AbstractVar
-from jaxtyping import Array, PyTree
 
-from ._custom_types import RealScalarLike
+from ._custom_types import Control, RealScalarLike
 
 
-class AbstractPath(eqx.Module):
+_Control = TypeVar("_Control", bound=Control)
+
+
+class AbstractPath(eqx.Module, Generic[_Control]):
     """Abstract base class for all paths.
 
     Every path has a start point `t0` and an end point `t1`. In between these values
     it is possible to `evaluate` the path, or (if it is differentiable, e.g. not
     Brownian motion) calculate its `derivative`.
 
     !!! example
@@ -44,15 +46,15 @@
 
     t0: AbstractVar[RealScalarLike]
     t1: AbstractVar[RealScalarLike]
 
     @abc.abstractmethod
     def evaluate(
         self, t0: RealScalarLike, t1: Optional[RealScalarLike] = None, left: bool = True
-    ) -> PyTree[Array]:
+    ) -> _Control:
         r"""Evaluate the path at any point in the interval $[t_0, t_1]$.
 
         **Arguments:**
 
         - `t0`: Any point in $[t_0, t_1]$ to evaluate the path at.
         - `t1`: If passed, then the increment from `t1` to `t0` is evaluated instead.
         - `left`: Across jump points: whether to treat the path as left-continuous
@@ -73,15 +75,15 @@
         The value of the path at `t0`.
 
         If `t1` is passed:
 
         The increment of the path between `t0` and `t1`.
         """
 
-    def derivative(self, t: RealScalarLike, left: bool = True) -> PyTree[Array]:
+    def derivative(self, t: RealScalarLike, left: bool = True) -> _Control:
         r"""Evaluate the derivative of the path. Essentially equivalent
         to `jax.jvp(self.evaluate, (t,), (jnp.ones_like(t),))` (and indeed this is its
         default implementation if no other is specified).
 
 
         **Arguments:**
```

### Comparing `diffrax-0.5.0/diffrax/_saveat.py` & `diffrax-0.5.1/diffrax/_saveat.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solution.py` & `diffrax-0.5.1/diffrax/_solution.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_term.py` & `diffrax-0.5.1/diffrax/_term.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from equinox.internal import ω
-from jaxtyping import Array, ArrayLike, PyTree, PyTreeDef
+from jaxtyping import ArrayLike, PyTree, PyTreeDef
 
 from ._custom_types import Args, Control, IntScalarLike, RealScalarLike, VF, Y
 from ._misc import upcast_or_raise
 from ._path import AbstractPath
 
 
-class AbstractTerm(eqx.Module):
+_VF = TypeVar("_VF", bound=VF)
+_Control = TypeVar("_Control", bound=Control)
+
+
+class AbstractTerm(eqx.Module, Generic[_VF, _Control]):
     r"""Abstract base class for all terms.
 
     Let $y$ solve some differential equation with vector field $f$ and control $x$.
 
     Let $y$ have PyTree structure $T$, let the output of the vector field have
     PyTree structure $S$, and let $x$ have PyTree structure $U$, Then
     $f : T \to S$ whilst the interaction $(f, x) \mapsto f \mathrm{d}x$ is a function
     $(S, U) \to T$.
     """
 
     @abc.abstractmethod
-    def vf(self, t: RealScalarLike, y: Y, args: Args) -> VF:
+    def vf(self, t: RealScalarLike, y: Y, args: Args) -> _VF:
         """The vector field.
 
         Represents a function $f(t, y(t), args)$.
 
         **Arguments:**
 
         - `t`: the integration time.
@@ -42,15 +46,15 @@
         **Returns:**
 
         A PyTree of structure $S$.
         """
         pass
 
     @abc.abstractmethod
-    def contr(self, t0: RealScalarLike, t1: RealScalarLike) -> Control:
+    def contr(self, t0: RealScalarLike, t1: RealScalarLike, **kwargs) -> _Control:
         r"""The control.
 
         Represents the $\mathrm{d}t$ in an ODE, or the $\mathrm{d}w(t)$ in an SDE, etc.
 
         Most numerical ODE solvers work by making a step of length
         $\Delta t = t_1 - t_0$. Likewise most numerical SDE solvers work by sampling
         some Brownian motion $\Delta w \sim \mathcal{N}(0, t_1 - t_0)$.
@@ -67,15 +71,15 @@
 
         A PyTree of structure $U$. For a control $x$ then the result should
         represent $x(t_1) - x(t_0)$.
         """
         pass
 
     @abc.abstractmethod
-    def prod(self, vf: VF, control: Control) -> Y:
+    def prod(self, vf: _VF, control: _Control) -> Y:
         r"""Determines the interaction between vector field and control.
 
         With a solution $y$ to a differential equation with vector field $f$ and
         control $x$, this computes $f(t, y(t), args) \Delta x(t)$ given
         $f(t, y(t), args)$ and $\Delta x(t)$.
 
         **Arguments:**
@@ -90,15 +94,15 @@
 
         !!! note
 
             This function must be bilinear.
         """
         pass
 
-    def vf_prod(self, t: RealScalarLike, y: Y, args: Args, control: Control) -> Y:
+    def vf_prod(self, t: RealScalarLike, y: Y, args: Args, control: _Control) -> Y:
         r"""The composition of [`diffrax.AbstractTerm.vf`][] and
         [`diffrax.AbstractTerm.prod`][].
 
         With a solution $y$ to a differential equation with vector field $f$ and
         control $x$, this computes $f(t, y(t), args) \Delta x(t)$ given $t$, $y(t)$,
         $args$, and $\Delta x(t)$.
 
@@ -151,15 +155,15 @@
         specific sense that it is cheaper to evaluate `vf_prod` twice than `vf` once.
 
         Some solvers use this to change their behaviour, so as to act more efficiently.
         """
         return False
 
 
-class ODETerm(AbstractTerm):
+class ODETerm(AbstractTerm[_VF, RealScalarLike]):
     r"""A term representing $f(t, y(t), args) \mathrm{d}t$. That is to say, the term
     appearing on the right hand side of an ODE, in which the control is time.
 
     `vector_field` should return some PyTree, with the same structure as the initial
     state `y0`, and with every leaf shape-broadcastable and dtype-upcastable to the
     equivalent leaf in `y0`.
 
@@ -168,17 +172,17 @@
         ```python
         vector_field = lambda t, y, args: -y
         ode_term = ODETerm(vector_field)
         diffeqsolve(ode_term, ...)
         ```
     """
 
-    vector_field: Callable[[RealScalarLike, Y, Args], VF]
+    vector_field: Callable[[RealScalarLike, Y, Args], _VF]
 
-    def vf(self, t: RealScalarLike, y: Y, args: Args) -> VF:
+    def vf(self, t: RealScalarLike, y: Y, args: Args) -> _VF:
         out = self.vector_field(t, y, args)
         if jtu.tree_structure(out) != jtu.tree_structure(y):
             raise ValueError(
                 "The vector field inside `ODETerm` must return a pytree with the "
                 "same structure as `y0`."
             )
 
@@ -190,18 +194,18 @@
                 "the vector field passed to `ODETerm`",
                 "the corresponding leaf of `y`",
             )
             return oi
 
         return jtu.tree_map(_broadcast_and_upcast, out, y)
 
-    def contr(self, t0: RealScalarLike, t1: RealScalarLike) -> RealScalarLike:
+    def contr(self, t0: RealScalarLike, t1: RealScalarLike, **kwargs) -> RealScalarLike:
         return t1 - t0
 
-    def prod(self, vf: VF, control: RealScalarLike) -> Y:
+    def prod(self, vf: _VF, control: RealScalarLike) -> Y:
         def _mul(v):
             c = upcast_or_raise(
                 control,
                 v,
                 "the output of `ODETerm.contr(...)`",
                 "the output of `ODETerm.vf(...)`",
             )
@@ -215,81 +219,88 @@
 - `vector_field`: A callable representing the vector field. This callable takes three
     arguments `(t, y, args)`. `t` is a scalar representing the integration time. `y` is
     the evolving state of the system. `args` are any static arguments as passed to
     [`diffrax.diffeqsolve`][].
 """
 
 
-class _CallableToPath(AbstractPath):
+class _CallableToPath(AbstractPath[_Control]):
     fn: Callable
 
     @property
     def t0(self):
         return -jnp.inf
 
     @property
     def t1(self):
         return jnp.inf
 
     def evaluate(
         self, t0: RealScalarLike, t1: Optional[RealScalarLike] = None, left: bool = True
-    ) -> PyTree[Array]:
+    ) -> _Control:
         return self.fn(t0, t1)
 
 
-def _callable_to_path(x):
+def _callable_to_path(
+    x: Union[
+        AbstractPath[_Control], Callable[[RealScalarLike, RealScalarLike], _Control]
+    ],
+) -> AbstractPath[_Control]:
     if isinstance(x, AbstractPath):
         return x
     else:
         return _CallableToPath(x)
 
 
 # vf: Shaped[Array, "*state *control"]
 # control: Shaped[Array, "*control"]
 # return: Shaped[Array, "*state"]
 def _prod(vf, control):
     return jnp.tensordot(vf, control, axes=jnp.ndim(control))
 
 
-class _ControlTerm(AbstractTerm):
-    vector_field: Callable[[RealScalarLike, Y, Args], VF]
-    control: Union[AbstractPath, Callable] = eqx.field(converter=_callable_to_path)
+class _AbstractControlTerm(AbstractTerm[_VF, _Control]):
+    vector_field: Callable[[RealScalarLike, Y, Args], _VF]
+    control: Union[
+        AbstractPath[_Control], Callable[[RealScalarLike, RealScalarLike], _Control]
+    ] = eqx.field(converter=_callable_to_path)  # pyright: ignore
 
     def vf(self, t: RealScalarLike, y: Y, args: Args) -> VF:
         return self.vector_field(t, y, args)
 
-    def contr(self, t0: RealScalarLike, t1: RealScalarLike) -> Control:
-        return self.control.evaluate(t0, t1)
+    def contr(self, t0: RealScalarLike, t1: RealScalarLike, **kwargs) -> _Control:
+        return self.control.evaluate(t0, t1, **kwargs)  # pyright: ignore
 
     def to_ode(self) -> ODETerm:
         r"""If the control is differentiable then $f(t, y(t), args) \mathrm{d}x(t)$
         may be thought of as an ODE as
 
         $f(t, y(t), args) \frac{\mathrm{d}x}{\mathrm{d}t}\mathrm{d}t$.
 
         This method converts this `ControlTerm` into the corresponding
         [`diffrax.ODETerm`][] in this way.
         """
         vector_field = _ControlToODE(self)
         return ODETerm(vector_field=vector_field)
 
 
-_ControlTerm.__init__.__doc__ = """**Arguments:**
+_AbstractControlTerm.__init__.__doc__ = """**Arguments:**
 
 - `vector_field`: A callable representing the vector field. This callable takes three
     arguments `(t, y, args)`. `t` is a scalar representing the integration time. `y` is
     the evolving state of the system. `args` are any static arguments as passed to
     [`diffrax.diffeqsolve`][].
-- `control`: A callable representing the control. Should have an `evaluate(t0, t1)`
-    method. If using [`diffrax.ControlTerm.to_ode`][] then it should have a
-    `derivative(t)` method.
+- `control`: The control. Should either be (A) a [`diffrax.AbstractPath`][], in which
+    case its `evaluate(t0, t1)` method will be used to give the increment of the control
+    over a time interval `[t0, t1]`, or (B) a callable `(t0, t1) -> increment`, which
+    returns the increment directly.
 """
 
 
-class ControlTerm(_ControlTerm):
+class ControlTerm(_AbstractControlTerm[_VF, _Control]):
     r"""A term representing the general case of $f(t, y(t), args) \mathrm{d}x(t)$, in
     which the vector field - control interaction is a matrix-vector product.
 
     `vector_field` and `control` should both return PyTrees, both with the same
     structure as the initial state `y0`. Every dimension of `control` is then
     contracted against the last dimensions of `vector_field`; that is to say if each
     leaf of `y0` has shape `(y1, ..., yN)`, and the corresponding leaf of `control`
@@ -319,19 +330,19 @@
         control = LinearInterpolation(ts, data)
         vector_field = lambda t, y, args: jnp.stack([y, y], axis=-1)
         cde_term = ControlTerm(vector_field, control)
         diffeqsolve(cde_term, ...)
         ```
     """
 
-    def prod(self, vf: VF, control: Control) -> Y:
+    def prod(self, vf: _VF, control: _Control) -> Y:
         return jtu.tree_map(_prod, vf, control)
 
 
-class WeaklyDiagonalControlTerm(_ControlTerm):
+class WeaklyDiagonalControlTerm(_AbstractControlTerm[_VF, _Control]):
     r"""A term representing the case of $f(t, y(t), args) \mathrm{d}x(t)$, in
     which the vector field - control interaction is a matrix-vector product, and the
     matrix is square and diagonal. In this case we may represent the matrix as a vector
     of just its diagonal elements. The matrix-vector product may be calculated by
     pointwise multiplying this vector with the control; this is more computationally
     efficient than writing out the full matrix and then doing a full matrix-vector
     product.
@@ -345,23 +356,24 @@
         Why "weakly" diagonal? Consider the matrix representation of the vector field,
         as a square diagonal matrix. In general, the (i,i)-th element may depending
         upon any of the values of `y`. It is only if the (i,i)-th element only depends
         upon the i-th element of `y` that the vector field is said to be "diagonal",
         without the "weak". (This stronger property is useful in some SDE solvers.)
     """
 
-    def prod(self, vf: VF, control: Control) -> Y:
-        return jtu.tree_map(operator.mul, vf, control)
+    def prod(self, vf: _VF, control: _Control) -> Y:
+        with jax.numpy_dtype_promotion("standard"):
+            return jtu.tree_map(operator.mul, vf, control)
 
 
 class _ControlToODE(eqx.Module):
-    control_term: _ControlTerm
+    control_term: _AbstractControlTerm
 
     def __call__(self, t: RealScalarLike, y: Y, args: Args) -> Y:
-        control = self.control_term.control.derivative(t)
+        control = self.control_term.control.derivative(t)  # pyright: ignore
         return self.control_term.vf_prod(t, y, args, control)
 
 
 def _sum(*x):
     return sum(x[1:], x[0])
 
 
@@ -396,17 +408,17 @@
         """
         self.terms = terms  # pyright: ignore
 
     def vf(self, t: RealScalarLike, y: Y, args: Args) -> tuple[PyTree[ArrayLike], ...]:
         return tuple(term.vf(t, y, args) for term in self.terms)
 
     def contr(
-        self, t0: RealScalarLike, t1: RealScalarLike
+        self, t0: RealScalarLike, t1: RealScalarLike, **kwargs
     ) -> tuple[PyTree[ArrayLike], ...]:
-        return tuple(term.contr(t0, t1) for term in self.terms)
+        return tuple(term.contr(t0, t1, **kwargs) for term in self.terms)
 
     def prod(
         self, vf: tuple[PyTree[ArrayLike], ...], control: tuple[PyTree[ArrayLike], ...]
     ) -> Y:
         out = [
             term.prod(vf_, control_)
             for term, vf_, control_ in zip(self.terms, vf, control)
@@ -432,31 +444,32 @@
         t1: RealScalarLike,
         y: Y,
         args: Args,
     ) -> bool:
         return any(term.is_vf_expensive(t0, t1, y, args) for term in self.terms)
 
 
-class WrapTerm(AbstractTerm):
-    term: AbstractTerm
+class WrapTerm(AbstractTerm[_VF, _Control]):
+    term: AbstractTerm[_VF, _Control]
     direction: IntScalarLike
 
-    def vf(self, t: RealScalarLike, y: Y, args: Args) -> VF:
+    def vf(self, t: RealScalarLike, y: Y, args: Args) -> _VF:
         t = t * self.direction
         return self.term.vf(t, y, args)
 
-    def contr(self, t0: RealScalarLike, t1: RealScalarLike) -> Control:
+    def contr(self, t0: RealScalarLike, t1: RealScalarLike, **kwargs) -> _Control:
         _t0 = jnp.where(self.direction == 1, t0, -t1)
         _t1 = jnp.where(self.direction == 1, t1, -t0)
-        return (self.direction * self.term.contr(_t0, _t1) ** ω).ω
+        return (self.direction * self.term.contr(_t0, _t1, **kwargs) ** ω).ω
 
-    def prod(self, vf: VF, control: Control) -> Y:
-        return self.term.prod(vf, control)
+    def prod(self, vf: _VF, control: _Control) -> Y:
+        with jax.numpy_dtype_promotion("standard"):
+            return self.term.prod(vf, control)
 
-    def vf_prod(self, t: RealScalarLike, y: Y, args: Args, control: Control) -> Y:
+    def vf_prod(self, t: RealScalarLike, y: Y, args: Args, control: _Control) -> Y:
         t = t * self.direction
         return self.term.vf_prod(t, y, args, control)
 
     def is_vf_expensive(
         self,
         t0: RealScalarLike,
         t1: RealScalarLike,
@@ -464,16 +477,16 @@
         args: Args,
     ) -> bool:
         _t0 = jnp.where(self.direction == 1, t0, -t1)
         _t1 = jnp.where(self.direction == 1, t1, -t0)
         return self.term.is_vf_expensive(_t0, _t1, y, args)
 
 
-class AdjointTerm(AbstractTerm):
-    term: AbstractTerm
+class AdjointTerm(AbstractTerm[_VF, _Control]):
+    term: AbstractTerm[_VF, _Control]
 
     def is_vf_expensive(
         self,
         t0: RealScalarLike,
         t1: RealScalarLike,
         y: tuple[
             PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike]
@@ -543,19 +556,19 @@
         if jtu.tree_structure(None) in (vf_prod_tree, control_tree):
             # An unusual/not-useful edge case to handle.
             raise NotImplementedError(
                 "`AdjointTerm.vf` not implemented for `None` controls or states."
             )
         return jtu.tree_transpose(vf_prod_tree, control_tree, jac)
 
-    def contr(self, t0: RealScalarLike, t1: RealScalarLike) -> PyTree[ArrayLike]:
-        return self.term.contr(t0, t1)
+    def contr(self, t0: RealScalarLike, t1: RealScalarLike, **kwargs) -> _Control:
+        return self.term.contr(t0, t1, **kwargs)
 
     def prod(
-        self, vf: PyTree[ArrayLike], control: Control
+        self, vf: PyTree[ArrayLike], control: _Control
     ) -> tuple[
         PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike]
     ]:
         # As per what is returned from `self.vf`, then `vf` has a PyTree structure of
         # (control_tree, vf_prod_tree)
 
         # Calculate vf_prod_tree by smuggling it out.
@@ -590,15 +603,15 @@
     def vf_prod(
         self,
         t: RealScalarLike,
         y: tuple[
             PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike]
         ],
         args: Args,
-        control: Control,
+        control: _Control,
     ) -> tuple[
         PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike], PyTree[ArrayLike]
     ]:
         # Note the inclusion of "implicit" parameters (as `term` might be a callable
         # PyTree a la Equinox) and "explicit" parameters (`args`)
         y, a_y, _, _ = y
         diff_args, nondiff_args = eqx.partition(args, eqx.is_inexact_array)
```

### Comparing `diffrax-0.5.0/diffrax/_brownian/base.py` & `diffrax-0.5.1/diffrax/_solver/midpoint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-import abc
-from typing import Optional, Union
+from collections.abc import Callable
+from typing import ClassVar
 
-from equinox.internal import AbstractVar
-from jaxtyping import Array, PyTree
+import numpy as np
 
-from .._custom_types import LevyArea, LevyVal, RealScalarLike
-from .._path import AbstractPath
+from .._local_interpolation import ThirdOrderHermitePolynomialInterpolation
+from .base import AbstractStratonovichSolver
+from .runge_kutta import AbstractERK, ButcherTableau
 
 
-class AbstractBrownianPath(AbstractPath):
-    """Abstract base class for all Brownian paths."""
+_midpoint_tableau = ButcherTableau(
+    a_lower=(np.array([0.5]),),
+    b_sol=np.array([0.0, 1.0]),
+    b_error=np.array([1.0, -1.0]),
+    c=np.array([0.5]),
+)
 
-    levy_area: AbstractVar[LevyArea]
 
-    @abc.abstractmethod
-    def evaluate(
-        self,
-        t0: RealScalarLike,
-        t1: Optional[RealScalarLike] = None,
-        left: bool = True,
-        use_levy: bool = False,
-    ) -> Union[PyTree[Array], LevyVal]:
-        r"""Samples a Brownian increment $w(t_1) - w(t_0)$.
+class Midpoint(AbstractERK, AbstractStratonovichSolver):
+    """Midpoint method.
 
-        Each increment has distribution $\mathcal{N}(0, t_1 - t_0)$.
+    2nd order explicit Runge--Kutta method. Has an embedded Euler method for adaptive
+    step sizing. Uses 2 stages. Uses 2nd order Hermite interpolation for dense/ts
+    output.
 
-        **Arguments:**
+    Also sometimes known as the "modified Euler method".
 
-        - `t0`: Any point in $[t_0, t_1]$ to evaluate the path at.
-        - `t1`: If passed, then the increment from `t1` to `t0` is evaluated instead.
-        - `left`: Ignored. (This determines whether to treat the path as
-            left-continuous or right-continuous at any jump points, but Brownian
-            motion has no jump points.)
-        - `use_levy`: If True, the return type will be a `LevyVal`, which contains
-            PyTrees of Brownian increments and their Levy areas.
+    When used to solve SDEs, converges to the Stratonovich solution.
+    """
 
-        **Returns:**
+    tableau: ClassVar[ButcherTableau] = _midpoint_tableau
+    interpolation_cls: ClassVar[
+        Callable[..., ThirdOrderHermitePolynomialInterpolation]
+    ] = ThirdOrderHermitePolynomialInterpolation.from_k
 
-        If `t1` is not passed:
+    def order(self, terms):
+        return 2
 
-        The value of the Brownian motion at `t0`.
-
-        If `t1` is passed:
-
-        The increment of the Brownian motion between `t0` and `t1`.
-        """
+    def strong_order(self, terms):
+        return 0.5
```

### Comparing `diffrax-0.5.0/diffrax/_brownian/path.py` & `diffrax-0.5.1/diffrax/_brownian/path.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,23 @@
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import jax.tree_util as jtu
 import lineax.internal as lxi
 from jaxtyping import Array, PRNGKeyArray, PyTree
+from lineax.internal import complex_to_real_dtype
 
-from .._custom_types import levy_tree_transpose, LevyArea, LevyVal, RealScalarLike
+from .._custom_types import (
+    AbstractBrownianIncrement,
+    BrownianIncrement,
+    levy_tree_transpose,
+    RealScalarLike,
+    SpaceTimeLevyArea,
+)
 from .._misc import (
     force_bitcast_convert_type,
     is_tuple_of_ints,
     split_by_tree,
 )
 from .base import AbstractBrownianPath
 
@@ -34,37 +41,47 @@
        floating-point arithmetic.)
 
     Internally this operates by just sampling a fresh normal random variable over every
     interval, ignoring the correlation between samples exhibited in true Brownian
     motion. Hence the restrictions above. (They describe the general case for which the
     correlation structure isn't needed.)
 
-    Depending on the `levy_area` argument, this can also be used to generate Levy area.
+    !!! info "Levy Area"
+
+        Can be initialised with `levy_area` set to `diffrax.BrownianIncrement`, or
+        `diffrax.SpaceTimeLevyArea`. If `levy_area=diffrax.SpaceTimeLevyArea`, then it
+        also computes space-time Lévy area `H`. This is an additional source of
+        randomness required for certain stochastic Runge--Kutta solvers; see
+        [`diffrax.AbstractSRK`][] for more information.
+
+        An error will be thrown during tracing if Lévy area is required but is not
+        available.
+
+        The choice here will impact the Brownian path, so even with the same key, the
+        trajectory will be different depending on the value of `levy_area`.
     """
 
     shape: PyTree[jax.ShapeDtypeStruct] = eqx.field(static=True)
-    levy_area: LevyArea = eqx.field(static=True)
+    levy_area: type[Union[BrownianIncrement, SpaceTimeLevyArea]] = eqx.field(
+        static=True
+    )
     key: PRNGKeyArray
 
     def __init__(
         self,
         shape: Union[tuple[int, ...], PyTree[jax.ShapeDtypeStruct]],
         key: PRNGKeyArray,
-        levy_area: LevyArea = "",
+        levy_area: type[Union[BrownianIncrement, SpaceTimeLevyArea]],
     ):
         self.shape = (
             jax.ShapeDtypeStruct(shape, lxi.default_floating_dtype())
             if is_tuple_of_ints(shape)
             else shape
         )
         self.key = key
-        if levy_area not in ["", "space-time"]:
-            raise ValueError(
-                f"levy_area must be one of '', 'space-time', but got {levy_area}."
-            )
         self.levy_area = levy_area
 
         if any(
             not jnp.issubdtype(x.dtype, jnp.inexact)
             for x in jtu.tree_leaves(self.shape)
         ):
             raise ValueError("UnsafeBrownianPath dtypes all have to be floating-point.")
@@ -80,15 +97,15 @@
     @eqx.filter_jit
     def evaluate(
         self,
         t0: RealScalarLike,
         t1: Optional[RealScalarLike] = None,
         left: bool = True,
         use_levy: bool = False,
-    ) -> Union[PyTree[Array], LevyVal]:
+    ) -> Union[PyTree[Array], AbstractBrownianIncrement]:
         del left
         if t1 is None:
             dtype = jnp.result_type(t0)
             t1 = t0
             t0 = jnp.array(0, dtype)
         else:
             with jax.numpy_dtype_promotion("standard"):
@@ -107,43 +124,44 @@
             lambda key, shape: self._evaluate_leaf(
                 t0, t1, key, shape, self.levy_area, use_levy
             ),
             key,
             self.shape,
         )
         if use_levy:
-            out = levy_tree_transpose(self.shape, self.levy_area, out)
-            assert isinstance(out, LevyVal)
+            out = levy_tree_transpose(self.shape, out)
+            assert isinstance(out, (BrownianIncrement, SpaceTimeLevyArea))
         return out
 
     @staticmethod
     def _evaluate_leaf(
         t0: RealScalarLike,
         t1: RealScalarLike,
         key,
         shape: jax.ShapeDtypeStruct,
-        levy_area: str,
+        levy_area: type[Union[BrownianIncrement, SpaceTimeLevyArea]],
         use_levy: bool,
     ):
         w_std = jnp.sqrt(t1 - t0).astype(shape.dtype)
+        w = jr.normal(key, shape.shape, shape.dtype) * w_std
+        dt = jnp.asarray(t1 - t0, dtype=complex_to_real_dtype(shape.dtype))
 
-        if levy_area == "space-time":
+        if levy_area is SpaceTimeLevyArea:
             key, key_hh = jr.split(key, 2)
             hh_std = w_std / math.sqrt(12)
             hh = jr.normal(key_hh, shape.shape, shape.dtype) * hh_std
-        elif levy_area == "":
-            hh = None
+            levy_val = SpaceTimeLevyArea(dt=dt, W=w, H=hh)
+        elif levy_area is BrownianIncrement:
+            levy_val = BrownianIncrement(dt=dt, W=w)
         else:
             assert False
-        w = jr.normal(key, shape.shape, shape.dtype) * w_std
 
         if use_levy:
-            return LevyVal(dt=t1 - t0, W=w, H=hh, bar_H=None, K=None, bar_K=None)
-        else:
-            return w
+            return levy_val
+        return w
 
 
 UnsafeBrownianPath.__init__.__doc__ = """
 **Arguments:**
 
 - `shape`: Should be a PyTree of `jax.ShapeDtypeStruct`s, representing the shape, 
     dtype, and PyTree structure of the output. For simplicity, `shape` can also just
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `diffrax-0.5.0/diffrax/_brownian/tree.py` & `diffrax-0.5.1/diffrax/_brownian/tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import math
-from typing import Literal, Optional, Union
+from typing import Literal, Optional, TypeVar, Union
 from typing_extensions import TypeAlias
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.random as jr
 import jax.tree_util as jtu
 import lineax.internal as lxi
-from jaxtyping import Array, Float, PRNGKeyArray, PyTree
+from jaxtyping import Array, Inexact, PRNGKeyArray, PyTree
+from lineax.internal import complex_to_real_dtype
 
 from .._custom_types import (
+    AbstractBrownianIncrement,
     BoolScalarLike,
+    BrownianIncrement,
     IntScalarLike,
     levy_tree_transpose,
-    LevyArea,
-    LevyVal,
     RealScalarLike,
+    SpaceTimeLevyArea,
 )
 from .._misc import (
     is_tuple_of_ints,
     linear_rescale,
     split_by_tree,
 )
 from .base import AbstractBrownianPath
@@ -49,57 +51,80 @@
 #   author = {Foster, James M.},
 #   year = {2020}
 # }
 # For more about space-time Levy area see Definition 4.2.1.
 # For the midpoint rule for generating space-time Levy area see Theorem 6.1.6.
 # For the general interpolation rule for space-time Levy area see Theorem 6.1.4.
 
-FloatDouble: TypeAlias = tuple[Float[Array, " *shape"], Float[Array, " *shape"]]
+FloatDouble: TypeAlias = tuple[Inexact[Array, " *shape"], Inexact[Array, " *shape"]]
 FloatTriple: TypeAlias = tuple[
-    Float[Array, " *shape"], Float[Array, " *shape"], Float[Array, " *shape"]
+    Inexact[Array, " *shape"], Inexact[Array, " *shape"], Inexact[Array, " *shape"]
 ]
 _Spline: TypeAlias = Literal["sqrt", "quad", "zero"]
+_BrownianReturn = TypeVar("_BrownianReturn", bound=AbstractBrownianIncrement)
 
 
 class _State(eqx.Module):
     level: IntScalarLike  # level of the tree
     s: RealScalarLike  # starting time of the interval
     w_s_u_su: FloatTriple  # W_s, W_u, W_{s,u}
     key: PRNGKeyArray
     bhh_s_u_su: Optional[FloatTriple]  # \bar{H}_s, _u, _{s,u}
     bkk_s_u_su: Optional[FloatTriple]  # \bar{K}_s, _u, _{s,u}
 
 
-def _levy_diff(x0: LevyVal, x1: LevyVal) -> LevyVal:
+def _levy_diff(_, x0: tuple, x1: tuple) -> AbstractBrownianIncrement:
     r"""Computes $(W_{s,u}, H_{s,u})$ from $(W_s, \bar{H}_{s,u})$ and
     $(W_u, \bar{H}_u)$, where $\bar{H}_u = u * H_u$.
 
     **Arguments:**
 
+    - `_`: unused, for the purposes of aligning the `jtu.tree_map`.
     - `x0`: `LevyVal` at time `s`.
     - `x1`: `LevyVal` at time `u`.
 
     **Returns:**
 
     `LevyVal(W_su, H_su)`
     """
 
-    su = jnp.asarray(x1.dt - x0.dt, dtype=x0.W.dtype)
-    w_su = x1.W - x0.W
-    if x0.H is None or x1.H is None:  # BM only case
-        return LevyVal(dt=su, W=w_su, H=None, bar_H=None, K=None, bar_K=None)
-
-    assert (x0.bar_H is not None) and (x1.bar_H is not None)
-    # if we are at this point levy_area == "space-time"
-    _su = jnp.where(jnp.abs(su) < jnp.finfo(su).eps, jnp.inf, su)
-    inverse_su = 1 / _su
-    u_bb_s = x1.dt * x0.W - x0.dt * x1.W
-    bhh_su = x1.bar_H - x0.bar_H - 0.5 * u_bb_s  # bhh_su = H_{s,u} * (u-s)
-    hh_su = inverse_su * bhh_su
-    return LevyVal(dt=su, W=w_su, H=hh_su, bar_H=None, K=None, bar_K=None)
+    if len(x0) == 2:  # BM only case
+        assert len(x1) == 2
+        dt0, w0 = x0
+        dt1, w1 = x1
+        su = jnp.asarray(dt1 - dt0, dtype=complex_to_real_dtype(w0.dtype))
+        return BrownianIncrement(dt=su, W=w1 - w0)
+
+    elif len(x0) == 4:  # space-time levy area case
+        assert len(x1) == 4
+        dt0, w0, hh0, bhh0 = x0
+        dt1, w1, hh1, bhh1 = x1
+
+        w_su = w1 - w0
+        su = jnp.asarray(dt1 - dt0, dtype=complex_to_real_dtype(w0.dtype))
+        _su = jnp.where(jnp.abs(su) < jnp.finfo(su).eps, jnp.inf, su)
+        inverse_su = 1 / _su
+        with jax.numpy_dtype_promotion("standard"):
+            u_bb_s = dt1 * w0 - dt0 * w1
+            bhh_su = bhh1 - bhh0 - 0.5 * u_bb_s  # bhh_su = H_{s,u} * (u-s)
+            hh_su = inverse_su * bhh_su
+        return SpaceTimeLevyArea(dt=su, W=w_su, H=hh_su)
+    else:
+        assert False
+
+
+def _make_levy_val(_, x: tuple) -> AbstractBrownianIncrement:
+    if len(x) == 2:
+        dt, w = x
+        return BrownianIncrement(dt=dt, W=w)
+    elif len(x) == 4:
+        dt, w, hh, bhh = x
+        return SpaceTimeLevyArea(dt=dt, W=w, H=hh)
+    else:
+        assert False
 
 
 def _split_interval(
     pred: BoolScalarLike, x_stu: FloatTriple, x_st_tu: FloatDouble
 ) -> FloatTriple:
     x_s, x_t, x_u = x_stu
     x_st, x_tu = x_st_tu
@@ -108,18 +133,27 @@
     x_su = jnp.where(pred, x_tu, x_st)
     return x_s, x_u, x_su
 
 
 class VirtualBrownianTree(AbstractBrownianPath):
     """Brownian simulation that discretises the interval `[t0, t1]` to tolerance `tol`.
 
-    Can be initialised with `levy_area` set to `""`, or `"space-time"`.
-    If `levy_area="space_time"`, then it also computes space-time Lévy area `H`.
-    This will impact the Brownian path, so even with the same key, the trajectory will
-    be different depending on the value of `levy_area`.
+    !!! info "Levy Area"
+
+        Can be initialised with `levy_area` set to `diffrax.BrownianIncrement`, or
+        `diffrax.SpaceTimeLevyArea`. If `levy_area=diffrax.SpaceTimeLevyArea`, then it
+        also computes space-time Lévy area `H`. This is an additional source of
+        randomness required for certain stochastic Runge--Kutta solvers; see
+        [`diffrax.AbstractSRK`][] for more information.
+
+        An error will be thrown during tracing if Lévy area is required but is not
+        available.
+
+        The choice here will impact the Brownian path, so even with the same key, the
+        trajectory will be different depending on the value of `levy_area`.
 
     ??? cite "Reference"
 
         Virtual Brownian trees were proposed in
         ```bibtex
         @article{li2020scalable,
           title={Scalable gradients for stochastic differential equations},
@@ -146,40 +180,39 @@
         an interpolation method which ensures the conditional 2nd moments are correct.
     """
 
     t0: RealScalarLike
     t1: RealScalarLike
     tol: RealScalarLike
     shape: PyTree[jax.ShapeDtypeStruct] = eqx.field(static=True)
-    levy_area: LevyArea = eqx.field(static=True)
+    levy_area: type[Union[BrownianIncrement, SpaceTimeLevyArea]] = eqx.field(
+        static=True
+    )
     key: PyTree[PRNGKeyArray]
     _spline: _Spline = eqx.field(static=True)
 
     @eqxi.doc_remove_args("_spline")
     def __init__(
         self,
         t0: RealScalarLike,
         t1: RealScalarLike,
         tol: RealScalarLike,
         shape: Union[tuple[int, ...], PyTree[jax.ShapeDtypeStruct]],
         key: PRNGKeyArray,
-        levy_area: LevyArea = "",
+        levy_area: type[
+            Union[BrownianIncrement, SpaceTimeLevyArea]
+        ] = BrownianIncrement,
         _spline: _Spline = "sqrt",
     ):
         (t0, t1) = eqx.error_if((t0, t1), t0 >= t1, "t0 must be strictly less than t1")
         self.t0 = t0
         self.t1 = t1
         # Since we rescale the interval to [0,1],
         # we need to rescale the tolerance too.
         self.tol = tol / (self.t1 - self.t0)
-
-        if levy_area not in ["", "space-time"]:
-            raise ValueError(
-                f"levy_area must be one of '', 'space-time', but got {levy_area}."
-            )
         self.levy_area = levy_area
         self._spline = _spline
         self.shape = (
             jax.ShapeDtypeStruct(shape, lxi.default_floating_dtype())
             if is_tuple_of_ints(shape)
             else shape
         )
@@ -188,101 +221,103 @@
             for x in jtu.tree_leaves(self.shape)
         ):
             raise ValueError(
                 "VirtualBrownianTree dtypes all have to be floating-point."
             )
         self.key = split_by_tree(key, self.shape)
 
-    def _denormalise_bm_inc(self, x: LevyVal) -> LevyVal:
+    def _denormalise_bm_inc(self, x: _BrownianReturn) -> _BrownianReturn:
         # Rescaling back from [0, 1] to the original interval [t0, t1].
         interval_len = self.t1 - self.t0  # can be any dtype
         sqrt_len = jnp.sqrt(interval_len)
 
         def mult(z):
             dtype = jnp.result_type(z)
             return jnp.astype(interval_len, dtype) * z
 
         def sqrt_mult(z):
             # need to cast to dtype of each leaf in PyTree
             dtype = jnp.result_type(z)
             return jnp.astype(sqrt_len, dtype) * z
 
-        return LevyVal(
-            dt=jtu.tree_map(mult, x.dt),
-            W=jtu.tree_map(sqrt_mult, x.W),
-            H=jtu.tree_map(sqrt_mult, x.H),
-            bar_H=None,
-            K=jtu.tree_map(sqrt_mult, x.K),
-            bar_K=None,
-        )
+        def is_dt(z):
+            return z is x.dt
+
+        dt, other = eqx.partition(x, is_dt)
+        dt_normalized = jtu.tree_map(mult, dt)
+        other_normalized = jtu.tree_map(sqrt_mult, other)
+        return eqx.combine(dt_normalized, other_normalized)
 
     @eqx.filter_jit
     def evaluate(
         self,
         t0: RealScalarLike,
         t1: Optional[RealScalarLike] = None,
         left: bool = True,
         use_levy: bool = False,
-    ) -> Union[PyTree[Array], LevyVal]:
-        def _is_levy_val(obj):
-            return isinstance(obj, LevyVal)
-
+    ) -> Union[PyTree[Array], AbstractBrownianIncrement]:
         t0 = eqxi.nondifferentiable(t0, name="t0")
         # map the interval [self.t0, self.t1] onto [0,1]
         t0 = linear_rescale(self.t0, t0, self.t1)
         levy_0 = self._evaluate(t0)
         if t1 is None:
             levy_out = levy_0
-
+            levy_out = jtu.tree_map(_make_levy_val, self.shape, levy_out)
         else:
             t1 = eqxi.nondifferentiable(t1, name="t1")
             # map the interval [self.t0, self.t1] onto [0,1]
             t1 = linear_rescale(self.t0, t1, self.t1)
             levy_1 = self._evaluate(t1)
-            levy_out = jtu.tree_map(_levy_diff, levy_0, levy_1, is_leaf=_is_levy_val)
+            levy_out = jtu.tree_map(_levy_diff, self.shape, levy_0, levy_1)
 
-        levy_out = levy_tree_transpose(self.shape, self.levy_area, levy_out)
+        levy_out = levy_tree_transpose(self.shape, levy_out)
         # now map [0,1] back onto [self.t0, self.t1]
         levy_out = self._denormalise_bm_inc(levy_out)
-        assert isinstance(levy_out, LevyVal)
+        assert isinstance(levy_out, (BrownianIncrement, SpaceTimeLevyArea))
         return levy_out if use_levy else levy_out.W
 
-    def _evaluate(self, r: RealScalarLike) -> PyTree[LevyVal]:
+    def _evaluate(self, r: RealScalarLike) -> PyTree:
         """Maps the _evaluate_leaf function at time r using self.key onto self.shape"""
         r = eqxi.error_if(
             r,
             (r < 0) | (r > 1),
             "Cannot evaluate VirtualBrownianTree outside of its range [t0, t1].",
         )
         map_func = lambda key, shape: self._evaluate_leaf(key, r, shape)
         return jtu.tree_map(map_func, self.key, self.shape)
 
     def _evaluate_leaf(
         self,
         key,
         r: RealScalarLike,
         struct: jax.ShapeDtypeStruct,
-    ) -> LevyVal:
+    ) -> Union[
+        tuple[RealScalarLike, Array], tuple[RealScalarLike, Array, Array, Array]
+    ]:
         shape, dtype = struct.shape, struct.dtype
+        tdtype = complex_to_real_dtype(dtype)
 
-        t0 = jnp.zeros((), dtype)
-        r = jnp.asarray(r, dtype)
+        t0 = jnp.zeros((), tdtype)
+        r = jnp.asarray(r, tdtype)
 
-        if self.levy_area == "space-time":
+        if self.levy_area is SpaceTimeLevyArea:
             state_key, init_key_w, init_key_la = jr.split(key, 3)
             bhh_1 = jr.normal(init_key_la, shape, dtype) / math.sqrt(12)
             bhh_0 = jnp.zeros_like(bhh_1)
             bhh = (bhh_0, bhh_1, bhh_1)
             bkk = None
 
-        else:
+        elif self.levy_area is BrownianIncrement:
             state_key, init_key_w = jr.split(key, 2)
             bhh = None
             bkk = None
 
+        else:
+            assert False
+
         w_0 = jnp.zeros(shape, dtype)
         w_1 = jr.normal(init_key_w, shape, dtype)
         w = (w_0, w_1, w_1)
 
         init_state = _State(
             level=0, s=t0, w_s_u_su=w, key=state_key, bhh_s_u_su=bhh, bkk_s_u_su=bkk
         )
@@ -309,21 +344,22 @@
             _level = _state.level + 1
             _cond = r > _t
             _s = jnp.where(_cond, _t, _state.s)
             _key_st, _key_tu = _keys
             _key = jnp.where(_cond, _key_st, _key_tu)
 
             _w = _split_interval(_cond, _w_stu, _w_inc)
-            if not self.levy_area == "":
+            _bkk = None
+            if self.levy_area is SpaceTimeLevyArea:
                 assert _bhh_stu is not None and _bhh_st_tu is not None
                 _bhh = _split_interval(_cond, _bhh_stu, _bhh_st_tu)
-                _bkk = None
-            else:
+            elif self.levy_area is BrownianIncrement:
                 _bhh = None
-                _bkk = None
+            else:
+                assert False
 
             return _State(
                 level=_level,
                 s=_s,
                 w_s_u_su=_w,
                 key=_key,
                 bhh_s_u_su=_bhh,
@@ -336,32 +372,15 @@
         su = 2.0**-final_state.level
 
         sr = jax.nn.relu(r - s)
         # make sure su = sr + ru regardless of cancellation error
         ru = jax.nn.relu(su - sr)
 
         w_s, w_u, w_su = final_state.w_s_u_su
-
-        # BM only case
-        if self.levy_area == "":
-            w_mean = w_s + sr / su * w_su
-            if self._spline == "sqrt":
-                z = jr.normal(final_state.key, shape, dtype)
-                bb = jnp.sqrt(sr * ru / su) * z
-            elif self._spline == "quad":
-                z = jr.normal(final_state.key, shape, dtype)
-                bb = (sr * ru / su) * z
-            elif self._spline == "zero":
-                bb = jnp.zeros(shape, dtype)
-            else:
-                assert False
-            w_r = w_mean + bb
-            return LevyVal(dt=r, W=w_r, H=None, bar_H=None, K=None, bar_K=None)
-
-        elif self.levy_area == "space-time":
+        if self.levy_area is SpaceTimeLevyArea:
             # This is based on Theorem 6.1.4 of Foster's thesis (see above).
 
             assert final_state.bhh_s_u_su is not None
             bhh_s, bhh_u, bhh_su = final_state.bhh_s_u_su
             sr3 = jnp.power(sr, 3)
             ru3 = jnp.power(ru, 3)
             su3 = jnp.power(su, 3)
@@ -373,37 +392,56 @@
                 x1 = jr.normal(key1, shape, dtype)
                 x2 = jr.normal(key2, shape, dtype)
             elif self._spline == "zero":
                 x1 = jnp.zeros(shape, dtype)
                 x2 = jnp.zeros(shape, dtype)
             else:
                 raise ValueError(
-                    f"When levy_area='space-time', only 'sqrt' and"
+                    f"When levy_area='SpaceTimeLevyArea', only 'sqrt' and"
                     f" 'zero' splines are permitted, got {self._spline}."
                 )
 
             sr_ru_half = jnp.sqrt(sr * ru)
             d = jnp.sqrt(sr3 + ru3)
             d_prime = 1 / (2 * su * d)
             a = d_prime * sr3 * sr_ru_half
             b = d_prime * ru3 * sr_ru_half
 
-            w_sr = sr / su * w_su + 6 * sr * ru / su3 * bhh_su + 2 * (a + b) / su * x1
-            w_r = w_s + w_sr
-            c = jnp.sqrt(3 * sr3 * ru3) / (6 * d)
-            bhh_sr = sr3 / su3 * bhh_su - a * x1 + c * x2
-            bhh_r = bhh_s + bhh_sr + 0.5 * (r * w_s - s * w_r)
-
-            inverse_r = 1 / jnp.where(jnp.abs(r) < jnp.finfo(r).eps, jnp.inf, r)
-            hh_r = inverse_r * bhh_r
+            with jax.numpy_dtype_promotion("standard"):
+                w_sr = (
+                    sr / su * w_su + 6 * sr * ru / su3 * bhh_su + 2 * (a + b) / su * x1
+                )
+                w_r = w_s + w_sr
+                c = jnp.sqrt(3 * sr3 * ru3) / (6 * d)
+                bhh_sr = sr3 / su3 * bhh_su - a * x1 + c * x2
+                bhh_r = bhh_s + bhh_sr + 0.5 * (r * w_s - s * w_r)
+
+                inverse_r = 1 / jnp.where(jnp.abs(r) < jnp.finfo(r).eps, jnp.inf, r)
+                hh_r = inverse_r * bhh_r
+
+        elif self.levy_area is BrownianIncrement:
+            with jax.numpy_dtype_promotion("standard"):
+                w_mean = w_s + sr / su * w_su
+                if self._spline == "sqrt":
+                    z = jr.normal(final_state.key, shape, dtype)
+                    bb = jnp.sqrt(sr * ru / su) * z
+                elif self._spline == "quad":
+                    z = jr.normal(final_state.key, shape, dtype)
+                    bb = (sr * ru / su) * z
+                elif self._spline == "zero":
+                    bb = jnp.zeros(shape, dtype)
+                else:
+                    assert False
+            w_r = w_mean + bb
+            return r, w_r
 
         else:
             assert False
 
-        return LevyVal(dt=r, W=w_r, H=hh_r, bar_H=bhh_r, K=None, bar_K=None)
+        return r, w_r, hh_r, bhh_r
 
     def _brownian_arch(
         self, _state: _State, shape, dtype
     ) -> tuple[
         RealScalarLike,
         FloatTriple,
         FloatDouble,
@@ -446,15 +484,15 @@
         st = su / 2
         s = _state.s
         t = s + st
         root_su = jnp.sqrt(su)
 
         w_s, w_u, w_su = _state.w_s_u_su
 
-        if self.levy_area == "space-time":
+        if self.levy_area is SpaceTimeLevyArea:
             assert _state.bhh_s_u_su is not None
             assert _state.bkk_s_u_su is None
             bhh_s, bhh_u, bhh_su = _state.bhh_s_u_su
 
             z1_key, z2_key = jr.split(midpoint_key, 2)
             z1 = jr.normal(z1_key, shape, dtype)
             z2 = jr.normal(z2_key, shape, dtype)
@@ -471,25 +509,29 @@
             bhh_term2 = su / 4 * n
             bhh_st = bhh_term1 + bhh_term2
             bhh_tu = bhh_term1 - bhh_term2
             bhh_st_tu = (bhh_st, bhh_tu)
 
             w_t = w_s + w_st
             w_stu = (w_s, w_t, w_u)
-
-            bhh_t = bhh_s + bhh_st + 0.5 * (t * w_s - s * w_t)
+            with jax.numpy_dtype_promotion("standard"):
+                bhh_t = bhh_s + bhh_st + 0.5 * (t * w_s - s * w_t)
             bhh_stu = (bhh_s, bhh_t, bhh_u)
             bkk_stu = None
             bkk_st_tu = None
 
-        else:
+        elif self.levy_area is BrownianIncrement:
             assert _state.bhh_s_u_su is None
             assert _state.bkk_s_u_su is None
             mean = 0.5 * w_su
             w_term2 = root_su / 2 * jr.normal(midpoint_key, shape, dtype)
             w_st = mean + w_term2
             w_tu = mean - w_term2
             w_st_tu = (w_st, w_tu)
             w_t = w_s + w_st
             w_stu = (w_s, w_t, w_u)
             bhh_stu, bhh_st_tu, bkk_stu, bkk_st_tu = None, None, None, None
+
+        else:
+            assert False
+
         return t, w_stu, w_st_tu, keys, bhh_stu, bhh_st_tu, bkk_stu, bkk_st_tu
```

### Comparing `diffrax-0.5.0/diffrax/_root_finder/_verychord.py` & `diffrax-0.5.1/diffrax/_root_finder/_verychord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from collections.abc import Callable
-from typing import Any
+from typing import Any, cast
 
 import equinox as eqx
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import lineax as lx
 import lineax.internal as lxi
 import optimistix as optx
 from equinox.internal import ω
 from jaxtyping import Array, Bool, PyTree, Scalar
+from lineax.internal import complex_to_real_dtype
 
 from .._custom_types import Y
 
 
+ω = cast(Callable, ω)
+
+
 def _small(diffsize: Scalar) -> Bool[Array, ""]:
     # TODO(kidger): make a more careful choice here -- the existence of this
     # function is pretty ad-hoc.
     resolution = 10 ** (2 - jnp.finfo(diffsize.dtype).precision)
     return diffsize < resolution
 
 
@@ -87,22 +91,23 @@
             init_later_state = self.linear_solver.init(jac, options={})
             dynamic, static = eqx.partition(init_later_state, eqx.is_array)
             dynamic = lax.stop_gradient(dynamic)
             init_later_state = eqx.combine(dynamic, static)
             linear_state = (jac, init_later_state)
             y_leaves = jtu.tree_leaves(y)
             if len(y_leaves) == 0:
-                y_dtype = lxi.default_floating_dtype()  # pyright: ignore
+                y_dtype = lxi.default_floating_dtype()
             else:
                 y_dtype = jnp.result_type(*y_leaves)
+            diff_dtype = complex_to_real_dtype(y_dtype)
             init_state = _VeryChordState(
                 linear_state=linear_state,
                 diff=jtu.tree_map(lambda x: jnp.full(x.shape, jnp.inf, x.dtype), y),
-                diffsize=jnp.array(jnp.inf, dtype=y_dtype),
-                diffsize_prev=jnp.array(1.0, dtype=y_dtype),
+                diffsize=jnp.array(jnp.inf, dtype=diff_dtype),
+                diffsize_prev=jnp.array(1.0, dtype=diff_dtype),
                 result=optx.RESULTS.successful,
                 step=jnp.array(0),
             )
         else:
             assert isinstance(init_state, _VeryChordState)
         return init_state
 
@@ -120,16 +125,18 @@
         jac, linear_state = state.linear_state
         linear_state = lax.stop_gradient(linear_state)
         sol = lx.linear_solve(
             jac, fx, self.linear_solver, state=linear_state, throw=False
         )
         diff = sol.value
         new_y = (y**ω - diff**ω).ω
-        scale = (self.atol + self.rtol * ω(new_y).call(jnp.abs)).ω
-        diffsize = self.norm((diff**ω / scale**ω).ω)
+
+        with jax.numpy_dtype_promotion("standard"):
+            scale = (self.atol + self.rtol * ω(new_y).call(jnp.abs)).ω
+            diffsize = self.norm((diff**ω / scale**ω).ω)
         new_state = _VeryChordState(
             linear_state=state.linear_state,
             diff=diff,
             diffsize=diffsize,
             diffsize_prev=state.diffsize,
             result=optx.RESULTS.promote(sol.result),
             step=state.step + 1,
```

### Comparing `diffrax-0.5.0/diffrax/_root_finder/_with_tols.py` & `diffrax-0.5.1/diffrax/_root_finder/_with_tols.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/__init__.py` & `diffrax-0.5.1/diffrax/_solver/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,10 +34,20 @@
     AbstractESDIRK as AbstractESDIRK,
     AbstractRungeKutta as AbstractRungeKutta,
     AbstractSDIRK as AbstractSDIRK,
     ButcherTableau as ButcherTableau,
     CalculateJacobian as CalculateJacobian,
     MultiButcherTableau as MultiButcherTableau,
 )
+from .sea import SEA as SEA
 from .semi_implicit_euler import SemiImplicitEuler as SemiImplicitEuler
+from .shark import ShARK as ShARK
+from .shark_general import GeneralShARK as GeneralShARK
 from .sil3 import Sil3 as Sil3
+from .slowrk import SlowRK as SlowRK
+from .spark import SPaRK as SPaRK
+from .sra1 import SRA1 as SRA1
+from .srk import (
+    AbstractSRK as AbstractSRK,
+    StochasticButcherTableau as StochasticButcherTableau,
+)
 from .tsit5 import Tsit5 as Tsit5
```

### Comparing `diffrax-0.5.0/diffrax/_solver/base.py` & `diffrax-0.5.1/diffrax/_solver/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 import abc
 from collections.abc import Callable
-from typing import Generic, Optional, Type, TYPE_CHECKING, TypeVar
+from typing import (
+    Any,
+    ClassVar,
+    Generic,
+    get_args,
+    get_origin,
+    Optional,
+    Type,
+    TYPE_CHECKING,
+    TypeVar,
+)
 
 import equinox as eqx
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import optimistix as optx
 
@@ -16,23 +26,23 @@
 from equinox.internal import ω
 from jaxtyping import PyTree
 
 from .._custom_types import Args, BoolScalarLike, DenseInfo, RealScalarLike, VF, Y
 from .._heuristics import is_sde
 from .._local_interpolation import AbstractLocalInterpolation
 from .._solution import RESULTS, update_result
-from .._term import AbstractTerm
+from .._term import AbstractTerm, MultiTerm
 
 
 _SolverState = TypeVar("_SolverState")
 
 
 def vector_tree_dot(a, b):
     return jtu.tree_map(
-        lambda bi: jnp.tensordot(a, bi, axes=1, precision=lax.Precision.HIGHEST),  # pyright: ignore
+        lambda bi: jnp.tensordot(a, bi, axes=1, precision=lax.Precision.HIGHEST),
         b,
     )
 
 
 class _MetaAbstractSolver(type(eqx.Module), type):
     def __instancecheck__(cls, obj):
         if super(_MetaAbstractSolver, AbstractWrappedSolver).__instancecheck__(obj):  # pyright: ignore
@@ -45,26 +55,43 @@
 
 
 # Sneak the metaclass past pyright, as otherwise it disables the dataclass-ness of
 # `eqx.Module`.
 _set_metaclass = dict(metaclass=_MetaAbstractSolver)
 
 
+def _term_compatible_contr_kwargs(term_structure):
+    origin = get_origin(term_structure)
+    if origin is MultiTerm:
+        [terms] = get_args(term_structure)
+        return tuple(_term_compatible_contr_kwargs(term) for term in get_args(terms))
+    if origin is not None:
+        term_structure = origin
+    if isinstance(term_structure, type) and issubclass(term_structure, AbstractTerm):
+        return {}
+    return jtu.tree_map(_term_compatible_contr_kwargs, term_structure)
+
+
 class AbstractSolver(eqx.Module, Generic[_SolverState], **_set_metaclass):
     """Abstract base class for all differential equation solvers.
 
     Subclasses should have a class-level attribute `terms`, specifying the PyTree
     structure of `terms` in `diffeqsolve(terms, ...)`.
     """
 
     # What PyTree structure `terms` should have when used with this solver.
     term_structure: AbstractClassVar[PyTree[Type[AbstractTerm]]]
     # How to interpolate the solution in between steps.
     interpolation_cls: AbstractClassVar[Callable[..., AbstractLocalInterpolation]]
 
+    # Any keyword arguments needed in `_term_compatible` in `_integrate.py`.
+    term_compatible_contr_kwargs: ClassVar[PyTree[dict[str, Any]]] = property(
+        lambda self: _term_compatible_contr_kwargs(self.term_structure)
+    )
+
     def order(self, terms: PyTree[AbstractTerm]) -> Optional[int]:
         """Order of the solver for solving ODEs."""
         return None
 
     def strong_order(self, terms: PyTree[AbstractTerm]) -> Optional[RealScalarLike]:
         """Strong order of the solver for solving SDEs."""
         return None
@@ -246,14 +273,18 @@
     def term_structure(self):
         return self.solver.term_structure
 
     @property
     def interpolation_cls(self):  # pyright: ignore
         return self.solver.interpolation_cls
 
+    @property
+    def term_compatible_contr_kwargs(self):
+        return self.solver.term_compatible_contr_kwargs
+
     def order(self, terms: PyTree[AbstractTerm]) -> Optional[int]:
         return self.solver.order(terms)
 
     def strong_order(self, terms: PyTree[AbstractTerm]) -> Optional[RealScalarLike]:
         return self.solver.strong_order(terms)
 
     def error_order(self, terms: PyTree[AbstractTerm]) -> Optional[RealScalarLike]:
```

### Comparing `diffrax-0.5.0/diffrax/_solver/bosh3.py` & `diffrax-0.5.1/diffrax/_solver/bosh3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/dopri5.py` & `diffrax-0.5.1/diffrax/_solver/dopri5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/dopri8.py` & `diffrax-0.5.1/diffrax/_solver/dopri8.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,16 @@
         self, t0: RealScalarLike, t1: Optional[RealScalarLike] = None, left: bool = True
     ) -> Y:
         del left
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
         t = linear_rescale(self.t0, t0, self.t1)
         coeffs = _vmap_polyval(jnp.asarray(self.eval_coeffs, dtype=t.dtype), t) * t
-        return (self.y0**ω + vector_tree_dot(coeffs, self.k) ** ω).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (self.y0**ω + vector_tree_dot(coeffs, self.k) ** ω).ω
 
 
 class Dopri8(AbstractERK):
     """Dormand--Prince's 8/7 method.
 
     8th order Runge--Kutta method. Has an embedded 7th order method for adaptive step
     sizing. Uses 14 stages with FSAL. Uses 8th order interpolation for dense/ts output.
```

### Comparing `diffrax-0.5.0/diffrax/_solver/euler.py` & `diffrax-0.5.1/diffrax/_solver/euler.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/euler_heun.py` & `diffrax-0.5.1/diffrax/_solver/euler_heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/heun.py` & `diffrax-0.5.1/diffrax/_solver/heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/implicit_euler.py` & `diffrax-0.5.1/diffrax/_solver/implicit_euler.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/kencarp3.py` & `diffrax-0.5.1/diffrax/_solver/kencarp3.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,16 @@
         if t1 is not None:
             return self.evaluate(t1) - self.evaluate(t0)
 
         t = linear_rescale(self.t0, t0, self.t1)
         explicit_k, implicit_k = self.k
         k = (explicit_k**ω + implicit_k**ω).ω
         coeffs = t * jax.vmap(lambda row: jnp.polyval(row, t))(self.coeffs)
-        return (self.y0**ω + vector_tree_dot(coeffs, k) ** ω).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (self.y0**ω + vector_tree_dot(coeffs, k) ** ω).ω
 
 
 class _KenCarp3Interpolation(KenCarpInterpolation):
     coeffs = np.array(
         [
             [-215264564351 / 13552729205753, 4655552711362 / 22874653954995],
             [17870216137069 / 13817060693119, -18682724506714 / 9892148508045],
```

### Comparing `diffrax-0.5.0/diffrax/_solver/kencarp4.py` & `diffrax-0.5.1/diffrax/_solver/kencarp4.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/kencarp5.py` & `diffrax-0.5.1/diffrax/_solver/kencarp5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/kvaerno3.py` & `diffrax-0.5.1/diffrax/_solver/kvaerno3.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/kvaerno4.py` & `diffrax-0.5.1/diffrax/_solver/kvaerno4.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/kvaerno5.py` & `diffrax-0.5.1/diffrax/_solver/kvaerno5.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/leapfrog_midpoint.py` & `diffrax-0.5.1/diffrax/_solver/leapfrog_midpoint.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/milstein.py` & `diffrax-0.5.1/diffrax/_solver/milstein.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     term_structure: ClassVar = MultiTerm[tuple[ODETerm, AbstractTerm]]
     interpolation_cls: ClassVar[
         Callable[..., LocalLinearInterpolation]
     ] = LocalLinearInterpolation
 
     def order(self, terms):
-        raise ValueError("`StratonovichMilstein` should not used to solve ODEs.")
+        raise ValueError("`StratonovichMilstein` should not be used to solve ODEs.")
 
     def strong_order(self, terms):
         return 1  # assuming commutative noise
 
     def init(
         self,
         terms: MultiTerm[tuple[ODETerm, AbstractTerm]],
@@ -118,15 +118,15 @@
 
     term_structure: ClassVar = MultiTerm[tuple[ODETerm, AbstractTerm]]
     interpolation_cls: ClassVar[
         Callable[..., LocalLinearInterpolation]
     ] = LocalLinearInterpolation
 
     def order(self, terms):
-        raise ValueError("`ItoMilstein` should not used to solve ODEs.")
+        raise ValueError("`ItoMilstein` should not be used to solve ODEs.")
 
     def strong_order(self, terms):
         return 1  # assuming commutative noise
 
     def init(
         self,
         terms: MultiTerm[tuple[ODETerm, AbstractTerm]],
@@ -210,15 +210,16 @@
         leaves_Δw, tree_Δw = jtu.tree_flatten(Δw)
         leaves_ΔwΔw = []
         for i1, l1 in enumerate(leaves_Δw):
             for i2, l2 in enumerate(leaves_Δw):
                 leaf = jnp.tensordot(l1[..., None], l2[None, ...], axes=1)
                 if i1 == i2:
                     eye = jnp.eye(l1.size).reshape(l1.shape + l1.shape)
-                    leaf = leaf - Δt * eye
+                    with jax.numpy_dtype_promotion("standard"):
+                        leaf = leaf - Δt * eye
                 leaves_ΔwΔw.append(leaf)
         tree_ΔwΔw = tree_Δw.compose(tree_Δw)
         ΔwΔw = jtu.tree_unflatten(tree_ΔwΔw, leaves_ΔwΔw)
         # ΔwΔw has structure (tree(Δw), tree(Δw), leaf(Δw), leaf(Δw))
 
         #
         # Next we construct g0_{k j1} g0_{i j2, k}.
@@ -232,15 +233,17 @@
             # _out has structure (tree(g0), leaf(g0))
             return _out
 
         def _to_vmap(_g0):
             # _g0 has structure (tree(y0), leaf(y0))
             _, _jvp = jax.jvp(_to_vjp, (y0,), (_g0,))
             # jvp has structure (tree(g0), leaf(g0))
-            _jvp_matrix = jax.jacfwd(lambda _Δw: diffusion.prod(_jvp, _Δw))(Δw)
+            _jvp_matrix = jax.jacfwd(
+                lambda _Δw: diffusion.prod(_jvp, _Δw), holomorphic=jnp.iscomplexobj(Δw)
+            )(Δw)
             # _jvp_matrix has structure (tree(y0), tree(Δw), leaf(y0), leaf(Δw))
             return _jvp_matrix
 
         # Aha! A new complexity.
         #
         # So the structure (tree(g0), leaf(g0)) is isomorphic to the structure
         # (tree(y0), tree(Δw), leaf(y0), leaf(Δw)).
@@ -278,15 +281,17 @@
             # _out has structure (tree(y0), tree(Δw), leaf(y0), leaf(Δw), leaf(Δw))
             return out
 
         y_treedef = jtu.tree_structure(y0)
         Δw_treedef = jtu.tree_structure(Δw)
         # g0 has structure (tree(g0), leaf(g0))
         # Which we now transform into its isomorphic matrix form, as above.
-        g0_matrix = jax.jacfwd(lambda _Δw: diffusion.prod(g0, _Δw))(Δw)
+        g0_matrix = jax.jacfwd(
+            lambda _Δw: diffusion.prod(g0, _Δw), holomorphic=jnp.iscomplexobj(Δw)
+        )(Δw)
         # g0_matrix has structure (tree(y0), tree(Δw), leaf(y0), leaf(Δw))
         g0_matrix = jtu.tree_transpose(y_treedef, Δw_treedef, g0_matrix)
         # g0_matrix has structure (tree(Δw), tree(y0), leaf(y0), leaf(Δw))
         v0_matrix = jtu.tree_map(_to_treemap, Δw, g0_matrix)
         # v0_matrix has structure (tree(Δw), tree(y0), tree(Δw), leaf(y0), leaf(Δw), leaf(Δw))  # noqa: E501
         v0_matrix = jtu.tree_transpose(
             Δw_treedef, y_treedef.compose(Δw_treedef), v0_matrix
```

### Comparing `diffrax-0.5.0/diffrax/_solver/ralston.py` & `diffrax-0.5.1/diffrax/_solver/ralston.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/reversible_heun.py` & `diffrax-0.5.1/diffrax/_solver/reversible_heun.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/runge_kutta.py` & `diffrax-0.5.1/diffrax/_solver/runge_kutta.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
         # (We could maybe implement a variable-length matvec by using a while loop --
         # not clear that that would necessarily get good performance though. Not
         # benchmarked.)
         #
 
         y0_leaves = jtu.tree_leaves(y0)
         if len(y0_leaves) == 0:
-            tableau_dtype = lxi.default_floating_dtype()  # pyright: ignore
+            tableau_dtype = lxi.default_floating_dtype()
         else:
             tableau_dtype = jnp.result_type(*y0_leaves)
 
         def embed_a_lower(tab):
             tab_a_lower = np.zeros(
                 (num_stages, num_stages), dtype=np.result_type(*tab.a_lower)
             )
@@ -803,15 +803,15 @@
 
         if implicit_tableau is not None:
             implicit_diagonal = jnp.asarray(
                 implicit_tableau.a_diagonal, dtype=tableau_dtype
             )
             implicit_predictor = np.zeros(
                 (num_stages, num_stages),
-                dtype=np.result_type(*implicit_tableau.a_predictor),  # pyright: ignore
+                dtype=np.result_type(*implicit_tableau.a_predictor),
             )
             for i, a_predictor_i in enumerate(implicit_tableau.a_predictor):  # pyright: ignore
                 implicit_predictor[i + 1, : i + 1] = a_predictor_i
             implicit_predictor = jnp.asarray(implicit_predictor, dtype=tableau_dtype)
             implicit_c = get_implicit(tableaus_c)
 
         if implicit_term is None:
```

### Comparing `diffrax-0.5.0/diffrax/_solver/semi_implicit_euler.py` & `diffrax-0.5.1/diffrax/_solver/semi_implicit_euler.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_solver/sil3.py` & `diffrax-0.5.1/diffrax/_solver/sil3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import ClassVar
+from collections.abc import Callable
+from typing import cast, ClassVar
 
 import numpy as np
 import optimistix as optx
 from equinox.internal import ω
 
 from .._local_interpolation import ThirdOrderHermitePolynomialInterpolation
 from .._root_finder import VeryChord, with_stepsize_controller_tols
@@ -11,14 +12,17 @@
     AbstractRungeKutta,
     ButcherTableau,
     CalculateJacobian,
     MultiButcherTableau,
 )
 
 
+ω = cast(Callable, ω)
+
+
 # See
 # https://docs.kidger.site/diffrax/devdocs/predictor_dirk/
 # for the construction of the a_predictor tableau, which is new here.
 _implicit_tableau = ButcherTableau(
     a_lower=(
         np.array([1 / 6]),
         np.array([1 / 3, 0]),
```

### Comparing `diffrax-0.5.0/diffrax/_solver/tsit5.py` & `diffrax-0.5.1/diffrax/_solver/tsit5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections.abc import Callable
 from typing import ClassVar, Optional
 
+import jax
 import jax.numpy as jnp
 import numpy as np
 from equinox.internal import ω
 from jaxtyping import Array, PyTree, Shaped
 
 from .._custom_types import RealScalarLike, Y
 from .._local_interpolation import AbstractLocalInterpolation
@@ -143,18 +144,19 @@
             47.37952196281928122
             * (t - 1.203071208372362603)
             * (t - 0.658047292653547382)
             * t**2
         )
         b6 = -34.87065786149660974 * (t - 1.2) * (t - 0.666666666666666667) * t**2
         b7 = 2.5 * (t - 1) * (t - 0.6) * t**2
-        return (
-            self.y0**ω
-            + vector_tree_dot(jnp.stack([b1, b2, b3, b4, b5, b6, b7]), self.k) ** ω
-        ).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (
+                self.y0**ω
+                + vector_tree_dot(jnp.stack([b1, b2, b3, b4, b5, b6, b7]), self.k) ** ω
+            ).ω
 
 
 class Tsit5(AbstractERK):
     r"""Tsitouras' 5/4 method.
 
     5th order explicit Runge--Kutta method. Has an embedded 4th order method for
     adaptive step sizing. Uses 7 stages with FSAL. Uses 5th order interpolation
```

### Comparing `diffrax-0.5.0/diffrax/_step_size_controller/adaptive.py` & `diffrax-0.5.1/diffrax/_step_size_controller/adaptive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 import typing
 from collections.abc import Callable
 from typing import cast, Optional, TYPE_CHECKING, TypeVar
 
 import equinox as eqx
 import equinox.internal as eqxi
+import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import lineax.internal as lxi
 import optimistix as optx
 from jaxtyping import Real
 
 
 if TYPE_CHECKING:
     from typing import ClassVar as AbstractVar
 else:
     from equinox import AbstractVar
 from equinox.internal import ω
 from jaxtyping import Array, PyTree
+from lineax.internal import complex_to_real_dtype
 
 from .._custom_types import (
     Args,
     BoolScalarLike,
     IntScalarLike,
     RealScalarLike,
     VF,
     Y,
 )
-from .._misc import upcast_or_raise
+from .._misc import static_select, upcast_or_raise
 from .._solution import RESULTS
 from .._term import AbstractTerm, ODETerm
 from .base import AbstractStepSizeController
 
 
+ω = cast(Callable, ω)
+
+
 def _select_initial_step(
     terms: PyTree[AbstractTerm],
     t0: RealScalarLike,
     y0: Y,
     args: Args,
     func: Callable[
         [PyTree[AbstractTerm], RealScalarLike, Y, Args],
@@ -175,14 +180,47 @@
 
         (Note that technically speaking, the meaning of `rtol` and `atol` is entirely
         dependent on the choice of `solver`. In practice however, most solvers tend to
         provide similar behaviour for similar values of `rtol`, `atol`. As such it is
         common to refer to solving an equation to specific tolerances, without
         necessarily stating which solver was used.)
 
+        ??? Example
+
+            The choice of `rtol` and `atol` can have a significant impact on the
+            accuracy of even simple systems.
+            Consider a simple pendulum with a small angle kick:
+            ```python
+            import diffrax as dfx
+
+            def dynamics(t, y, args):
+                dtheta = y["omega"]
+                domega = - jnp.sin(y["theta"])
+                return dict(theta=dtheta, omega=domega)
+
+            y0 = dict(theta=0.1, omega=0)
+            term = dfx.ODETerm(dynamics)
+            sol = dfx.diffeqsolve(
+                term, solver, t0=0, t1=1000, dt0=0.1, y0,
+                saveat=dfx.SaveAts(ts=jnp.linspace(0, 1000, 10000),
+                max_steps=2**20,
+                stepsize_controller=...
+            )
+            ```
+            to compare the effect of different tolerances:
+            ```python
+            PID_controller_incorrect = diffrax.PIDController(rtol=1e-3, atol=1e-6)
+            PID_controller_correct = diffrax.PIDController(rtol=1e-7, atol=1e-9)
+            Constant_controller = diffrax.ConstantStepSize()
+            ```
+            The phase portraits of the pendulum from the different tolerances clearly
+            illustrate the impact of the choice of `rtol` and `atol` on the accuracy of
+            the solution.
+            ![Phase portrait of pendulum](../imgs/pendulum_adaptive_steps.png)
+
     ??? tip "Choosing PID coefficients"
 
         This controller can be reduced to any special case (e.g. just a PI controller,
         or just an I controller) by setting `pcoeff`, `icoeff` or `dcoeff` to zero
         as appropriate.
 
         For smoothly-varying (i.e. easy to solve) problems then an I controller, or a
@@ -213,14 +251,15 @@
         coefficients subject to `pcoeff>=0.2`, `icoeff>=0.3`, `pcoeff + icoeff <= 0.7`.
         You can check the number of steps made via:
         ```python
         sol = diffeqsolve(...)
         print(sol.stats["num_steps"])
         ```
 
+
     ??? cite "References"
 
         Both the initial step size selection algorithm for ODEs, and the use of
         an I controller for ODEs, are from Section II.4 of:
 
         ```bibtex
         @book{hairer2008solving-i,
@@ -412,23 +451,23 @@
             dt0 = jnp.maximum(dt0, self.dtmin)
 
         t1 = self._clip_step_ts(t0, t0 + dt0)
         t1, jump_next_step = self._clip_jump_ts(t0, t1)
 
         y_leaves = jtu.tree_leaves(y0)
         if len(y_leaves) == 0:
-            y_dtype = lxi.default_floating_dtype()  # pyright: ignore
+            y_dtype = lxi.default_floating_dtype()
         else:
             y_dtype = jnp.result_type(*y_leaves)
         return t1, (
             jump_next_step,
             at_dtmin,
             dt0,
-            jnp.array(1.0, dtype=y_dtype),
-            jnp.array(1.0, dtype=y_dtype),
+            jnp.array(1.0, dtype=complex_to_real_dtype(y_dtype)),
+            jnp.array(1.0, dtype=complex_to_real_dtype(y_dtype)),
         )
 
     def adapt_step_size(
         self,
         t0: RealScalarLike,
         t1: RealScalarLike,
         y0: Y,
@@ -528,15 +567,16 @@
 
         def _scale(_y0, _y1_candidate, _y_error):
             # In case the solver steps into a region for which the vector field isn't
             # defined.
             _nan = jnp.isnan(_y1_candidate).any()
             _y1_candidate = jnp.where(_nan, _y0, _y1_candidate)
             _y = jnp.maximum(jnp.abs(_y0), jnp.abs(_y1_candidate))
-            return _y_error / (self.atol + _y * self.rtol)
+            with jax.numpy_dtype_promotion("standard"):
+                return _y_error / (self.atol + _y * self.rtol)
 
         scaled_error = self.norm(jtu.tree_map(_scale, y0, y1_candidate, y_error))
         keep_step = scaled_error < 1
         if self.dtmin is not None:
             keep_step = keep_step | at_dtmin
         # Make sure it's not a Python scalar and thus getting a ZeroDivisionError.
         inv_scaled_error = 1 / jnp.asarray(scaled_error)
@@ -566,15 +606,15 @@
             a_max=self.factormax,
         )
         # Once again, see above. In case we have gradients on {i,p,d}coeff.
         # (Probably quite common for them to have zero tangents if passed across
         # a grad API boundary as part of a larger model.)
         factor = lax.stop_gradient(factor)
         factor = eqxi.nondifferentiable(factor)
-        dt = prev_dt * factor
+        dt = prev_dt * factor.astype(prev_dt)
 
         # E.g. we failed an implicit step, so y_error=inf, so inv_scaled_error=0,
         # so factor=factormin, and we shrunk our step.
         # If we're using a PI or PID controller we shouldn't then force shrinking on
         # the next or next two steps as well!
         pred = (inv_scaled_error == 0) | jnp.isinf(inv_scaled_error)
         inv_scaled_error = jnp.where(pred, 1, inv_scaled_error)
@@ -600,15 +640,15 @@
 
         if jnp.issubdtype(jnp.result_type(t1), jnp.inexact):
             # Two nextafters. If made_jump then t1 = prevbefore(jump location)
             # so now _t1 = nextafter(jump location)
             # This is important because we don't know whether or not the jump is as a
             # result of a left- or right-discontinuity, so we have to skip the jump
             # location altogether.
-            _t1 = jnp.where(made_jump, eqxi.nextafter(eqxi.nextafter(t1)), t1)
+            _t1 = static_select(made_jump, eqxi.nextafter(eqxi.nextafter(t1)), t1)
         else:
             _t1 = t1
         next_t0 = jnp.where(keep_step, _t1, t0)
         next_t1 = self._clip_step_ts(next_t0, next_t0 + dt)
         next_t1, next_made_jump = self._clip_jump_ts(next_t0, next_t1)
 
         inv_scaled_error = jnp.where(keep_step, inv_scaled_error, prev_inv_scaled_error)
```

### Comparing `diffrax-0.5.0/diffrax/_step_size_controller/base.py` & `diffrax-0.5.1/diffrax/_step_size_controller/base.py`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/diffrax/_step_size_controller/constant.py` & `diffrax-0.5.1/diffrax/_step_size_controller/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self,
         t0: RealScalarLike,
         t1: RealScalarLike,
         y0: Y,
         y1_candidate: Y,
         args: Args,
         y_error: Optional[Y],
-        error_order: RealScalarLike,
+        error_order: Optional[RealScalarLike],
         controller_state: RealScalarLike,
     ) -> tuple[bool, RealScalarLike, RealScalarLike, bool, RealScalarLike, RESULTS]:
         del t0, y0, y1_candidate, args, y_error, error_order
         return (
             True,
             t1,
             t1 + controller_state,
```

### Comparing `diffrax-0.5.0/LICENSE` & `diffrax-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffrax-0.5.0/README.md` & `diffrax-0.5.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -57,28 +57,25 @@
 }
 ```
 
 (Also consider starring the project on GitHub.)
 
 ## See also: other libraries in the JAX ecosystem
 
-[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
+**Always useful**  
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks and everything not already in core JAX!  
+[jaxtyping](https://github.com/patrick-kidger/jaxtyping): type annotations for shape/dtype of arrays.  
+
+**Deep learning**  
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.  
+[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).  
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).  
+
+**Scientific computing**  
+[Optimistix](https://github.com/patrick-kidger/optimistix): root finding, minimisation, fixed points, and least squares.  
+[Lineax](https://github.com/patrick-kidger/lineax): linear solvers.  
+[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.  
+[sympy2jax](https://github.com/patrick-kidger/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.  
+[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)  
 
-[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
-
-[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
-
-[Optimistix](https://github.com/patrick-kidger/optimistix): root finding, minimisation, fixed points, and least squares.
-
-[Lineax](https://github.com/google/lineax): linear solvers.
-
-[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.
-
-[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).
-
-[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
-
-[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
-
-[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
-
-[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)
+**Awesome JAX**  
+[Awesome JAX](https://github.com/n2cholas/awesome-jax): a longer list of other JAX projects.
```

### Comparing `diffrax-0.5.0/PKG-INFO` & `diffrax-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: diffrax
-Version: 0.5.0
+Version: 0.5.1
 Summary: GPU+autodiff-capable ODE/SDE/CDE solvers written in JAX.
 Project-URL: repository, https://github.com/patrick-kidger/diffrax
 Author-email: Patrick Kidger <contact@kidger.site>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,18 +216,19 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: ~=3.9
 Requires-Dist: equinox>=0.11.2
-Requires-Dist: jax>=0.4.18
+Requires-Dist: jax>=0.4.23
 Requires-Dist: jaxtyping>=0.2.24
-Requires-Dist: lineax>=0.0.4
-Requires-Dist: optimistix>=0.0.6
+Requires-Dist: lineax>=0.0.5
+Requires-Dist: optimistix>=0.0.7
+Requires-Dist: typeguard==2.13.3
 Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
 
 <h1 align='center'>Diffrax</h1>
 <h2 align='center'>Numerical differential equation solvers in JAX. Autodifferentiable and GPU-capable.</h2>
 
 Diffrax is a [JAX](https://github.com/google/jax)-based library providing numerical differential equation solvers.
@@ -286,28 +287,25 @@
 }
 ```
 
 (Also consider starring the project on GitHub.)
 
 ## See also: other libraries in the JAX ecosystem
 
-[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
+**Always useful**  
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks and everything not already in core JAX!  
+[jaxtyping](https://github.com/patrick-kidger/jaxtyping): type annotations for shape/dtype of arrays.  
+
+**Deep learning**  
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.  
+[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).  
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).  
+
+**Scientific computing**  
+[Optimistix](https://github.com/patrick-kidger/optimistix): root finding, minimisation, fixed points, and least squares.  
+[Lineax](https://github.com/patrick-kidger/lineax): linear solvers.  
+[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.  
+[sympy2jax](https://github.com/patrick-kidger/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.  
+[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)  
 
-[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
-
-[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
-
-[Optimistix](https://github.com/patrick-kidger/optimistix): root finding, minimisation, fixed points, and least squares.
-
-[Lineax](https://github.com/google/lineax): linear solvers.
-
-[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.
-
-[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).
-
-[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
-
-[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
-
-[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
-
-[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)
+**Awesome JAX**  
+[Awesome JAX](https://github.com/n2cholas/awesome-jax): a longer list of other JAX projects.
```

