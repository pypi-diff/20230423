# Comparing `tmp/monaco-0.9.0.tar.gz` & `tmp/monaco-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monaco-0.9.0.tar", max compression
+gzip compressed data, was "monaco-0.9.1.tar", max compression
```

## Comparing `monaco-0.9.0.tar` & `monaco-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0    35823 2020-04-23 19:30:06.746000 monaco-0.9.0/LICENSE.md
--rwxr-xr-x   0        0        0     5600 2022-08-15 23:45:10.194915 monaco-0.9.0/README.md
--rwxr-xr-x   0        0        0     1335 2023-02-08 21:27:01.301055 monaco-0.9.0/pyproject.toml
--rwxr-xr-x   0        0        0      657 2022-05-02 00:41:48.820075 monaco-0.9.0/src/monaco/__init__.py
--rwxr-xr-x   0        0        0     2667 2022-09-26 00:04:02.092753 monaco-0.9.0/src/monaco/case_runners.py
--rwxr-xr-x   0        0        0    11412 2022-08-19 05:24:43.097752 monaco-0.9.0/src/monaco/dvars_sensitivity.py
--rwxr-xr-x   0        0        0     3970 2022-05-02 00:41:48.834074 monaco-0.9.0/src/monaco/gaussian_statistics.py
--rwxr-xr-x   0        0        0     6823 2022-05-10 04:28:43.442217 monaco-0.9.0/src/monaco/helper_functions.py
--rwxr-xr-x   0        0        0     9987 2022-05-08 20:08:52.523566 monaco-0.9.0/src/monaco/integration_statistics.py
--rwxr-xr-x   0        0        0     5595 2022-07-12 04:48:24.481448 monaco-0.9.0/src/monaco/mc_case.py
--rwxr-xr-x   0        0        0     2944 2022-07-09 21:57:18.586042 monaco-0.9.0/src/monaco/mc_enums.py
--rwxr-xr-x   0        0        0    17749 2022-07-12 04:48:24.497084 monaco-0.9.0/src/monaco/mc_multi_plot.py
--rwxr-xr-x   0        0        0    52827 2023-02-08 21:27:01.317055 monaco-0.9.0/src/monaco/mc_plot.py
--rwxr-xr-x   0        0        0     4695 2022-05-02 00:41:48.913071 monaco-0.9.0/src/monaco/mc_sampling.py
--rwxr-xr-x   0        0        0    57654 2023-02-08 22:27:04.659649 monaco-0.9.0/src/monaco/mc_sim.py
--rwxr-xr-x   0        0        0     8484 2022-07-12 04:48:24.528451 monaco-0.9.0/src/monaco/mc_val.py
--rwxr-xr-x   0        0        0    20887 2022-06-15 05:37:24.928350 monaco-0.9.0/src/monaco/mc_var.py
--rwxr-xr-x   0        0        0    25180 2022-07-13 17:17:08.685177 monaco-0.9.0/src/monaco/mc_varstat.py
--rwxr-xr-x   0        0        0    20214 2022-07-09 21:57:18.644780 monaco-0.9.0/src/monaco/order_statistics.py
--rwxr-xr-x   0        0        0     3517 2022-05-02 00:41:48.958072 monaco-0.9.0/src/monaco/tqdm_dask_distributed.py
--rw-r--r--   0        0        0     6769 1970-01-01 00:00:00.000000 monaco-0.9.0/setup.py
--rw-r--r--   0        0        0     7144 1970-01-01 00:00:00.000000 monaco-0.9.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2020-04-23 19:30:06.746000 monaco-0.9.1/LICENSE.md
+-rwxr-xr-x   0        0        0     5546 2023-02-16 16:45:30.490587 monaco-0.9.1/README.md
+-rwxr-xr-x   0        0        0     1401 2023-02-16 17:09:32.826280 monaco-0.9.1/pyproject.toml
+-rwxr-xr-x   0        0        0      657 2022-05-02 00:41:48.820075 monaco-0.9.1/src/monaco/__init__.py
+-rwxr-xr-x   0        0        0     2667 2022-09-26 00:04:02.092753 monaco-0.9.1/src/monaco/case_runners.py
+-rwxr-xr-x   0        0        0    11472 2023-02-16 16:45:30.630698 monaco-0.9.1/src/monaco/dvars_sensitivity.py
+-rwxr-xr-x   0        0        0     3970 2022-05-02 00:41:48.834074 monaco-0.9.1/src/monaco/gaussian_statistics.py
+-rwxr-xr-x   0        0        0     6823 2022-05-10 04:28:43.442217 monaco-0.9.1/src/monaco/helper_functions.py
+-rwxr-xr-x   0        0        0     9987 2022-05-08 20:08:52.523566 monaco-0.9.1/src/monaco/integration_statistics.py
+-rwxr-xr-x   0        0        0     5595 2022-07-12 04:48:24.481448 monaco-0.9.1/src/monaco/mc_case.py
+-rwxr-xr-x   0        0        0     2944 2022-07-09 21:57:18.586042 monaco-0.9.1/src/monaco/mc_enums.py
+-rwxr-xr-x   0        0        0    17749 2022-07-12 04:48:24.497084 monaco-0.9.1/src/monaco/mc_multi_plot.py
+-rwxr-xr-x   0        0        0    52827 2023-02-08 21:27:01.317055 monaco-0.9.1/src/monaco/mc_plot.py
+-rwxr-xr-x   0        0        0     4695 2022-05-02 00:41:48.913071 monaco-0.9.1/src/monaco/mc_sampling.py
+-rwxr-xr-x   0        0        0    57654 2023-02-08 22:27:04.659649 monaco-0.9.1/src/monaco/mc_sim.py
+-rwxr-xr-x   0        0        0     8484 2022-07-12 04:48:24.528451 monaco-0.9.1/src/monaco/mc_val.py
+-rwxr-xr-x   0        0        0    20887 2022-06-15 05:37:24.928350 monaco-0.9.1/src/monaco/mc_var.py
+-rwxr-xr-x   0        0        0    24734 2023-02-16 16:45:30.653931 monaco-0.9.1/src/monaco/mc_varstat.py
+-rwxr-xr-x   0        0        0    20214 2022-07-09 21:57:18.644780 monaco-0.9.1/src/monaco/order_statistics.py
+-rwxr-xr-x   0        0        0     3517 2022-05-02 00:41:48.958072 monaco-0.9.1/src/monaco/tqdm_dask_distributed.py
+-rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 monaco-0.9.1/setup.py
+-rw-r--r--   0        0        0     7268 1970-01-01 00:00:00.000000 monaco-0.9.1/PKG-INFO
```

### Comparing `monaco-0.9.0/LICENSE.md` & `monaco-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/README.md` & `monaco-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-<p float="center" align="center">
-<img width="570" height="150" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/monaco_logo.png">  
-</p>
-
-![Release](https://img.shields.io/github/v/release/scottshambaugh/monaco?sort=semver)
-![Builds](https://github.com/scottshambaugh/monaco/actions/workflows/builds.yml/badge.svg)
-![Tests](https://github.com/scottshambaugh/monaco/actions/workflows/tests.yml/badge.svg)
-[![Docs](https://readthedocs.org/projects/monaco/badge/?version=latest)](https://monaco.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monaco)
-
-Quantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.
-
-### Overview
-
-At the heart of all serious forecasting, whether that be of elections, the spread of pandemics, weather, or the path of a rocket on its way to Mars, is a statistical tool known as the [Monte Carlo method](https://en.wikipedia.org/wiki/Monte_Carlo_method). The Monte Carlo method, named for the rolling of the dice at the famous Monte Carlo casino located in Monaco, allows you to quantify uncertainty by introducing randomness to otherwise deterministic processes, and seeing what the range of results is.
-
-<p float="left" align="center">
-<img width="500" height="250" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/analysis_process.png">
-</p>
-
-`monaco` is a python library for analyzing uncertainties and sensitivities in your computational models by setting up, running, and analyzing a Monte Carlo simulation wrapped around that model. Users can define random input variables drawn using chosen sampling methods from any of SciPy's continuous or discrete distributions (including custom distributions), preprocess and structure that data as needed to feed to their main simulation, run that simulation in parallel anywhere from 1 to millions of times, and postprocess the simulation outputs to obtain meaningful, statistically significant conclusions. Plotting and statistical functions specific to use cases that might be encountered are provided, and repeatability of results is ensured through careful management of random seeds.
-
-<p float="left" align="center">
-<img width="350" height="350" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/baseball_trajectory.png">
-<img width="440" height="330" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/launch_angle_vs_landing.png">
-</p>
-
-### Quick Start
-First, install `monaco`:
-```
-pip install monaco
-```
-Then, copy the two files from the [template directory](https://github.com/scottshambaugh/monaco/tree/main/template), which contains a simple, well commented Monte Carlo simulation of flipping coins. That link also contains some exercises for you to do, to help you familiarize yourself with how `monaco` is structured.
-
-After working through the template exercises, check out the other [examples](https://github.com/scottshambaugh/monaco/tree/main/examples) for inspiration and more in-depth usage of `monaco`'s features.
-
-### Documentation / API Reference / SciPy 2022 Talk
-
-Documentation is being built up - read the docs here: https://monaco.readthedocs.io
-
-Currently there is a complete [API reference](https://monaco.readthedocs.io/en/latest/api_reference.html), more detailed [installation, test, and publishing](https://monaco.readthedocs.io/en/latest/installation.html) instructions, an overview of the [basic architecture](https://monaco.readthedocs.io/en/latest/basic_architecture.html) and [basic workflow](https://monaco.readthedocs.io/en/latest/basic_workflow.html), and some details on [statistical distributions](https://monaco.readthedocs.io/en/latest/statistical_distributions.html) and [sampling methods](https://monaco.readthedocs.io/en/latest/sampling_methods.html). 
-
-Monaco was presented at the SciPy 2022 Conference, and the conference resources should give another good overview of the library. Check out [the paper](https://conference.scipy.org/proceedings/scipy2022/pdfs/scott_shambaugh.pdf), [the video of the talk](https://www.youtube.com/watch?v=yB539OIol_s), and [the talk's slides and notebooks](https://github.com/scottshambaugh/monaco-scipy2022).
-
-### License / Citation
-Copyright 2020-2022 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).
-
-If you use `monaco` to do research that gets published, please cite the conference paper using the below or [monaco.bib](monaco.bib):    
-> W. Scott Shambaugh (2022). Monaco: A Monte Carlo Library for Performing Uncertainty and Sensitivity Analyses. *In Proceedings of the 21st Python in Science Conference* (pp. 202 - 208).
-
-### Further Reading
-* [Hanson, J. M., and B. B. Beard. "Applying Monte Carlo simulation to launch vehicle design and requirements analysis." National Aeronautics and Space Administration, Marshall Space Flight Center, 1 September 2010.](https://ntrs.nasa.gov/citations/20100038453)
-* [Razavi, S. et. al. "The future of sensitivity analysis: an essential discipline for systems modeling and policy support." Environmental Modelling & Software Volume 137, March 2021.](https://www.sciencedirect.com/science/article/pii/S1364815220310112)
-* [Satelli, A. et. al. "Why so many published sensitivity analyses are false: A systematic review of sensitivity analysis practices." Environmental Modelling & Software Volume 114, April 2019.](https://www.sciencedirect.com/science/article/pii/S1364815218302822)
+<p float="center" align="center">
+<img width="570" height="150" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/monaco_logo.png">  
+</p>
+
+![Release](https://img.shields.io/github/v/release/scottshambaugh/monaco?sort=semver)
+![Builds](https://github.com/scottshambaugh/monaco/actions/workflows/builds.yml/badge.svg)
+![Tests](https://github.com/scottshambaugh/monaco/actions/workflows/tests.yml/badge.svg)
+[![Docs](https://readthedocs.org/projects/monaco/badge/?version=latest)](https://monaco.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monaco)
+
+Quantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.
+
+### Overview
+
+At the heart of all serious forecasting, whether that be of elections, the spread of pandemics, weather, or the path of a rocket on its way to Mars, is a statistical tool known as the [Monte Carlo method](https://en.wikipedia.org/wiki/Monte_Carlo_method). The Monte Carlo method, named for the rolling of the dice at the famous Monte Carlo casino located in Monaco, allows you to quantify uncertainty by introducing randomness to otherwise deterministic processes, and seeing what the range of results is.
+
+<p float="left" align="center">
+<img width="500" height="250" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/analysis_process.png">
+</p>
+
+`monaco` is a python library for analyzing uncertainties and sensitivities in your computational models by setting up, running, and analyzing a Monte Carlo simulation wrapped around that model. Users can define random input variables drawn using chosen sampling methods from any of SciPy's continuous or discrete distributions (including custom distributions), preprocess and structure that data as needed to feed to their main simulation, run that simulation in parallel anywhere from 1 to millions of times, and postprocess the simulation outputs to obtain meaningful, statistically significant conclusions. Plotting and statistical functions specific to use cases that might be encountered are provided, and repeatability of results is ensured through careful management of random seeds.
+
+<p float="left" align="center">
+<img width="350" height="350" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/baseball_trajectory.png">
+<img width="440" height="330" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/launch_angle_vs_landing.png">
+</p>
+
+### Quick Start
+First, install `monaco`:
+```
+pip install monaco
+```
+Then, copy the two files from the [template directory](https://github.com/scottshambaugh/monaco/tree/main/template), which contains a simple, well commented Monte Carlo simulation of flipping coins. That link also contains some exercises for you to do, to help you familiarize yourself with how `monaco` is structured.
+
+After working through the template exercises, check out the other [examples](https://github.com/scottshambaugh/monaco/tree/main/examples) for inspiration and more in-depth usage of `monaco`'s features.
+
+### Documentation / API Reference / SciPy 2022 Talk
+
+Documentation is being built up - read the docs here: https://monaco.readthedocs.io
+
+Currently there is a complete [API reference](https://monaco.readthedocs.io/en/latest/api_reference.html), more detailed [installation, test, and publishing](https://monaco.readthedocs.io/en/latest/installation.html) instructions, an overview of the [basic architecture](https://monaco.readthedocs.io/en/latest/basic_architecture.html) and [basic workflow](https://monaco.readthedocs.io/en/latest/basic_workflow.html), and some details on [statistical distributions](https://monaco.readthedocs.io/en/latest/statistical_distributions.html) and [sampling methods](https://monaco.readthedocs.io/en/latest/sampling_methods.html). 
+
+Monaco was presented at the SciPy 2022 Conference, and the conference resources should give another good overview of the library. Check out [the paper](https://conference.scipy.org/proceedings/scipy2022/pdfs/scott_shambaugh.pdf), [the video of the talk](https://www.youtube.com/watch?v=yB539OIol_s), and [the talk's slides and notebooks](https://github.com/scottshambaugh/monaco-scipy2022).
+
+### License / Citation
+Copyright 2020-2023 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).
+
+If you use `monaco` to do research that gets published, please cite the conference paper using the below or [monaco.bib](monaco.bib):    
+> W. Scott Shambaugh (2022). Monaco: A Monte Carlo Library for Performing Uncertainty and Sensitivity Analyses. *In Proceedings of the 21st Python in Science Conference* (pp. 202 - 208).
+
+### Further Reading
+* [Hanson, J. M., and B. B. Beard. "Applying Monte Carlo simulation to launch vehicle design and requirements analysis." National Aeronautics and Space Administration, Marshall Space Flight Center, 1 September 2010.](https://ntrs.nasa.gov/citations/20100038453)
+* [Razavi, S. et. al. "The future of sensitivity analysis: an essential discipline for systems modeling and policy support." Environmental Modelling & Software Volume 137, March 2021.](https://www.sciencedirect.com/science/article/pii/S1364815220310112)
+* [Satelli, A. et. al. "Why so many published sensitivity analyses are false: A systematic review of sensitivity analysis practices." Environmental Modelling & Software Volume 114, April 2019.](https://www.sciencedirect.com/science/article/pii/S1364815218302822)
```

### Comparing `monaco-0.9.0/pyproject.toml` & `monaco-0.9.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monaco"
-version = "0.9.0"
+version = "0.9.1"
 description = "Quantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library."
 authors = ["Scott Shambaugh <scott@theshamblog.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/scottshambaugh/monaco/"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,39 +12,41 @@
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<3.11"
-numpy = "^1.22"
+python = ">=3.8.0,<3.12"
+numpy = "^1.23"
 scipy = "^1.10"
 matplotlib = "^3.6"
 tqdm = "^4.0"
 psutil = "^5.0"
-numba = "^0.55"
 distributed = "^2022"
 cloudpickle = "^2.0"
 pillow = ">=9.3.0"
 
 pandas = {version = "^1.5", optional = true}
 
+numba = {version = "^0.56", python = "<3.11", optional = true}
+
 sphinx = {version = "^4.2", optional = true}
 sphinx_rtd_theme = {version = "^1.0", optional = true}
 myst-parser = {version = ">=0.15", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2"
 coverage = "^7.0"
 mypy = ">=1.0"
 flake8 = "^5.000"
 pre-commit = "^3.0"
 requests = "^2.0"
 
 [tool.poetry.extras]
 pandas = ["pandas"]
+numba = ["numba"]
 docs = ["sphinx", "sphinx_rtd_theme", "myst-parser"]
 
 [build-system]
 requires = ["setuptools", "poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `monaco-0.9.0/src/monaco/__init__.py` & `monaco-0.9.1/src/monaco/__init__.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/case_runners.py` & `monaco-0.9.1/src/monaco/case_runners.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/dvars_sensitivity.py` & `monaco-0.9.1/src/monaco/dvars_sensitivity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,352 +1,367 @@
-# dvars_sensitivity.py
-from __future__ import annotations
-
-# Somewhat hacky type checking to avoid circular imports:
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from monaco.mc_sim import Sim
-
-from monaco.helper_functions import vprint
-import numpy as np
-from scipy.optimize import minimize
-from numba import jit
-
-
-def calc_sensitivities(sim        : 'Sim',
-                       outvarname : str,
-                       Hj         : float = 1.0,
-                       tol        : float = 1e-6,
-                       verbose    : bool  = False,
-                       ) -> tuple[np.ndarray, np.ndarray]:
-    """
-    Calculates the global sensitivity indices and ratios for a specific output
-    variable to each of a simulation's input variables.
-
-    This implements the D-VARS algorithm as dscribed in Reference [1]_ to
-    calculate global sensitivity indices from a set of given data. The
-    implementation largely follows the Reference's supplementary notes, though
-    Multi-SQP is replaced with scipy's minimize function implementing L-BFGS-B.
-    See also Reference [2]_ for some theoretical background on the VARS and
-    IVARS methods of calculating sensitivity indices.
-
-    Parameters
-    ----------
-    sim : monaco.mc_sim.Sim
-        The input simulation.
-    outvarname : str
-        The name of the output variable to calculate sensitivities for. Note
-        that the output variable must be scalar.
-    Hj : float, default: 1.0
-        The fraction of the total parameter space to integrate over. Note that
-        the linear correlation function only has one hyperparameter, so as the
-        Reference notes it is unable to distinguish variogram effects at varying
-        length scales. So, this should not be set to anything other than 1 in
-        practice.
-    tol : float, default 1e-6
-        The convergence tolerance for scipy's minimize function acting on the
-        negative log likelihood function.
-    verbose : bool, default False
-        Whether to print diagnostic information.
-
-    Returns
-    -------
-    sensitivities : numpy.ndarray
-        The global sensitivity indices for the output variable for each of the
-        sim's input variables.
-    ratios : numpy.ndarray
-        The global sensitivity ratios for the output variable for each of the
-        sim's input variables, essentially the fraction of each input variable's
-        ability to explain the output variance.
-
-    References
-    ----------
-    .. [1] Sheikholeslami, Razi, and Saman Razavi. "A fresh look at variography:
-           measuring dependence and possible sensitivities across geophysical
-           systems from any given data." Geophysical Research Letters 47.20
-           (2020): e2020GL089829.
-    .. [2] Razavi, Saman, and Hoshin V. Gupta. "A new framework for
-           comprehensive, robust, and efficient global sensitivity analysis:
-           1. Theory." Water Resources Research 52.1 (2016): 423-439.
-    """
-    phi_opt = calc_phi_opt(sim, outvarname, tol, verbose)
-
-    variance = np.var(np.array([sim.outvars[outvarname].nums]))
-    sensitivities = np.zeros(sim.ninvars)
-    for j in range(sim.ninvars):
-        sensitivities[j] = calc_Gammaj(Hj, phi_opt[j], variance)
-    ratios = sensitivities/sum(sensitivities)
-
-    return sensitivities, ratios
-
-
-def calc_phi_opt(sim        : 'Sim',
-                 outvarname : str,
-                 tol        : float = 1e-6,
-                 verbose    : bool = False
-                 ) -> np.ndarray:
-    """
-    Calculate the optimal hyperparameters for the covariance functions between
-    the output variable and each of the input variables via maximum likelihood
-    estimation (MLE). MLE works by minimizing a negative log-likelihood
-    function.
-
-    Parameters
-    ----------
-    sim : monaco.mc_sim.Sim
-        The input simulation.
-    outvarname : str
-        The name of the output variable to calculate sensitivities for. Note
-        that the output variable must be scalar.
-    tol : float, default 1e-6
-        The convergence tolerance for scipy's minimize function acting on the
-        negative log likelihood function.
-    verbose : bool, default False
-        Whether to print diagnostic information.
-
-    Returns
-    -------
-    phi_opt : numpy.ndarray
-        The learned hyperparameters for the covariance functions.
-    """
-    phi_max = 1e6
-    phi_min = 0
-    phi0 = 1
-
-    phi0s = []
-    bounds = []
-    for _ in range(sim.ninvars):
-        phi0s.append(phi0)
-        bounds.append((phi_min, phi_max))
-
-    vprint(sim.verbose, 'Calculating optimal hyperparameters Φ for ' +
-                       f"'{outvarname}' covariances...")
-    X, Y = full_states(sim, outvarname)
-    res = minimize(L_runner, phi0s, args=(X, Y, verbose), bounds=bounds,
-                   tol=tol, method='L-BFGS-B')
-    phi_opt = res.x
-    vprint(sim.verbose, 'Done calculating optimal hyperparameters.')
-
-    return phi_opt
-
-
-def full_states(sim : 'Sim',
-                outvarname : str,
-                ) -> tuple[np.ndarray, np.ndarray]:
-    """
-    Get the full input and output states in combined matrices.
-
-    Parameters
-    ----------
-    sim : monaco.mc_sim.Sim
-        The input simulation.
-    outvarname : str
-        The name of the output variable to calculate sensitivities for. Note
-        that the output variable must be scalar.
-
-    Returns
-    -------
-    X : numpy.ndarray
-        The input variables' percentiles.
-    Y : numpy.ndarray
-        The output variable's nums.
-    """
-    X = np.zeros((sim.ncases, sim.ninvars))
-    Y = np.zeros((sim.ncases, 1))
-    for i, varname in enumerate(sim.invars):
-        X[:, i] = sim.invars[varname].pcts
-    Y[:, 0] = sim.outvars[outvarname].nums
-    return X, Y
-
-
-def calc_Gammaj(Hj       : float,
-                phij     : float,
-                variance : float
-                ) -> float:
-    """
-    Calculates the IVARS sensitivity index from a learned covariance function.
-
-    This integrates the directional variogram for a specific input variable
-    using trapezoidal integration.
-
-    Parameters
-    ----------
-    Hj : float
-        The fraction of the total parameter space to integrate over. Note that
-        the linear correlation function only has one hyperparameter, so as the
-        Reference notes it is unable to distinguish variogram effects at varying
-        length scales. So, this should not be set to anything other than 1 in
-        practice.
-    phij : float
-        The learned hyperparameter for the covariance function between the
-        output and input variable.
-    variance : float
-        The variance of the output variable.
-
-    Returns
-    -------
-    Gammaj : float
-        The global sensitivity index for this output-input variable pair.
-    """
-    dh = 1e-3
-    q = int(np.floor(Hj/dh))
-    rjs = np.zeros(q+1)
-    for i in range(q+1):
-        rjs[i] = calc_rj(dh*i, phij)
-
-    Gammaj = np.trapz(1 - rjs) * dh * variance
-    return Gammaj
-
-
-def L_runner(phi     : np.ndarray,
-             X       : np.ndarray,
-             Y       : np.ndarray,
-             verbose : bool = False
-             ) -> float:
-    """
-    A wrapper function for calculating the negative log-likelihood cost.
-
-    Parameters
-    ----------
-    phi : numpy.ndarray
-        The hyperparameters for the covariance function.
-    X : numpy.ndarray
-        The state matrix for all the input variables percentiles.
-    Y : numpy.ndarray
-        The state matrix for the output variables nums.
-    verbose : bool
-        Whether to print the values at each step.
-
-    Returns
-    -------
-    L : float
-        The negative log-likelihood cost.
-    """
-    L = calc_L(phi, X, Y)
-    vprint(verbose, f'L = {L:0.4f}, Φ = {phi}')
-    return L
-
-
-@jit(nopython=True, cache=True)
-def calc_L(phi : np.ndarray,
-           X   : np.ndarray,
-           Y   : np.ndarray
-           ) -> float:
-    """
-    Calculate the negative log-likelihood cost. Note that this is just-in-time
-    compiled by numba for increased speed.
-
-    Parameters
-    ----------
-    phi : numpy.ndarray
-        The hyperparameters for the covariance function.
-    X : numpy.ndarray
-        The state matrix for all the input variables percentiles.
-    Y : numpy.ndarray
-        The state matrix for the output variables nums.
-
-    Returns
-    -------
-    L : float
-        The negative log-likelihood cost.
-    """
-    m = len(Y)
-    M = np.ones((m, 1))
-    R = calc_R(phi, X)
-    Rinv = np.linalg.inv(R)
-    Rdet = max(np.linalg.det(R), 1e-12)  # Protect for poor conditioning
-
-    mu = np.linalg.inv(M.T @ Rinv @ M) @ (M.T @ Rinv @ Y)
-
-    L_inner = Y - M*mu
-    L = np.log(Rdet)/m + m*np.log(L_inner.T @ Rinv @ L_inner)
-    L = L[0][0]
-    return L
-
-
-@jit(nopython=True, cache=True)
-def calc_R(phi : np.ndarray,
-           X   : np.ndarray,
-           ) -> np.ndarray:
-    """
-    Calculate the correlation matrix between each of the input states.
-    Note that this is just-in-time compiled by numba for increased speed.
-
-    Parameters
-    ----------
-    phi : numpy.ndarray
-        The hyperparameters for the covariance function.
-    X : numpy.ndarray
-        The state matrix for all the input variables percentiles.
-
-    Returns
-    -------
-    R : float
-        The correlation matrix.
-    """
-    m = X.shape[0]
-    R = np.ones((m, m))
-    for u in range(1, m):
-        # do lower triangle only and duplicate across diag
-        # diag will be all 1s
-        for w in range(1, u):
-            Ruw = calc_Ruw(phi, X[u, :], X[w, :])
-            R[u, w] = Ruw
-            R[w, u] = Ruw
-    return R
-
-
-@jit(nopython=True, cache=True)
-def calc_Ruw(phi : np.ndarray,
-             Xu  : np.ndarray,
-             Xw  : np.ndarray
-             ) -> float:
-    """
-    Calculate the correlation between two input states.
-    Note that this is just-in-time compiled by numba for increased speed.
-
-    Parameters
-    ----------
-    phi : numpy.ndarray
-        The hyperparameters for the covariance function.
-    Xu : numpy.ndarray
-        The u'th input state.
-    Xw : numpy.ndarray
-        The w'th input state.
-
-    Returns
-    -------
-    Ruw : float
-        The correlation between the two states.
-    """
-    h = Xu - Xw
-    Ruw = 1
-    for j, hj in enumerate(h):
-        Ruw = Ruw*calc_rj(hj, phi[j])
-    return Ruw
-
-
-@jit(nopython=True, cache=True)
-def calc_rj(hj   : float,
-            phij : float
-            ) -> float:
-    """
-    The covariance function (also called a kernel). We currently use a linear
-    kernel which has a single hyperparameter that must be learned.
-    Note that this is just-in-time compiled by numba for increased speed.
-
-    Parameters
-    ----------
-    hj : float
-        The distance between two state elements.
-    phij : float
-        The hyperparameter for the function.
-
-    Returns
-    -------
-    rj : float
-        The covariance.
-    """
-    rj = max(0, 1 - phij*abs(hj))  # linear covariance function
-    # rj = np.exp(-(abs(hj)/phij))  # exponential covariance function
-    # rj = np.exp(-(hj/phij)**2)  # squared exponential covariance function
-    return rj
+# dvars_sensitivity.py
+from __future__ import annotations
+
+# Somewhat hacky type checking to avoid circular imports:
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from monaco.mc_sim import Sim
+
+import numpy as np
+from monaco.helper_functions import vprint
+from scipy.optimize import minimize
+from warnings import warn
+
+# numba is recommended for speed, as this will be very slow otherwise
+try:
+    from numba import jit
+except ImportError:
+    warn("Consider installing numba for better performance", UserWarning)
+    # create a dummy decorator
+    def jit(f=None, *args, **kwargs):
+        def decorator(func):
+            return func 
+
+        if callable(f):
+            return f
+        else:
+            return decorator
+
+
+def calc_sensitivities(sim        : 'Sim',
+                       outvarname : str,
+                       Hj         : float = 1.0,
+                       tol        : float = 1e-6,
+                       verbose    : bool  = False,
+                       ) -> tuple[np.ndarray, np.ndarray]:
+    """
+    Calculates the global sensitivity indices and ratios for a specific output
+    variable to each of a simulation's input variables.
+
+    This implements the D-VARS algorithm as dscribed in Reference [1]_ to
+    calculate global sensitivity indices from a set of given data. The
+    implementation largely follows the Reference's supplementary notes, though
+    Multi-SQP is replaced with scipy's minimize function implementing L-BFGS-B.
+    See also Reference [2]_ for some theoretical background on the VARS and
+    IVARS methods of calculating sensitivity indices.
+
+    Parameters
+    ----------
+    sim : monaco.mc_sim.Sim
+        The input simulation.
+    outvarname : str
+        The name of the output variable to calculate sensitivities for. Note
+        that the output variable must be scalar.
+    Hj : float, default: 1.0
+        The fraction of the total parameter space to integrate over. Note that
+        the linear correlation function only has one hyperparameter, so as the
+        Reference notes it is unable to distinguish variogram effects at varying
+        length scales. So, this should not be set to anything other than 1 in
+        practice.
+    tol : float, default 1e-6
+        The convergence tolerance for scipy's minimize function acting on the
+        negative log likelihood function.
+    verbose : bool, default False
+        Whether to print diagnostic information.
+
+    Returns
+    -------
+    sensitivities : numpy.ndarray
+        The global sensitivity indices for the output variable for each of the
+        sim's input variables.
+    ratios : numpy.ndarray
+        The global sensitivity ratios for the output variable for each of the
+        sim's input variables, essentially the fraction of each input variable's
+        ability to explain the output variance.
+
+    References
+    ----------
+    .. [1] Sheikholeslami, Razi, and Saman Razavi. "A fresh look at variography:
+           measuring dependence and possible sensitivities across geophysical
+           systems from any given data." Geophysical Research Letters 47.20
+           (2020): e2020GL089829.
+    .. [2] Razavi, Saman, and Hoshin V. Gupta. "A new framework for
+           comprehensive, robust, and efficient global sensitivity analysis:
+           1. Theory." Water Resources Research 52.1 (2016): 423-439.
+    """
+    phi_opt = calc_phi_opt(sim, outvarname, tol, verbose)
+
+    variance = np.var(np.array([sim.outvars[outvarname].nums]))
+    sensitivities = np.zeros(sim.ninvars)
+    for j in range(sim.ninvars):
+        sensitivities[j] = calc_Gammaj(Hj, phi_opt[j], variance)
+    ratios = sensitivities/sum(sensitivities)
+
+    return sensitivities, ratios
+
+
+def calc_phi_opt(sim        : 'Sim',
+                 outvarname : str,
+                 tol        : float = 1e-6,
+                 verbose    : bool = False
+                 ) -> np.ndarray:
+    """
+    Calculate the optimal hyperparameters for the covariance functions between
+    the output variable and each of the input variables via maximum likelihood
+    estimation (MLE). MLE works by minimizing a negative log-likelihood
+    function.
+
+    Parameters
+    ----------
+    sim : monaco.mc_sim.Sim
+        The input simulation.
+    outvarname : str
+        The name of the output variable to calculate sensitivities for. Note
+        that the output variable must be scalar.
+    tol : float, default 1e-6
+        The convergence tolerance for scipy's minimize function acting on the
+        negative log likelihood function.
+    verbose : bool, default False
+        Whether to print diagnostic information.
+
+    Returns
+    -------
+    phi_opt : numpy.ndarray
+        The learned hyperparameters for the covariance functions.
+    """
+    phi_max = 1e6
+    phi_min = 0
+    phi0 = 1
+
+    phi0s = []
+    bounds = []
+    for _ in range(sim.ninvars):
+        phi0s.append(phi0)
+        bounds.append((phi_min, phi_max))
+
+    vprint(sim.verbose, 'Calculating optimal hyperparameters Φ for ' +
+                       f"'{outvarname}' covariances...")
+    X, Y = full_states(sim, outvarname)
+    res = minimize(L_runner, phi0s, args=(X, Y, verbose), bounds=bounds,
+                   tol=tol, method='L-BFGS-B')
+    phi_opt = res.x
+    vprint(sim.verbose, 'Done calculating optimal hyperparameters.')
+
+    return phi_opt
+
+
+def full_states(sim : 'Sim',
+                outvarname : str,
+                ) -> tuple[np.ndarray, np.ndarray]:
+    """
+    Get the full input and output states in combined matrices.
+
+    Parameters
+    ----------
+    sim : monaco.mc_sim.Sim
+        The input simulation.
+    outvarname : str
+        The name of the output variable to calculate sensitivities for. Note
+        that the output variable must be scalar.
+
+    Returns
+    -------
+    X : numpy.ndarray
+        The input variables' percentiles.
+    Y : numpy.ndarray
+        The output variable's nums.
+    """
+    X = np.zeros((sim.ncases, sim.ninvars))
+    Y = np.zeros((sim.ncases, 1))
+    for i, varname in enumerate(sim.invars):
+        X[:, i] = sim.invars[varname].pcts
+    Y[:, 0] = sim.outvars[outvarname].nums
+    return X, Y
+
+
+def calc_Gammaj(Hj       : float,
+                phij     : float,
+                variance : float
+                ) -> float:
+    """
+    Calculates the IVARS sensitivity index from a learned covariance function.
+
+    This integrates the directional variogram for a specific input variable
+    using trapezoidal integration.
+
+    Parameters
+    ----------
+    Hj : float
+        The fraction of the total parameter space to integrate over. Note that
+        the linear correlation function only has one hyperparameter, so as the
+        Reference notes it is unable to distinguish variogram effects at varying
+        length scales. So, this should not be set to anything other than 1 in
+        practice.
+    phij : float
+        The learned hyperparameter for the covariance function between the
+        output and input variable.
+    variance : float
+        The variance of the output variable.
+
+    Returns
+    -------
+    Gammaj : float
+        The global sensitivity index for this output-input variable pair.
+    """
+    dh = 1e-3
+    q = int(np.floor(Hj/dh))
+    rjs = np.zeros(q+1)
+    for i in range(q+1):
+        rjs[i] = calc_rj(dh*i, phij)
+
+    Gammaj = np.trapz(1 - rjs) * dh * variance
+    return Gammaj
+
+
+def L_runner(phi     : np.ndarray,
+             X       : np.ndarray,
+             Y       : np.ndarray,
+             verbose : bool = False
+             ) -> float:
+    """
+    A wrapper function for calculating the negative log-likelihood cost.
+
+    Parameters
+    ----------
+    phi : numpy.ndarray
+        The hyperparameters for the covariance function.
+    X : numpy.ndarray
+        The state matrix for all the input variables percentiles.
+    Y : numpy.ndarray
+        The state matrix for the output variables nums.
+    verbose : bool
+        Whether to print the values at each step.
+
+    Returns
+    -------
+    L : float
+        The negative log-likelihood cost.
+    """
+    L = calc_L(phi, X, Y)
+    vprint(verbose, f'L = {L:0.4f}, Φ = {phi}')
+    return L
+
+
+@jit(nopython=True, cache=True)
+def calc_L(phi : np.ndarray,
+           X   : np.ndarray,
+           Y   : np.ndarray
+           ) -> float:
+    """
+    Calculate the negative log-likelihood cost. Note that this is just-in-time
+    compiled by numba for increased speed.
+
+    Parameters
+    ----------
+    phi : numpy.ndarray
+        The hyperparameters for the covariance function.
+    X : numpy.ndarray
+        The state matrix for all the input variables percentiles.
+    Y : numpy.ndarray
+        The state matrix for the output variables nums.
+
+    Returns
+    -------
+    L : float
+        The negative log-likelihood cost.
+    """
+    m = len(Y)
+    M = np.ones((m, 1))
+    R = calc_R(phi, X)
+    Rinv = np.linalg.inv(R)
+    Rdet = max(np.linalg.det(R), 1e-12)  # Protect for poor conditioning
+
+    mu = np.linalg.inv(M.T @ Rinv @ M) @ (M.T @ Rinv @ Y)
+
+    L_inner = Y - M*mu
+    L = np.log(Rdet)/m + m*np.log(L_inner.T @ Rinv @ L_inner)
+    L = L[0][0]
+    return L
+
+
+@jit(nopython=True, cache=True)
+def calc_R(phi : np.ndarray,
+           X   : np.ndarray,
+           ) -> np.ndarray:
+    """
+    Calculate the correlation matrix between each of the input states.
+    Note that this is just-in-time compiled by numba for increased speed.
+
+    Parameters
+    ----------
+    phi : numpy.ndarray
+        The hyperparameters for the covariance function.
+    X : numpy.ndarray
+        The state matrix for all the input variables percentiles.
+
+    Returns
+    -------
+    R : float
+        The correlation matrix.
+    """
+    m = X.shape[0]
+    R = np.ones((m, m))
+    for u in range(1, m):
+        # do lower triangle only and duplicate across diag
+        # diag will be all 1s
+        for w in range(1, u):
+            Ruw = calc_Ruw(phi, X[u, :], X[w, :])
+            R[u, w] = Ruw
+            R[w, u] = Ruw
+    return R
+
+
+@jit(nopython=True, cache=True)
+def calc_Ruw(phi : np.ndarray,
+             Xu  : np.ndarray,
+             Xw  : np.ndarray
+             ) -> float:
+    """
+    Calculate the correlation between two input states.
+    Note that this is just-in-time compiled by numba for increased speed.
+
+    Parameters
+    ----------
+    phi : numpy.ndarray
+        The hyperparameters for the covariance function.
+    Xu : numpy.ndarray
+        The u'th input state.
+    Xw : numpy.ndarray
+        The w'th input state.
+
+    Returns
+    -------
+    Ruw : float
+        The correlation between the two states.
+    """
+    h = Xu - Xw
+    Ruw = 1
+    for j, hj in enumerate(h):
+        Ruw = Ruw*calc_rj(hj, phi[j])
+    return Ruw
+
+
+@jit(nopython=True, cache=True)
+def calc_rj(hj   : float,
+            phij : float
+            ) -> float:
+    """
+    The covariance function (also called a kernel). We currently use a linear
+    kernel which has a single hyperparameter that must be learned.
+    Note that this is just-in-time compiled by numba for increased speed.
+
+    Parameters
+    ----------
+    hj : float
+        The distance between two state elements.
+    phij : float
+        The hyperparameter for the function.
+
+    Returns
+    -------
+    rj : float
+        The covariance.
+    """
+    rj = max(0, 1 - phij*abs(hj))  # linear covariance function
+    # rj = np.exp(-(abs(hj)/phij))  # exponential covariance function
+    # rj = np.exp(-(hj/phij)**2)  # squared exponential covariance function
+    return rj
```

### Comparing `monaco-0.9.0/src/monaco/gaussian_statistics.py` & `monaco-0.9.1/src/monaco/gaussian_statistics.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/helper_functions.py` & `monaco-0.9.1/src/monaco/helper_functions.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/integration_statistics.py` & `monaco-0.9.1/src/monaco/integration_statistics.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_case.py` & `monaco-0.9.1/src/monaco/mc_case.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_enums.py` & `monaco-0.9.1/src/monaco/mc_enums.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_multi_plot.py` & `monaco-0.9.1/src/monaco/mc_multi_plot.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_plot.py` & `monaco-0.9.1/src/monaco/mc_plot.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_sampling.py` & `monaco-0.9.1/src/monaco/mc_sampling.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_sim.py` & `monaco-0.9.1/src/monaco/mc_sim.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_val.py` & `monaco-0.9.1/src/monaco/mc_val.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_var.py` & `monaco-0.9.1/src/monaco/mc_var.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/mc_varstat.py` & `monaco-0.9.1/src/monaco/mc_varstat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,582 +1,587 @@
-# mc_varstat.py
-from __future__ import annotations
-
-# Somewhat hacky type checking to avoid circular imports:
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from monaco.mc_var import Var
-
-import numpy as np
-from copy import copy
-from statistics import mode
-from scipy.stats import bootstrap, moment, skew, kurtosis
-from scipy.stats.mstats import gmean
-from monaco.helper_functions import get_list
-from monaco.gaussian_statistics import pct2sig, sig2pct
-from monaco.order_statistics import (order_stat_TI_n, order_stat_TI_k,
-                                     order_stat_P_k, get_iP)
-from monaco.mc_enums import StatBound, VarStatType, VarStatSide
-from typing import Any, Callable
-
-
-class VarStat:
-    """
-    A variable statistic for a Monte Carlo variable.
-
-    Parameters
-    ----------
-    var : monaco.mc_var.Var
-        The variable to generate statistics for.
-    stat : monaco.mc_enums.VarStatType | Callable
-        The statistic to generate. Can be custom. If custom, must be able to
-        accept an "axis" kwarg for bootstrap vectorization.
-    statkwargs : dict[str:Any]
-        The keyword arguments for the variable statistic.
-    bootstrap : bool (default: True)
-        Whether to use bootstrapping to generate confidence intervals for the
-        statistic.
-    bootstrap_k : int (default: 10)
-        The k'th order statistic to determine the number of bootstrap draws for
-        the given confidence level. Must be >= 1. Set higher for a smoother
-        bootstrap distribution.
-    conf : float (default: 0.95)
-        The confidence level for the confidence interval.
-    seed : int (default: np.random.get_state(legacy=False)['state']['key'][0])
-        The random seed to use for bootstrapping.
-    name : str
-        The name of the variable statistic.
-
-    Attributes
-    ----------
-    nums : numpy.ndarray
-        The output of the variable statistic function applied to `var.nums`
-    confidence_interval_low_nums : numpy.ndarray
-        The nums for the low side of the confidence interval (None if no CI).
-    confidence_interval_high_nums : numpy.ndarray
-        The nums for the high side of the confidence interval (None if no CI).
-    vals : list[Any]
-        The values for the `nums` as determined by `var.nummap`
-    confidence_interval_low_vals : list[Any]
-        The values for `confidence_interval_low_nums` via `var.nummap`
-    confidence_interval_high_vals : list[Any]
-        The values for `confidence_interval_high_nums` via `var.nummap`
-    bootstrap_n : int
-        The number of bootstrap samples.
-
-    Notes
-    -----
-    These are the valid stats with their statkwargs
-
-    max()
-        No kwargs
-    min()
-        No kwargs
-    median()
-        No kwargs
-    mean()
-        No kwargs
-    geomean()
-        No kwargs
-    mode()
-        No kwargs
-    variance()
-        No kwargs
-    skewness()
-        No kwargs
-    kurtosis()
-        No kwargs
-    moment(n : int)
-        `n` is the n'th moment, `n > 0`.
-    percentile(p : float)
-        `p` is the percentile, `0 < p < 1`.
-    sigma(sig : float, bound : monaco.mc_enums.StatBound)
-        `sig` is the gaussian sigma value, `-inf < sig < inf`.
-
-        `bound` is the statistical bound, ether `'1-sided'` or `'2-sided'`.
-        Default is `'2-sided'`.
-    gaussianP(p : float, bound : monaco.mc_enums.StatBound)
-        `p` is the percentile, `0 < p < 1`.
-
-        `bound` is the statistical bound, ether `'1-sided'` or `'2-sided'`.
-        Default is `'2-sided'`.
-    orderstatTI(p : float, c : float, bound : monaco.mc_enums.StatBound)
-        `p` is the percentage, `0 < p < 1`
-
-        `c` is the confidence, `0 < c < 1`. Default is `0.95`.
-
-        `bound` is the statistical bound, ether `'1-sided'`, `'2-sided'`, or
-        `'all'`. Default is `'2-sided'`.
-    orderstatP(p : float, c : float, bound : monaco.mc_enums.StatBound)
-        `p` is the percentage, `0 < p < 1`
-
-        `c` is the confidence, `0 < c < 1`. Default is `0.95`.
-
-        `bound` is the statistical bound, ether `'1-sided lower'`,
-        `'1-sided upper'`, `'2-sided'`, `'all'`, or '`nearest'`. Default is
-        `'2-sided'`.
-    """
-    def __init__(self,
-                 var         : Var,
-                 stat        : VarStatType | Callable,
-                 statkwargs  : dict[str, Any] = None,
-                 bootstrap   : bool = True,
-                 bootstrap_k : int = 10,
-                 conf        : float = 0.95,
-                 seed        : int = np.random.get_state(legacy=False)['state']['key'][0],
-                 name        : str = None,
-                 ):
-
-        self.var = var
-        self.stat = stat
-        if statkwargs is None:
-            statkwargs = dict()
-        self.statkwargs = statkwargs
-
-        self.nums : np.ndarray = np.array([])
-        self.vals : list[Any] | np.ndarray = []
-        self.name = name
-
-        self.bootstrap = bootstrap
-        if bootstrap_k < 1:
-            raise ValueError(f'bootstrap_k = {bootstrap_k} must be >= 1')
-        self.bootstrap_k = bootstrap_k
-        self.conf = conf
-        self.confidence_interval_low_nums : np.ndarray = None
-        self.confidence_interval_high_nums : np.ndarray = None
-        self.confidence_interval_low_vals : list[Any] | np.ndarray = []
-        self.confidence_interval_high_vals : list[Any] | np.ndarray = []
-        self.bootstrap_n = None
-        self.seed = seed
-
-        if isinstance(stat, Callable):
-            self.setName(f'{self.var.name} {str(stat)}')
-            self.genStatsFunction(fcn=stat, fcnkwargs=statkwargs)
-        elif stat == VarStatType.MAX:
-            self.setName(f'{self.var.name} Max')
-            self.genStatsFunction(fcn=np.max)
-        elif stat == VarStatType.MIN:
-            self.setName(f'{self.var.name} Min')
-            self.genStatsFunction(fcn=np.min)
-        elif stat == VarStatType.MEDIAN:
-            self.setName(f'{self.var.name} Median')
-            self.genStatsFunction(fcn=np.median)
-        elif stat == VarStatType.MEAN:
-            self.setName(f'{self.var.name} Mean')
-            self.genStatsFunction(fcn=np.mean)
-        elif stat == VarStatType.GEOMEAN:
-            self.setName(f'{self.var.name} Geometric Mean')
-            self.genStatsFunction(fcn=gmean)
-        elif stat == VarStatType.MODE:
-            self.setName(f'{self.var.name} Mode')
-            self.genStatsFunction(fcn=mode)
-        elif stat == VarStatType.VARIANCE:
-            self.setName(f'{self.var.name} Variance')
-            self.genStatsFunction(fcn=np.var)
-        elif stat == VarStatType.SKEWNESS:
-            self.setName(f'{self.var.name} Skewness')
-            self.genStatsFunction(fcn=skew)
-        elif stat == VarStatType.KURTOSIS:
-            self.setName(f'{self.var.name} Kurtosis')
-            self.genStatsFunction(fcn=kurtosis)
-        elif stat == VarStatType.MOMENT:
-            self.genStatsMoment()
-        elif stat == VarStatType.PERCENTILE:
-            self.genStatsPercentile()
-        elif stat == VarStatType.SIGMA:
-            self.genStatsSigma()
-        elif stat == VarStatType.GAUSSIANP:
-            self.genStatsGaussianP()
-        elif stat == VarStatType.ORDERSTATTI:
-            self.genStatsOrderStatTI()
-        elif stat == VarStatType.ORDERSTATP:
-            self.genStatsOrderStatP()
-        else:
-            raise ValueError(f'{stat=} must be callable, or one of the following: ' +
-                             f'{VarStatType.MAX}, {VarStatType.MIN}, {VarStatType.MEDIAN}, ' +
-                             f'{VarStatType.MEAN}, {VarStatType.GEOMEAN}, {VarStatType.MODE}, ' +
-                             f'{VarStatType.PERCENTILE}, {VarStatType.SIGMA}, ' +
-                             f'{VarStatType.GAUSSIANP}, {VarStatType.ORDERSTATTI}, ' +
-                             f'{VarStatType.ORDERSTATP}')
-
-
-    def genStatsMoment(self) -> None:
-        """
-        Get the n'th moment about the mean of the variable.
-        """
-        if 'n' not in self.statkwargs:
-            raise ValueError(f'{self.stat} requires the kwarg ''n''')
-
-        self.n = self.statkwargs['n']
-        self.setName(f'{self.var.name} {self.n}''th Moment')
-        self.genStatsFunction(moment, {'moment': self.n})
-
-
-    def genStatsPercentile(self) -> None:
-        """
-        Get the value of the variable at the inputted percentile.
-        """
-        if 'p' not in self.statkwargs:
-            raise ValueError(f'{self.stat} requires the kwarg ''p''')
-
-        self.p = self.statkwargs['p']
-        self.setName(f'{self.var.name} {self.p*100}% Percentile')
-        self.genStatsFunction(np.quantile, {'q': self.p})
-
-
-    def genStatsSigma(self) -> None:
-        """
-        Get the value of the variable at the inputted sigma value, assuming
-        a gaussian distribution.
-        """
-        if 'sig' not in self.statkwargs:
-            raise ValueError(f'{self.stat} requires the kwarg ''sig''')
-        if 'bound' not in self.statkwargs:
-            self.bound = StatBound.TWOSIDED
-        else:
-            self.bound = self.statkwargs['bound']
-
-        self.sig = self.statkwargs['sig']
-        self.p = sig2pct(self.sig, bound=self.bound)
-        self.setName(f'{self.var.name} {self.sig} Sigma')
-        self.genStatsFunction(self.sigma, {'sig': self.sig})
-
-
-    def genStatsGaussianP(self) -> None:
-        """
-        Get the value of the variable at the inputted percentile value,
-        assuming a gaussian distribution.
-        """
-        if 'p' not in self.statkwargs:
-            raise ValueError(f'{self.stat} requires the kwarg ''p''')
-        if 'bound' not in self.statkwargs:
-            self.bound = StatBound.TWOSIDED
-        else:
-            self.bound = self.statkwargs['bound']
-
-        self.p = self.statkwargs['p']
-        self.sig = pct2sig(self.p, bound=self.bound)
-        self.setName(f'{self.var.name} Guassian {self.p*100}%')
-        self.genStatsFunction(self.sigma, {'sig': self.sig})
-
-
-    def sigma(self,
-              x,  # TODO: explicit typing here
-              sig  : float,
-              axis : int = None,
-              ) -> float:
-        """
-        Calculate the sigma value of a normally distributed list of numbers.
-
-        Parameters
-        ----------
-        x : TODO typing
-            The numbers to calculate the sigma value for.
-        sig : float
-            The sigma value.
-        axis : int (default: None)
-            The axis of x to calculate along.
-        """
-        std = np.std(x, axis=axis)
-        return np.mean(x, axis=axis) + sig*std
-
-
-    def statsFunctionWrapper(self,
-                             x : Any,
-                             axis : int = None,  # Needed for bootstrap vectorization
-                             ) -> Any:
-        """
-        A wrapper function to allow using a bootstrap function that uses kwargs.
-        Relies on self.fcn and self.fcnkwargs already being set. Note that fcn
-        must accept an `axis` kwarg if bootstrapping.
-
-        Parameters
-        ----------
-        x : Any
-            The input for the function.
-        axis : int (default: None)
-            The axis of x to calculate along.
-        """
-        return self.fcn(x, **self.fcnkwargs, axis=axis)
-
-
-    def genStatsFunction(self,
-                         fcn       : Callable,
-                         fcnkwargs : dict[str, Any] = None,
-                         ) -> None:
-        """
-        A wrapper function to generate statistics via a generic function.
-
-        Parameters
-        ----------
-        fcn : Callable
-            The function used to generate the desired statistics.
-        fcnkwargs : dict[str, Any]
-            The keyword arguments for the function.
-        """
-        self.fcn = fcn
-        if fcnkwargs is None:
-            fcnkwargs = dict()
-        self.fcnkwargs = fcnkwargs
-        if self.bootstrap:
-            self.bootstrap_n = order_stat_TI_n(self.bootstrap_k, p=0.5, c=self.conf)
-
-        # Scalar Variables
-        if self.var.isscalar:
-            # Calculate nums and confidence interval for each point in the sequence
-            self.nums = self.statsFunctionWrapper(self.var.nums)
-            if self.bootstrap:
-                # Switch to method='Bca' once https://github.com/scipy/scipy/issues/15883 resolved
-                res = bootstrap((np.array(self.var.nums),), self.statsFunctionWrapper,
-                                confidence_level=self.conf,
-                                n_resamples=self.bootstrap_n,
-                                random_state=self.seed, method='basic')
-                self.confidence_interval_low_nums = res.confidence_interval.low
-                self.confidence_interval_high_nums = res.confidence_interval.high
-
-            # Calculate the corresponding vals based on the nummap
-            self.vals = copy(self.nums)
-            if self.bootstrap:
-                self.confidence_interval_low_vals = copy(self.confidence_interval_low_nums)
-                self.confidence_interval_high_vals = copy(self.confidence_interval_high_nums)
-            if self.var.nummap is not None:
-                self.vals = [self.var.nummap[num] for num in self.nums]
-                if self.bootstrap:
-                    self.confidence_interval_low_vals = \
-                        [self.var.nummap[num] for num in self.confidence_interval_low_nums]
-                    self.confidence_interval_high_vals = \
-                        [self.var.nummap[num] for num in self.confidence_interval_high_nums]
-
-        # 1-D Variables
-        elif self.var.maxdim == 1:
-            nums_list = get_list(self.var.nums)
-            npoints = max(len(x) for x in nums_list)
-            if self.bootstrap:
-                confidence_interval_low_nums = []
-                confidence_interval_high_nums = []
-
-            # Calculate nums and confidence interval for each point in the sequence
-            nums = []
-            for i in range(npoints):
-                numsatidx = np.array([x[i] for x in nums_list if len(x) > i])
-                nums.append(self.statsFunctionWrapper(numsatidx))
-                if self.bootstrap:
-                    # Switch to Bca once https://github.com/scipy/scipy/issues/15883 resolved
-                    res = bootstrap((numsatidx,), self.statsFunctionWrapper,
-                                    confidence_level=self.conf,
-                                    n_resamples=self.bootstrap_n,
-                                    random_state=self.seed, method='basic')
-                    confidence_interval_low_nums.append(res.confidence_interval.low)
-                    confidence_interval_high_nums.append(res.confidence_interval.high)
-            self.nums = nums
-            if self.bootstrap:
-                self.confidence_interval_low_nums = confidence_interval_low_nums
-                self.confidence_interval_high_nums = confidence_interval_high_nums
-
-            # Calculate the corresponding vals based on the nummap
-            self.vals = copy(self.nums)
-            if self.bootstrap:
-                self.confidence_interval_low_vals = copy(self.confidence_interval_low_nums)
-                self.confidence_interval_high_vals = copy(self.confidence_interval_high_nums)
-            if self.var.nummap is not None:
-                self.vals = [[self.var.nummap[x] for x in y] for y in self.nums]
-                if self.bootstrap:
-                    self.confidence_interval_low_vals \
-                        = [[self.var.nummap[x] for x in y]
-                           for y in self.confidence_interval_low_nums]
-                    self.confidence_interval_low_vals \
-                        = [[self.var.nummap[x] for x in y]
-                           for y in self.confidence_interval_high_nums]
-
-        else:
-            # Suppress warning since this will become valid when Var is split
-            # warn('VarStat only available for scalar or 1-D data')
-            pass
-
-
-    def genStatsOrderStatTI(self) -> None:
-        """Get the order statistic tolerance interval value of the variable."""
-        self.checkOrderStatsKWArgs()
-
-        if self.bound == StatBound.ONESIDED and self.p >= 0.5:
-            self.side = VarStatSide.HIGH
-        elif self.bound == StatBound.ONESIDED:
-            self.side = VarStatSide.LOW
-        elif self.bound == StatBound.TWOSIDED:
-            self.side = VarStatSide.BOTH
-        elif self.bound == StatBound.ALL:
-            self.bound = StatBound.TWOSIDED
-            self.side = VarStatSide.ALL
-        else:
-            raise ValueError(f'{self.bound} is not a valid bound for genStatsOrderStatTI')
-
-        self.setName(f'{self.var.name} ' +
-                     f'{self.bound} P{round(self.p*100,4)}/{round(self.c*100,4)}% ' +
-                      'Confidence Interval')
-
-        self.k = order_stat_TI_k(n=self.var.ncases, p=self.p, c=self.c, bound=self.bound)
-
-        if self.var.isscalar:
-            sortednums = sorted(self.var.nums)
-            if self.side == VarStatSide.LOW:
-                sortednums.reverse()
-            if self.side in (VarStatSide.HIGH, VarStatSide.LOW):
-                self.nums = np.array(sortednums[-self.k])
-                if self.var.nummap is not None:
-                    self.vals = self.var.nummap[self.nums.item()]
-            elif self.side == VarStatSide.BOTH:
-                self.nums = np.array([sortednums[self.k-1], sortednums[-self.k]])
-                if self.var.nummap is not None:
-                    self.vals = np.array([self.var.nummap[self.nums[0]],
-                                          self.var.nummap[self.nums[1]]])
-            elif self.side == VarStatSide.ALL:
-                self.nums = np.array([sortednums[self.k-1],
-                                      np.median(sortednums),
-                                      sortednums[-self.k]])
-                if self.var.nummap is not None:
-                    self.vals = np.array([self.var.nummap[self.nums[0]],
-                                          self.var.nummap[self.nums[1]],
-                                          self.var.nummap[self.nums[2]]])
-            if self.var.nummap is None:
-                self.vals = copy(self.nums)
-
-        elif self.var.maxdim == 1:
-            npoints = max(x.shape[0] if len(x.shape) > 0 else 0 for x in self.var.nums)
-            self.nums = np.empty(npoints)
-            if self.side == VarStatSide.BOTH:
-                self.nums = np.empty((npoints, 2))
-            elif self.side == VarStatSide.ALL:
-                self.nums = np.empty((npoints, 3))
-            for i in range(npoints):
-                numsatidx = [x[i] for x in self.var.nums
-                             if (len(x.shape) > 0 and x.shape[0] > i)]
-                sortednums = sorted(numsatidx)
-                if self.side == VarStatSide.LOW:
-                    sortednums.reverse()
-                if self.side in (VarStatSide.HIGH, VarStatSide.LOW):
-                    self.nums[i] = sortednums[-self.k]
-                elif self.side == VarStatSide.BOTH:
-                    self.nums[i, :] = [sortednums[self.k - 1], sortednums[-self.k]]
-                elif self.side == VarStatSide.ALL:
-                    self.nums[i, :] = [sortednums[self.k - 1],
-                                       sortednums[int(np.round(len(sortednums)/2)-1)],
-                                       sortednums[-self.k]]
-            if self.var.nummap is not None:
-                self.vals = np.array([[self.var.nummap[x] for x in y] for y in self.nums])
-            else:
-                self.vals = copy(self.nums)
-
-        else:
-            # Suppress warning since this will become valid when Var is split
-            # warn('VarStat only available for scalar or 1-D data')
-            pass
-
-
-    def genStatsOrderStatP(self) -> None:
-        """Get the order statistic percentile value of the variable."""
-        self.checkOrderStatsKWArgs()
-
-        bound = self.bound
-        if self.bound not in (StatBound.ONESIDED_UPPER, StatBound.ONESIDED_LOWER,
-                              StatBound.TWOSIDED, StatBound.NEAREST, StatBound.ALL):
-            raise ValueError(f'{self.bound} is not a valid bound for genStatsOrderStatP')
-        elif self.bound in (StatBound.NEAREST, StatBound.ALL):
-            bound = StatBound.TWOSIDED
-
-        self.setName(f'{self.var.name} ' +
-                     f'{self.bound} {self.c*100}% Confidence Bound around ' +
-                     f'{self.p*100}th Percentile')
-
-        self.k = order_stat_P_k(n=self.var.ncases, P=self.p, c=self.c, bound=bound)
-
-        (iPl, iP, iPu) = get_iP(n=self.var.ncases, P=self.p)
-        if self.var.isscalar:
-            sortednums = sorted(self.var.nums)
-            if self.bound == StatBound.ONESIDED_LOWER:
-                self.nums = np.array(sortednums[iPl - self.k])
-            elif self.bound == StatBound.ONESIDED_UPPER:
-                self.nums = np.array(sortednums[iPu + self.k])
-            elif self.bound == StatBound.NEAREST:
-                self.nums = np.array(sortednums[iP])
-            if self.bound in (StatBound.ONESIDED_LOWER,
-                              StatBound.ONESIDED_UPPER,
-                              StatBound.NEAREST):
-                if self.var.nummap is not None:
-                    self.vals = self.var.nummap[self.nums.item()]
-            elif self.bound == StatBound.TWOSIDED:
-                self.nums = np.array([sortednums[iPl - self.k], sortednums[iPu + self.k]])
-                if self.var.nummap is not None:
-                    self.vals = np.array([self.var.nummap[self.nums[0]],
-                                          self.var.nummap[self.nums[1]]])
-            elif self.bound == StatBound.ALL:
-                self.nums = np.array([sortednums[iPl - self.k],
-                                      sortednums[iP],
-                                      sortednums[iPu + self.k]])
-                if self.var.nummap is not None:
-                    self.vals = np.array([self.var.nummap[self.nums[0]],
-                                          self.var.nummap[self.nums[1]],
-                                          self.var.nummap[self.nums[2]]])
-            if self.var.nummap is None:
-                self.vals = copy(self.nums)
-
-        elif self.var.maxdim == 1:
-            npoints = max(len(get_list(x)) for x in self.var.nums)
-            self.nums = np.empty(npoints)
-            if self.bound == StatBound.TWOSIDED:
-                self.nums = np.empty((npoints, 2))
-            elif self.bound == StatBound.ALL:
-                self.nums = np.empty((npoints, 3))
-            for i in range(npoints):
-                numsatidx = [get_list(x)[i] for x in self.var.nums if len(get_list(x)) > i]
-                sortednums = sorted(numsatidx)
-                if self.bound == StatBound.ONESIDED_LOWER:
-                    self.nums[i] = sortednums[iPl - self.k]
-                elif self.bound == StatBound.ONESIDED_UPPER:
-                    self.nums[i] = sortednums[iPu + self.k]
-                elif self.bound == StatBound.NEAREST:
-                    self.nums[i] = sortednums[iP]
-                elif self.bound == StatBound.TWOSIDED:
-                    self.nums[i, :] = [sortednums[iPl - self.k], sortednums[iPu + self.k]]
-                elif self.bound == StatBound.ALL:
-                    self.nums[i, :] = [sortednums[iPl - self.k],
-                                       sortednums[iP],
-                                       sortednums[iPu + self.k]]
-            if self.var.nummap is not None:
-                self.vals = np.array([[self.var.nummap[x] for x in y] for y in self.nums])
-            else:
-                self.vals = copy(self.nums)
-
-        else:
-            # Suppress warning since this will become valid when Var is split
-            # warn('VarStat only available for scalar or 1-D data')
-            pass
-
-
-    def checkOrderStatsKWArgs(self) -> None:
-        """Check the order statistic keyword arguments."""
-        if 'p' not in self.statkwargs:
-            raise ValueError(f'{self.stat} requires the kwarg ''p''')
-        else:
-            self.p = self.statkwargs['p']
-        if 'c' not in self.statkwargs:
-            self.c = 0.95
-        else:
-            self.c = self.statkwargs['c']
-        if 'bound' not in self.statkwargs:
-            self.bound = StatBound.TWOSIDED
-        else:
-            self.bound = self.statkwargs['bound']
-
-
-    def setName(self,
-                name : str,
-                ) -> None:
-        """
-        Set the name for this variable statistic.
-
-        Parameters
-        ----------
-        name : str
-            The new name.
-        """
-        if self.name is None:
-            self.name = name
+# mc_varstat.py
+from __future__ import annotations
+
+# Somewhat hacky type checking to avoid circular imports:
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from monaco.mc_var import Var
+
+import numpy as np
+from copy import copy
+from statistics import mode
+from scipy.stats import bootstrap, moment, skew, kurtosis
+from scipy.stats.mstats import gmean
+from monaco.helper_functions import get_list
+from monaco.gaussian_statistics import pct2sig, sig2pct
+from monaco.order_statistics import (order_stat_TI_n, order_stat_TI_k,
+                                     order_stat_P_k, get_iP)
+from monaco.mc_enums import StatBound, VarStatType, VarStatSide
+from typing import Any, Callable
+
+
+class VarStat:
+    """
+    A variable statistic for a Monte Carlo variable.
+
+    Parameters
+    ----------
+    var : monaco.mc_var.Var
+        The variable to generate statistics for.
+    stat : monaco.mc_enums.VarStatType | Callable
+        The statistic to generate. Can be custom. If custom, must be able to
+        accept an "axis" kwarg for bootstrap vectorization.
+    statkwargs : dict[str:Any]
+        The keyword arguments for the variable statistic.
+    bootstrap : bool (default: True)
+        Whether to use bootstrapping to generate confidence intervals for the
+        statistic.
+    bootstrap_k : int (default: 10)
+        The k'th order statistic to determine the number of bootstrap draws for
+        the given confidence level. Must be >= 1. Set higher for a smoother
+        bootstrap distribution.
+    conf : float (default: 0.95)
+        The confidence level for the confidence interval.
+    seed : int (default: np.random.get_state(legacy=False)['state']['key'][0])
+        The random seed to use for bootstrapping.
+    name : str
+        The name of the variable statistic.
+
+    Attributes
+    ----------
+    nums : numpy.ndarray
+        The output of the variable statistic function applied to `var.nums`
+    confidence_interval_low_nums : numpy.ndarray
+        The nums for the low side of the confidence interval (None if no CI).
+    confidence_interval_high_nums : numpy.ndarray
+        The nums for the high side of the confidence interval (None if no CI).
+    vals : list[Any]
+        The values for the `nums` as determined by `var.nummap`
+    confidence_interval_low_vals : list[Any]
+        The values for `confidence_interval_low_nums` via `var.nummap`
+    confidence_interval_high_vals : list[Any]
+        The values for `confidence_interval_high_nums` via `var.nummap`
+    bootstrap_n : int
+        The number of bootstrap samples.
+
+    Notes
+    -----
+    These are the valid stats with their statkwargs
+
+    max()
+        No kwargs
+    min()
+        No kwargs
+    median()
+        No kwargs
+    mean()
+        No kwargs
+    geomean()
+        No kwargs
+    mode()
+        No kwargs
+    variance()
+        No kwargs
+    skewness()
+        No kwargs
+    kurtosis()
+        No kwargs
+    moment(n : int)
+        `n` is the n'th moment, `n > 0`.
+    percentile(p : float)
+        `p` is the percentile, `0 < p < 1`.
+    sigma(sig : float, bound : monaco.mc_enums.StatBound)
+        `sig` is the gaussian sigma value, `-inf < sig < inf`.
+
+        `bound` is the statistical bound, ether `'1-sided'` or `'2-sided'`.
+        Default is `'2-sided'`.
+    gaussianP(p : float, bound : monaco.mc_enums.StatBound)
+        `p` is the percentile, `0 < p < 1`.
+
+        `bound` is the statistical bound, ether `'1-sided'` or `'2-sided'`.
+        Default is `'2-sided'`.
+    orderstatTI(p : float, c : float, bound : monaco.mc_enums.StatBound)
+        `p` is the percentage, `0 < p < 1`
+
+        `c` is the confidence, `0 < c < 1`. Default is `0.95`.
+
+        `bound` is the statistical bound, ether `'1-sided'`, `'2-sided'`, or
+        `'all'`. Default is `'2-sided'`.
+    orderstatP(p : float, c : float, bound : monaco.mc_enums.StatBound)
+        `p` is the percentage, `0 < p < 1`
+
+        `c` is the confidence, `0 < c < 1`. Default is `0.95`.
+
+        `bound` is the statistical bound, ether `'1-sided lower'`,
+        `'1-sided upper'`, `'2-sided'`, `'all'`, or '`nearest'`. Default is
+        `'2-sided'`.
+    """
+    def __init__(self,
+                 var         : Var,
+                 stat        : VarStatType | Callable,
+                 statkwargs  : dict[str, Any] = None,
+                 bootstrap   : bool = True,
+                 bootstrap_k : int = 10,
+                 conf        : float = 0.95,
+                 seed        : int = np.random.get_state(legacy=False)['state']['key'][0],
+                 name        : str = None,
+                 ):
+
+        self.var = var
+        self.stat = stat
+        if statkwargs is None:
+            statkwargs = dict()
+        self.statkwargs = statkwargs
+
+        self.nums : np.ndarray = np.array([])
+        self.vals : list[Any] | np.ndarray = []
+        self.name = name
+
+        self.bootstrap = bootstrap
+        if bootstrap_k < 1:
+            raise ValueError(f'bootstrap_k = {bootstrap_k} must be >= 1')
+        self.bootstrap_k = bootstrap_k
+        self.conf = conf
+        self.confidence_interval_low_nums : np.ndarray = None
+        self.confidence_interval_high_nums : np.ndarray = None
+        self.confidence_interval_low_vals : list[Any] | np.ndarray = []
+        self.confidence_interval_high_vals : list[Any] | np.ndarray = []
+        self.bootstrap_n = None
+        self.seed = seed
+
+        if isinstance(stat, Callable):
+            self.setName(f'{self.var.name} {str(stat)}')
+            self.genStatsFunction(fcn=stat, fcnkwargs=statkwargs)
+        elif stat == VarStatType.MAX:
+            self.setName(f'{self.var.name} Max')
+            self.genStatsFunction(fcn=np.max)
+        elif stat == VarStatType.MIN:
+            self.setName(f'{self.var.name} Min')
+            self.genStatsFunction(fcn=np.min)
+        elif stat == VarStatType.MEDIAN:
+            self.setName(f'{self.var.name} Median')
+            self.genStatsFunction(fcn=np.median)
+        elif stat == VarStatType.MEAN:
+            self.setName(f'{self.var.name} Mean')
+            self.genStatsFunction(fcn=np.mean)
+        elif stat == VarStatType.GEOMEAN:
+            self.setName(f'{self.var.name} Geometric Mean')
+            self.genStatsFunction(fcn=gmean)
+        elif stat == VarStatType.MODE:
+            self.setName(f'{self.var.name} Mode')
+            self.genStatsFunction(fcn=mode)
+        elif stat == VarStatType.VARIANCE:
+            self.setName(f'{self.var.name} Variance')
+            self.genStatsFunction(fcn=np.var)
+        elif stat == VarStatType.SKEWNESS:
+            self.setName(f'{self.var.name} Skewness')
+            self.genStatsFunction(fcn=skew)
+        elif stat == VarStatType.KURTOSIS:
+            self.setName(f'{self.var.name} Kurtosis')
+            self.genStatsFunction(fcn=kurtosis)
+        elif stat == VarStatType.MOMENT:
+            self.genStatsMoment()
+        elif stat == VarStatType.PERCENTILE:
+            self.genStatsPercentile()
+        elif stat == VarStatType.SIGMA:
+            self.genStatsSigma()
+        elif stat == VarStatType.GAUSSIANP:
+            self.genStatsGaussianP()
+        elif stat == VarStatType.ORDERSTATTI:
+            self.genStatsOrderStatTI()
+        elif stat == VarStatType.ORDERSTATP:
+            self.genStatsOrderStatP()
+        else:
+            raise ValueError(f'{stat=} must be callable, or one of the following: ' +
+                             f'{VarStatType.MAX}, {VarStatType.MIN}, {VarStatType.MEDIAN}, ' +
+                             f'{VarStatType.MEAN}, {VarStatType.GEOMEAN}, {VarStatType.MODE}, ' +
+                             f'{VarStatType.PERCENTILE}, {VarStatType.SIGMA}, ' +
+                             f'{VarStatType.GAUSSIANP}, {VarStatType.ORDERSTATTI}, ' +
+                             f'{VarStatType.ORDERSTATP}')
+
+
+    def genStatsMoment(self) -> None:
+        """
+        Get the n'th moment about the mean of the variable.
+        """
+        if 'n' not in self.statkwargs:
+            raise ValueError(f'{self.stat} requires the kwarg ''n''')
+
+        self.n = self.statkwargs['n']
+        self.setName(f'{self.var.name} {self.n}''th Moment')
+        self.genStatsFunction(moment, {'moment': self.n})
+
+
+    def genStatsPercentile(self) -> None:
+        """
+        Get the value of the variable at the inputted percentile.
+        """
+        if 'p' not in self.statkwargs:
+            raise ValueError(f'{self.stat} requires the kwarg ''p''')
+
+        self.p = self.statkwargs['p']
+        self.setName(f'{self.var.name} {self.p*100}% Percentile')
+        self.genStatsFunction(np.quantile, {'q': self.p})
+
+
+    def genStatsSigma(self) -> None:
+        """
+        Get the value of the variable at the inputted sigma value, assuming
+        a gaussian distribution.
+        """
+        if 'sig' not in self.statkwargs:
+            raise ValueError(f'{self.stat} requires the kwarg ''sig''')
+        if 'bound' not in self.statkwargs:
+            self.bound = StatBound.TWOSIDED
+        else:
+            self.bound = self.statkwargs['bound']
+
+        self.sig = self.statkwargs['sig']
+        self.p = sig2pct(self.sig, bound=self.bound)
+        self.setName(f'{self.var.name} {self.sig} Sigma')
+        self.genStatsFunction(self.sigma, {'sig': self.sig})
+
+
+    def genStatsGaussianP(self) -> None:
+        """
+        Get the value of the variable at the inputted percentile value,
+        assuming a gaussian distribution.
+        """
+        if 'p' not in self.statkwargs:
+            raise ValueError(f'{self.stat} requires the kwarg ''p''')
+        if 'bound' not in self.statkwargs:
+            self.bound = StatBound.TWOSIDED
+        else:
+            self.bound = self.statkwargs['bound']
+
+        self.p = self.statkwargs['p']
+        self.sig = pct2sig(self.p, bound=self.bound)
+        self.setName(f'{self.var.name} Guassian {self.p*100}%')
+        self.genStatsFunction(self.sigma, {'sig': self.sig})
+
+
+    def sigma(self,
+              x,  # TODO: explicit typing here
+              sig  : float,
+              axis : int = None,
+              ) -> float:
+        """
+        Calculate the sigma value of a normally distributed list of numbers.
+
+        Parameters
+        ----------
+        x : TODO typing
+            The numbers to calculate the sigma value for.
+        sig : float
+            The sigma value.
+        axis : int (default: None)
+            The axis of x to calculate along.
+        """
+        std = np.std(x, axis=axis)
+        return np.mean(x, axis=axis) + sig*std
+
+
+    def statsFunctionWrapper(self,
+                             x : Any,
+                             axis : int = None,  # Needed for bootstrap vectorization
+                             ) -> Any:
+        """
+        A wrapper function to allow using a bootstrap function that uses kwargs.
+        Relies on self.fcn and self.fcnkwargs already being set. Note that fcn
+        must accept an `axis` kwarg if bootstrapping.
+
+        Parameters
+        ----------
+        x : Any
+            The input for the function.
+        axis : int (default: None)
+            The axis of x to calculate along.
+        """
+        return self.fcn(x, **self.fcnkwargs, axis=axis)
+
+
+    def genStatsFunction(self,
+                         fcn       : Callable,
+                         fcnkwargs : dict[str, Any] = None,
+                         ) -> None:
+        """
+        A wrapper function to generate statistics via a generic function.
+
+        Parameters
+        ----------
+        fcn : Callable
+            The function used to generate the desired statistics.
+        fcnkwargs : dict[str, Any]
+            The keyword arguments for the function.
+        """
+        self.fcn = fcn
+        if fcnkwargs is None:
+            fcnkwargs = dict()
+        self.fcnkwargs = fcnkwargs
+        if self.bootstrap:
+            self.bootstrap_n = order_stat_TI_n(self.bootstrap_k, p=0.5, c=self.conf)
+
+        # Scalar Variables
+        if self.var.isscalar:
+            # Calculate nums and confidence interval for each point in the sequence
+            self.nums = self.statsFunctionWrapper(self.var.nums)
+            if self.bootstrap:
+                # Switch to method='Bca' once https://github.com/scipy/scipy/issues/15883 resolved
+                res = bootstrap((np.array(self.var.nums),), self.statsFunctionWrapper,
+                                confidence_level=self.conf,
+                                n_resamples=self.bootstrap_n,
+                                random_state=self.seed, method='basic')
+                self.confidence_interval_low_nums = res.confidence_interval.low
+                self.confidence_interval_high_nums = res.confidence_interval.high
+
+            # Calculate the corresponding vals based on the nummap
+            self.vals = copy(self.nums)
+            if self.bootstrap:
+                self.confidence_interval_low_vals = copy(self.confidence_interval_low_nums)
+                self.confidence_interval_high_vals = copy(self.confidence_interval_high_nums)
+            if self.var.nummap is not None:
+                self.vals = [self.var.nummap[num] for num in self.nums]
+                if self.bootstrap:
+                    self.confidence_interval_low_vals = \
+                        [self.var.nummap[num] for num in self.confidence_interval_low_nums]
+                    self.confidence_interval_high_vals = \
+                        [self.var.nummap[num] for num in self.confidence_interval_high_nums]
+
+        # 1-D Variables
+        elif self.var.maxdim == 1:
+            nums_list = get_list(self.var.nums)
+            npoints = max(len(x) for x in nums_list)
+            if self.bootstrap:
+                confidence_interval_low_nums = []
+                confidence_interval_high_nums = []
+
+            # Calculate nums and confidence interval for each point in the sequence
+            nums = []
+            for i in range(npoints):
+                numsatidx = np.array([x[i] for x in nums_list if len(x) > i])
+                nums.append(self.statsFunctionWrapper(numsatidx))
+                if self.bootstrap:
+                    # Switch to Bca once https://github.com/scipy/scipy/issues/15883 resolved
+                    res = bootstrap((numsatidx,), self.statsFunctionWrapper,
+                                    confidence_level=self.conf,
+                                    n_resamples=self.bootstrap_n,
+                                    random_state=self.seed, method='basic')
+                    confidence_interval_low_nums.append(res.confidence_interval.low)
+                    confidence_interval_high_nums.append(res.confidence_interval.high)
+            self.nums = nums
+            if self.bootstrap:
+                self.confidence_interval_low_nums = confidence_interval_low_nums
+                self.confidence_interval_high_nums = confidence_interval_high_nums
+
+            # Calculate the corresponding vals based on the nummap
+            self.vals = copy(self.nums)
+            if self.bootstrap:
+                self.confidence_interval_low_vals = copy(self.confidence_interval_low_nums)
+                self.confidence_interval_high_vals = copy(self.confidence_interval_high_nums)
+            if self.var.nummap is not None:
+                self.vals = [[self.var.nummap[x] for x in y] for y in self.nums]
+                if self.bootstrap:
+                    self.confidence_interval_low_vals \
+                        = [[self.var.nummap[x] for x in y]
+                           for y in self.confidence_interval_low_nums]
+                    self.confidence_interval_low_vals \
+                        = [[self.var.nummap[x] for x in y]
+                           for y in self.confidence_interval_high_nums]
+
+        else:
+            # Suppress warning since this will become valid when Var is split
+            # warn('VarStat only available for scalar or 1-D data')
+            pass
+
+
+    def genStatsOrderStatTI(self) -> None:
+        """Get the order statistic tolerance interval value of the variable."""
+        self.checkOrderStatsKWArgs()
+
+        if self.bound == StatBound.ONESIDED and self.p >= 0.5:
+            self.side = VarStatSide.HIGH
+        elif self.bound == StatBound.ONESIDED:
+            self.side = VarStatSide.LOW
+        elif self.bound == StatBound.TWOSIDED:
+            self.side = VarStatSide.BOTH
+        elif self.bound == StatBound.ALL:
+            self.bound = StatBound.TWOSIDED
+            self.side = VarStatSide.ALL
+        else:
+            raise ValueError(f'{self.bound} is not a valid bound for genStatsOrderStatTI')
+
+        if isinstance(self.bound, StatBound):
+            bound_str = self.bound.value
+        else:
+            bound_str = self.bound
+
+        self.setName(f'{self.var.name} ' +
+                     f'{bound_str} P{round(self.p*100,4)}/{round(self.c*100,4)}% ' +
+                      'Confidence Interval')
+
+        self.k = order_stat_TI_k(n=self.var.ncases, p=self.p, c=self.c, bound=self.bound)
+
+        if self.var.isscalar:
+            sortednums = sorted(self.var.nums)
+            if self.side == VarStatSide.LOW:
+                sortednums.reverse()
+            if self.side in (VarStatSide.HIGH, VarStatSide.LOW):
+                self.nums = np.array(sortednums[-self.k])
+                if self.var.nummap is not None:
+                    self.vals = self.var.nummap[self.nums.item()]
+            elif self.side == VarStatSide.BOTH:
+                self.nums = np.array([sortednums[self.k-1], sortednums[-self.k]])
+                if self.var.nummap is not None:
+                    self.vals = np.array([self.var.nummap[self.nums[0]],
+                                          self.var.nummap[self.nums[1]]])
+            elif self.side == VarStatSide.ALL:
+                self.nums = np.array([sortednums[self.k-1],
+                                      np.median(sortednums),
+                                      sortednums[-self.k]])
+                if self.var.nummap is not None:
+                    self.vals = np.array([self.var.nummap[self.nums[0]],
+                                          self.var.nummap[self.nums[1]],
+                                          self.var.nummap[self.nums[2]]])
+            if self.var.nummap is None:
+                self.vals = copy(self.nums)
+
+        elif self.var.maxdim == 1:
+            npoints = max(x.shape[0] if len(x.shape) > 0 else 0 for x in self.var.nums)
+            self.nums = np.empty(npoints)
+            if self.side == VarStatSide.BOTH:
+                self.nums = np.empty((npoints, 2))
+            elif self.side == VarStatSide.ALL:
+                self.nums = np.empty((npoints, 3))
+            for i in range(npoints):
+                numsatidx = [x[i] for x in self.var.nums
+                             if (len(x.shape) > 0 and x.shape[0] > i)]
+                sortednums = sorted(numsatidx)
+                if self.side == VarStatSide.LOW:
+                    sortednums.reverse()
+                if self.side in (VarStatSide.HIGH, VarStatSide.LOW):
+                    self.nums[i] = sortednums[-self.k]
+                elif self.side == VarStatSide.BOTH:
+                    self.nums[i, :] = [sortednums[self.k - 1], sortednums[-self.k]]
+                elif self.side == VarStatSide.ALL:
+                    self.nums[i, :] = [sortednums[self.k - 1],
+                                       sortednums[int(np.round(len(sortednums)/2)-1)],
+                                       sortednums[-self.k]]
+            if self.var.nummap is not None:
+                self.vals = np.array([[self.var.nummap[x] for x in y] for y in self.nums])
+            else:
+                self.vals = copy(self.nums)
+
+        else:
+            # Suppress warning since this will become valid when Var is split
+            # warn('VarStat only available for scalar or 1-D data')
+            pass
+
+
+    def genStatsOrderStatP(self) -> None:
+        """Get the order statistic percentile value of the variable."""
+        self.checkOrderStatsKWArgs()
+
+        bound = self.bound
+        if self.bound not in (StatBound.ONESIDED_UPPER, StatBound.ONESIDED_LOWER,
+                              StatBound.TWOSIDED, StatBound.NEAREST, StatBound.ALL):
+            raise ValueError(f'{self.bound} is not a valid bound for genStatsOrderStatP')
+        elif self.bound in (StatBound.NEAREST, StatBound.ALL):
+            bound = StatBound.TWOSIDED
+
+        self.setName(f'{self.var.name} ' +
+                     f'{self.bound} {self.c*100}% Confidence Bound around ' +
+                     f'{self.p*100}th Percentile')
+
+        self.k = order_stat_P_k(n=self.var.ncases, P=self.p, c=self.c, bound=bound)
+
+        (iPl, iP, iPu) = get_iP(n=self.var.ncases, P=self.p)
+        if self.var.isscalar:
+            sortednums = sorted(self.var.nums)
+            if self.bound == StatBound.ONESIDED_LOWER:
+                self.nums = np.array(sortednums[iPl - self.k])
+            elif self.bound == StatBound.ONESIDED_UPPER:
+                self.nums = np.array(sortednums[iPu + self.k])
+            elif self.bound == StatBound.NEAREST:
+                self.nums = np.array(sortednums[iP])
+            if self.bound in (StatBound.ONESIDED_LOWER,
+                              StatBound.ONESIDED_UPPER,
+                              StatBound.NEAREST):
+                if self.var.nummap is not None:
+                    self.vals = self.var.nummap[self.nums.item()]
+            elif self.bound == StatBound.TWOSIDED:
+                self.nums = np.array([sortednums[iPl - self.k], sortednums[iPu + self.k]])
+                if self.var.nummap is not None:
+                    self.vals = np.array([self.var.nummap[self.nums[0]],
+                                          self.var.nummap[self.nums[1]]])
+            elif self.bound == StatBound.ALL:
+                self.nums = np.array([sortednums[iPl - self.k],
+                                      sortednums[iP],
+                                      sortednums[iPu + self.k]])
+                if self.var.nummap is not None:
+                    self.vals = np.array([self.var.nummap[self.nums[0]],
+                                          self.var.nummap[self.nums[1]],
+                                          self.var.nummap[self.nums[2]]])
+            if self.var.nummap is None:
+                self.vals = copy(self.nums)
+
+        elif self.var.maxdim == 1:
+            npoints = max(len(get_list(x)) for x in self.var.nums)
+            self.nums = np.empty(npoints)
+            if self.bound == StatBound.TWOSIDED:
+                self.nums = np.empty((npoints, 2))
+            elif self.bound == StatBound.ALL:
+                self.nums = np.empty((npoints, 3))
+            for i in range(npoints):
+                numsatidx = [get_list(x)[i] for x in self.var.nums if len(get_list(x)) > i]
+                sortednums = sorted(numsatidx)
+                if self.bound == StatBound.ONESIDED_LOWER:
+                    self.nums[i] = sortednums[iPl - self.k]
+                elif self.bound == StatBound.ONESIDED_UPPER:
+                    self.nums[i] = sortednums[iPu + self.k]
+                elif self.bound == StatBound.NEAREST:
+                    self.nums[i] = sortednums[iP]
+                elif self.bound == StatBound.TWOSIDED:
+                    self.nums[i, :] = [sortednums[iPl - self.k], sortednums[iPu + self.k]]
+                elif self.bound == StatBound.ALL:
+                    self.nums[i, :] = [sortednums[iPl - self.k],
+                                       sortednums[iP],
+                                       sortednums[iPu + self.k]]
+            if self.var.nummap is not None:
+                self.vals = np.array([[self.var.nummap[x] for x in y] for y in self.nums])
+            else:
+                self.vals = copy(self.nums)
+
+        else:
+            # Suppress warning since this will become valid when Var is split
+            # warn('VarStat only available for scalar or 1-D data')
+            pass
+
+
+    def checkOrderStatsKWArgs(self) -> None:
+        """Check the order statistic keyword arguments."""
+        if 'p' not in self.statkwargs:
+            raise ValueError(f'{self.stat} requires the kwarg ''p''')
+        else:
+            self.p = self.statkwargs['p']
+        if 'c' not in self.statkwargs:
+            self.c = 0.95
+        else:
+            self.c = self.statkwargs['c']
+        if 'bound' not in self.statkwargs:
+            self.bound = StatBound.TWOSIDED
+        else:
+            self.bound = self.statkwargs['bound']
+
+
+    def setName(self,
+                name : str,
+                ) -> None:
+        """
+        Set the name for this variable statistic.
+
+        Parameters
+        ----------
+        name : str
+            The new name.
+        """
+        if self.name is None:
+            self.name = name
```

### Comparing `monaco-0.9.0/src/monaco/order_statistics.py` & `monaco-0.9.1/src/monaco/order_statistics.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/src/monaco/tqdm_dask_distributed.py` & `monaco-0.9.1/src/monaco/tqdm_dask_distributed.py`

 * *Files identical despite different names*

### Comparing `monaco-0.9.0/setup.py` & `monaco-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cloudpickle>=2.0,<3.0',
  'distributed>=2022,<2023',
  'matplotlib>=3.6,<4.0',
- 'numba>=0.55,<0.56',
- 'numpy>=1.22,<2.0',
+ 'numpy>=1.23,<2.0',
  'pillow>=9.3.0',
  'psutil>=5.0,<6.0',
  'scipy>=1.10,<2.0',
  'tqdm>=4.0,<5.0']
 
 extras_require = \
 {'docs': ['sphinx>=4.2,<5.0',
           'sphinx_rtd_theme>=1.0,<2.0',
           'myst-parser>=0.15'],
+ 'numba:python_version < "3.11"': ['numba>=0.56,<0.57'],
  'pandas': ['pandas>=1.5,<2.0']}
 
 setup_kwargs = {
     'name': 'monaco',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Quantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.',
-    'long_description': '<p float="center" align="center">\n<img width="570" height="150" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/monaco_logo.png">  \n</p>\n\n![Release](https://img.shields.io/github/v/release/scottshambaugh/monaco?sort=semver)\n![Builds](https://github.com/scottshambaugh/monaco/actions/workflows/builds.yml/badge.svg)\n![Tests](https://github.com/scottshambaugh/monaco/actions/workflows/tests.yml/badge.svg)\n[![Docs](https://readthedocs.org/projects/monaco/badge/?version=latest)](https://monaco.readthedocs.io/en/latest/?badge=latest)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monaco)\n\nQuantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.\n\n### Overview\n\nAt the heart of all serious forecasting, whether that be of elections, the spread of pandemics, weather, or the path of a rocket on its way to Mars, is a statistical tool known as the [Monte Carlo method](https://en.wikipedia.org/wiki/Monte_Carlo_method). The Monte Carlo method, named for the rolling of the dice at the famous Monte Carlo casino located in Monaco, allows you to quantify uncertainty by introducing randomness to otherwise deterministic processes, and seeing what the range of results is.\n\n<p float="left" align="center">\n<img width="500" height="250" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/analysis_process.png">\n</p>\n\n`monaco` is a python library for analyzing uncertainties and sensitivities in your computational models by setting up, running, and analyzing a Monte Carlo simulation wrapped around that model. Users can define random input variables drawn using chosen sampling methods from any of SciPy\'s continuous or discrete distributions (including custom distributions), preprocess and structure that data as needed to feed to their main simulation, run that simulation in parallel anywhere from 1 to millions of times, and postprocess the simulation outputs to obtain meaningful, statistically significant conclusions. Plotting and statistical functions specific to use cases that might be encountered are provided, and repeatability of results is ensured through careful management of random seeds.\n\n<p float="left" align="center">\n<img width="350" height="350" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/baseball_trajectory.png">\n<img width="440" height="330" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/launch_angle_vs_landing.png">\n</p>\n\n### Quick Start\nFirst, install `monaco`:\n```\npip install monaco\n```\nThen, copy the two files from the [template directory](https://github.com/scottshambaugh/monaco/tree/main/template), which contains a simple, well commented Monte Carlo simulation of flipping coins. That link also contains some exercises for you to do, to help you familiarize yourself with how `monaco` is structured.\n\nAfter working through the template exercises, check out the other [examples](https://github.com/scottshambaugh/monaco/tree/main/examples) for inspiration and more in-depth usage of `monaco`\'s features.\n\n### Documentation / API Reference / SciPy 2022 Talk\n\nDocumentation is being built up - read the docs here: https://monaco.readthedocs.io\n\nCurrently there is a complete [API reference](https://monaco.readthedocs.io/en/latest/api_reference.html), more detailed [installation, test, and publishing](https://monaco.readthedocs.io/en/latest/installation.html) instructions, an overview of the [basic architecture](https://monaco.readthedocs.io/en/latest/basic_architecture.html) and [basic workflow](https://monaco.readthedocs.io/en/latest/basic_workflow.html), and some details on [statistical distributions](https://monaco.readthedocs.io/en/latest/statistical_distributions.html) and [sampling methods](https://monaco.readthedocs.io/en/latest/sampling_methods.html). \n\nMonaco was presented at the SciPy 2022 Conference, and the conference resources should give another good overview of the library. Check out [the paper](https://conference.scipy.org/proceedings/scipy2022/pdfs/scott_shambaugh.pdf), [the video of the talk](https://www.youtube.com/watch?v=yB539OIol_s), and [the talk\'s slides and notebooks](https://github.com/scottshambaugh/monaco-scipy2022).\n\n### License / Citation\nCopyright 2020-2022 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).\n\nIf you use `monaco` to do research that gets published, please cite the conference paper using the below or [monaco.bib](monaco.bib):    \n> W. Scott Shambaugh (2022). Monaco: A Monte Carlo Library for Performing Uncertainty and Sensitivity Analyses. *In Proceedings of the 21st Python in Science Conference* (pp. 202 - 208).\n\n### Further Reading\n* [Hanson, J. M., and B. B. Beard. "Applying Monte Carlo simulation to launch vehicle design and requirements analysis." National Aeronautics and Space Administration, Marshall Space Flight Center, 1 September 2010.](https://ntrs.nasa.gov/citations/20100038453)\n* [Razavi, S. et. al. "The future of sensitivity analysis: an essential discipline for systems modeling and policy support." Environmental Modelling & Software Volume 137, March 2021.](https://www.sciencedirect.com/science/article/pii/S1364815220310112)\n* [Satelli, A. et. al. "Why so many published sensitivity analyses are false: A systematic review of sensitivity analysis practices." Environmental Modelling & Software Volume 114, April 2019.](https://www.sciencedirect.com/science/article/pii/S1364815218302822)\n',
+    'long_description': '<p float="center" align="center">\n<img width="570" height="150" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/monaco_logo.png">  \n</p>\n\n![Release](https://img.shields.io/github/v/release/scottshambaugh/monaco?sort=semver)\n![Builds](https://github.com/scottshambaugh/monaco/actions/workflows/builds.yml/badge.svg)\n![Tests](https://github.com/scottshambaugh/monaco/actions/workflows/tests.yml/badge.svg)\n[![Docs](https://readthedocs.org/projects/monaco/badge/?version=latest)](https://monaco.readthedocs.io/en/latest/?badge=latest)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monaco)\n\nQuantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.\n\n### Overview\n\nAt the heart of all serious forecasting, whether that be of elections, the spread of pandemics, weather, or the path of a rocket on its way to Mars, is a statistical tool known as the [Monte Carlo method](https://en.wikipedia.org/wiki/Monte_Carlo_method). The Monte Carlo method, named for the rolling of the dice at the famous Monte Carlo casino located in Monaco, allows you to quantify uncertainty by introducing randomness to otherwise deterministic processes, and seeing what the range of results is.\n\n<p float="left" align="center">\n<img width="500" height="250" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/docs/images/analysis_process.png">\n</p>\n\n`monaco` is a python library for analyzing uncertainties and sensitivities in your computational models by setting up, running, and analyzing a Monte Carlo simulation wrapped around that model. Users can define random input variables drawn using chosen sampling methods from any of SciPy\'s continuous or discrete distributions (including custom distributions), preprocess and structure that data as needed to feed to their main simulation, run that simulation in parallel anywhere from 1 to millions of times, and postprocess the simulation outputs to obtain meaningful, statistically significant conclusions. Plotting and statistical functions specific to use cases that might be encountered are provided, and repeatability of results is ensured through careful management of random seeds.\n\n<p float="left" align="center">\n<img width="350" height="350" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/baseball_trajectory.png">\n<img width="440" height="330" src="https://raw.githubusercontent.com/scottshambaugh/monaco/main/examples/baseball/launch_angle_vs_landing.png">\n</p>\n\n### Quick Start\nFirst, install `monaco`:\n```\npip install monaco\n```\nThen, copy the two files from the [template directory](https://github.com/scottshambaugh/monaco/tree/main/template), which contains a simple, well commented Monte Carlo simulation of flipping coins. That link also contains some exercises for you to do, to help you familiarize yourself with how `monaco` is structured.\n\nAfter working through the template exercises, check out the other [examples](https://github.com/scottshambaugh/monaco/tree/main/examples) for inspiration and more in-depth usage of `monaco`\'s features.\n\n### Documentation / API Reference / SciPy 2022 Talk\n\nDocumentation is being built up - read the docs here: https://monaco.readthedocs.io\n\nCurrently there is a complete [API reference](https://monaco.readthedocs.io/en/latest/api_reference.html), more detailed [installation, test, and publishing](https://monaco.readthedocs.io/en/latest/installation.html) instructions, an overview of the [basic architecture](https://monaco.readthedocs.io/en/latest/basic_architecture.html) and [basic workflow](https://monaco.readthedocs.io/en/latest/basic_workflow.html), and some details on [statistical distributions](https://monaco.readthedocs.io/en/latest/statistical_distributions.html) and [sampling methods](https://monaco.readthedocs.io/en/latest/sampling_methods.html). \n\nMonaco was presented at the SciPy 2022 Conference, and the conference resources should give another good overview of the library. Check out [the paper](https://conference.scipy.org/proceedings/scipy2022/pdfs/scott_shambaugh.pdf), [the video of the talk](https://www.youtube.com/watch?v=yB539OIol_s), and [the talk\'s slides and notebooks](https://github.com/scottshambaugh/monaco-scipy2022).\n\n### License / Citation\nCopyright 2020-2023 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).\n\nIf you use `monaco` to do research that gets published, please cite the conference paper using the below or [monaco.bib](monaco.bib):    \n> W. Scott Shambaugh (2022). Monaco: A Monte Carlo Library for Performing Uncertainty and Sensitivity Analyses. *In Proceedings of the 21st Python in Science Conference* (pp. 202 - 208).\n\n### Further Reading\n* [Hanson, J. M., and B. B. Beard. "Applying Monte Carlo simulation to launch vehicle design and requirements analysis." National Aeronautics and Space Administration, Marshall Space Flight Center, 1 September 2010.](https://ntrs.nasa.gov/citations/20100038453)\n* [Razavi, S. et. al. "The future of sensitivity analysis: an essential discipline for systems modeling and policy support." Environmental Modelling & Software Volume 137, March 2021.](https://www.sciencedirect.com/science/article/pii/S1364815220310112)\n* [Satelli, A. et. al. "Why so many published sensitivity analyses are false: A systematic review of sensitivity analysis practices." Environmental Modelling & Software Volume 114, April 2019.](https://www.sciencedirect.com/science/article/pii/S1364815218302822)\n',
     'author': 'Scott Shambaugh',
     'author_email': 'scott@theshamblog.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scottshambaugh/monaco/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8.0,<3.11',
+    'python_requires': '>=3.8.0,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `monaco-0.9.0/PKG-INFO` & `monaco-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: monaco
-Version: 0.9.0
+Version: 0.9.1
 Summary: Quantify uncertainty and sensitivities in your computer models with an industry-grade Monte Carlo library.
 Home-page: https://github.com/scottshambaugh/monaco/
 License: GPL-3.0-or-later
 Author: Scott Shambaugh
 Author-email: scott@theshamblog.com
-Requires-Python: >=3.8.0,<3.11
+Requires-Python: >=3.8.0,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Provides-Extra: docs
+Provides-Extra: numba
 Provides-Extra: pandas
 Requires-Dist: cloudpickle (>=2.0,<3.0)
 Requires-Dist: distributed (>=2022,<2023)
 Requires-Dist: matplotlib (>=3.6,<4.0)
 Requires-Dist: myst-parser (>=0.15) ; extra == "docs"
-Requires-Dist: numba (>=0.55,<0.56)
-Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: numba (>=0.56,<0.57) ; (python_version < "3.11") and (extra == "numba")
+Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=1.5,<2.0) ; extra == "pandas"
 Requires-Dist: pillow (>=9.3.0)
 Requires-Dist: psutil (>=5.0,<6.0)
 Requires-Dist: scipy (>=1.10,<2.0)
 Requires-Dist: sphinx (>=4.2,<5.0) ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme (>=1.0,<2.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.0,<5.0)
@@ -77,15 +79,15 @@
 Documentation is being built up - read the docs here: https://monaco.readthedocs.io
 
 Currently there is a complete [API reference](https://monaco.readthedocs.io/en/latest/api_reference.html), more detailed [installation, test, and publishing](https://monaco.readthedocs.io/en/latest/installation.html) instructions, an overview of the [basic architecture](https://monaco.readthedocs.io/en/latest/basic_architecture.html) and [basic workflow](https://monaco.readthedocs.io/en/latest/basic_workflow.html), and some details on [statistical distributions](https://monaco.readthedocs.io/en/latest/statistical_distributions.html) and [sampling methods](https://monaco.readthedocs.io/en/latest/sampling_methods.html). 
 
 Monaco was presented at the SciPy 2022 Conference, and the conference resources should give another good overview of the library. Check out [the paper](https://conference.scipy.org/proceedings/scipy2022/pdfs/scott_shambaugh.pdf), [the video of the talk](https://www.youtube.com/watch?v=yB539OIol_s), and [the talk's slides and notebooks](https://github.com/scottshambaugh/monaco-scipy2022).
 
 ### License / Citation
-Copyright 2020-2022 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).
+Copyright 2020-2023 Scott Shambaugh, distributed under [the GPLv3.0 (or later) license](LICENSE.md).
 
 If you use `monaco` to do research that gets published, please cite the conference paper using the below or [monaco.bib](monaco.bib):    
 > W. Scott Shambaugh (2022). Monaco: A Monte Carlo Library for Performing Uncertainty and Sensitivity Analyses. *In Proceedings of the 21st Python in Science Conference* (pp. 202 - 208).
 
 ### Further Reading
 * [Hanson, J. M., and B. B. Beard. "Applying Monte Carlo simulation to launch vehicle design and requirements analysis." National Aeronautics and Space Administration, Marshall Space Flight Center, 1 September 2010.](https://ntrs.nasa.gov/citations/20100038453)
 * [Razavi, S. et. al. "The future of sensitivity analysis: an essential discipline for systems modeling and policy support." Environmental Modelling & Software Volume 137, March 2021.](https://www.sciencedirect.com/science/article/pii/S1364815220310112)
```

