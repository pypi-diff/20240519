# Comparing `tmp/apygee-1.0.3.tar.gz` & `tmp/apygee-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apygee-1.0.3.tar", max compression
+gzip compressed data, was "apygee-1.0.4.tar", max compression
```

## Comparing `apygee-1.0.3.tar` & `apygee-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1060 2024-05-17 19:22:34.520795 apygee-1.0.3/LICENSE.md
--rw-r--r--   0        0        0    11402 2024-05-17 19:22:34.520795 apygee-1.0.3/README.md
--rw-r--r--   0        0        0      555 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/__init__.py
--rw-r--r--   0        0        0     4014 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/constants.py
--rw-r--r--   0        0        0    10159 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/kepler.py
--rw-r--r--   0        0        0     2863 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/nb.py
--rw-r--r--   0        0        0    37115 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/orbit.py
--rw-r--r--   0        0        0    19714 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/plot.py
--rw-r--r--   0        0        0     6262 2024-05-17 19:22:34.520795 apygee-1.0.3/apygee/utils.py
--rw-r--r--   0        0        0      734 2024-05-17 19:22:34.528795 apygee-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    11967 1970-01-01 00:00:00.000000 apygee-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-19 14:12:12.650635 apygee-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0    11387 2024-05-19 14:12:12.650635 apygee-1.0.4/README.md
+-rw-r--r--   0        0        0      555 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/__init__.py
+-rw-r--r--   0        0        0     4033 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/constants.py
+-rw-r--r--   0        0        0    10178 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/kepler.py
+-rw-r--r--   0        0        0    37363 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/orbit.py
+-rw-r--r--   0        0        0    19837 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/plot.py
+-rw-r--r--   0        0        0     6270 2024-05-19 14:12:12.650635 apygee-1.0.4/apygee/utils.py
+-rw-r--r--   0        0        0      734 2024-05-19 14:12:12.670635 apygee-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11952 1970-01-01 00:00:00.000000 apygee-1.0.4/PKG-INFO
```

### Comparing `apygee-1.0.3/LICENSE.md` & `apygee-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apygee-1.0.3/README.md` & `apygee-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Apygee
 
 <p align="start">
   <a href="https://github.com/Pocket-titan/apygee">
-    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.jpg" alt="Logo" width="200">
+    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.png" alt="Logo" height="200px">
   </a>
 </p>
 
 Apygee (apogee + `py`) is a lightweight Python package for creating, manipulating and visualizing Kepler orbits.
 
 ## Installation
 
@@ -102,28 +102,28 @@
 
 
 
 ![png](https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/examples_5_0.png)
 
 
 
-### Visualize an orbit (requires plotly)
+### Visualize an orbit
 
 
 
 ```python
 from apygee import Orbit, MU_EARTH
 
 orbit = Orbit([2e6], mu=MU_EARTH)
 orbit.visualize()
 ```
 
 
 
-<img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/orbitvis.png" alt="Orbit visualization" width="400px" />
+<img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/orbitvis.gif" alt="Orbit visualization" width="400px" />
 
 
 
 ### Hohmann transfer from Earth to Mars
```

### Comparing `apygee-1.0.3/apygee/__init__.py` & `apygee-1.0.4/apygee/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from apygee.kepler import cart_to_kep, kep_to_cart, sphere_of_influence
 from apygee.constants import (
-    MU_SUN,
-    MU_MERCURY,
+    EARTH,
+    JUPITER,
+    MARS,
+    MERCURY,
     MU_EARTH,
-    MU_MARS,
     MU_JUPITER,
+    MU_MARS,
+    MU_MERCURY,
+    MU_NEPTUNE,
     MU_SATURN,
+    MU_SUN,
     MU_URANUS,
-    MU_NEPTUNE,
-    MERCURY,
-    VENUS,
-    EARTH,
-    MARS,
-    JUPITER,
+    NEPTUNE,
     SATURN,
     URANUS,
-    NEPTUNE,
+    VENUS,
 )
+from apygee.kepler import cart_to_kep, kep_to_cart, sphere_of_influence
 from apygee.orbit import Orbit
 from apygee.plot import (
     plot_angle,
     plot_angle_2d,
     plot_angle_3d,
     plot_vector,
     plot_vector_2d,
```

### Comparing `apygee-1.0.3/apygee/constants.py` & `apygee-1.0.4/apygee/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # [2] https://ssd.jpl.nasa.gov/planets/phys_par.html
 # [3] https://nssdc.gsfc.nasa.gov/planetary/factsheet/moonfact.html
 # [4] https://nssdc.gsfc.nasa.gov/planetary/factsheet/sunfact.html
 # [5] https://www.iau.org/static/resolutions/IAU2012_English.pdf
 # [6] de Pater, I., & Lissauer, J. J. (2015). Planetary Sciences (2nd ed.). Cambridge: Cambridge University Press.
 # [7] https://ssd.jpl.nasa.gov/horizons/app.html#/
 
-from apygee.orbit import Orbit
 import numpy as np
 
+from apygee.orbit import Orbit
+
 G = 6.67428e-11  # [m^3 kg^-1 s^-2] [1]
 
 AU = 149_597_870_700  # [m] [5]
 
 M_SUN = 1_988_500e24  # [kg] [4]
 R_SUN = 695_700e3  # [m] [4]
 MU_SUN = G * M_SUN
@@ -22,15 +23,17 @@
 R_MERCURY = 2439.4e3  # [m] [2]
 MU_MERCURY = G * M_MERCURY
 A_MERCURY = 0.38709880 * AU  # [m] [6]
 E_MERCURY = 0.20563175  # [6]
 I_MERCURY = np.deg2rad(7.00499)  # [rad] [6]
 OMEGA_MERCURY = np.deg2rad(48.3309)  # [rad] [6]
 LOMEGA_MERCURY = np.deg2rad(77.4561)  # [rad] [6]
-MERCURY = Orbit([A_MERCURY, E_MERCURY, I_MERCURY, LOMEGA_MERCURY, OMEGA_MERCURY], mu=MU_SUN)
+MERCURY = Orbit(
+    [A_MERCURY, E_MERCURY, I_MERCURY, LOMEGA_MERCURY, OMEGA_MERCURY], mu=MU_SUN
+)
 
 M_VENUS = 4.86731e24  # [kg] [2]
 R_VENUS = 6051.8e3  # [m] [2]
 MU_VENUS = G * M_VENUS
 A_VENUS = 0.72333201 * AU  # [m] [6]
 E_VENUS = 0.00677177  # [6]
 I_VENUS = np.deg2rad(3.39447)  # [6]
@@ -72,15 +75,17 @@
 R_JUPITER = 69911e3  # [m] [2]
 MU_JUPITER = G * M_JUPITER
 A_JUPITER = 5.2027584 * AU  # [m] [6]
 E_JUPITER = 0.048495  # [6]
 I_JUPITER = np.deg2rad(1.3033)  # [6]
 OMEGA_JUPITER = np.deg2rad(100.464)  # [6]
 LOMEGA_JUPITER = np.deg2rad(14.331)  # [6]
-JUPITER = Orbit([A_JUPITER, E_JUPITER, I_JUPITER, LOMEGA_JUPITER, OMEGA_JUPITER], mu=MU_SUN)
+JUPITER = Orbit(
+    [A_JUPITER, E_JUPITER, I_JUPITER, LOMEGA_JUPITER, OMEGA_JUPITER], mu=MU_SUN
+)
 
 M_SATURN = 568.317e24  # [kg] [2]
 R_SATURN = 58232e3  # [m] [2]
 MU_SATURN = G * M_SATURN
 A_SATURN = 9.5428244 * AU  # [m] [6]
 E_SATURN = 0.055509  # [6]
 I_SATURN = np.deg2rad(2.4889)  # [6]
@@ -102,8 +107,10 @@
 R_NEPTUNE = 24622e3  # [m] [2]
 MU_NEPTUNE = G * M_NEPTUNE
 A_NEPTUNE = 30.06893 * AU  # [m] [6]
 E_NEPTUNE = 0.00899  # [6]
 I_NEPTUNE = np.deg2rad(1.770)  # [6]
 OMEGA_NEPTUNE = np.deg2rad(131.78)  # [6]
 LOMEGA_NEPTUNE = np.deg2rad(48.12)  # [6]
-NEPTUNE = Orbit([A_NEPTUNE, E_NEPTUNE, I_NEPTUNE, LOMEGA_NEPTUNE, OMEGA_NEPTUNE], mu=MU_SUN)
+NEPTUNE = Orbit(
+    [A_NEPTUNE, E_NEPTUNE, I_NEPTUNE, LOMEGA_NEPTUNE, OMEGA_NEPTUNE], mu=MU_SUN
+)
```

### Comparing `apygee-1.0.3/apygee/kepler.py` & `apygee-1.0.4/apygee/kepler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from numpy.typing import ArrayLike
 
-from apygee.utils import dot
 import numpy as np
 
+from apygee.utils import dot
+
 
 def kep_to_cart(kep: ArrayLike, mu: float | ArrayLike) -> np.ndarray:
     """
     Parameters
     ----------
     kep : array_like
         keplerian elements: [a, e, i, Ω, ω, θ]
@@ -193,15 +194,17 @@
     return np.sqrt(mu * a * (1 - e**2))
 
 
 def parabolic_angular_momentum(a: float, mu: float) -> float:
     return np.sqrt(mu * np.abs(a))  # p = a, not p = 2 * a
 
 
-def specific_orbital_energy(r: float | ArrayLike, v: float | ArrayLike, mu: float) -> float:
+def specific_orbital_energy(
+    r: float | ArrayLike, v: float | ArrayLike, mu: float
+) -> float:
     if not isinstance(r, (int, float)):
         r = np.asarray(r, dtype=np.float64).reshape((-1, 3))
         r = np.linalg.norm(r, axis=-1)
     if not isinstance(v, (int, float)):
         v = np.asarray(v, dtype=np.float64).reshape((-1, 3))
         v = np.linalg.norm(v, axis=-1)
 
@@ -232,15 +235,17 @@
     return np.sqrt(-mu / a**3)
 
 
 def mean_anomaly(n: float, t: float, tau: float = 0.0) -> float:
     return n * (t - tau)
 
 
-def eccentric_anomaly(M: float, e: float, atol: float = 1e-9, max_iter: int = 1000) -> float:
+def eccentric_anomaly(
+    M: float, e: float, atol: float = 1e-9, max_iter: int = 1000
+) -> float:
     converged = False
     E = M
     i = 0
 
     while i < max_iter:
         E_new = M + e * np.sin(E)
 
@@ -267,15 +272,17 @@
     return theta
 
 
 def M_from_E(E: float, e: float) -> float:
     return E - e * np.sin(E)
 
 
-def hyperbolic_anomaly(M: float, e: float, atol: float = 1e-9, max_iter: int = 1000) -> float:
+def hyperbolic_anomaly(
+    M: float, e: float, atol: float = 1e-9, max_iter: int = 1000
+) -> float:
     """
     Newton iteration
     """
     converged = False
     F = M
     i = 0
```

### Comparing `apygee-1.0.3/apygee/orbit.py` & `apygee-1.0.4/apygee/orbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Literal, Self
 from numpy.typing import ArrayLike
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from apygee.plot import plot_vector, plot_angle
 from apygee.kepler import (
     E_from_theta,
     F_from_theta,
     M_from_E,
     M_from_F,
     barkers_equation,
     cart_to_kep,
@@ -23,26 +22,27 @@
     orbital_plane,
     orbital_velocity,
     t_from_M,
     t_from_M_parabolic,
     theta_from_E,
     theta_from_F,
 )
+from apygee.plot import plot_angle, plot_vector
 from apygee.utils import (
     angle_between,
     darken,
     deep_diff,
     deep_update,
     flatten,
     lighten,
+    maybe_unwrap,
     omit,
-    scale_vector,
     rotate_vector,
+    scale_vector,
     shorten_fstring_number,
-    maybe_unwrap,
 )
 
 
 class Orbit:
     """
     A class that represents a Keplerian orbit.
 
@@ -260,26 +260,36 @@
         if Delta < 0:
             return False
 
         rp = (A + np.sqrt(Delta)) / B
         rm = (A - np.sqrt(Delta)) / B
 
         if not (
-            ((a1 * (1 - e1) <= rp <= a1 * (1 + e1)) or (a2 * (1 - e2) <= rp <= a2 * (1 + e2)))
-            and ((a1 * (1 - e1) <= rm <= a1 * (1 + e1)) or (a2 * (1 - e2) <= rm <= a2 * (1 + e2)))
+            (
+                (a1 * (1 - e1) <= rp <= a1 * (1 + e1))
+                or (a2 * (1 - e2) <= rp <= a2 * (1 + e2))
+            )
+            and (
+                (a1 * (1 - e1) <= rm <= a1 * (1 + e1))
+                or (a2 * (1 - e2) <= rm <= a2 * (1 + e2))
+            )
         ):
             return False
 
         cp = (a1 * (1 - e1**2) - rp) / (rp * e1)
-        sp = (a2 * (1 - e2**2) - rp) / (rp * e2) * (1 / np.sin(domega)) - cp * (1 / np.tan(domega))
+        sp = (a2 * (1 - e2**2) - rp) / (rp * e2) * (1 / np.sin(domega)) - cp * (
+            1 / np.tan(domega)
+        )
 
         print(np.sin(domega), np.tan(domega))
 
         cm = (a1 * (1 - e1**2) - rm) / (rm * e1)
-        sm = (a2 * (1 - e2**2) - rm) / (rm * e2) * (1 / np.sin(domega)) - cm * (1 / np.tan(domega))
+        sm = (a2 * (1 - e2**2) - rm) / (rm * e2) * (1 / np.sin(domega)) - cm * (
+            1 / np.tan(domega)
+        )
 
         return (rp * np.array([cp, sp, 0]), rp * np.array([cm, sm, 0]))
 
     def isclose(self, orbit: Self) -> bool:
         """
         Returns whether the orbits current position in space `isclose` to the given orbit's position in space.
 
@@ -620,18 +630,22 @@
         if not np.isclose(self.i, [0, np.pi]).any():
             asc_node = _self.at_theta(-_self.omega).r_vec
 
             if _map["n"]:
                 plot_vector(asc_node, text=label_map["n"], **vkwargs)
 
             if _map["i"] and is_3d:
-                plot_angle(z_dir, h_dir, text=label_map["i"], radius=angle_radius, **akwargs)
+                plot_angle(
+                    z_dir, h_dir, text=label_map["i"], radius=angle_radius, **akwargs
+                )
 
             if _map["omega"] and not np.isclose(_self.omega, [0, np.pi]).any():
-                plot_angle(asc_node, r_p, text=label_map["omega"], radius=angle_radius, **akwargs)
+                plot_angle(
+                    asc_node, r_p, text=label_map["omega"], radius=angle_radius, **akwargs
+                )
 
             if _map["Omega"] and not np.isclose(_self.Omega, [0, 2 * np.pi]).any():
                 ref_in_plane = rotate_vector(x_dir, asc_node, _self.i)
                 x_theta = angle_between(r_p, ref_in_plane)
                 x_dir = rotate_vector(_self.at_theta(x_theta).r_vec, asc_node, -_self.i)
                 plot_angle(
                     x_dir,
@@ -700,20 +714,20 @@
         kwargs : dict, optional
             additional keyword arguments to pass to ?
         """
         import plotly.express as px
         import plotly.graph_objects as go
         from IPython.display import display
         from ipywidgets import (
-            interactive_output,
             FloatSlider,
             GridBox,
             IntSlider,
             Label,
             Layout,
+            interactive_output,
         )
 
         colors = [
             "#66C2A5",
             "#FC8D62",
             "#8DA0CB",
             "#E78AC3",
@@ -869,15 +883,17 @@
                 theta=theta,
             ),
         )
 
         display(ui, fig)
 
     # Transfer methods
-    def impulsive_shot(self, dv: float | ArrayLike, x: float = None, theta: float = None) -> Self:
+    def impulsive_shot(
+        self, dv: float | ArrayLike, x: float = None, theta: float = None
+    ) -> Self:
         """
         Perform an impulsive shot maneuver. This is an idealized maneuver where the delta-v is applied instantaneously.
 
         Parameters
         ----------
         dv : float or array_like
             delta-v vector. if a scalar, `x` must be provided
@@ -911,15 +927,17 @@
             if x is not None:
                 print("Warning: x is ignored if dv is a vector")
 
             dv = np.asarray(dv).ravel()
             assert dv.size == 3, "dv must be a 3d vector"
             v1 = v0 + dv
 
-        return Orbit.from_cart(np.concatenate([self.at_theta(theta).r_vec, v1]), mu=self.mu)
+        return Orbit.from_cart(
+            np.concatenate([self.at_theta(theta).r_vec, v1]), mu=self.mu
+        )
 
     def coplanar_transfer(self, orbit: Self, theta_dep: float, theta_arr: float) -> Self:
         """
         If `theta_arr` > `theta_dep`, the transfer orbit is prograde. Otherwise, it's retrograde.
         Example: setting `theta_dep` to π and `theta_arr` to 0 will result in a *retrograde* transfer orbit.
         Setting `theta_dep` to π and `theta_arr` to 2π will result in a *prograde* transfer orbit.
```

### Comparing `apygee-1.0.3/apygee/plot.py` & `apygee-1.0.4/apygee/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Unpack, TypedDict
+from typing import TypedDict, Unpack
 from numpy.typing import ArrayLike
 
 import matplotlib.pyplot as plt
 import numpy as np
-
 from matplotlib.colors import to_rgba
-from mpl_toolkits.mplot3d.art3d import Patch3D
 from matplotlib.patches import Arc, FancyArrowPatch
 from matplotlib.transforms import Bbox, IdentityTransform, TransformedBbox
+from mpl_toolkits.mplot3d.art3d import Patch3D
 from mpl_toolkits.mplot3d.proj3d import proj_transform
 
 from apygee.utils import mix_colors, omit
 
 
 def plot_dummy_line(pts: ArrayLike, ax=None):
     """Expands limits so `pts` is in view, and returns the next color in the cycle"""
@@ -216,17 +215,23 @@
         ax.plot(*(origin + np.stack([[0, 0, v[2]], [0, v[1], v[2]]])).T, **kwl)
 
         ax.plot(*(origin + np.stack([[v[0], v[1], 0], v])).T, **kwl)
         ax.plot(*(origin + np.stack([[v[0], 0, v[2]], v])).T, **kwl)
         ax.plot(*(origin + np.stack([[0, v[1], v[2]], v])).T, **kwl)
 
         kw = omit({**arrowprops}, "color")
-        _x = arrow3D([v[0], 0, 0], origin, ax=ax, arrow_kwargs={"color": "#E66B4C", **kw}, text="x")
-        _y = arrow3D([0, v[1], 0], origin, ax=ax, arrow_kwargs={"color": "#A4E64B", **kw}, text="y")
-        _z = arrow3D([0, 0, v[2]], origin, ax=ax, arrow_kwargs={"color": "#4C72E6", **kw}, text="z")
+        _x = arrow3D(
+            [v[0], 0, 0], origin, ax=ax, arrow_kwargs={"color": "#E66B4C", **kw}, text="x"
+        )
+        _y = arrow3D(
+            [0, v[1], 0], origin, ax=ax, arrow_kwargs={"color": "#A4E64B", **kw}, text="y"
+        )
+        _z = arrow3D(
+            [0, 0, v[2]], origin, ax=ax, arrow_kwargs={"color": "#4C72E6", **kw}, text="z"
+        )
 
     # Plot main vector after to ensure it's on top
     _arrow = arrow3D(
         v,
         origin,
         ax=ax,
         text=vtext,
@@ -312,28 +317,33 @@
 
     if "facecolor" in angle_kwargs:
         arc = np.concatenate([arc, [origin]], axis=0)
         default_edgecolor = "none"
     else:
         default_edgecolor = "k"
 
-    edgecolor = angle_kwargs.get("edgecolor") or angle_kwargs.pop("color", default_edgecolor)
+    edgecolor = angle_kwargs.get("edgecolor") or angle_kwargs.pop(
+        "color", default_edgecolor
+    )
     angleprops = dict(
         edgecolor=edgecolor,
         facecolor="none",
         linewidth=1,
     )
     angleprops.update(angle_kwargs)
 
     patch = Patch3D(**angleprops)
     patch.set_3d_properties(arc[:, :2], zs=arc[:, 2], zdir="z")
     ax.add_artist(patch)
 
     if text is not None:
-        c = arc[0] + ((arc[-2] if "facecolor" in angle_kwargs else arc[-1]) - arc[0]) * 0.5
+        c = (
+            arc[0]
+            + ((arc[-2] if "facecolor" in angle_kwargs else arc[-1]) - arc[0]) * 0.5
+        )
         phic = np.arctan2(c[1], c[0])
         thetac = np.arccos(c[2] / np.linalg.norm(c))
         center = (
             np.array(
                 [
                     np.sin(thetac) * np.cos(phic),
                     np.sin(thetac) * np.sin(phic),
@@ -642,15 +652,16 @@
 
     arrowstyle = dict(
         tail_width=0.1,
         head_width=0.45,
         head_length=0.45,
     )
     arrowprops = dict(
-        arrowstyle="Simple, " + ", ".join(map(lambda x: f"{x[0]}={x[1]}", arrowstyle.items())),
+        arrowstyle="Simple, "
+        + ", ".join(map(lambda x: f"{x[0]}={x[1]}", arrowstyle.items())),
         mutation_scale=20,
     )
     arrowprops.update(arrow_kwargs)
 
     arrow = Arrow3D(*origin, *v, **arrowprops)
     ax.add_artist(arrow)
```

### Comparing `apygee-1.0.3/apygee/utils.py` & `apygee-1.0.4/apygee/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 from numpy.typing import ArrayLike
 
 import matplotlib.pyplot as plt
 import numpy as np
-
 from matplotlib.colors import hsv_to_rgb, rgb_to_hsv, to_hex, to_rgb, to_rgba
 
 
 def maybe_unwrap(x: np.ndarray | Any) -> Any:
     if hasattr(x, "item") and np.size(x) == 1:
         return x.item()
 
@@ -156,15 +155,16 @@
     return np.sum(a * b, axis=-1)
 
 
 def angle_between(a: ArrayLike, b: ArrayLike) -> float:
     a = np.asarray(a, dtype=np.float64)
     b = np.asarray(b, dtype=np.float64)
     return np.round(
-        np.arccos(np.clip(np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b)), -1, 1)), 15
+        np.arccos(np.clip(np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b)), -1, 1)),
+        15,
     )
 
 
 def mix_colors(
     color1: str | tuple[float],
     color2: str | tuple[float],
     fraction: float = 0.5,
```

### Comparing `apygee-1.0.3/pyproject.toml` & `apygee-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apygee"
-version = "1.0.3"
+version = "1.0.4"
 description = "A package for creating, manipulating and visualizing Kepler orbits"
 authors = ["Jelmar Gerritsen <jelmargerritsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 matplotlib = "^3.8.3"
```

### Comparing `apygee-1.0.3/PKG-INFO` & `apygee-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apygee
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for creating, manipulating and visualizing Kepler orbits
 Author: Jelmar Gerritsen
 Author-email: jelmargerritsen@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
@@ -14,15 +14,15 @@
 Requires-Dist: plotly (>=5.20.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Apygee
 
 <p align="start">
   <a href="https://github.com/Pocket-titan/apygee">
-    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.jpg" alt="Logo" width="200">
+    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.png" alt="Logo" height="200px">
   </a>
 </p>
 
 Apygee (apogee + `py`) is a lightweight Python package for creating, manipulating and visualizing Kepler orbits.
 
 ## Installation
 
@@ -118,28 +118,28 @@
 
 
 
 ![png](https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/examples_5_0.png)
 
 
 
-### Visualize an orbit (requires plotly)
+### Visualize an orbit
 
 
 
 ```python
 from apygee import Orbit, MU_EARTH
 
 orbit = Orbit([2e6], mu=MU_EARTH)
 orbit.visualize()
 ```
 
 
 
-<img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/orbitvis.png" alt="Orbit visualization" width="400px" />
+<img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/examples/examples_files/orbitvis.gif" alt="Orbit visualization" width="400px" />
 
 
 
 ### Hohmann transfer from Earth to Mars
```

