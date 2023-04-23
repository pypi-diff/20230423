# Comparing `tmp/hmcode-1.0.1.tar.gz` & `tmp/hmcode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmcode-1.0.1.tar", max compression
+gzip compressed data, was "hmcode-1.1.0.tar", max compression
```

## Comparing `hmcode-1.0.1.tar` & `hmcode-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1023 2023-02-22 15:20:40.854089 hmcode-1.0.1/LICENSE
--rw-r--r--   0        0        0     8402 2023-03-03 16:00:08.822036 hmcode-1.0.1/README.md
--rw-r--r--   0        0        0       25 2023-02-28 19:51:12.054675 hmcode-1.0.1/hmcode/__init__.py
--rw-r--r--   0        0        0     1520 2023-02-22 15:35:46.911665 hmcode-1.0.1/hmcode/camb_stuff.py
--rw-r--r--   0        0        0      622 2023-02-27 13:04:59.996680 hmcode-1.0.1/hmcode/constants.py
--rw-r--r--   0        0        0    10197 2023-02-27 17:37:02.247489 hmcode-1.0.1/hmcode/cosmology.py
--rw-r--r--   0        0        0    13457 2023-02-28 19:33:41.516011 hmcode-1.0.1/hmcode/hmcode.py
--rw-r--r--   0        0        0     3918 2023-02-27 13:05:19.637254 hmcode-1.0.1/hmcode/linear_growth.py
--rw-r--r--   0        0        0     1687 2023-02-28 19:47:28.465586 hmcode-1.0.1/hmcode/utility.py
--rw-r--r--   0        0        0      557 2023-03-10 21:32:13.833588 hmcode-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9282 1970-01-01 00:00:00.000000 hmcode-1.0.1/setup.py
--rw-r--r--   0        0        0     9243 1970-01-01 00:00:00.000000 hmcode-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1023 2023-02-22 15:20:40.854089 hmcode-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9291 2023-04-23 14:27:19.425647 hmcode-1.1.0/README.md
+-rw-r--r--   0        0        0       25 2023-04-14 21:37:50.414430 hmcode-1.1.0/hmcode/__init__.py
+-rw-r--r--   0        0        0     1879 2023-04-23 14:27:19.428579 hmcode-1.1.0/hmcode/camb_stuff.py
+-rw-r--r--   0        0        0      641 2023-04-23 14:27:19.429409 hmcode-1.1.0/hmcode/constants.py
+-rw-r--r--   0        0        0    10200 2023-04-23 14:27:19.429907 hmcode-1.1.0/hmcode/cosmology.py
+-rw-r--r--   0        0        0    17838 2023-04-23 14:27:19.430740 hmcode-1.1.0/hmcode/hmcode.py
+-rw-r--r--   0        0        0     3882 2023-04-23 14:27:19.431432 hmcode-1.1.0/hmcode/linear_growth.py
+-rw-r--r--   0        0        0     1690 2023-04-23 14:27:19.431902 hmcode-1.1.0/hmcode/utility.py
+-rw-r--r--   0        0        0      557 2023-04-23 14:28:26.892650 hmcode-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10180 1970-01-01 00:00:00.000000 hmcode-1.1.0/setup.py
+-rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 hmcode-1.1.0/PKG-INFO
```

### Comparing `hmcode-1.0.1/LICENSE` & `hmcode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmcode-1.0.1/README.md` & `hmcode-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # HMcode
 
+![image](https://user-images.githubusercontent.com/9140961/228345397-f33d2f94-e8e4-4eb0-9fc9-9b27df407fbc.png)
+
 A pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.
 
 ## Installation
 
 Either
-```
-pip install hmcode
+```bash
+> pip install hmcode
 ```
 or, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then
-```
-poetry install
+```bash
+> poetry install
 ```
 to create a virtual environment with everything you need to get going.
 
 ## Dependencies
 
 - `numpy`
 - `scipy`
@@ -27,43 +29,50 @@
 import numpy as np
 import camb
 import hmcode
 
 # Ranges
 k = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]
 zs = [3., 2., 1., 0.5, 0.]  # Redshifts
+T_AGN = 10**7.8             # Feedback temperature [K]
 
 # Run CAMB
 parameters = camb.CAMBparams(WantCls=False)
 parameters.set_cosmology(H0=70.)
 parameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest
 results = camb.get_results(parameters)
 
 # HMcode
-Pk = hmcode.power(k, zs, results)
+Pk = hmcode.power(k, zs, results, T_AGN)
 ```
 
 ## Note
 
 To whom it may concern,
 
 I coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...
 
 You might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.
 
 I compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:
-- LCDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.21%
-- k-LCDM: Mean error: 0.11%; Std error: 0.03%; Worst error; 0.23%
-- w-CDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.20%
-- w(a)-CDM: Mean error: 0.13%; Std error: 0.06%; Worst error; 0.48%
-- nu-LCDM: Mean error: 0.47%; Std error: 0.44%; Worst error; 2.01% (larger errors strongly correlated with neutrino mass)
-- nu-k-w(a)-CDM: Mean error: 0.42%; Std error: 0.43%; Worst error; 2.02% (larger errors strongly correlated with neutrino mass)
+- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.21%
+- k-LCDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.23%
+- w-CDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.20%
+- w(a)-CDM: Mean error: 0.13%; Standard deviation of error: 0.06%; Worst-case error; 0.48%
+- nu-LCDM: Mean error: 0.47%; Standard deviation of error: 0.44%; Worst-case error; 2.01% (larger errors strongly correlated with neutrino mass)
+- nu-k-w(a)-CDM: Mean error: 0.42%; Standard deviation of error: 0.43%; Worst-case error; 2.02% (larger errors strongly correlated with neutrino mass)
 
 These comparisons can be reproduced using the `comparisons/CAMB.py` script.
 
+The power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:
+- LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%
+- nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)
+
+The comparisons can be reproduced using the `comparisons/CAMB_feedback.py` script.
+
 While the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:
 - Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.
 - Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).
 - If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.
 
 Using the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.
 
@@ -74,15 +83,15 @@
 - The $\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)
 - The linear growth ODE solution
 - Root finding for the halo-collapse redshift and for $R_\mathrm{nl}$
 
 But I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.
 
 While writing this code I had a few ideas for future improvements:
-- Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.
+- ~~Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.~~ (Thanks Laila Linke!)
 - The predictions are a bit sensitive to the smoothing $\sigma$ used for the dewiggling. This should probably be a fitted parameter.
 - It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$.
 - I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).
 - Redshift 'infinity' for the Dolag correction is actually $z_\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.
 - The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.
 - I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.
 - The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\delta_\mathrm{c}$; $\Delta_\mathrm{v}$; $\sigma(R)$; $R_\mathrm{nl}$; $n_\mathrm{eff}$; $c(M)$.
```

### Comparing `hmcode-1.0.1/hmcode/constants.py` & `hmcode-1.1.0/hmcode/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Standard imports
 from math import pi
 
 # Physical constants
 G = 6.6743e-11 # Newton constant [m^3 kg^-1 s^-2]
 
 # Astronomy
 Sun_mass = 1.9884e30 # Mass of the Sun [kg]
```

### Comparing `hmcode-1.0.1/hmcode/cosmology.py` & `hmcode-1.1.0/hmcode/cosmology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Standard imports
+# Third-party imports
 import numpy as np
 import scipy.integrate as integrate
 
 # Project imports
 from . import constants as const
 
 # Constants
```

### Comparing `hmcode-1.0.1/hmcode/hmcode.py` & `hmcode-1.1.0/hmcode/hmcode.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # Standard imports
-import numpy as np
 from time import time
 
 # Third-party imports
+import numpy as np
 import camb
 import pyhalomodel as halo
 
 # Project imports
 from . import utility as util
 from . import cosmology
 from . import linear_growth
 
 # Parameters
 Pk_lin_extrap_kmax = 1e10 # NOTE: This interplays with the sigmaV integration in a disconcerting way
 sigma_cold_approx = False # Should the Eisenstein & Hu (1999) approximation be used for the cold transfer function?
 
-def power(k:np.array, zs:np.array, CAMB_results:camb.CAMBdata, 
-          Mmin=1e0, Mmax=1e18, nM=256, verbose=False) -> np.ndarray:
+def power(k:np.array, zs:np.array, CAMB_results:camb.CAMBdata, T_AGN=None,
+          Mmin=1e0, Mmax=1e18, nM=256, tweaks=True, verbose=False) -> np.ndarray:
     '''
     Calculates the HMcode matter-matter power spectrum
     Args:
         k: Array of comoving wavenumbers [h/Mpc]
         zs: Array of redshifts (ordered from high to low)
         CAMB_results: CAMBdata structure
+        T_AGN: AGN feedback temperature [K] (None to disable)
         Mmin: Minimum mass for the halo-model calculation [Msun/h]
         Mmax: Maximum mass for the halo-model calculation [Msun/h]
         nM: Number of mass bins for the halo-model calculation
+        tweaks: Use the changes to the vanilla halo model from HMCode2020 if true
     Returns:
         Array of matter power spectra: Pk[z, k]
     '''
 
     # Checks
     if verbose: t_start = time()
     if not util.is_array_monotonic(-np.array(zs)):
-        raise ValueError('Redshift must be monotonically decreasing')
+        raise ValueError('Redshifts must be monotonically decreasing')
 
     # Halo mass range
     M = util.logspace(Mmin, Mmax, nM)
     zc = 10. # Redshift 'infinity' for the Dolay correction
     ac = cosmology.scalefactor_from_redshift(zc)
 
     # Background cosmology at z=0
@@ -56,14 +58,28 @@
         print('HMcode parameters')
         print('Halo mass range: 10^{:.1f} -> 10^{:.1f} Msun/h'.format(np.log10(Mmin), np.log10(Mmax)))
         print('Omega_m: {:.3}'.format(Om_m))
         print('Neutrino mass fraction: {:.2%}'.format(f_nu))
         print('Linear growth at z=0: {:.3}'.format(growth(1.)))
         print()
 
+    # Baryonic feedback
+    if T_AGN:
+        feedback_params = _get_feedback_parameters(T_AGN)
+        if verbose:
+            print('Using baryonic feedback model from HMCode2020')
+            print('log_10(T_AGN/K): {:.2f}'.format(np.log10(T_AGN)))
+            print('B_0: {:.4f}'.format(feedback_params['B0']))
+            print('B_z: {:.4f}'.format(feedback_params['Bz']))
+            print('Mb_0: {:.1e}'.format(feedback_params['Mb0']))
+            print('Mb_z: {:.4f}'.format(feedback_params['Mbz']))
+            print('f*_0: {:.4f}'.format(feedback_params['f0']))
+            print('f*_z: {:.4f}'.format(feedback_params['fz']))
+            print()
+
     # Linear power interpolator
     interp, _, k_interp = CAMB_results.get_matter_power_interpolator(nonlinear=False, 
                                                                      return_z_k=True,
                                                                      extrap_kmax=Pk_lin_extrap_kmax)
     Pk_lin_interp = interp.P
     kmin = k_interp[0] # Minimum wavenumber used for the CAMB interpolator [h/Mpc]
 
@@ -92,14 +108,15 @@
         if verbose:
             print('Un-normalisaed growth (= a for a << 1): {:.3}'.format(g))
             print('Normalised growth (= 1 at z = 0): {:.3}'.format(g/growth(1.)))
             print('Accumulated growth (= a for a << 1): {:.3}'.format(G))
             print('Linear collapse threshold: {:.4}'.format(dc))
             print('Virial halo overdensity: {:.4}'.format(Dv))
 
+
         # Initialise halo model
         hmod = halo.model(z, Om_m, name='Sheth & Tormen (1999)', Dv=Dv, dc=dc)
 
         # Linear power and associated quantities
         # Note that the cold matter spectrum is defined via 1+delta_c = rho_c/\bar{rho}_c
         # Where \bar{rho}_c is the mean background *cold* matter density
         # This means that the *cold* linear spectrum and the *cold* field variance are
@@ -126,60 +143,90 @@
         if verbose:
             print('Non-linear Lagrangian radius: {:.4} Mpc/h'.format(Rnl))
             print('RMS in matter field at 8 Mpc/h: {:.4}'.format(sigma8))
             print('RMS in matter displacement field: {:.4} Mpc/h'.format(sigmaV))
             print('Effective index at collapse scale: {:.4}'.format(neff))
 
         # HMcode parameters (Table 2 of https://arxiv.org/pdf/2009.01858.pdf)
-        kd = 0.05699*sigma8**-1.089  # Two-halo damping wavenumber; equation (16)
-        f = 0.2696*sigma8**0.9403    # Two-halo fractional damping; equation (16)
-        nd = 2.853                   # Two-halo damping power; equation (16)
         ks = 0.05618*sigma8**-1.013  # One-halo damping wavenumber; equation (17)
-        eta = 0.1281*sigma8**-0.3644 # Halo bloating parameter; equation (19)
-        B = 5.196                    # Minimum halo concentration; equation (20)
-        alpha = 1.875*(1.603)**neff  # Transition smoothing; equation (23)
+        if tweaks: 
+            kd = 0.05699*sigma8**-1.089  # Two-halo damping wavenumber; equation (16)
+            f = 0.2696*sigma8**0.9403    # Two-halo fractional damping; equation (16)
+            nd = 2.853                   # Two-halo damping power; equation (16)
+            ks = 0.05618*sigma8**-1.013  # One-halo damping wavenumber; equation (17)
+            eta = 0.1281*sigma8**-0.3644 # Halo bloating parameter; equation (19)
+            B = 5.196                  # Minimum halo concentration; equation (20)
+            alpha = 1.875*(1.603)**neff  # Transition smoothing; equation (23)
+        else: # Use vanilla-ish halo model if no HMcode tweaks used (still uses one-halo term suppression)
+            eta = 0.
+            B = 4.
+
+        if T_AGN and not tweaks:
+            B = feedback_params['B0']*np.power(10, z*feedback_params['Bz'])
+            Mb = feedback_params['Mb0']*np.power(10, z*feedback_params['Mbz'])
+            fstar = feedback_params['f0']*np.power(10, z*feedback_params['fz'])
+
         if verbose:
-           print('Two-halo damping wavenumber; kd: {:.4} h/Mpc'.format(kd))
-           print('Two-halo fractional damping; f: {:.4}'.format(f))
-           print('Two-halo damping power; nd: {:.4}'.format(nd))
-           print('One-halo damping wavenumber; k*: {:.4} h/Mpc'.format(ks))
-           print('Halo bloating; eta: {:.4}'.format(eta))
-           print('Minimum halo concentration; B: {:.4}'.format(B))#, B/4.)
-           print('Transition smoothing; alpha: {:.4}'.format(alpha))
-           print()
+            if tweaks:
+                print('Two-halo damping wavenumber; kd: {:.4} h/Mpc'.format(kd))
+                print('Two-halo fractional damping; f: {:.4}'.format(f))
+                print('Two-halo damping power; nd: {:.4}'.format(nd))
+                print('One-halo damping wavenumber; k*: {:.4} h/Mpc'.format(ks))
+                print('Halo bloating; eta: {:.4}'.format(eta))
+                print('Minimum halo concentration; B: {:.4}'.format(B))#, B/4.)
+                print('Transition smoothing; alpha: {:.4}'.format(alpha))
+            if T_AGN and not tweaks:
+                print('Gas-loss halo-mass parameter Mb: {:1e}'.format(Mb))
+                print('Effective halo stellar-mass fraction f*: {:.4f}'.format(f))
+            print()
 
         # Halo concentration
         zf = _get_halo_collapse_redshifts(M, z, iz, dc, growth, CAMB_results, cold=True) # Halo formation redshift
         c = B*(1+zf)/(1.+z)                                                              # Halo concentration; equation (20)
         c *= (growth(ac)/growth_LCDM(ac))*(growth_LCDM(a)/growth(a))                     # Dolag correction; equation (22)
 
         # Halo profile
         # Note the correction for neutrino mass in the profile amplitude here
         rv = hmod.virial_radius(M) 
         Uk = np.ones((len(k), len(M)))
         for iM, (_rv, _c, _nu) in enumerate(zip(rv, c, nu)): # TODO: Remove loop for speed?
-            Uk[:, iM] = _win_NFW(k*(_nu**eta), _rv, _c)[:, 0]
-        profile = halo.profile.Fourier(k, M, Uk, amplitude=M*(1.-f_nu)/hmod.rhom, mass_tracer=True) # NOTE: Factor of 1-f_nu
+            if T_AGN and not tweaks:
+                Uk[:, iM] = _win_NFW_baryons(k*(_nu**eta), _rv, _c, M[iM], Mb, fstar, Om_m, Om_c, Om_b)[:, 0]
+            else:
+                Uk[:, iM] = _win_NFW(k*(_nu**eta), _rv, _c)[:, 0]
+        if T_AGN and not tweaks: # NOTE: No Factor of 1-f_nu for baryonic, because this effect is already included!
+            profile = halo.profile.Fourier(k, M, Uk, amplitude=M/hmod.rhom, mass_tracer=True) 
+        else: # NOTE: Factor of 1-f_nu in profile amplitude
+            profile = halo.profile.Fourier(k, M, Uk, amplitude=M*(1.-f_nu)/hmod.rhom, mass_tracer=True) 
 
         # Vanilla power spectrum calculation
-        _, Pk_1h, _ = hmod.power_spectrum(k, Pk_lin, M, sigmaM, {'m': profile}, simple_twohalo=True)
+        _, _Pk_1h, _ = hmod.power_spectrum(k, Pk_lin, M, sigmaM, {'m': profile}, simple_twohalo=True)
 
         # HMcode tweaks
-        P_wig = _get_Pk_wiggle(k, Pk_lin, CAMB_results)   # Isolate spectral wiggle; footnote 7
-        Pk_dwl = Pk_lin-(1.-np.exp(-(k*sigmaV)**2))*P_wig # Constuct linear spectrum with smoothed wiggle; equation (15)
-        Pk_2h = Pk_dwl*(1.-f*(k/kd)**nd/(1.+(k/kd)**nd))  # Two-halo term; equation (16)
-        Pk_1h = (k/ks)**4/(1.+(k/ks)**4)*Pk_1h['m-m']     # One-halo term; equation (17)
-        Pk_hm = (Pk_2h**alpha+Pk_1h**alpha)**(1./alpha)   # Total prediction via smoothed sum; equation (23)
+        # Still uses one-halo term dampening even if tweaks=False
+        Pk_1h = (k/ks)**4/(1.+(k/ks)**4)*_Pk_1h['m-m'] # One-halo term; equation (17)
+        if tweaks:
+            Pk_wig = _get_Pk_wiggle(k, Pk_lin, CAMB_results)   # Isolate spectral wiggle; footnote 7
+            Pk_dwl = Pk_lin-(1.-np.exp(-(k*sigmaV)**2))*Pk_wig # Constuct linear spectrum with smoothed wiggle; equation (15)
+            Pk_2h = Pk_dwl*(1.-f*(k/kd)**nd/(1.+(k/kd)**nd))   # Two-halo term; equation (16)
+            Pk_hm = (Pk_2h**alpha+Pk_1h**alpha)**(1./alpha)    # Total prediction via smoothed sum; equation (23)
+        else: 
+            Pk_hm = Pk_lin+Pk_1h
         Pk_HMcode[iz, :] = Pk_hm
 
+    if T_AGN and tweaks:
+        suppression = _get_feedback_suppression(k, zs, CAMB_results, T_AGN, Mmin=Mmin, Mmax=Mmax, nM=nM, verbose=False)
+        Pk_HMcode *= suppression
+
     # Finish
     if verbose:
         t_finish = time()
         print('HMcode predictions complete for {:} redshifts'.format(len(zs)))
         print('Total HMcode run time: {:.3f}s'.format(t_finish-t_start))
+        print()
     return Pk_HMcode
 
 
 def _get_Pk_wiggle(k:np.ndarray, Pk_lin:np.ndarray, CAMB_results:camb.CAMBdata, sigma_dlnk=0.25) -> np.ndarray:
     '''
     Extract the wiggle from the linear power spectrum
     TODO: Should get to work for uneven log(k) spacing
@@ -272,8 +319,57 @@
     Sisv, Cisv = sici(ks+kv)
     Sis, Cis = sici(ks)
     f1 = np.cos(ks)*(Cisv-Cis)
     f2 = np.sin(ks)*(Sisv-Sis)
     f3 = np.sin(kv)/(ks+kv)
     f4 = np.log(1.+c)-c/(1.+c)
     Wk = (f1+f2-f3)/f4
-    return Wk
+    return Wk
+
+
+def _win_NFW_baryons(k:np.ndarray, rv:np.ndarray, c:np.ndarray, 
+                     M:np.ndarray, Mb:float, fstar:float, 
+                     Om_m:float, Om_c:float, Om_b:float) -> np.ndarray:
+    '''
+    Normalised Fourier transform for NFW profile, including baryonic effects
+    Equation (25) from Mead et al. (2021)
+    Calls _win_NFW
+    '''
+    Wk = _win_NFW(k, rv, c)
+    fg = (Om_b/Om_m-fstar)*(M/Mb)**2/(1.+(M/Mb)**2) # Gas content (Eq. 24 with beta=2)
+    Wk = (Om_c/Om_m+fg)*Wk
+    Wk += fstar
+    return Wk
+
+
+def _get_feedback_parameters(T_AGN:float) -> dict:
+    '''
+    Maps one-Param baryon feedback model from HMCode2020 to 6 baryonic parameters
+    Uses parameters from Table 5 in Mead et al. (2021)
+    This fit was obtained using the vanilla halo model! 
+    If the hmcode tweaks are used, different values are likely needed.
+    '''
+    theta = np.log10(T_AGN/np.power(10, 7.8))
+    params = {
+        'B0': 3.44-0.496*theta,
+        'Bz': -0.0671-0.0371*theta,
+        'Mb0': np.power(10, 13.87+1.81*theta), # [Msun/h]
+        'Mbz': -0.108+0.195*theta,
+        'f0': (2.01-0.3*theta)*1e-2,
+        'fz': 0.409+0.0224*theta,
+    }
+    return params
+
+
+def _get_feedback_suppression(k:np.array, zs:np.array, CAMB_results:camb.CAMBdata, T_AGN:float, 
+                              Mmin=1e0, Mmax=1e18, nM=256, verbose=False) -> np.ndarray:
+    '''
+    Calculates the ratio of the powerspectrum with baryonic effects to that of dark-matter-only
+    Assumes the one-parameter T_AGN model from HMCode2020
+    Warning: Since the fit for the baryonic effects was obtained with the vanilla halo model, 
+    it is not safe to set tweaks=True below
+    '''
+    Pk_gravity = power(k, zs, CAMB_results, T_AGN=None, Mmin=Mmin, Mmax=Mmax, nM=nM, 
+                       tweaks=False, verbose=verbose)
+    Pk_feedback = power(k, zs, CAMB_results, T_AGN=T_AGN, Mmin=Mmin, Mmax=Mmax, nM=nM, 
+                        tweaks=False, verbose=verbose)
+    return Pk_feedback/Pk_gravity
```

### Comparing `hmcode-1.0.1/hmcode/linear_growth.py` & `hmcode-1.1.0/hmcode/linear_growth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,71 @@
-# Standard imports
-import numpy as np
-
 # Third-party imports
-import camb
+import numpy as np
+from camb import CAMBdata
 
 # Parameters
 a_init = 1e-4 # Initial scale-factor for growth ODE integration
 
-def _w(a:float, CAMB_results:camb.CAMBdata, LCDM=False) -> float:
+def _w(a:float, CAMB_results:CAMBdata, LCDM=False) -> float:
     '''
     Dark energy equation of state for w0, wa models
     '''
     w0, wa = (-1., 0.) if LCDM else (CAMB_results.Params.DarkEnergy.w, CAMB_results.Params.DarkEnergy.wa)
     return w0+(1.-a)*wa
 
 
-def _X_w(a:float, CAMB_results:camb.CAMBdata, LCDM=False) -> float:
+def _X_w(a:float, CAMB_results:CAMBdata, LCDM=False) -> float:
     '''
     Cosmological dark energy density for w0, wa models
     '''
     w0, wa = (-1., 0.) if LCDM else (CAMB_results.Params.DarkEnergy.w, CAMB_results.Params.DarkEnergy.wa)
     return a**(-3.*(1.+w0+wa))*np.exp(-3.*wa*(1.-a))
 
 
-def _Omega_m(a:float, CAMB_results:camb.CAMBdata, LCDM=False) -> float:
+def _Omega_m(a:float, CAMB_results:CAMBdata, LCDM=False) -> float:
     '''
     Evolution of Omgea_m with scale-factor ignoring radiation
     '''
     Om_c = CAMB_results.get_Omega(var='cdm', z=0.)
     Om_b = CAMB_results.get_Omega(var='baryon', z=0.)
     Om_nu = CAMB_results.get_Omega(var='nu', z=0.)
     Om_m = Om_c+Om_b+Om_nu
     return Om_m*a**-3/_Hubble2(a, CAMB_results, LCDM)
 
 
-def _Hubble2(a:float, CAMB_results:camb.CAMBdata, LCDM=False) -> float:
+def _Hubble2(a:float, CAMB_results:CAMBdata, LCDM=False) -> float:
     '''
     Squared Hubble parameter ignoring radiation
     Massive neutrinos are counted as 'matter'
     '''
     Om_c = CAMB_results.get_Omega(var='cdm', z=0.)
     Om_b = CAMB_results.get_Omega(var='baryon', z=0.)
     Om_nu = CAMB_results.get_Omega(var='nu', z=0.)
     Om_m = Om_c+Om_b+Om_nu
     Om_w = 1.-Om_m if LCDM else CAMB_results.get_Omega(var='de', z=0.)
     Om = 1. if LCDM else 1.-CAMB_results.get_Omega(var='K', z=0.)
     H2 = Om_m*a**-3+Om_w*_X_w(a, CAMB_results, LCDM)+(1.-Om)*a**-2
     return H2
 
 
-def _AH(a:float, CAMB_results:camb.CAMBdata, LCDM=False) -> float:
+def _AH(a:float, CAMB_results:CAMBdata, LCDM=False) -> float:
     '''
     Acceleration parameter ignoring radiation
     Massive neutrinos are counted as 'matter'
     '''
     Om_c = CAMB_results.get_Omega(var='cdm', z=0.)
     Om_b = CAMB_results.get_Omega(var='baryon', z=0.)
     Om_nu = CAMB_results.get_Omega(var='nu', z=0.)
     Om_m = Om_c+Om_b+Om_nu
     Om_w = 1.-Om_m if LCDM else CAMB_results.get_Omega(var='de', z=0.)
     AH = -0.5*(Om_m*a**-3+(1.+3.*_w(a, CAMB_results, LCDM))*Om_w*_X_w(a, CAMB_results, LCDM))
     return AH
 
 
-def get_growth_interpolator(CAMB_results:camb.CAMBdata, LCDM=False) -> callable:
+def get_growth_interpolator(CAMB_results:CAMBdata, LCDM=False) -> callable:
     '''
     Solve the linear growth ODE and returns an interpolating function for the solution
     LCDM = True forces w = -1 and imposes flatness by modifying the dark-energy density
     TODO: w dependence for initial conditions; f here is correct for w=0 only
     TODO: Could use d_init = a(1+(w-1)/(w(6w-5))*(Om_w/Om_m)*a**-3w) at early times with w = w(a<<1)
     '''
     from scipy.integrate import solve_ivp
```

### Comparing `hmcode-1.0.1/hmcode/utility.py` & `hmcode-1.1.0/hmcode/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Standard imports
+# Third-party imports
 import numpy as np
 
 def derivative_from_samples(x:float, xs:np.array, fs:np.array) -> float:
     '''
     Calculates the derivative of the function f(x) which is sampled as fs at values xs
     Approximates the function as quadratic using the samples and Legendre polynomials
     Args:
```

### Comparing `hmcode-1.0.1/pyproject.toml` & `hmcode-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hmcode"
-version = "1.0.1"
+version = "1.1.0"
 description = "Pure Python implementation of HMcode"
 authors = ["Alexander Mead <alexander.j.mead@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/alexander-mead/HMcode-python"
 
 [tool.poetry.dependencies]
```

### Comparing `hmcode-1.0.1/setup.py` & `hmcode-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['camb>=1.4.0,<2.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pyhalomodel>=1.0.1,<2.0.0',
  'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'hmcode',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'Pure Python implementation of HMcode',
-    'long_description': "# HMcode\n\nA pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.\n\n## Installation\n\nEither\n```\npip install hmcode\n```\nor, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then\n```\npoetry install\n```\nto create a virtual environment with everything you need to get going.\n\n## Dependencies\n\n- `numpy`\n- `scipy`\n- `camb`\n- `pyhalomodel`\n\n## Use\n\n```\nimport numpy as np\nimport camb\nimport hmcode\n\n# Ranges\nk = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]\nzs = [3., 2., 1., 0.5, 0.]  # Redshifts\n\n# Run CAMB\nparameters = camb.CAMBparams(WantCls=False)\nparameters.set_cosmology(H0=70.)\nparameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest\nresults = camb.get_results(parameters)\n\n# HMcode\nPk = hmcode.power(k, zs, results)\n```\n\n## Note\n\nTo whom it may concern,\n\nI coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...\n\nYou might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.\n\nI compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:\n- LCDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.21%\n- k-LCDM: Mean error: 0.11%; Std error: 0.03%; Worst error; 0.23%\n- w-CDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.20%\n- w(a)-CDM: Mean error: 0.13%; Std error: 0.06%; Worst error; 0.48%\n- nu-LCDM: Mean error: 0.47%; Std error: 0.44%; Worst error; 2.01% (larger errors strongly correlated with neutrino mass)\n- nu-k-w(a)-CDM: Mean error: 0.42%; Std error: 0.43%; Worst error; 2.02% (larger errors strongly correlated with neutrino mass)\n\nThese comparisons can be reproduced using the `comparisons/CAMB.py` script.\n\nWhile the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:\n- Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.\n- Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).\n- If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.\n\nUsing the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.\n\nI think any residual differences between codes must therefore stem from:\n- The BAO de-wiggling process (different `k` grids)\n- The $\\sigma_\\mathrm{v}$ numerical integration\n- The $n_\\mathrm{eff}$ calculation (numerical differentiation here; numerical integration in `CAMB-HMcode`)\n- The $\\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)\n- The linear growth ODE solution\n- Root finding for the halo-collapse redshift and for $R_\\mathrm{nl}$\n\nBut I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.\n\nWhile writing this code I had a few ideas for future improvements:\n- Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.\n- The predictions are a bit sensitive to the smoothing $\\sigma$ used for the dewiggling. This should probably be a fitted parameter.\n- It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$.\n- I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).\n- Redshift 'infinity' for the Dolag correction is actually $z_\\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.\n- The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.\n- I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.\n- The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\\delta_\\mathrm{c}$; $\\Delta_\\mathrm{v}$; $\\sigma(R)$; $R_\\mathrm{nl}$; $n_\\mathrm{eff}$; $c(M)$.\n- Refit model (including $\\sigma$ for BAO smoothing and $z_\\infty$ for [Dolag et al. 2004](https://arxiv.org/abs/astro-ph/0309771)) to new emulator(s) (e.g., [Mira Titan IV](https://arxiv.org/abs/2207.12345)).\n- Don't be under any illusions that the `HMcode` parameters, or the forms of their dependence on the underlying power spectrum, are special in any particular way. A lot of experimentation went into finding these, but it was by no means exhaustive. However, please note that obviously these parameters should only depend on the underlying linear spectrum (rather than being random functions of $z$, $\\Omega_\\mathrm{m}$, $w$, or whatever).\n\nHave fun,\n\nAlexander Mead (2023/02/28)\n",
+    'long_description': "# HMcode\n\n![image](https://user-images.githubusercontent.com/9140961/228345397-f33d2f94-e8e4-4eb0-9fc9-9b27df407fbc.png)\n\nA pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.\n\n## Installation\n\nEither\n```bash\n> pip install hmcode\n```\nor, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then\n```bash\n> poetry install\n```\nto create a virtual environment with everything you need to get going.\n\n## Dependencies\n\n- `numpy`\n- `scipy`\n- `camb`\n- `pyhalomodel`\n\n## Use\n\n```\nimport numpy as np\nimport camb\nimport hmcode\n\n# Ranges\nk = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]\nzs = [3., 2., 1., 0.5, 0.]  # Redshifts\nT_AGN = 10**7.8             # Feedback temperature [K]\n\n# Run CAMB\nparameters = camb.CAMBparams(WantCls=False)\nparameters.set_cosmology(H0=70.)\nparameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest\nresults = camb.get_results(parameters)\n\n# HMcode\nPk = hmcode.power(k, zs, results, T_AGN)\n```\n\n## Note\n\nTo whom it may concern,\n\nI coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...\n\nYou might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.\n\nI compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:\n- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.21%\n- k-LCDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.23%\n- w-CDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.20%\n- w(a)-CDM: Mean error: 0.13%; Standard deviation of error: 0.06%; Worst-case error; 0.48%\n- nu-LCDM: Mean error: 0.47%; Standard deviation of error: 0.44%; Worst-case error; 2.01% (larger errors strongly correlated with neutrino mass)\n- nu-k-w(a)-CDM: Mean error: 0.42%; Standard deviation of error: 0.43%; Worst-case error; 2.02% (larger errors strongly correlated with neutrino mass)\n\nThese comparisons can be reproduced using the `comparisons/CAMB.py` script.\n\nThe power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:\n- LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%\n- nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)\n\nThe comparisons can be reproduced using the `comparisons/CAMB_feedback.py` script.\n\nWhile the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:\n- Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.\n- Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).\n- If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.\n\nUsing the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.\n\nI think any residual differences between codes must therefore stem from:\n- The BAO de-wiggling process (different `k` grids)\n- The $\\sigma_\\mathrm{v}$ numerical integration\n- The $n_\\mathrm{eff}$ calculation (numerical differentiation here; numerical integration in `CAMB-HMcode`)\n- The $\\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)\n- The linear growth ODE solution\n- Root finding for the halo-collapse redshift and for $R_\\mathrm{nl}$\n\nBut I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.\n\nWhile writing this code I had a few ideas for future improvements:\n- ~~Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.~~ (Thanks Laila Linke!)\n- The predictions are a bit sensitive to the smoothing $\\sigma$ used for the dewiggling. This should probably be a fitted parameter.\n- It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$.\n- I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).\n- Redshift 'infinity' for the Dolag correction is actually $z_\\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.\n- The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\\delta_\\mathrm{c}$, $\\Delta_\\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.\n- I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.\n- The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\\delta_\\mathrm{c}$; $\\Delta_\\mathrm{v}$; $\\sigma(R)$; $R_\\mathrm{nl}$; $n_\\mathrm{eff}$; $c(M)$.\n- Refit model (including $\\sigma$ for BAO smoothing and $z_\\infty$ for [Dolag et al. 2004](https://arxiv.org/abs/astro-ph/0309771)) to new emulator(s) (e.g., [Mira Titan IV](https://arxiv.org/abs/2207.12345)).\n- Don't be under any illusions that the `HMcode` parameters, or the forms of their dependence on the underlying power spectrum, are special in any particular way. A lot of experimentation went into finding these, but it was by no means exhaustive. However, please note that obviously these parameters should only depend on the underlying linear spectrum (rather than being random functions of $z$, $\\Omega_\\mathrm{m}$, $w$, or whatever).\n\nHave fun,\n\nAlexander Mead (2023/02/28)\n",
     'author': 'Alexander Mead',
     'author_email': 'alexander.j.mead@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/alexander-mead/HMcode-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `hmcode-1.0.1/PKG-INFO` & `hmcode-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmcode
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pure Python implementation of HMcode
 Home-page: https://github.com/alexander-mead/HMcode-python
 License: MIT
 Author: Alexander Mead
 Author-email: alexander.j.mead@googlemail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -18,25 +18,27 @@
 Requires-Dist: pyhalomodel (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/alexander-mead/HMcode-python
 Description-Content-Type: text/markdown
 
 # HMcode
 
+![image](https://user-images.githubusercontent.com/9140961/228345397-f33d2f94-e8e4-4eb0-9fc9-9b27df407fbc.png)
+
 A pure-`Python` implementation of the `HMcode-2020` method ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) for computing accurate non-linear matter power spectra across a wide range of cosmological parameters for $w(a)$-CDM models including curvature and massive neutrinos.
 
 ## Installation
 
 Either
-```
-pip install hmcode
+```bash
+> pip install hmcode
 ```
 or, if you want to edit the code, use the demo notebook, or run the tests or consistency checks, then clone the repository, `cd` into the directory, and then
-```
-poetry install
+```bash
+> poetry install
 ```
 to create a virtual environment with everything you need to get going.
 
 ## Dependencies
 
 - `numpy`
 - `scipy`
@@ -49,43 +51,50 @@
 import numpy as np
 import camb
 import hmcode
 
 # Ranges
 k = np.logspace(-3, 1, 100) # Wavenumbers [h/Mpc]
 zs = [3., 2., 1., 0.5, 0.]  # Redshifts
+T_AGN = 10**7.8             # Feedback temperature [K]
 
 # Run CAMB
 parameters = camb.CAMBparams(WantCls=False)
 parameters.set_cosmology(H0=70.)
 parameters.set_matter_power(redshifts=zs, kmax=100.) # kmax should be much larger than the wavenumber of interest
 results = camb.get_results(parameters)
 
 # HMcode
-Pk = hmcode.power(k, zs, results)
+Pk = hmcode.power(k, zs, results, T_AGN)
 ```
 
 ## Note
 
 To whom it may concern,
 
 I coded this `Python` version of `HMcode-2020` ([Mead et al. 2021](https://arxiv.org/abs/2009.01858)) up quite quickly before leaving academia in February 2023. It is written in pure `Python` and doesn't use any of the original Fortran code whatsoever. There is something amazing/dispiriting about coding something up in 3 days that previously took 5 years. A tragic last hoorah! At least I switched to `Python` eventually...
 
 You might also be interested in [`pyhalomodel`](https://pypi.org/project/pyhalomodel/), upon which this code depends, which implements a vanilla halo-model calculation for any desired large-scale-structure tracer. Alternatively, and very confusingly, you might be interested in this [`pyhmcode`](https://pypi.org/project/pyhmcode/), which provides a wrapper around the original `Fortran` `HMcode` implementation.
 
 I compared it against the `CAMB-HMcode` version for 100 random sets of cosmological parameters ($k < 10 h\mathrm{Mpc}^{-1}$; $z < 3$). The level of agreement between the two codes is as follows:
-- LCDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.21%
-- k-LCDM: Mean error: 0.11%; Std error: 0.03%; Worst error; 0.23%
-- w-CDM: Mean error: 0.10%; Std error: 0.03%; Worst error; 0.20%
-- w(a)-CDM: Mean error: 0.13%; Std error: 0.06%; Worst error; 0.48%
-- nu-LCDM: Mean error: 0.47%; Std error: 0.44%; Worst error; 2.01% (larger errors strongly correlated with neutrino mass)
-- nu-k-w(a)-CDM: Mean error: 0.42%; Std error: 0.43%; Worst error; 2.02% (larger errors strongly correlated with neutrino mass)
+- LCDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.21%
+- k-LCDM: Mean error: 0.11%; Standard deviation of error: 0.03%; Worst-case error; 0.23%
+- w-CDM: Mean error: 0.10%; Standard deviation of error: 0.03%; Worst-case error; 0.20%
+- w(a)-CDM: Mean error: 0.13%; Standard deviation of error: 0.06%; Worst-case error; 0.48%
+- nu-LCDM: Mean error: 0.47%; Standard deviation of error: 0.44%; Worst-case error; 2.01% (larger errors strongly correlated with neutrino mass)
+- nu-k-w(a)-CDM: Mean error: 0.42%; Standard deviation of error: 0.43%; Worst-case error; 2.02% (larger errors strongly correlated with neutrino mass)
 
 These comparisons can be reproduced using the `comparisons/CAMB.py` script.
 
+The power-spectrum suppression caused by baryonic feedback has also been implemented, and the level of agreement between the *suppression* predicted by this code and the same implementation in `CAMB` is as follows:
+- LCDM: Mean error: 0.02%; Standard deviation of error: <0.01%; Worst-case error; 0.03%
+- nu-k-w(a)-CDM: Mean error: 0.06%; Standard deviation of error: 0.07%; Worst-case error; 0.49% (larger errors strongly correlated with neutrino mass)
+
+The comparisons can be reproduced using the `comparisons/CAMB_feedback.py` script.
+
 While the quoted accuracy of `HMcode-2020` relative to simulations is RMS ~2.5%, note that the accuracy is anti-correlated with neutrino masses (cf. Fig. 2 of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)). The larger discrepancies between the codes for massive neutrinos (2% for ~1eV) may seem worrisome, but here are some reasons why I am not that worried:
 - Here, neutrinos are treated as completely cold matter when calculating the linear growth factors, whereas in `CAMB-HMcode` the transition from behaving like radiation to behaving like matter is accounted for in the linear growth.
 - Here the *cold* matter power spectrum is taken directly from `CAMB` whereas in `CAMB-HMcode` the *cold* spectrum is calculated approximately from the total matter power spectrum using approximations for the scale-dependent growth rate from [Eisenstein & Hu (1999)](https://arxiv.org/abs/astro-ph/9710252).
 - If I resort to the old approximation for the *cold* matter power spectrum (and therefore the cold $\sigma(R)$) then the level of agreement between the codes for nu-k-w(a)-CDM improves to: Mean error: 0.15%; Std error: 0.11%; Worst error; 1.15%.
 
 Using the actual cold matter spectrum is definitely an improvement from a theoretical perspective (and for speed), so I decided to keep that at the cost of the disagreement between this code at `CAMB-HMcode` for models with very high neutrino mass. If better agreement between this code and `CAMB-HMcode` is important to you then the old approximate cold spectrum can be used by changing the `sigma_cold_approx` flag at the top of `hmcode.py`. Note that while ignoring the actual energy-density scaling of massive neutrinos might seem to be a (small) problem, keep in mind the comments below regarding the linear growth factor.
 
@@ -96,15 +105,15 @@
 - The $\sigma(R)$ numerical integration (using `CAMB` here; done internally in `CAMB-HMcode`)
 - The linear growth ODE solution
 - Root finding for the halo-collapse redshift and for $R_\mathrm{nl}$
 
 But I didn't have time to investigate these differences more thoroughly. Note that there are accuracy parameters in `CAMB-HMcode` fixed at the $10^{-4}$ level, so you would never expect better than 0.01% agreement. Given that `HMcode` is only accurate at the ~2.5% level compared to simulated power spectra, the level of agreement between the codes seems okay to me, with the caveats above regarding very massive neutrinos.
 
 While writing this code I had a few ideas for future improvements:
-- Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.
+- ~~Add the `HMcode-2020` baryon-feedback model; this would not be too hard for the enthusiastic student/postdoc.~~ (Thanks Laila Linke!)
 - The predictions are a bit sensitive to the smoothing $\sigma$ used for the dewiggling. This should probably be a fitted parameter.
 - It's annoying having to calculate linear growth functions (all, LCDM), especially since the linear growth doesn't really exist. One should probably use the $P(k)$ amplitude evolution over time at some cleverly chosen scale instead, or instead the evolution of $\sigma(R)$ over time at some pertinent $R$ value. Note that the growth factors are *only* used to calculate the [Dolag et al. (2004)](https://arxiv.org/abs/astro-ph/0309771) correction and [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$.
 - I never liked the halo bloating parameter, it's hard to understand the effect of modifying halo profiles in Fourier space. Someone should get rid of this (maybe modify the halo mass function instead?).
 - Redshift 'infinity' for the Dolag correction is actually $z_\infty = 10$. `HMcode` predictions *are* sensitive to this (particularly w(a)CDM). Either the redshift 'infinity' should be fitted or the halo-concentration model for beyond-LCDM should be improved.
 - The massive neutrino correction for the [Mead (2017)](https://arxiv.org/abs/1606.05345) $\delta_\mathrm{c}$, $\Delta_\mathrm{v}$ formulae (appendix A of [Mead et al. 2021](https://arxiv.org/abs/2009.01858)) is crude and should be improved. I guess using the intuition that hot neutrinos are ~smoothly distributed on halo scales. Currently neutrinos are treated as cold matter in the linear/accumulated growth calculation (used by [Mead 2017](https://arxiv.org/abs/1606.05345)), which seems a bit wrong.
 - I haven't checked how fast this code is, but there are a couple of TODO in the code that might improve speed if necessary.
 - The choices regarding how to account for massive neutrinos could usefully be revisited. This whole subject is a bit confusing and the code doesn't help to alleviate the confusion. Choices like what to use for: $\delta_\mathrm{c}$; $\Delta_\mathrm{v}$; $\sigma(R)$; $R_\mathrm{nl}$; $n_\mathrm{eff}$; $c(M)$.
```

