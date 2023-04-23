# Comparing `tmp/jax-moseq-0.0.1.tar.gz` & `tmp/jax-moseq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-moseq-0.0.1.tar", last modified: Mon Mar 27 14:16:15 2023, max compression
+gzip compressed data, was "jax-moseq-0.0.2.tar", last modified: Sun Apr 23 11:41:17 2023, max compression
```

## Comparing `jax-moseq-0.0.1.tar` & `jax-moseq-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.047676 jax-moseq-0.0.1/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-03-26 05:27:05.000000 jax-moseq-0.0.1/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-03-27 14:16:15.047809 jax-moseq-0.0.1/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1689 2023-03-26 05:27:05.000000 jax-moseq-0.0.1/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.007762 jax-moseq-0.0.1/jax_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       51 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.031421 jax-moseq-0.0.1/jax_moseq/models/
--rw-rw-r--   0 calebweinreb   (501) staff       (20)       67 2023-01-25 16:50:06.000000 jax-moseq-0.0.1/jax_moseq/models/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.035357 jax-moseq-0.0.1/jax_moseq/models/arhmm/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      182 2023-03-08 21:10:51.000000 jax-moseq-0.0.1/jax_moseq/models/arhmm/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6584 2023-03-08 21:10:51.000000 jax-moseq-0.0.1/jax_moseq/models/arhmm/generate.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6334 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/arhmm/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8064 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/arhmm/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3422 2023-01-13 01:06:04.000000 jax-moseq-0.0.1/jax_moseq/models/arhmm/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.039134 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      215 2023-01-10 16:23:57.000000 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13504 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/alignment.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    10739 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    14485 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4833 2023-01-13 01:14:21.000000 jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.042546 jax-moseq-0.0.1/jax_moseq/models/slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      133 2023-01-10 16:23:57.000000 jax-moseq-0.0.1/jax_moseq/models/slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9776 2023-03-08 02:07:28.000000 jax-moseq-0.0.1/jax_moseq/models/slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    10217 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/models/slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4081 2023-03-23 23:22:11.000000 jax-moseq-0.0.1/jax_moseq/models/slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.047198 jax-moseq-0.0.1/jax_moseq/utils/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       35 2023-01-10 16:23:57.000000 jax-moseq-0.0.1/jax_moseq/utils/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1148 2023-01-13 01:04:53.000000 jax-moseq-0.0.1/jax_moseq/utils/autoregression.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2584 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/utils/distributions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4287 2023-03-10 20:57:13.000000 jax-moseq-0.0.1/jax_moseq/utils/kalman.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11693 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/utils/transitions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9619 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/jax_moseq/utils/utils.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-27 14:16:15.030940 jax-moseq-0.0.1/jax_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-03-27 14:16:14.000000 jax-moseq-0.0.1/jax_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      955 2023-03-27 14:16:14.000000 jax-moseq-0.0.1/jax_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-03-27 14:16:14.000000 jax-moseq-0.0.1/jax_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       31 2023-03-27 14:16:14.000000 jax-moseq-0.0.1/jax_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-03-27 14:16:14.000000 jax-moseq-0.0.1/jax_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-03-27 14:16:15.048334 jax-moseq-0.0.1/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      706 2023-03-27 14:15:59.000000 jax-moseq-0.0.1/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.314046 jax-moseq-0.0.2/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-04-23 11:41:17.314255 jax-moseq-0.0.2/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1689 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.267315 jax-moseq-0.0.2/jax_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       51 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.274356 jax-moseq-0.0.2/jax_moseq/models/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       67 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.278501 jax-moseq-0.0.2/jax_moseq/models/arhmm/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      182 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6584 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/generate.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6677 2023-04-22 07:30:26.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8064 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     3422 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.283383 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      215 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13504 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/alignment.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11127 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    14485 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4833 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.307825 jax-moseq-0.0.2/jax_moseq/models/slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      133 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9776 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    10217 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4081 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.313097 jax-moseq-0.0.2/jax_moseq/utils/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       35 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1148 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/autoregression.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2584 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/distributions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4287 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/kalman.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11693 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/transitions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11079 2023-04-21 10:38:44.000000 jax-moseq-0.0.2/jax_moseq/utils/utils.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.272970 jax-moseq-0.0.2/jax_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      955 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       38 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-23 11:41:17.315075 jax-moseq-0.0.2/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      840 2023-04-23 11:39:38.000000 jax-moseq-0.0.2/setup.py
```

### Comparing `jax-moseq-0.0.1/LICENSE.md` & `jax-moseq-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/README.md` & `jax-moseq-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/arhmm/generate.py` & `jax-moseq-0.0.2/jax_moseq/models/arhmm/generate.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/arhmm/gibbs.py` & `jax-moseq-0.0.2/jax_moseq/models/arhmm/gibbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 
-from jax_moseq.utils import pad_affine, psd_solve, psd_inv
+from jax_moseq.utils import pad_affine, psd_solve, psd_inv, convert_data_precision
 
 from jax_moseq.utils.distributions import (
     sample_mniw,
     sample_hmm_stateseq
 )
 from jax_moseq.utils.autoregression import (
     get_lags,
@@ -51,15 +51,15 @@
 
     log_likelihoods = jax.lax.map(partial(ar_log_likelihood, x), (Ab, Q))
     _, z = jax.vmap(sample_hmm_stateseq, in_axes=(0,na,0,0))(
         jr.split(seed, num_samples),
         pi,
         jnp.moveaxis(log_likelihoods,0,-1),
         mask.astype(float)[:,nlags:])
-    return z
+    return convert_data_precision(z)
 
 
 @partial(jax.jit, static_argnames=('num_states','nlags'))
 def resample_ar_params(seed, *, nlags, num_states, mask, x, z,
                        nu_0, S_0, M_0, K_0, **kwargs):
     """
     Resamples the AR parameters ``Ab`` and ``Q``.
@@ -150,16 +150,17 @@
     K_n = psd_inv(K_n_inv)
     M_n = psd_solve(K_n_inv.T, K_0_inv @ M_0.T + S_out_in.T).T  
      
     S_n = S_0 + S_out_out + (M_0 @ K_0_inv @ M_0.T - M_n @ K_n_inv @ M_n.T)
     return sample_mniw(seed, nu_0 + mask.sum(), S_n, M_n, K_n)
 
 
+
 def resample_model(data, seed, states, params, hypparams,
-                   states_only=False, **kwargs):
+                   states_only=False, verbose=False, **kwargs):
     """
     Resamples the ARHMM model given the hyperparameters, data,
     current states, and current parameters.
 
     Parameters
     ----------
     data : dict
@@ -170,34 +171,39 @@
         State values for each latent variable.
     params : dict
         Values for each model parameter.
     hypparams : dict
         Values for each group of hyperparameters.
     states_only : bool, default=False
         Whether to restrict sampling to states.
+    verbose : bool, default=False
+        Whether to print progress info during resampling.
     **kwargs : dict
         Overflow, for convenience.
 
     Returns
     ------
     model : dict
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
     seed = jr.split(seed)[1]
 
     if not states_only: 
+        if verbose: print('Resampling pi (transition matrix)')
         params['betas'], params['pi'] = resample_hdp_transitions(
             seed, **data, **states, **params, 
             **hypparams['trans_hypparams'])
 
+        if verbose: print('Resampling Ab,Q (AR parameters)')
         params['Ab'], params['Q']= resample_ar_params(
             seed, **data, **states, **params, 
             **hypparams['ar_hypparams'])
 
+    if verbose: print('Resampling z (discrete latent states)')
     states['z'] = resample_discrete_stateseqs(
         seed, **data, **states, **params)
 
     return {'seed': seed,
             'states': states, 
             'params': params, 
             'hypparams': hypparams}
```

### Comparing `jax-moseq-0.0.1/jax_moseq/models/arhmm/initialize.py` & `jax-moseq-0.0.2/jax_moseq/models/arhmm/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/arhmm/log_prob.py` & `jax-moseq-0.0.2/jax_moseq/models/arhmm/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/alignment.py` & `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/alignment.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/gibbs.py` & `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/gibbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -283,17 +283,19 @@
     in_axes = (0,0,0,0,na,na,na,na,na,na,na,0)
     v = jax.vmap(kalman_sample, in_axes)(
         seed, mu, mask[:,:-1], zz, m0,
         S0, A, B, Q, C, D, R)
     return v
 
 
+
 def resample_model(data, seed, states, params, hypparams,
                    noise_prior, ar_only=False, states_only=False,
-                   skip_noise=False, fix_heading=False, **kwargs):
+                   skip_noise=False, fix_heading=False, verbose=False,
+                   **kwargs):
     """
     Resamples the Keypoint SLDS model given the hyperparameters,
     data, noise prior, current states, and current parameters.
 
     Parameters
     ----------
     data : dict
@@ -312,50 +314,55 @@
         Whether to restrict sampling to ARHMM components.
     states_only : bool, default=False
         Whether to restrict sampling to states.
     skip_noise : bool, default=False
         Whether to exclude ``sigmasq`` and ``s`` from resampling.
     fix_heading : bool, default=False
         Whether to exclude ``h`` from resampling.
-    **kwargs : dict
-        Overflow, for convenience.
+    verbose : bool, default=False
+        Whether to print progress info during resampling.
 
     Returns
     ------
     model : dict
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
     model = arhmm.resample_model(data, seed, states, params,
-                                 hypparams, states_only)
+                                 hypparams, states_only, verbose=verbose)
     if ar_only:
         model['noise_prior'] = noise_prior
         return model
     
     seed = model['seed']
     params = model['params']
     states = model['states']
 
     if not (states_only or skip_noise):
+        if verbose: print('Resampling sigmasq (global noise scales)')
         params['sigmasq'] = resample_obs_variance(
             seed, **data, **states, **params, 
             s_0=noise_prior, **hypparams['obs_hypparams'])
 
+    if verbose: print('Resampling x (continuous latent states)')
     states['x'] = resample_continuous_stateseqs(
         seed, **data, **states, **params)
 
     if not fix_heading:
+        if verbose: print('Resampling h (heading)')
         states['h'] = resample_heading(
             seed, **data, **states, **params)
 
+    if verbose: print('Resampling v (location)')
     states['v'] = resample_location(
         seed, **data, **states, **params, 
         **hypparams['cen_hypparams'])
 
     if not skip_noise:
+        if verbose: print('Resampling s (local noise scales)')
         states['s'] = resample_scales(
             seed, **data, **states, **params, 
             s_0=noise_prior, **hypparams['obs_hypparams'])
 
     return {'seed': seed,
             'states': states, 
             'params': params,
```

### Comparing `jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/initialize.py` & `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/keypoint_slds/log_prob.py` & `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/slds/gibbs.py` & `jax-moseq-0.0.2/jax_moseq/models/slds/gibbs.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/slds/initialize.py` & `jax-moseq-0.0.2/jax_moseq/models/slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/models/slds/log_prob.py` & `jax-moseq-0.0.2/jax_moseq/models/slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/utils/autoregression.py` & `jax-moseq-0.0.2/jax_moseq/utils/autoregression.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/utils/distributions.py` & `jax-moseq-0.0.2/jax_moseq/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/utils/kalman.py` & `jax-moseq-0.0.2/jax_moseq/utils/kalman.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/utils/transitions.py` & `jax-moseq-0.0.2/jax_moseq/utils/transitions.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.1/jax_moseq/utils/utils.py` & `jax-moseq-0.0.2/jax_moseq/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from jax.tree_util import tree_map
 from sklearn.decomposition import PCA
 from jax.scipy.linalg import cho_factor, cho_solve
 import inspect
 import functools
 from textwrap import fill
 
+# JAX has its own implementation of `tree_flatten_with_path` 
+# but it's only in version of 0.4.6 or later, and currently 
+# some platforms (e.g. Windows) require installing < 0.4.6
+from optree import tree_flatten_with_path
+
+
 
 def symmetrize(A):
     """Symmetrize a matrix."""
     return (A + A.swapaxes(-1, -2)) / 2
 
 def psd_solve(A, B, diagonal_boost=1e-6):
     """
@@ -281,8 +287,49 @@
     def convert(x):
         x = jnp.asarray(x)
         if jnp.issubdtype(x.dtype, jnp.integer):
             return x.astype(jnp.int64 if x64 else jnp.int32)
         elif jnp.issubdtype(x.dtype, jnp.floating):
             return x.astype(jnp.float64 if x64 else jnp.float32)
     
-    return jax.tree_map(convert, data)
+    return jax.tree_map(convert, data)
+
+
+def check_for_nans(data):
+    """
+    Check for NaNs in all arrays of a pytree.
+
+    Parameters
+    ----------
+    data: pytree (dict, list, tuple, array, or any nested combination thereof)
+        The data to check for NaNs in.
+    
+    Returns
+    -------
+    any_nans: bool
+        Whether any of the arrays in ``data`` contain a NaN.
+
+    nan_info: list of tuples
+        List of arrays containing a NaN, in the form of pairs
+        ``(path, number_of_nans)`` where ``path`` is a sequence of
+        keys that define the location of the array in the pytree.
+
+    messages: list of str
+        List of messages; one for each elements of ``nan_info``.
+    """
+
+    def _format(path, num_nan):
+        path = '/'.join(map(str,path))
+        msg  = f"{num_nan} NaNs found in {path}"
+        return msg
+        
+    nan_info = []
+    messages = []
+    for path,value in zip(*tree_flatten_with_path(data)[:2]):
+        if isinstance(value, jnp.ndarray):
+            if jnp.isnan(value).any():
+                num_nans = jnp.isnan(value).sum().item()
+                nan_info.append((path, num_nans))
+                messages.append(_format(path, num_nans))
+    
+    any_nans = len(nan_info)>0
+    return any_nans, nan_info, messages
```

### Comparing `jax-moseq-0.0.1/jax_moseq.egg-info/SOURCES.txt` & `jax-moseq-0.0.2/jax_moseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

