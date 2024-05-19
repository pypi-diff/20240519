# Comparing `tmp/ewstools-2.1.0.tar.gz` & `tmp/ewstools-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewstools-2.1.0.tar", last modified: Tue Dec 13 19:16:31 2022, max compression
+gzip compressed data, was "ewstools-2.1.2.tar", last modified: Sun May 19 02:22:13 2024, max compression
```

## Comparing `ewstools-2.1.0.tar` & `ewstools-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tbury      (501) staff       (20)        0 2022-12-13 19:16:31.309360 ewstools-2.1.0/
--rw-------   0 tbury      (501) staff       (20)     1073 2019-07-01 17:33:01.000000 ewstools-2.1.0/LICENSE
--rw-r--r--   0 tbury      (501) staff       (20)     8477 2022-12-13 19:16:31.309193 ewstools-2.1.0/PKG-INFO
--rw-r--r--   0 tbury      (501) staff       (20)     8044 2022-12-13 18:59:36.000000 ewstools-2.1.0/README.md
-drwxr-xr-x   0 tbury      (501) staff       (20)        0 2022-12-13 19:16:31.308513 ewstools-2.1.0/ewstools/
--rw-r--r--   0 tbury      (501) staff       (20)      191 2022-12-09 17:57:21.000000 ewstools-2.1.0/ewstools/__init__.py
--rw-r--r--   0 tbury      (501) staff       (20)    51150 2022-12-13 17:06:51.000000 ewstools-2.1.0/ewstools/core.py
--rw-r--r--   0 tbury      (501) staff       (20)    28980 2022-12-09 17:57:21.000000 ewstools-2.1.0/ewstools/helpers.py
--rw-r--r--   0 tbury      (501) staff       (20)    11622 2022-12-09 17:57:21.000000 ewstools-2.1.0/ewstools/models.py
-drwxr-xr-x   0 tbury      (501) staff       (20)        0 2022-12-13 19:16:31.309040 ewstools-2.1.0/ewstools.egg-info/
--rw-r--r--   0 tbury      (501) staff       (20)     8477 2022-12-13 19:16:31.000000 ewstools-2.1.0/ewstools.egg-info/PKG-INFO
--rw-r--r--   0 tbury      (501) staff       (20)      262 2022-12-13 19:16:31.000000 ewstools-2.1.0/ewstools.egg-info/SOURCES.txt
--rw-r--r--   0 tbury      (501) staff       (20)        1 2022-12-13 19:16:31.000000 ewstools-2.1.0/ewstools.egg-info/dependency_links.txt
--rw-r--r--   0 tbury      (501) staff       (20)      115 2022-12-13 19:16:31.000000 ewstools-2.1.0/ewstools.egg-info/requires.txt
--rw-r--r--   0 tbury      (501) staff       (20)        9 2022-12-13 19:16:31.000000 ewstools-2.1.0/ewstools.egg-info/top_level.txt
--rw-r--r--   0 tbury      (501) staff       (20)       38 2022-12-13 19:16:31.309408 ewstools-2.1.0/setup.cfg
--rw-r--r--   0 tbury      (501) staff       (20)      994 2022-12-13 19:00:22.000000 ewstools-2.1.0/setup.py
+drwxr-xr-x   0 tbury      (501) staff       (20)        0 2024-05-19 02:22:13.934411 ewstools-2.1.2/
+-rw-------   0 tbury      (501) staff       (20)     1073 2019-07-01 17:33:01.000000 ewstools-2.1.2/LICENSE
+-rw-r--r--   0 tbury      (501) staff       (20)     8254 2024-05-19 02:22:13.934229 ewstools-2.1.2/PKG-INFO
+-rw-r--r--   0 tbury      (501) staff       (20)     7821 2024-05-19 02:16:31.000000 ewstools-2.1.2/README.md
+drwxr-xr-x   0 tbury      (501) staff       (20)        0 2024-05-19 02:22:13.933430 ewstools-2.1.2/ewstools/
+-rw-r--r--   0 tbury      (501) staff       (20)      225 2024-05-08 16:53:58.000000 ewstools-2.1.2/ewstools/__init__.py
+-rw-r--r--   0 tbury      (501) staff       (20)    62221 2024-05-19 02:13:45.000000 ewstools-2.1.2/ewstools/core.py
+-rw-r--r--   0 tbury      (501) staff       (20)    28980 2022-12-09 17:57:21.000000 ewstools-2.1.2/ewstools/helpers.py
+-rw-r--r--   0 tbury      (501) staff       (20)    11622 2022-12-09 17:57:21.000000 ewstools-2.1.2/ewstools/models.py
+drwxr-xr-x   0 tbury      (501) staff       (20)        0 2024-05-19 02:22:13.934057 ewstools-2.1.2/ewstools.egg-info/
+-rw-r--r--   0 tbury      (501) staff       (20)     8254 2024-05-19 02:22:13.000000 ewstools-2.1.2/ewstools.egg-info/PKG-INFO
+-rw-r--r--   0 tbury      (501) staff       (20)      262 2024-05-19 02:22:13.000000 ewstools-2.1.2/ewstools.egg-info/SOURCES.txt
+-rw-r--r--   0 tbury      (501) staff       (20)        1 2024-05-19 02:22:13.000000 ewstools-2.1.2/ewstools.egg-info/dependency_links.txt
+-rw-r--r--   0 tbury      (501) staff       (20)      131 2024-05-19 02:22:13.000000 ewstools-2.1.2/ewstools.egg-info/requires.txt
+-rw-r--r--   0 tbury      (501) staff       (20)        9 2024-05-19 02:22:13.000000 ewstools-2.1.2/ewstools.egg-info/top_level.txt
+-rw-r--r--   0 tbury      (501) staff       (20)       38 2024-05-19 02:22:13.934461 ewstools-2.1.2/setup.cfg
+-rw-r--r--   0 tbury      (501) staff       (20)      922 2024-05-19 02:20:58.000000 ewstools-2.1.2/setup.py
```

### Comparing `ewstools-2.1.0/LICENSE` & `ewstools-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ewstools-2.1.0/PKG-INFO` & `ewstools-2.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,41 @@
-Metadata-Version: 2.1
-Name: ewstools
-Version: 2.1.0
-Summary: Python package to compute early warning signals (EWS) 
-Home-page: https://github.com/ThomasMBury/ewstools
-Author: Thomas M Bury
-Author-email: tombury182@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/ewstools.svg)](https://badge.fury.io/py/ewstools)
 [![Downloads](https://pepy.tech/badge/ewstools)](https://pepy.tech/project/ewstools)
 [![Documentation Status](https://readthedocs.org/projects/ewstools/badge/?version=latest)](https://ewstools.readthedocs.io/en/latest/?badge=latest)
 [![tests](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/ThomasMBury/ewstools/branch/main/graph/badge.svg?token=Q5LGRV6TLF)](https://codecov.io/gh/ThomasMBury/ewstools)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05038/status.svg)](https://doi.org/10.21105/joss.05038)
 
 # ewstools
 **A Python package for early warning signals (EWS) of bifurcations in time series data.**
 
 ## Overview
 
 Many systems in nature and society have the capacity to undergo critical transitions--sudden and profound changes in dynamics that are hard to reverse. Examples include the outbreak of disease, the collapse of an ecosystem, or the onset of a cardiac arrhythmia. From a mathematical perspective, these transitions may be understood as the crossing of a bifurcation (tipping point) in an appropriate dynamical system model. In 2009, Scheffer and colleagues proposed early warning signals (EWS) for bifurcations based on statistics of noisy fluctuations in time series data ([Scheffer et al. 2009](https://www.nature.com/articles/nature08227)). This spurred massive interest in the subject, resulting in a multitude of different EWS for anticipating bifurcations ([Clements & Ozgul 2018](https://onlinelibrary.wiley.com/doi/full/10.1111/ele.12948)). More recently, EWS from deep learning classifiers have outperformed conventional EWS on several model and empirical datasets, whilst also providing information on the type of bifurcation ([Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118)).
 
 `ewstools` is an accessible toolbox for computing, analysing and visualising EWS in time series data. It complements an existing EWS package in R ([Dakos et al. 2012](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0041010)). Given the recent surge in popularity of the Python programming langauge ([PYPL, 2022](https://pypl.github.io/PYPL.html)), a Python-based implementation of EWS should be useful.
 
 The package provides:
 
-  - An intuitive, object-oriented framework for working with EWS in a given time series
+  - An intuitive, object-oriented framework for computing EWS for a given time series
   - Time series detrending methods using
     - A Gaussian kernel
     - LOWESS (Locally Weighted Scatterplot Smoothing)
   - Computation of CSD-based early warning signals including:
     - Variance and associated metrics (standard deviation, coefficient of variation)
     - Autocorrelation (at specified lag times)
     - Higher-order statistical moments (skewness, kurtosis)
     - Power spectrum and associated metrics
+    - Various entropy measures
   - Computation of Kendall tau values to quantify trends
   - Application of deep learning classifiers for bifurcation prediction as in [Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118).
-  - Block-bootstrapping of time-series to obtain confidence intervals on EWS estimates
   - Visualisation tools to display output
   - Built-in theoretical models to test EWS
 
-`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
+`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [EntropyHub](https://www.entropyhub.xyz/index.html) for entropy computations, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
 
 
 ## Install
 
 Requires Python 3.7 or later. You can install `ewstools` with pip using the commands
 
 ```bash
@@ -65,15 +53,15 @@
 'numpy>=1.14.0',
 'plotly>=2.3.0',
 'lmfit>=0.9.0', 
 'arch>=4.4',
 'statsmodels>=0.9.0',
 'scipy>=1.0.1',
 ```
-and should be installed automatically. To use any of the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) v2.0.0 or later.
+and should be installed automatically. To use the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) with version later than 2.0 and earlier than 2.12.
 
 To install the latest *development* version, use the command
 ```bash
 pip install git+https://github.com/thomasmbury/ewstools.git#egg=ewstools
 ```
 NB: the development version comes with the risk of undergoing continual changes, and has not undergone the level of scrutiny of official releases.
 
@@ -137,14 +125,10 @@
 
 This work is currently supported by an FRQNT (Fonds de recherche du Québec - Nature et Technologies) postdoctoral research scholarship awarded to Dr. Thomas Bury. In the past, it has also been supported by NSERC (Natural Sciences and Engineering Research Council) Discovery Grants awarded to Dr. Chris Bauch and Dr. Madhur Anand.
 
 ## Citation info
 
 If you like the respoitory, please give it a star :D
 
-If your research uses the deep learning functionality of `ewstools`, please cite
-
-Bury, Thomas M., et al. "[Deep learning for early warning signals of tipping points.](https://www.pnas.org/doi/abs/10.1073/pnas.2106140118)" *Proceedings of the National Academy of Sciences* 118.39 (2021): e2106140118.
-
-If your research computes spectral EWS using `ewstools`, please cite
+If your research makes use of it, please cite
 
-Bury, Thomas M., Chris T. Bauch, and Madhur Anand. "[Detecting and distinguishing tipping points using spectral early warning signals.](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2020.0482)" *Journal of the Royal Society Interface* 17.170 (2020): 20200482.
+Bury, Thomas M. "[ewstools: A Python package for early warning signals of bifurcations in time series data.](https://joss.theoj.org/papers/10.21105/joss.05038.pdf)" *Journal of Open Source Software* 8.82 (2023): 5038.
```

### Comparing `ewstools-2.1.0/README.md` & `ewstools-2.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,54 @@
+Metadata-Version: 2.1
+Name: ewstools
+Version: 2.1.2
+Summary: Python package to compute early warning signals (EWS) 
+Home-page: https://github.com/ThomasMBury/ewstools
+Author: Thomas M Bury
+Author-email: tombury182@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI version](https://badge.fury.io/py/ewstools.svg)](https://badge.fury.io/py/ewstools)
 [![Downloads](https://pepy.tech/badge/ewstools)](https://pepy.tech/project/ewstools)
 [![Documentation Status](https://readthedocs.org/projects/ewstools/badge/?version=latest)](https://ewstools.readthedocs.io/en/latest/?badge=latest)
 [![tests](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/ThomasMBury/ewstools/branch/main/graph/badge.svg?token=Q5LGRV6TLF)](https://codecov.io/gh/ThomasMBury/ewstools)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05038/status.svg)](https://doi.org/10.21105/joss.05038)
 
 # ewstools
 **A Python package for early warning signals (EWS) of bifurcations in time series data.**
 
 ## Overview
 
 Many systems in nature and society have the capacity to undergo critical transitions--sudden and profound changes in dynamics that are hard to reverse. Examples include the outbreak of disease, the collapse of an ecosystem, or the onset of a cardiac arrhythmia. From a mathematical perspective, these transitions may be understood as the crossing of a bifurcation (tipping point) in an appropriate dynamical system model. In 2009, Scheffer and colleagues proposed early warning signals (EWS) for bifurcations based on statistics of noisy fluctuations in time series data ([Scheffer et al. 2009](https://www.nature.com/articles/nature08227)). This spurred massive interest in the subject, resulting in a multitude of different EWS for anticipating bifurcations ([Clements & Ozgul 2018](https://onlinelibrary.wiley.com/doi/full/10.1111/ele.12948)). More recently, EWS from deep learning classifiers have outperformed conventional EWS on several model and empirical datasets, whilst also providing information on the type of bifurcation ([Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118)).
 
 `ewstools` is an accessible toolbox for computing, analysing and visualising EWS in time series data. It complements an existing EWS package in R ([Dakos et al. 2012](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0041010)). Given the recent surge in popularity of the Python programming langauge ([PYPL, 2022](https://pypl.github.io/PYPL.html)), a Python-based implementation of EWS should be useful.
 
 The package provides:
 
-  - An intuitive, object-oriented framework for working with EWS in a given time series
+  - An intuitive, object-oriented framework for computing EWS for a given time series
   - Time series detrending methods using
     - A Gaussian kernel
     - LOWESS (Locally Weighted Scatterplot Smoothing)
   - Computation of CSD-based early warning signals including:
     - Variance and associated metrics (standard deviation, coefficient of variation)
     - Autocorrelation (at specified lag times)
     - Higher-order statistical moments (skewness, kurtosis)
     - Power spectrum and associated metrics
+    - Various entropy measures
   - Computation of Kendall tau values to quantify trends
   - Application of deep learning classifiers for bifurcation prediction as in [Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118).
-  - Block-bootstrapping of time-series to obtain confidence intervals on EWS estimates
   - Visualisation tools to display output
   - Built-in theoretical models to test EWS
 
-`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
+`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [EntropyHub](https://www.entropyhub.xyz/index.html) for entropy computations, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
 
 
 ## Install
 
 Requires Python 3.7 or later. You can install `ewstools` with pip using the commands
 
 ```bash
@@ -52,15 +66,15 @@
 'numpy>=1.14.0',
 'plotly>=2.3.0',
 'lmfit>=0.9.0', 
 'arch>=4.4',
 'statsmodels>=0.9.0',
 'scipy>=1.0.1',
 ```
-and should be installed automatically. To use any of the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) v2.0.0 or later.
+and should be installed automatically. To use the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) with version later than 2.0 and earlier than 2.12.
 
 To install the latest *development* version, use the command
 ```bash
 pip install git+https://github.com/thomasmbury/ewstools.git#egg=ewstools
 ```
 NB: the development version comes with the risk of undergoing continual changes, and has not undergone the level of scrutiny of official releases.
 
@@ -124,14 +138,10 @@
 
 This work is currently supported by an FRQNT (Fonds de recherche du Québec - Nature et Technologies) postdoctoral research scholarship awarded to Dr. Thomas Bury. In the past, it has also been supported by NSERC (Natural Sciences and Engineering Research Council) Discovery Grants awarded to Dr. Chris Bauch and Dr. Madhur Anand.
 
 ## Citation info
 
 If you like the respoitory, please give it a star :D
 
-If your research uses the deep learning functionality of `ewstools`, please cite
-
-Bury, Thomas M., et al. "[Deep learning for early warning signals of tipping points.](https://www.pnas.org/doi/abs/10.1073/pnas.2106140118)" *Proceedings of the National Academy of Sciences* 118.39 (2021): e2106140118.
-
-If your research computes spectral EWS using `ewstools`, please cite
+If your research makes use of it, please cite
 
-Bury, Thomas M., Chris T. Bauch, and Madhur Anand. "[Detecting and distinguishing tipping points using spectral early warning signals.](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2020.0482)" *Journal of the Royal Society Interface* 17.170 (2020): 20200482.
+Bury, Thomas M. "[ewstools: A Python package for early warning signals of bifurcations in time series data.](https://joss.theoj.org/papers/10.21105/joss.05038.pdf)" *Journal of Open Source Software* 8.82 (2023): 5038.
```

### Comparing `ewstools-2.1.0/ewstools/core.py` & `ewstools-2.1.2/ewstools/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,462 +50,540 @@
 import ewstools.helpers as helpers
 
 # Plotly modules for visualisation
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
+import EntropyHub as EH
 
 # For deprecating old functions
 import deprecation
 
 
-
 # ---------------
 # Classes
 # --------------
 
+
 class TimeSeries:
     """
-    Univariate time series data on which to compute early warning signals.
+    Class to hold univariate time series data on which to
+    compute early warning signals.
 
     Parameters
     ----------
     data : list, numpy.ndarray or pandas.Series
         1D list of data that makes up time series. If given as a pandas.Series,
         then the index, which should represent time values, is carried over.
     transition : float
         Time value at which transition occurs, if any. If defined, early warning signals
         are only computed up to this point in the time series.
 
     """
 
     def __init__(self, data, transition=None):
-
         # Put data into a pandas DataFrame
         if type(data) in [list, np.ndarray]:
-            df_state = pd.DataFrame({'time': np.arange(len(data)), 'state': data})
-            df_state.set_index('time', inplace=True)
-        
+            df_state = pd.DataFrame({"time": np.arange(len(data)), "state": data})
+            df_state.set_index("time", inplace=True)
+
         # If given as pandas series, carry index forward
         elif type(data) == pd.Series:
-            df_state = pd.DataFrame({'state': data.values})
+            df_state = pd.DataFrame({"state": data.values})
             df_state.index = data.index
             # Rename index if no name given
             if not df_state.index.name:
-                df_state.index.name = 'time'
-                
+                df_state.index.name = "time"
+
         # If data is not provided as either of these, flag error
         else:
-            print('\nERROR: data has been provided as type {}'.format(type(data)))
-            print('Make sure to provide data as either a list, np.ndarray or pd.Series\n')
-        
+            print("\nERROR: data has been provided as type {}".format(type(data)))
+            print(
+                "Make sure to provide data as either a list, np.ndarray or pd.Series\n"
+            )
+            return
+
         # Set state and transition attributes
         self.state = df_state
         self.transition = float(transition) if transition else transition
-        
+
         # Initialise other attributes
         self.ews = pd.DataFrame(index=df_state.index)
         self.dl_preds = pd.DataFrame()
         self.ktau = dict()
         self.pspec = None
         self.pspec_fits = None
         self.ews_spec = pd.DataFrame()
-        
 
-    def detrend(self, method='Gaussian', bandwidth=0.2, span=0.2):
-        '''
+    def detrend(self, method="Gaussian", bandwidth=0.2, span=0.2):
+        """
         Detrend the time series using a chosen method.
-        Add column to the dataframe for 'smoothing' and 'residuals'
+        Output is stored in the self.state dataframe.
 
         Parameters
         ----------
         method : str, optional
-            Method of detrending to use. 
+            Method of detrending to use.
             Select from ['Gaussian', 'Lowess']
             The default is 'Gaussian'.
         bandwidth : float, optional
             Bandwidth of Gaussian kernel. Provide as a proportion of data length
             or as a number of data points. As in the R function ksmooth
             (used by the earlywarnings package in R), we define the bandwidth
             such that the kernel has its quartiles at +/- 0.25*bandwidth.
             The default is 0.2.
         span : float, optional
-            Span of time-series data used for Lowess filtering. Provide as a 
-            proportion of data length or as a number of data points. 
+            Span of time-series data used for Lowess filtering. Provide as a
+            proportion of data length or as a number of data points.
             The default is 0.2.
 
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
 
-
-        if method == 'Gaussian':
+        if method == "Gaussian":
             # Get size of bandwidth in terms of num. datapoints if given as a proportion
             if 0 < bandwidth <= 1:
                 bw_num = bandwidth * len(df_pre)
             else:
                 bw_num = bandwidth
 
             # Use the gaussian_filter function provided by Scipy
             # Standard deviation of kernel given bandwidth
             # Note that for a Gaussian, quartiles are at +/- 0.675*sigma
             sigma = (0.25 / 0.675) * bw_num
-            smooth_values = gf(df_pre['state'].values, sigma=sigma, mode='reflect')
+            smooth_values = gf(df_pre["state"].values, sigma=sigma, mode="reflect")
             smooth_series = pd.Series(smooth_values, index=df_pre.index)
 
-
-        if method == 'Lowess':
+        if method == "Lowess":
             # Convert span to a proportion of the length of the data
             if not 0 < span <= 1:
                 span_prop = span / len(df_pre)
             else:
                 span_prop = span
 
-            smooth_values = lowess(df_pre['state'].values, 
-                                   df_pre.index.values, 
-                                   frac=span_prop)[:,1]
+            smooth_values = lowess(
+                df_pre["state"].values, df_pre.index.values, frac=span_prop
+            )[:, 1]
             smooth_series = pd.Series(smooth_values, index=df_pre.index)
 
-    
         # Add smoothed data and residuals to the 'state' DataFrame
         self.state["smoothing"] = smooth_series
         self.state["residuals"] = self.state["state"] - self.state["smoothing"]
 
-
-
     def compute_var(self, rolling_window=0.25):
-        '''
+        """
         Compute variance over a rolling window.
         If residuals have not been computed, computation will be
         performed over state variable.
-        
-        Put into 'ews' dataframe
+        Output is stored in the self.ews dataframe.
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
-            
+
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            var_values = df_pre['residuals'].rolling(window=rw_absolute).var()
+        if "residuals" in df_pre.columns:
+            var_values = df_pre["residuals"].rolling(window=rw_absolute).var()
         # Else, compute over state variable
         else:
-            var_values = df_pre['state'].rolling(window=rw_absolute).var()
-        
-        self.ews['variance'] = var_values
-        
-        
-        
+            var_values = df_pre["state"].rolling(window=rw_absolute).var()
+
+        self.ews["variance"] = var_values
+
     def compute_std(self, rolling_window=0.25):
-        '''
+        """
         Compute standard deviation over a rolling window.
         If residuals have not been computed, computation will be
         performed over state variable.
-        
-        Put into 'ews' dataframe
+        Output is stored in the self.ews dataframe.
+
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
-            
+
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            std_values = df_pre['residuals'].rolling(window=rw_absolute).std()
+        if "residuals" in df_pre.columns:
+            std_values = df_pre["residuals"].rolling(window=rw_absolute).std()
         # Else, compute over state variable
         else:
-            std_values = df_pre['state'].rolling(window=rw_absolute).std()
-        
-        self.ews['std'] = std_values        
+            std_values = df_pre["state"].rolling(window=rw_absolute).std()
 
+        self.ews["std"] = std_values
 
     def compute_cv(self, rolling_window=0.25):
-        '''
+        """
         Compute coefficient of variation over a rolling window.
         This is the standard deviation of the residuals divided by the
         mean of the state variable.
         If residuals have not been computed, computation will be
         performed over state variable.
-        
-        Put into 'ews' dataframe
+        Output is stored in the self.ews dataframe.
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
-            
+
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # Get standard deviation values
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            std_values = df_pre['residuals'].rolling(window=rw_absolute).std()
+        if "residuals" in df_pre.columns:
+            std_values = df_pre["residuals"].rolling(window=rw_absolute).std()
         # Else, compute over state variable
         else:
-            std_values = df_pre['state'].rolling(window=rw_absolute).std()
-        
-        # Get mean values from state variable
-        mean_values = df_pre['state'].rolling(window=rw_absolute).mean()
-        
-        cv_values = std_values/mean_values
-        
-        self.ews['cv'] = cv_values        
-
-
+            std_values = df_pre["state"].rolling(window=rw_absolute).std()
 
+        # Get mean values from state variable
+        mean_values = df_pre["state"].rolling(window=rw_absolute).mean()
 
+        cv_values = std_values / mean_values
 
+        self.ews["cv"] = cv_values
 
     def compute_auto(self, rolling_window=0.25, lag=1):
-        '''
-        Compute autocorrelation over a rolling window. Add to dataframe.
+        """
+        Compute autocorrelation at a give lag over a rolling window.
+        If residuals have not been computed, computation will be
+        performed over state variable.
+        Output is stored in the self.ews dataframe.
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute autocorrelation. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
         lag : int
             Lag of autocorrelation
-            
+
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            ac_values = df_pre['residuals'].rolling(window=rw_absolute).apply(
-                func=lambda x: pd.Series(x).autocorr(lag=lag), raw=True
+        if "residuals" in df_pre.columns:
+            ac_values = (
+                df_pre["residuals"]
+                .rolling(window=rw_absolute)
+                .apply(func=lambda x: pd.Series(x).autocorr(lag=lag), raw=True)
             )
         # Else, compute over state variable
         else:
-            ac_values = df_pre['state'].rolling(window=rw_absolute).apply(
-                func=lambda x: pd.Series(x).autocorr(lag=lag), raw=True
-            )                    
-            
-        self.ews['ac{}'.format(lag)] = ac_values
+            ac_values = (
+                df_pre["state"]
+                .rolling(window=rw_absolute)
+                .apply(func=lambda x: pd.Series(x).autocorr(lag=lag), raw=True)
+            )
 
+        self.ews["ac{}".format(lag)] = ac_values
 
     def compute_skew(self, rolling_window=0.25):
-        '''
+        """
         Compute skew over a rolling window.
         If residuals have not been computed, computation will be
         performed over state variable.
-        
-        Add to dataframe.
+        Output is stored in the self.ews dataframe.
+
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
-            
+
         Returns
         -------
         None.
 
-        '''
-        
+        """
+
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            skew_values = df_pre['residuals'].rolling(window=rw_absolute).skew()
+        if "residuals" in df_pre.columns:
+            skew_values = df_pre["residuals"].rolling(window=rw_absolute).skew()
         # Else, compute over state variable
         else:
-            skew_values = df_pre['state'].rolling(window=rw_absolute).skew()
-        
-        self.ews['skew'] = skew_values
-
+            skew_values = df_pre["state"].rolling(window=rw_absolute).skew()
 
+        self.ews["skew"] = skew_values
 
     def compute_kurt(self, rolling_window=0.25):
-        '''
+        """
         Compute kurtosis over a rolling window.
         If residuals have not been computed, computation will be
         performed over state variable.
-        
-        Add to dataframe.
+        Output is stored in the self.ews dataframe.
+
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
-            
+
         Returns
         -------
         None.
 
-        '''
+        """
 
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
-    
+
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            kurt_values = df_pre['residuals'].rolling(window=rw_absolute).kurt()
+        if "residuals" in df_pre.columns:
+            kurt_values = df_pre["residuals"].rolling(window=rw_absolute).kurt()
         # Else, compute over state variable
         else:
-            kurt_values = df_pre['state'].rolling(window=rw_absolute).kurt()
-        
-        self.ews['kurtosis'] = kurt_values
+            kurt_values = df_pre["state"].rolling(window=rw_absolute).kurt()
+
+        self.ews["kurtosis"] = kurt_values
+
+    def compute_entropy(self, rolling_window=0.25, method="sample", **kwargs):
+        """
+        Compute entropy using a given method over a rolling window.
+        Uses EntropyHub https://www.entropyhub.xyz/Home.html.
+        If residuals have not been computed, computation will be
+        performed over state variable.
+        Output is stored in the self.ews dataframe.
+
+        Parameters
+        ----------
+        rolling_window : float
+            Length of rolling window used to compute variance. Can be specified
+            as an absolute value or as a proportion of the length of the
+            data being analysed. Default is 0.25.
+        method : str
+            The method by which to compute entropy. Options include 'sample',
+            'approximate', and 'kolmogorov'
+        **kwargs
+            Keyword arguments for the EntropyHub function
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # Get time series data prior to transition
+        if self.transition:
+            df_pre = self.state[self.state.index <= self.transition]
+        else:
+            df_pre = self.state
 
+        # Get absolute size of rollling window if given as a proportion
+        if 0 < rolling_window <= 1:
+            rw_absolute = int(rolling_window * len(df_pre))
+        else:
+            rw_absolute = rolling_window
 
+        # Get data on which to compute entropy
+        if "residuals" in df_pre.columns:
+            ts_vals = df_pre["residuals"]
+        else:
+            ts_vals = df_pre["state"]
 
+        # Compute sample entropy
+        if method == "sample":
 
-    def compute_ktau(self, tmin='earliest', tmax='latest'):
-        '''
+            def entropy_func(series):
+                Samp, A, B = EH.SampEn(series.values, **kwargs)
+                return Samp
+
+        # Compute approxiamte entropy
+        if method == "approximate":
+
+            def entropy_func(series):
+                Ap, Phi = EH.ApEn(series.values, **kwargs)
+                return Ap
+
+        # Compute komogorov entropy
+        if method == "kolmogorov":
+
+            def entropy_func(series):
+                K2, Ci = EH.K2En(series.values, **kwargs)
+                return K2
+
+        list_times = []
+        list_entropy = []
+        # Set up rolling window (cannot use pandas.rolling as multi-output fn)
+        for k in np.arange(0, len(ts_vals) - (rw_absolute - 1)):
+            # Select subset of series contained in window
+            window_series = ts_vals.iloc[k : k + rw_absolute]
+            # Assign the time value for the metrics (right end point of window)
+            t_point = ts_vals.index[k + (rw_absolute - 1)]
+            # Compute entropy (value for each channel)
+            entropy = entropy_func(window_series)
+
+            list_times.append(t_point)
+            list_entropy.append(entropy)
+
+        ar_entropy = np.array(list_entropy)
+
+        df_entropy = pd.DataFrame()
+        df_entropy["time"] = list_times
+        num_embedding_dims = ar_entropy.shape[1]
+        for dim in range(num_embedding_dims):
+            df_entropy["{}-entropy-{}".format(method, dim)] = ar_entropy[:, dim]
+        df_entropy.set_index("time", inplace=True)
+
+        # Add info to self.ews dataframe
+        for col in df_entropy.columns:
+            self.ews[col] = df_entropy[col]
+        # self.ews = pd.merge(self.ews, df_entropy, how="left", on="time")
+
+    def compute_ktau(self, tmin="earliest", tmax="latest"):
+        """
         Compute kendall tau values of CSD-based EWS.
-        Output is placed in the attribute *ktau*, which is a Python 
+        Output is placed in the attribute *ktau*, which is a Python
         dictionary contianing Kendall tau values for each CSD-based EWS.
 
         Parameters
         ----------
         tmin : float or 'earliest'
             Start time for kendall tau computation. If 'earliest', then
             time is taken as earliest time point in EWS time series.
         tmax : float or 'latest'
             End time for kendall tau computation. If 'latest', then time is
             taken as latest time point in EWS time series, which could be
             the end of the state time series, or a defined transtion point.
 
-        '''
-        
-        
+        """
+
         # Get tmin and tmax values if using extrema
-        if tmin == 'earliest':
-            tmin = self.ews.dropna().index[0]
-        
-        if tmax == 'latest':
-            tmax = self.ews.dropna().index[-1]
-        
+        if tmin == "earliest":
+            tmin = self.ews.dropna(how="all").index[0]
+
+        if tmax == "latest":
+            tmax = self.ews.dropna(how="all").index[-1]
+
         # Get cropped data
-        df_ews = self.ews[(self.ews.index >= tmin) &\
-                          (self.ews.index <= tmax)].copy()
-        
+        df_ews = self.ews[(self.ews.index >= tmin) & (self.ews.index <= tmax)].copy()
+
         # Include smax in Kendall tau computation if it exists
-        if 'smax' in self.ews_spec.columns:
-            df_ews = df_ews.join(self.ews_spec['smax'])
-            
+        if "smax" in self.ews_spec.columns:
+            df_ews = df_ews.join(self.ews_spec["smax"])
+
         # Make a series with the time values
         time_values = pd.Series(data=df_ews.index, index=df_ews.index)
         ktau_out = df_ews.corrwith(time_values, method="kendall", axis=0)
         self.ktau = dict(ktau_out)
-        
 
-    def apply_classifier(self, classifier, tmin, tmax, 
-                        name='c1', verbose=1):
-        '''
+    def apply_classifier(self, classifier, tmin, tmax, name="c1", verbose=1):
+        """
         Apply a deep learning classifier to the residual time series from
-        tmin to tmax. 
+        tmin to tmax.
         If time series has not been detrended, apply to the raw data.
         Predictions from the classifier are saved into the attribute dl_preds.
 
         Parameters
         ----------
         classifier : keras.engine.sequential.Sequential
             Tensorflow classifier
@@ -514,63 +592,65 @@
         tmax : float
             Latest time in time series segment (not inclusive)
         name : str, optional
             Name assigned to the classifier. The default is 'c1'.
         verbose : int, optional
             Verbosity of update messages from TensorFlow. 0 = silent, 1 = progress bar, 2 = single line.
             The default is 1.
-        
+
         Returns
         -------
         None.
 
-        '''
-        
+        """
+
         # Length of time series required as input to classifier
         input_len = classifier.layers[0].input_shape[1]
-        
+
         # Get time series segment. Use residuals if detrending performed.
         # Otherwise use state variable.
-        if 'residuals' in self.state.columns:
-            series = self.state[(self.state.index >= tmin) &\
-                                (self.state.index < tmax)]['residuals']      
-        else:
-            series = self.state[(self.state.index >= tmin) &\
-                                (self.state.index < tmax)]['state']
-        
+        if "residuals" in self.state.columns:
+            series = self.state[(self.state.index >= tmin) & (self.state.index < tmax)][
+                "residuals"
+            ]
+        else:
+            series = self.state[(self.state.index >= tmin) & (self.state.index < tmax)][
+                "state"
+            ]
+
         # Get values in series
         data = series.values
-        
+
         # If time series segment is larger than input dimension of classifier
         if len(data) > input_len:
-            print('ERROR: Length of time series segment is too long for the classifier. You can modify the tmin and tmax parameters to select a smaller segment.')
+            print(
+                "ERROR: Length of time series segment is too long for the classifier. You can modify the tmin and tmax parameters to select a smaller segment."
+            )
             return
-        
+
         # Normalise by mean of absolute value
-        data_norm = data/(abs(data).mean())
+        data_norm = data / (abs(data).mean())
 
         # Prepend with zeros to make appropriate length for classifier
         num_zeros = input_len - len(data_norm)
-        input_data = np.concatenate((np.zeros(num_zeros),data_norm)).reshape(1,-1, 1)
-        
+        input_data = np.concatenate((np.zeros(num_zeros), data_norm)).reshape(1, -1, 1)
+
         # Get DL prediction
         dl_pred = classifier.predict(input_data, verbose=verbose)[0]
         # Put info into dataframe
-        dict_dl_pred = {i:val for (i,val) in zip(np.arange(len(dl_pred)), dl_pred)}
-        dict_dl_pred['time'] = series.index[-1]
-        dict_dl_pred['classifier'] = name      
+        dict_dl_pred = {i: val for (i, val) in zip(np.arange(len(dl_pred)), dl_pred)}
+        dict_dl_pred["time"] = series.index[-1]
+        dict_dl_pred["classifier"] = name
         df_dl_pred = pd.DataFrame(dict_dl_pred, index=[len(self.dl_preds)])
 
         # Append to dataframe contiaining DL predictions
         self.dl_preds = pd.concat([self.dl_preds, df_dl_pred], ignore_index=True)
 
-
-
-    def apply_classifier_inc(self, classifier, inc=10, name='c1', verbose=1):
-        '''
+    def apply_classifier_inc(self, classifier, inc=10, name="c1", verbose=1):
+        """
         Apply a deep learning classifier to incrementally increasing time
         series lengths. First prediction is made on time series segment from
         data point at index 0 to data point at index inc. Second prediction
         is made on time series segment from 0 to 2*inc. Third prediction is
         made on time series segment from 0 to 3*inc. Etc.
 
         Parameters
@@ -579,117 +659,117 @@
             TensorFlow classifier.
         inc : int, optional
             Increment to tmax (the end time of each time series segment) after each classification.
             The default is 10.
         name : str, optional
             Name assigned to the classifier. The default is 'c1'.
         verbose : int, optional
-            Verbosity of update messages from TensorFlow. 
+            Verbosity of update messages from TensorFlow.
             0 = silent, 1 = progress bar, 2 = single line.
             The default is 1.
 
         Returns
         -------
         None.
 
-        '''
-        
-        dt = self.state.index[1]-self.state.index[0]
+        """
+
+        dt = self.state.index[1] - self.state.index[0]
         tmin = self.state.index[0]
         tend = self.state.index[-1] if not self.transition else self.transition
-        tend += dt # Make transition point inclusive
-        
+        tend += dt  # Make transition point inclusive
+
         # Tmax values for each time series segment
-        tmax_vals = np.arange(tmin+inc, tend+dt, inc)
+        tmax_vals = np.arange(tmin + inc, tend + dt, inc)
         for tmax in tmax_vals:
-            self.apply_classifier(classifier, name=name, tmin=tmin, tmax=tmax, 
-                                verbose=verbose)
-    
-    
-
+            self.apply_classifier(
+                classifier, name=name, tmin=tmin, tmax=tmax, verbose=verbose
+            )
 
     def clear_dl_preds(self):
-        '''
+        """
         Clear the attribute *dl_preds*
 
         Returns
         -------
         None.
-        '''
-        
-        self.dl_preds = pd.DataFrame()
-
+        """
 
+        self.dl_preds = pd.DataFrame()
 
-    def compute_spectrum(self, rolling_window=0.25, ham_length=40,
-                         ham_offset=0.5, pspec_roll_offset=20,
-                         w_cutoff=1):
-        '''
+    def compute_spectrum(
+        self,
+        rolling_window=0.25,
+        ham_length=40,
+        ham_offset=0.5,
+        pspec_roll_offset=20,
+        w_cutoff=1,
+    ):
+        """
         Compute the power spectrum over a rolling window.
         Stores the power spectra as a DataFrame in TimeSeries.pspec
 
         Parameters
         ----------
         rolling_window : float
             Length of rolling window used to compute variance. Can be specified
             as an absolute value or as a proportion of the length of the
             data being analysed. Default is 0.25.
         ham_length : int
-            Length of the Hamming window used to compute the power spectrum. 
+            Length of the Hamming window used to compute the power spectrum.
             The default is 40.
         ham_offset : float
-            Hamming offset as a proportion of the Hamming window size. 
+            Hamming offset as a proportion of the Hamming window size.
             The default is 0.5.
         pspec_roll_offset : int
             Rolling window offset used when computing power spectra. Power spectrum
             computation is relatively expensive so this is rarely taken as 1
             (as is the case for the other EWS). The default is 20.
         w_cutoff : floag
             Cutoff frequency used in power spectrum. Given as a proportion of the
             maximum permissable frequency in the empirical power spectrum.
 
         Returns
         -------
         None.
 
-        '''
-        
+        """
+
         # Get time series data prior to transition
         if self.transition:
             df_pre = self.state[self.state.index <= self.transition]
         else:
             df_pre = self.state
 
         # Get absolute size of rollling window if given as a proportion
         if 0 < rolling_window <= 1:
             rw_absolute = int(rolling_window * len(df_pre))
         else:
             rw_absolute = rolling_window
 
         # If residuals column exists, compute over residuals.
-        if 'residuals' in df_pre.columns:
-            series = df_pre['residuals']
+        if "residuals" in df_pre.columns:
+            series = df_pre["residuals"]
         # Else, compute over state variable
         else:
-            series = df_pre['state']
+            series = df_pre["state"]
 
         # Number of components in the residual time-series
         num_comps = len(df_pre)
 
         # Rolling window offset (can make larger to save on computation time)
         roll_offset = int(pspec_roll_offset)
         # Time separation between data points (need for frequency values of power spectrum)
         dt = series.index[1] - series.index[0]
 
         # Initialise a list to store the power spectra
         list_pspec = []
 
         # Loop through window locations shifted by roll_offset
         for k in np.arange(0, num_comps - (rw_absolute - 1), roll_offset):
-
             # Select subset of series contained in window
             window_series = series.iloc[k : k + rw_absolute]
             # Asisgn the time value for the metrics (right end point of window)
             t_point = series.index[k + (rw_absolute - 1)]
 
             ## Compute the power spectrum using function pspec_welch
             pspec = helpers.pspec_welch(
@@ -704,47 +784,44 @@
             ## Create DataFrame for empirical power spectrum
             df_pspec_empirical = pspec.to_frame().reset_index()
             # Rename column
             df_pspec_empirical.rename(
                 columns={"Power spectrum": "empirical"}, inplace=True
             )
             # Include a column for the time-stamp
-            df_pspec_empirical['time'] = t_point * np.ones(len(pspec))
+            df_pspec_empirical["time"] = t_point * np.ones(len(pspec))
             list_pspec.append(df_pspec_empirical)
-        
+
         # Concatenate power spectra dataframes and store in attribute pspec
         self.pspec = pd.concat(list_pspec)
 
-
-
     def compute_smax(self):
-        '''
+        """
         Compute Smax (the maximum power in the power spectrum).
         This can only be applied after applying compute_spectrum().
         Stores Smax values in TimeSeries.ews_spec
 
         Returns
         -------
         None.
 
-        '''
-        
+        """
+
         if self.pspec is None:
-            print('ERROR: The power spectrum must be computed before computing\
+            print(
+                "ERROR: The power spectrum must be computed before computing\
                   spectral EWS such as Smax. The power spectrum can be\
-                  computed using compute_pspec()')
-        
-        smax_values = self.pspec[['time','power']].groupby(['time']).max()
-        self.ews_spec['smax'] = smax_values
-
-
+                  computed using compute_pspec()"
+            )
 
+        smax_values = self.pspec[["time", "power"]].groupby(["time"]).max()
+        self.ews_spec["smax"] = smax_values
 
     def compute_spec_type(self, sweep=False):
-        '''
+        """
         Fit the analytical forms of the Fold, Hopf and Null power spectrum
         to the empirical power spectrum. Get Akaike Information Criterion
         (AIC) weights to determine best fit.
         Store AIC weights in TimeSeries.ews_spec
         Store fitted power spectra in TimeSeries.pspec_fits
 
         Parameters
@@ -755,39 +832,40 @@
             longer computation. If 'False', intialisation parameter is taken as the
             'best guess'. The default is False.
 
         Returns
         -------
         None.
 
-        '''
-        
-        
+        """
+
         if self.pspec is None:
-            print('ERROR: The power spectrum must be computed before computing\
+            print(
+                "ERROR: The power spectrum must be computed before computing\
                   the spectrum type. The power spectrum can be\
-                  computed using compute_pspec()')    
-    
+                  computed using compute_pspec()"
+            )
+
         list_aic = []
         list_pspec_fits = []
-        
+
         # Loop through time values
-        for time in self.pspec['time'].unique():
-            pspec = self.pspec[self.pspec['time']==time]
-            pspec_series = pspec.set_index('frequency')['power']
-            
+        for time in self.pspec["time"].unique():
+            pspec = self.pspec[self.pspec["time"] == time]
+            pspec_series = pspec.set_index("frequency")["power"]
+
             ## Compute the AIC values
-            metrics = helpers.pspec_metrics(pspec_series, ews=['aic'], sweep=sweep)
+            metrics = helpers.pspec_metrics(pspec_series, ews=["aic"], sweep=sweep)
             dict_aic = {}
-            dict_aic['fold'] = metrics['AIC fold']
-            dict_aic['hopf'] = metrics['AIC hopf']
-            dict_aic['null'] = metrics['AIC null']
-            dict_aic['time'] = time
+            dict_aic["fold"] = metrics["AIC fold"]
+            dict_aic["hopf"] = metrics["AIC hopf"]
+            dict_aic["null"] = metrics["AIC null"]
+            dict_aic["time"] = time
             list_aic.append(dict_aic)
-            
+
             # Generate data to plot the fitted power spectra
 
             # Create fine-scale frequency values
             wVals = np.linspace(min(pspec.index), max(pspec.index), 100)
             # Fold fit
             pspec_fold = helpers.psd_fold(
                 wVals,
@@ -802,329 +880,562 @@
                 metrics["Params hopf"]["w0"],
             )
             # Null fit
             pspec_null = helpers.psd_null(wVals, metrics["Params null"]["sigma"])
 
             ## Put spectrum fits into a dataframe
             dict_fits = {
-                'time': time * np.ones(len(wVals)),
-                'frequency': wVals,
+                "time": time * np.ones(len(wVals)),
+                "frequency": wVals,
                 "fit fold": pspec_fold,
                 "fit hopf": pspec_hopf,
                 "fit null": pspec_null,
             }
             df_pspec_fits = pd.DataFrame(dict_fits)
             list_pspec_fits.append(df_pspec_fits)
 
         # Concatenate
-        df_aic = pd.DataFrame(list_aic).set_index('time')
+        df_aic = pd.DataFrame(list_aic).set_index("time")
         df_pspec_fits = pd.concat(list_pspec_fits)
 
         self.ews_spec = self.ews_spec.join(df_aic)
         self.pspec_fits = df_pspec_fits
-    
-
-
 
     def make_plotly(self, kendall_tau=True, ens_avg=False):
-        '''
+        """
         Make an interactive Plotly figure to view all EWS computed
 
         Parameters
         ----------
 
         kendall_tau : bool, optional
             Set as true to show Kendall tau values (if they have been computed)
             Default is True.
         ens_avg : bool, optional
-            Plot the ensenble average of DL predictions. 
+            Plot the ensenble average of DL predictions.
             Default is False.
 
         Returns
         -------
         Plotly figure
 
-        '''
-        
+        """
+
         # Trace colours
         colours = px.colors.qualitative.Plotly
         # Count number of panels for Plotly subplots
         row_count = 0
         # Always a row for state varialbe
         row_count += 1
         # Row for autocorrelation
-        ac_labels = [s for s in self.ews.columns if s[:2]=='ac']
-        if len(ac_labels)>0:
-            row_count+=1
+        ac_labels = [s for s in self.ews.columns if s[:2] == "ac"]
+        if len(ac_labels) > 0:
+            row_count += 1
         # Row for each other EWS
-        row_count += len(self.ews.columns)-len(ac_labels)
+        row_count += len(self.ews.columns) - len(ac_labels)
         # Row for Smax if included
-        if 'smax' in self.ews_spec.columns:
-            row_count+=1
+        if "smax" in self.ews_spec.columns:
+            row_count += 1
         # Row for AIC weights if computed
-        if 'fold' in self.ews_spec.columns:
-            row_count+=1
+        if "fold" in self.ews_spec.columns:
+            row_count += 1
         # Row for DL predictions if computed
-        if len(self.dl_preds.columns)>0:
-            row_count+=1
-        
+        if len(self.dl_preds.columns) > 0:
+            row_count += 1
+
         num_rows = row_count
-        row_count = 1 # reset row counter
-            
+        row_count = 1  # reset row counter
+
         # Make Plotly subplots frame
-        fig = make_subplots(rows=num_rows, cols=1, 
-                            shared_xaxes=True,
-                            x_title='Time',
-                            vertical_spacing=0.02
-                            )
-        
+        fig = make_subplots(
+            rows=num_rows,
+            cols=1,
+            shared_xaxes=True,
+            x_title="Time",
+            vertical_spacing=0.02,
+        )
+
         # Plot state variable
         fig.add_trace(
-            go.Scatter(x=self.state.index.values,
-                       y=self.state['state'].values,
-                       name='state',
-                       ),
-            row=row_count, col=1
-            )
-        fig.update_yaxes(title='State', row=row_count)
+            go.Scatter(
+                x=self.state.index.values,
+                y=self.state["state"].values,
+                name="state",
+            ),
+            row=row_count,
+            col=1,
+        )
+        fig.update_yaxes(title="State", row=row_count)
 
-        
         # Plot smoothing if computed
-        if 'smoothing' in self.state.columns:
+        if "smoothing" in self.state.columns:
             fig.add_trace(
-                go.Scatter(x=self.state.index.values,
-                           y=self.state['smoothing'].values,
-                           name='smoothing',
-                           ),
-                row=row_count, col=1
-                )
-        
+                go.Scatter(
+                    x=self.state.index.values,
+                    y=self.state["smoothing"].values,
+                    name="smoothing",
+                ),
+                row=row_count,
+                col=1,
+            )
+
         # Plot variance if computed
-        if 'variance' in self.ews.columns:
+        if "variance" in self.ews.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('variance' in self.ktau.keys()):
-                ktau = self.ktau['variance']
-                name = 'variance (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("variance" in self.ktau.keys()):
+                ktau = self.ktau["variance"]
+                name = "variance (ktau={:.2f})".format(ktau)
             else:
-                name = 'variance'
-            
+                name = "variance"
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews['variance'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Variance', row=row_count)
-            
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews["variance"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Variance", row=row_count)
+
         # Plot standard deviation if computed
-        if 'std' in self.ews.columns:
+        if "std" in self.ews.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('std' in self.ktau.keys()):
-                ktau = self.ktau['std']
-                name = 'std (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("std" in self.ktau.keys()):
+                ktau = self.ktau["std"]
+                name = "std (ktau={:.2f})".format(ktau)
             else:
-                name = 'std'
-            
+                name = "std"
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews['std'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='St. Dev.', row=row_count)
-            
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews["std"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="St. Dev.", row=row_count)
+
         # Plot coefficient of variation if computed
-        if 'cv' in self.ews.columns:
+        if "cv" in self.ews.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('cv' in self.ktau.keys()):
-                ktau = self.ktau['cv']
-                name = 'cv (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("cv" in self.ktau.keys()):
+                ktau = self.ktau["cv"]
+                name = "cv (ktau={:.2f})".format(ktau)
             else:
-                name = 'cv'
-            
+                name = "cv"
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews['cv'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Coeff. of Var.', row=row_count)
-            
-                                    
-            
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews["cv"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Coeff. of Var.", row=row_count)
+
         # Plot autocorrelation metrics if computed
-        if len(ac_labels)!=0:
-            row_count+=1
+        if len(ac_labels) != 0:
+            row_count += 1
         for ac_label in ac_labels:
-            
             # Add kendall tau to name
             if kendall_tau and (ac_label in self.ktau.keys()):
                 ktau = self.ktau[ac_label]
-                name = '{} (ktau={:.2f})'.format(ac_label, ktau)
+                name = "{} (ktau={:.2f})".format(ac_label, ktau)
             else:
-                name = ac_label            
-            
+                name = ac_label
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews[ac_label].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Autocorrelation', row=row_count)
-            
-                     
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews[ac_label].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Autocorrelation", row=row_count)
+
         # Plot skew if computed
-        if 'skew' in self.ews.columns:
+        if "skew" in self.ews.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('skew' in self.ktau.keys()):
-                ktau = self.ktau['skew']
-                name = 'skew (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("skew" in self.ktau.keys()):
+                ktau = self.ktau["skew"]
+                name = "skew (ktau={:.2f})".format(ktau)
             else:
-                name = 'skew'
-                
+                name = "skew"
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews['skew'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Skew', row=row_count)
-                        
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews["skew"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Skew", row=row_count)
+
         # Plot kurtosis if computed
-        if 'kurtosis' in self.ews.columns:
+        if "kurtosis" in self.ews.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('kurtosis' in self.ktau.keys()):
-                ktau = self.ktau['kurtosis']
-                name = 'kurtosis (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("kurtosis" in self.ktau.keys()):
+                ktau = self.ktau["kurtosis"]
+                name = "kurtosis (ktau={:.2f})".format(ktau)
             else:
-                name = 'kurtosis'   
-                
+                name = "kurtosis"
+
             fig.add_trace(
-                go.Scatter(x=self.ews.index.values,
-                           y=self.ews['kurtosis'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Kurtosis', row=row_count)
-               
-            
+                go.Scatter(
+                    x=self.ews.index.values,
+                    y=self.ews["kurtosis"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Kurtosis", row=row_count)
+
         # Plot Smax if computd
-        if 'smax' in self.ews_spec.columns:
+        if "smax" in self.ews_spec.columns:
             row_count += 1
-            
+
             # Add kendall tau to name
-            if kendall_tau and ('smax' in self.ktau.keys()):
-                ktau = self.ktau['smax']
-                name = 'smax (ktau={:.2f})'.format(ktau)
+            if kendall_tau and ("smax" in self.ktau.keys()):
+                ktau = self.ktau["smax"]
+                name = "smax (ktau={:.2f})".format(ktau)
             else:
-                name = 'smax'   
-                            
+                name = "smax"
+
             fig.add_trace(
-                go.Scatter(x=self.ews_spec.index.values,
-                           y=self.ews_spec['smax'].values,
-                           name=name,
-                           ),
-                row=row_count, col=1
-                )  
-            fig.update_yaxes(title='Smax', row=row_count)
-                          
-            
+                go.Scatter(
+                    x=self.ews_spec.index.values,
+                    y=self.ews_spec["smax"].values,
+                    name=name,
+                ),
+                row=row_count,
+                col=1,
+            )
+            fig.update_yaxes(title="Smax", row=row_count)
+
         # Plot AIC weights if computd
-        if 'fold' in self.ews_spec.columns:
+        if "fold" in self.ews_spec.columns:
             row_count += 1
-            aic_labels = ['fold', 'hopf', 'null']
+            aic_labels = ["fold", "hopf", "null"]
             for aic_label in aic_labels:
                 fig.add_trace(
-                    go.Scatter(x=self.ews_spec.index.values,
-                               y=self.ews_spec[aic_label].values,
-                               name=aic_label,
-                               ),
-                    row=row_count, col=1
-                    )  
-                
-            fig.update_yaxes(title='AIC weights', row=row_count)
-                       
-            
-                        
+                    go.Scatter(
+                        x=self.ews_spec.index.values,
+                        y=self.ews_spec[aic_label].values,
+                        name=aic_label,
+                    ),
+                    row=row_count,
+                    col=1,
+                )
+
+            fig.update_yaxes(title="AIC weights", row=row_count)
+
         # Plot DL predictions if computed
-        if len(self.dl_preds)>0:
+        if len(self.dl_preds) > 0:
             row_count += 1
-            class_labels = [s for s in self.dl_preds.columns if s not in ['time', 'classifier']]
-            classifiers = self.dl_preds['classifier'].unique()
-            
+            class_labels = [
+                s for s in self.dl_preds.columns if s not in ["time", "classifier"]
+            ]
+            classifiers = self.dl_preds["classifier"].unique()
+
             # If plotting predictions from every classifier
             if not ens_avg:
                 # Loop through class labels and classifier names
                 for idx, class_label in enumerate(class_labels):
                     for idx2, classifier in enumerate(classifiers):
-                        df_plot = self.dl_preds[self.dl_preds['classifier']==classifier]
+                        df_plot = self.dl_preds[
+                            self.dl_preds["classifier"] == classifier
+                        ]
                         fig.add_trace(
-                            go.Scatter(x=df_plot['time'].values,
-                                       y=df_plot[class_label].values,
-                                       name='DL class {}'.format(class_label),
-                                       legendgroup='DL class {}'.format(class_label),
-                                       showlegend=True if idx2==0 else False,
-                                       line=dict(color=colours[idx])
-                                       ),
-                            row=row_count, col=1
-                            )
-                        
+                            go.Scatter(
+                                x=df_plot["time"].values,
+                                y=df_plot[class_label].values,
+                                name="DL class {}".format(class_label),
+                                legendgroup="DL class {}".format(class_label),
+                                showlegend=True if idx2 == 0 else False,
+                                line=dict(color=colours[idx]),
+                            ),
+                            row=row_count,
+                            col=1,
+                        )
+
             # If plotting ensemble average over classifiers
             else:
-                df_plot = self.dl_preds.groupby(['time']).mean().reset_index()
+                df = self.dl_preds.drop(["classifier"], axis=1)  # JJV
+                df_plot = df.groupby(["time"]).mean().reset_index()  # JJV
+
                 # Loop through class labels
                 for idx, class_label in enumerate(class_labels):
                     fig.add_trace(
-                        go.Scatter(x=df_plot['time'].values,
-                                   y=df_plot[class_label].values,
-                                   name='DL class {}'.format(class_label),
-                                   line=dict(color=colours[idx])
-                                   ),
-                        row=row_count, col=1
-                        )    
-                    
-            fig.update_yaxes(title='DL predictions', row=row_count)
-                              
+                        go.Scatter(
+                            x=df_plot["time"].values,
+                            y=df_plot[class_label].values,
+                            name="DL class {}".format(class_label),
+                            line=dict(color=colours[idx]),
+                        ),
+                        row=row_count,
+                        col=1,
+                    )
 
+            fig.update_yaxes(title="DL predictions", row=row_count)
 
+        # Set figure dimensions
+        fig.update_layout(height=200 * num_rows, width=800)
 
-        # Set figure dimensions 
-        fig.update_layout(height=200*num_rows,
-                          width=800)
-        
         # Separation between legend entries
         fig.layout.legend.tracegroupgap = 0
 
         return fig
 
 
+class MultiTimeSeries:
+    """
+    Multivariate time series data on which to compute early warning signals.
+
+    Parameters
+    ----------
+    data : pandas.DataFrame
+        Contains each time series as a column. Index represents time values and
+        is carried over.
+    transition : float
+        Time value at which transition occurs, if any. If defined, early warning signals
+        are only computed up to this point in the time series
+    """
+
+    def __init__(self, data, transition=None):
+        # If data is not provided as a dataframe, flag error
+        if type(data) != pd.DataFrame:
+            print("\nERROR: data has been provided as type {}".format(type(data)))
+            print("Please provide data as a pandas DataFrame.\n")
+            return
+
+        # Set state and transition attributes
+        self.state = data
+        self.transition = float(transition) if transition else transition
+        self.var_names = data.columns
+
+        # Initialise other attributes
+        self.ews = pd.DataFrame(index=data.index)
+        self.ktau = dict()
+
+    def detrend(self, method="Gaussian", bandwidth=0.2, span=0.2):
+        """
+        Detrend the time series using a chosen method.
+        Add column to the dataframe for 'smoothing' and 'residuals' for each variable
+
+        Parameters
+        ----------
+        method : str, optional
+            Method of detrending to use.
+            Select from ['Gaussian', 'Lowess']
+            The default is 'Gaussian'.
+        bandwidth : float, optional
+            Bandwidth of Gaussian kernel. Provide as a proportion of data length
+            or as a number of data points. As in the R function ksmooth
+            (used by the earlywarnings package in R), we define the bandwidth
+            such that the kernel has its quartiles at +/- 0.25*bandwidth.
+            The default is 0.2.
+        span : float, optional
+            Span of time-series data used for Lowess filtering. Provide as a
+            proportion of data length or as a number of data points.
+            The default is 0.2.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # Error messages
+        if method not in ["Lowess", "Gaussian"]:
+            print("ERROR: {} is not a valid detrending method.\n".format(method))
+
+        # Get time series data prior to transition
+        if self.transition:
+            df_pre = self.state[self.state.index <= self.transition]
+        else:
+            df_pre = self.state
+
+        if method == "Gaussian":
+            # Get size of bandwidth in terms of num. datapoints if given as a proportion
+            if 0 < bandwidth <= 1:
+                bw_num = bandwidth * len(df_pre)
+            else:
+                bw_num = bandwidth
+
+            # Use the gaussian_filter function provided by Scipy
+            # Standard deviation of kernel given bandwidth
+            # Note that for a Gaussian, quartiles are at +/- 0.675*sigma
+            sigma = (0.25 / 0.675) * bw_num
 
+            # Do guassian smoothing on each variable
+            for var_name in self.var_names:
+                smooth_values = gf(df_pre[var_name].values, sigma=sigma, mode="reflect")
+                smooth_series = pd.Series(smooth_values, index=df_pre.index)
+                # Add smoothed data and residuals to the 'state' DataFrame
+                self.state["{}_smoothing".format(var_name)] = smooth_series
+                self.state["{}_residuals".format(var_name)] = (
+                    self.state[var_name] - self.state["{}_smoothing".format(var_name)]
+                )
 
+        if method == "Lowess":
+            # Convert span to a proportion of the length of the data
+            if not 0 < span <= 1:
+                span_prop = span / len(df_pre)
+            else:
+                span_prop = span
+
+            # Do Lowess smoothing on each variable
+            for var_name in self.var_names:
+                smooth_values = lowess(
+                    df_pre[var_name].values, df_pre.index.values, frac=span_prop
+                )[:, 1]
+                smooth_series = pd.Series(smooth_values, index=df_pre.index)
+                # Add smoothed data and residuals to the 'state' DataFrame
+                self.state["{}_smoothing".format(var_name)] = smooth_series
+                self.state["{}_residuals".format(var_name)] = (
+                    self.state[var_name] - self.state["{}_smoothing".format(var_name)]
+                )
+
+    def compute_covar(self, rolling_window=0.25, leading_eval=False):
+        """
+        Compute the covariance matrix over a rolling window.
+        If residuals have not been computed, computation will be
+        performed over state variable.
+
+        Put covariance matrices into self.covar
+        Put leading eigenvalue into self.ews
+
+        Parameters
+        ----------
+        rolling_window : float
+            Length of rolling window used to compute variance. Can be specified
+            as an absolute value or as a proportion of the length of the
+            data being analysed. Default is 0.25.
+        leading_eval : bool
+            Whether to compute the leading eigenvalue of the covariance matrix.
+            This has been suggested as an early warning signal (Carpenter et al. 2008, Ecol. Letters)
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # Get time series data prior to transition
+        if self.transition:
+            df_pre = self.state[self.state.index <= self.transition]
+        else:
+            df_pre = self.state
+
+        # Get absolute size of rollling window if given as a proportion
+        if 0 < rolling_window <= 1:
+            rw_absolute = int(rolling_window * len(df_pre))
+        else:
+            rw_absolute = rolling_window
+
+        # If residuals column exists, compute over residuals.
+        if "{}_residuals".format(self.var_names[0]) in df_pre.columns:
+            col_names_to_compute = [
+                "{}_residuals".format(var) for var in self.var_names
+            ]
+        else:
+            col_names_to_compute = self.var_names
+
+        # Compute covariance matrix
+        df_covar = df_pre[col_names_to_compute].rolling(window=rw_absolute).cov()
+        self.covar = df_covar
+
+        # Compute leading eigenvalue
+        if leading_eval:
+            covar_matrices = df_covar.values.reshape(
+                -1, len(self.var_names), len(self.var_names)
+            )
+            ar_evals = np.zeros(len(df_pre))
+            for idx, mat in enumerate(covar_matrices):
+                # Only compute eval if there are no NaN entries
+                if not np.any(np.isnan(mat)):
+                    evals, evecs = np.linalg.eig(mat)
+                    ar_evals[idx] = max(evals)
+                else:
+                    ar_evals[idx] = np.nan
+            series_evals = pd.Series(ar_evals, index=df_pre.index)
+            self.ews["covar_leading_eval"] = series_evals
+
+    def compute_corr(self, rolling_window=0.25):
+        """
+        Compute the (Pearson) correlation matrix over a rolling window.
+        If residuals have not been computed, computation will be
+        performed over state variable.
+
+        Put correlation matrices into self.corr
+
+        Parameters
+        ----------
+        rolling_window : float
+            Length of rolling window used to compute variance. Can be specified
+            as an absolute value or as a proportion of the length of the
+            data being analysed. Default is 0.25.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # Get time series data prior to transition
+        if self.transition:
+            df_pre = self.state[self.state.index <= self.transition]
+        else:
+            df_pre = self.state
+
+        # Get absolute size of rollling window if given as a proportion
+        if 0 < rolling_window <= 1:
+            rw_absolute = int(rolling_window * len(df_pre))
+        else:
+            rw_absolute = rolling_window
+
+        # If residuals column exists, compute over residuals.
+        if "{}_residuals".format(self.var_names[0]) in df_pre.columns:
+            col_names_to_compute = [
+                "{}_residuals".format(var) for var in self.var_names
+            ]
+        else:
+            col_names_to_compute = self.var_names
+
+        # Compute correlation matrix
+        df_corr = df_pre[col_names_to_compute].rolling(window=rw_absolute).corr()
+        self.corr = df_corr
 
 
 # -----------------------------
 # Eigenvalue reconstruction
 # ------------------------------
 
+
 def eval_recon_rolling(
     df_in,
     roll_window=0.4,
     roll_offset=1,
     smooth="Lowess",
     span=0.1,
     band_width=0.2,
@@ -1189,27 +1500,25 @@
     else:
         span = span
 
     # Compute smoothed data and residuals
     if smooth == "Gaussian":
         # Loop through variables
         for var in var_names:
-
             smooth_data = gf(df_pre[var].values, sigma=bw_size, mode="reflect")
             smooth_series = pd.Series(smooth_data, index=df_pre.index)
             residuals = df_pre[var].values - smooth_data
             resid_series = pd.Series(residuals, index=df_pre.index)
             # Add smoothed data and residuals to df_pre
             df_pre[var + "_s"] = smooth_series
             df_pre[var + "_r"] = resid_series
 
     if smooth == "Lowess":
         # Loop through variabless
         for var in var_names:
-
             smooth_data = lowess(df_pre[var].values, df_pre.index.values, frac=span)[
                 :, 1
             ]
             smooth_series = pd.Series(smooth_data, index=df_pre.index)
             residuals = df_pre[var].values - smooth_data
             resid_series = pd.Series(residuals, index=df_pre.index)
             # Add smoothed data and residuals to df_pre
@@ -1227,30 +1536,29 @@
     roll_offset = int(roll_offset)
 
     # Initialise a list of dictionaries containing eval data
     list_evaldata = []
 
     # Loop through window locations shifted by roll_offset
     for k in np.arange(0, num_comps - (rw_size - 1), roll_offset):
-
         # Select subset of residuals contained in window
         df_window = df_pre[[var + "_r" for var in var_names]].iloc[k : k + rw_size]
         # Asisgn the time value for the metrics (right end point of window)
         t_point = df_pre.index[k + (rw_size - 1)]
 
         # Do eigenvalue reconstruction on residuals
         dic_eval_recon = helpers.eval_recon(df_window)
         # Add time component
-        dic_eval_recon['time'] = t_point
+        dic_eval_recon["time"] = t_point
         # Add them to list
         list_evaldata.append(dic_eval_recon)
 
     # Create dataframe from list of dicts of eval data
     df_evaldata = pd.DataFrame(list_evaldata)
-    df_evaldata.set_index('time', inplace=True)
+    df_evaldata.set_index("time", inplace=True)
 
     # Create output dataframe that merges all useful info
     df_out = pd.concat(
         [
             df_in,
             df_pre[
                 [var + "_r" for var in var_names] + [var + "_s" for var in var_names]
@@ -1265,15 +1573,14 @@
 
 # ----------------------------------------------
 # Bootstrapping
 # –--------------------------------------------
 
 
 def block_bootstrap(series, n_samples, bs_type="Stationary", block_size=10):
-
     """
     Computes block-bootstrap samples of series.
 
     Args
     ----
     series: pd.Series
         Time-series data in the form of a Pandas Series indexed by time
@@ -1299,37 +1606,35 @@
     # Stationary bootstrapping
     if bs_type == "Stationary":
         bs = StationaryBootstrap(block_size, series)
 
         # Count for sample number
         count = 1
         for data in bs.bootstrap(n_samples):
-
             df_temp = pd.DataFrame(
-                {"sample": count, 'time': series.index.values, "x": data[0][0]}
+                {"sample": count, "time": series.index.values, "x": data[0][0]}
             )
             list_samples.append(df_temp)
             count += 1
 
     if bs_type == "Circular":
         bs = CircularBlockBootstrap(block_size, series)
 
         # Count for sample number
         count = 1
         for data in bs.bootstrap(n_samples):
-
             df_temp = pd.DataFrame(
-                {"sample": count, 'time': series.index.values, "x": data[0][0]}
+                {"sample": count, "time": series.index.values, "x": data[0][0]}
             )
             list_samples.append(df_temp)
             count += 1
 
     # Concatenate list of samples
     df_samples = pd.concat(list_samples)
-    df_samples.set_index(["sample", 'time'], inplace=True)
+    df_samples.set_index(["sample", "time"], inplace=True)
 
     # Output DataFrame of samples
     return df_samples
 
 
 def roll_bootstrap(
     raw_series,
@@ -1337,15 +1642,14 @@
     roll_window=0.25,
     roll_offset=1,
     upto="Full",
     n_samples=20,
     bs_type="Stationary",
     block_size=10,
 ):
-
     """
     Smooths raw_series and computes residuals over a rolling window.
     Bootstraps each segment and outputs samples.
 
     Args
     ----
     raw_series: pd.Series
@@ -1414,32 +1718,31 @@
     list_samples = []
 
     # Counter
     i = 0
 
     # Loop through window locations shifted by roll_offset
     for k in np.arange(0, num_comps - (rw_size - 1), roll_offset):
-
         # Select subset of series contained in window
         window_series = resid_series.iloc[k : k + rw_size]
         # Asisgn the time value for the metrics (right end point of window)
         t_point = resid_series.index[k + (rw_size - 1)]
 
         # Compute bootstrap samples of residauls within rolling window
         df_samples_temp = block_bootstrap(window_series, n_samples, bs_type, block_size)
         df_samples_temp.reset_index(inplace=True)
-        df_samples_temp['wintime'] = df_samples_temp['time']
-        
+        df_samples_temp["wintime"] = df_samples_temp["time"]
+
         # Add column with real time (end of window)
-        df_samples_temp['time'] = t_point
+        df_samples_temp["time"] = t_point
 
         # Reorganise index
-        
+
         df_samples_temp.reset_index(inplace=True)
-        df_samples_temp.set_index(['time', "sample", 'wintime'], inplace=True)
+        df_samples_temp.set_index(["time", "sample", "wintime"], inplace=True)
 
         # Append the list of samples
         list_samples.append(df_samples_temp)
 
         #        # Print update
         #        if i % 1 ==0:
         #            print('Bootstrap samples for window at t = %.2f complete' % (t_point))
```

### Comparing `ewstools-2.1.0/ewstools/helpers.py` & `ewstools-2.1.2/ewstools/helpers.py`

 * *Files identical despite different names*

### Comparing `ewstools-2.1.0/ewstools/models.py` & `ewstools-2.1.2/ewstools/models.py`

 * *Files identical despite different names*

### Comparing `ewstools-2.1.0/ewstools.egg-info/PKG-INFO` & `ewstools-2.1.2/ewstools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewstools
-Version: 2.1.0
+Version: 2.1.2
 Summary: Python package to compute early warning signals (EWS) 
 Home-page: https://github.com/ThomasMBury/ewstools
 Author: Thomas M Bury
 Author-email: tombury182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,42 +12,43 @@
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/ewstools.svg)](https://badge.fury.io/py/ewstools)
 [![Downloads](https://pepy.tech/badge/ewstools)](https://pepy.tech/project/ewstools)
 [![Documentation Status](https://readthedocs.org/projects/ewstools/badge/?version=latest)](https://ewstools.readthedocs.io/en/latest/?badge=latest)
 [![tests](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ThomasMBury/ewstools/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/ThomasMBury/ewstools/branch/main/graph/badge.svg?token=Q5LGRV6TLF)](https://codecov.io/gh/ThomasMBury/ewstools)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05038/status.svg)](https://doi.org/10.21105/joss.05038)
 
 # ewstools
 **A Python package for early warning signals (EWS) of bifurcations in time series data.**
 
 ## Overview
 
 Many systems in nature and society have the capacity to undergo critical transitions--sudden and profound changes in dynamics that are hard to reverse. Examples include the outbreak of disease, the collapse of an ecosystem, or the onset of a cardiac arrhythmia. From a mathematical perspective, these transitions may be understood as the crossing of a bifurcation (tipping point) in an appropriate dynamical system model. In 2009, Scheffer and colleagues proposed early warning signals (EWS) for bifurcations based on statistics of noisy fluctuations in time series data ([Scheffer et al. 2009](https://www.nature.com/articles/nature08227)). This spurred massive interest in the subject, resulting in a multitude of different EWS for anticipating bifurcations ([Clements & Ozgul 2018](https://onlinelibrary.wiley.com/doi/full/10.1111/ele.12948)). More recently, EWS from deep learning classifiers have outperformed conventional EWS on several model and empirical datasets, whilst also providing information on the type of bifurcation ([Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118)).
 
 `ewstools` is an accessible toolbox for computing, analysing and visualising EWS in time series data. It complements an existing EWS package in R ([Dakos et al. 2012](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0041010)). Given the recent surge in popularity of the Python programming langauge ([PYPL, 2022](https://pypl.github.io/PYPL.html)), a Python-based implementation of EWS should be useful.
 
 The package provides:
 
-  - An intuitive, object-oriented framework for working with EWS in a given time series
+  - An intuitive, object-oriented framework for computing EWS for a given time series
   - Time series detrending methods using
     - A Gaussian kernel
     - LOWESS (Locally Weighted Scatterplot Smoothing)
   - Computation of CSD-based early warning signals including:
     - Variance and associated metrics (standard deviation, coefficient of variation)
     - Autocorrelation (at specified lag times)
     - Higher-order statistical moments (skewness, kurtosis)
     - Power spectrum and associated metrics
+    - Various entropy measures
   - Computation of Kendall tau values to quantify trends
   - Application of deep learning classifiers for bifurcation prediction as in [Bury et al. 2021](https://www.pnas.org/doi/10.1073/pnas.2106140118).
-  - Block-bootstrapping of time-series to obtain confidence intervals on EWS estimates
   - Visualisation tools to display output
   - Built-in theoretical models to test EWS
 
-`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
+`ewstools` makes use of [pandas](https://pandas.pydata.org/) for dataframe handling, [numpy](https://numpy.org/) for fast numerical computing, [plotly](https://plotly.com/graphing-libraries/) for visuliastion, [lmfit](https://lmfit.github.io/lmfit-py/) for least-squares minimisation, [arch](https://github.com/bashtage/arch) for bootstrapping methods, [EntropyHub](https://www.entropyhub.xyz/index.html) for entropy computations, [statsmodels](https://www.statsmodels.org/stable/index.html) and [scipy](https://scipy.org/) for detrending methods, and [TensorFlow](https://www.tensorflow.org/install) for deep learning.
 
 
 ## Install
 
 Requires Python 3.7 or later. You can install `ewstools` with pip using the commands
 
 ```bash
@@ -65,15 +66,15 @@
 'numpy>=1.14.0',
 'plotly>=2.3.0',
 'lmfit>=0.9.0', 
 'arch>=4.4',
 'statsmodels>=0.9.0',
 'scipy>=1.0.1',
 ```
-and should be installed automatically. To use any of the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) v2.0.0 or later.
+and should be installed automatically. To use the deep learning functionality, you will need to install [TensorFlow](https://www.tensorflow.org/install) with version later than 2.0 and earlier than 2.12.
 
 To install the latest *development* version, use the command
 ```bash
 pip install git+https://github.com/thomasmbury/ewstools.git#egg=ewstools
 ```
 NB: the development version comes with the risk of undergoing continual changes, and has not undergone the level of scrutiny of official releases.
 
@@ -137,14 +138,10 @@
 
 This work is currently supported by an FRQNT (Fonds de recherche du Québec - Nature et Technologies) postdoctoral research scholarship awarded to Dr. Thomas Bury. In the past, it has also been supported by NSERC (Natural Sciences and Engineering Research Council) Discovery Grants awarded to Dr. Chris Bauch and Dr. Madhur Anand.
 
 ## Citation info
 
 If you like the respoitory, please give it a star :D
 
-If your research uses the deep learning functionality of `ewstools`, please cite
+If your research makes use of it, please cite
 
-Bury, Thomas M., et al. "[Deep learning for early warning signals of tipping points.](https://www.pnas.org/doi/abs/10.1073/pnas.2106140118)" *Proceedings of the National Academy of Sciences* 118.39 (2021): e2106140118.
-
-If your research computes spectral EWS using `ewstools`, please cite
-
-Bury, Thomas M., Chris T. Bauch, and Madhur Anand. "[Detecting and distinguishing tipping points using spectral early warning signals.](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2020.0482)" *Journal of the Royal Society Interface* 17.170 (2020): 20200482.
+Bury, Thomas M. "[ewstools: A Python package for early warning signals of bifurcations in time series data.](https://joss.theoj.org/papers/10.21105/joss.05038.pdf)" *Journal of Open Source Software* 8.82 (2023): 5038.
```

### Comparing `ewstools-2.1.0/setup.py` & `ewstools-2.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = ['pandas>=0.23.0',
-                'numpy>=1.14.0',
-                'plotly>=2.3.0',
-                'lmfit>=0.9.0', 
-                'arch>=4.4',
-                'statsmodels>=0.9.0',
-                'scipy>=1.0.1',
-                'deprecation>=2.0',
-                ]
+requirements = [
+    "pandas>=0.23.0",
+    "numpy>=1.14.0",
+    "plotly>=2.3.0",
+    "lmfit>=0.9.0",
+    "arch>=4.4",
+    "statsmodels>=0.9.0",
+    "scipy>=1.0.1",
+    "deprecation>=2.0",
+    "entropyhub>=2.0",
+]
 
 setuptools.setup(
     name="ewstools",
-    version="2.1.0",
+    version="2.1.2",
     author="Thomas M Bury",
     author_email="tombury182@gmail.com",
     description="""Python package to compute early warning signals (EWS) 
     from time series data""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ThomasMBury/ewstools",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

