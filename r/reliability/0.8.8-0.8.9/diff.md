# Comparing `tmp/reliability-0.8.8.tar.gz` & `tmp/reliability-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliability-0.8.8.tar", last modified: Tue Feb 21 11:55:34 2023, max compression
+gzip compressed data, was "reliability-0.8.9.tar", last modified: Sun Apr 23 04:58:07 2023, max compression
```

## Comparing `reliability-0.8.8.tar` & `reliability-0.8.9.tar`

### file list

```diff
@@ -1,399 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:34.372801 reliability-0.8.8/
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:32.543218 reliability-0.8.8/.github/
--rw-rw-rw-   0        0        0     3435 2021-03-27 08:39:34.000000 reliability-0.8.8/.github/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1673 2021-03-05 02:36:51.000000 reliability-0.8.8/.github/CONTRIBUTING.md
--rw-rw-rw-   0        0        0       24 2020-12-20 22:47:06.000000 reliability-0.8.8/.github/FUNDING.yml
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:32.558843 reliability-0.8.8/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      421 2021-03-19 09:41:42.000000 reliability-0.8.8/.github/ISSUE_TEMPLATE/all-other-issues.md
--rw-rw-rw-   0        0        0      543 2021-03-19 09:41:42.000000 reliability-0.8.8/.github/ISSUE_TEMPLATE/bug_report.md
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:32.574467 reliability-0.8.8/.github/workflows/
--rw-rw-rw-   0        0        0     1042 2023-02-21 11:03:12.000000 reliability-0.8.8/.github/workflows/build_and_test_on_linux.yml
--rw-rw-rw-   0        0        0      770 2023-02-21 11:00:25.000000 reliability-0.8.8/.github/workflows/codecov.yml
--rw-rw-rw-   0        0        0     2804 2022-08-19 10:00:43.000000 reliability-0.8.8/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0      191 2023-02-21 11:42:45.000000 reliability-0.8.8/.readthedocs.yaml
--rw-rw-rw-   0        0        0     7817 2020-04-27 03:35:53.000000 reliability-0.8.8/LICENSE
--rw-rw-rw-   0        0        0       92 2019-08-04 00:35:42.000000 reliability-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6508 2023-02-21 11:55:34.372801 reliability-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     4789 2022-08-19 10:00:43.000000 reliability-0.8.8/README.md
--rw-rw-rw-   0        0        0       49 2021-02-27 04:02:31.000000 reliability-0.8.8/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.090093 reliability-0.8.8/docs/
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.152592 reliability-0.8.8/docs/API/
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.293908 reliability-0.8.8/docs/API/ALT_fitters/
--rw-rw-rw-   0        0        0      279 2021-03-22 09:44:59.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Everything_ALT.rst
--rw-rw-rw-   0        0        0      321 2021-03-22 09:43:08.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Dual_Exponential.rst
--rw-rw-rw-   0        0        0      303 2021-03-22 09:43:25.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Dual_Power.rst
--rw-rw-rw-   0        0        0      306 2021-03-22 09:43:37.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Exponential.rst
--rw-rw-rw-   0        0        0      291 2021-03-22 09:43:48.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Eyring.rst
--rw-rw-rw-   0        0        0      288 2021-03-22 09:44:00.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Power.rst
--rw-rw-rw-   0        0        0      324 2021-03-22 09:44:14.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Exponential_Power_Exponential.rst
--rw-rw-rw-   0        0        0      315 2021-03-22 09:37:39.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Dual_Exponential.rst
--rw-rw-rw-   0        0        0      297 2021-03-22 09:37:52.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Dual_Power.rst
--rw-rw-rw-   0        0        0      300 2021-03-22 09:38:04.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Exponential.rst
--rw-rw-rw-   0        0        0      285 2021-03-22 09:38:22.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Eyring.rst
--rw-rw-rw-   0        0        0      282 2021-03-22 09:38:34.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Power.rst
--rw-rw-rw-   0        0        0      318 2021-03-22 09:38:48.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Lognormal_Power_Exponential.rst
--rw-rw-rw-   0        0        0      306 2021-03-22 09:40:31.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Dual_Exponential.rst
--rw-rw-rw-   0        0        0      288 2021-03-22 09:40:25.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Dual_Power.rst
--rw-rw-rw-   0        0        0      291 2021-03-22 09:40:44.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Exponential.rst
--rw-rw-rw-   0        0        0      276 2021-03-22 09:40:56.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Eyring.rst
--rw-rw-rw-   0        0        0      273 2021-03-22 09:41:12.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Power.rst
--rw-rw-rw-   0        0        0      309 2021-03-22 09:41:27.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Normal_Power_Exponential.rst
--rw-rw-rw-   0        0        0      309 2021-03-22 09:33:05.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Dual_Exponential.rst
--rw-rw-rw-   0        0        0      291 2021-03-22 09:34:21.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Dual_Power.rst
--rw-rw-rw-   0        0        0      294 2021-03-22 09:34:50.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Exponential.rst
--rw-rw-rw-   0        0        0      279 2021-03-22 09:35:50.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Eyring.rst
--rw-rw-rw-   0        0        0      276 2021-03-22 09:35:21.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Power.rst
--rw-rw-rw-   0        0        0      312 2021-03-22 09:33:49.000000 reliability-0.8.8/docs/API/ALT_fitters/Fit_Weibull_Power_Exponential.rst
--rw-rw-rw-   0        0        0      235 2021-03-22 09:46:26.000000 reliability-0.8.8/docs/API/ALT_fitters.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.340782 reliability-0.8.8/docs/API/Convert_data/
--rw-rw-rw-   0        0        0      256 2021-03-22 09:55:20.000000 reliability-0.8.8/docs/API/Convert_data/FNRN_to_FR.rst
--rw-rw-rw-   0        0        0      259 2021-03-22 09:54:22.000000 reliability-0.8.8/docs/API/Convert_data/FNRN_to_XCN.rst
--rw-rw-rw-   0        0        0      256 2021-03-22 09:54:51.000000 reliability-0.8.8/docs/API/Convert_data/FR_to_FNRN.rst
--rw-rw-rw-   0        0        0      253 2021-03-22 09:53:27.000000 reliability-0.8.8/docs/API/Convert_data/FR_to_XCN.rst
--rw-rw-rw-   0        0        0      259 2021-03-22 09:55:50.000000 reliability-0.8.8/docs/API/Convert_data/XCN_to_FNRN.rst
--rw-rw-rw-   0        0        0      253 2021-03-22 09:56:13.000000 reliability-0.8.8/docs/API/Convert_data/XCN_to_FR.rst
--rw-rw-rw-   0        0        0      262 2021-03-22 09:48:29.000000 reliability-0.8.8/docs/API/Convert_data/xlsx_to_FNRN.rst
--rw-rw-rw-   0        0        0      256 2021-03-22 09:48:08.000000 reliability-0.8.8/docs/API/Convert_data/xlsx_to_FR.rst
--rw-rw-rw-   0        0        0      259 2021-03-22 09:47:31.000000 reliability-0.8.8/docs/API/Convert_data/xlsx_to_XCN.rst
--rw-rw-rw-   0        0        0      238 2021-11-09 03:17:55.000000 reliability-0.8.8/docs/API/Convert_data.rst
--rw-rw-rw-   0        0        0      238 2021-03-22 05:04:23.000000 reliability-0.8.8/docs/API/Datasets.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.387657 reliability-0.8.8/docs/API/Distributions/
--rw-rw-rw-   0        0        0      278 2021-03-22 08:53:54.000000 reliability-0.8.8/docs/API/Distributions/Beta_Distribution.rst
--rw-rw-rw-   0        0        0      290 2021-03-22 08:56:46.000000 reliability-0.8.8/docs/API/Distributions/Competing_Risks_Model.rst
--rw-rw-rw-   0        0        0      257 2021-07-20 11:39:12.000000 reliability-0.8.8/docs/API/Distributions/DSZI_Model.rst
--rw-rw-rw-   0        0        0      299 2021-03-22 08:47:18.000000 reliability-0.8.8/docs/API/Distributions/Exponential_Distribution.rst
--rw-rw-rw-   0        0        0      281 2021-03-22 08:54:24.000000 reliability-0.8.8/docs/API/Distributions/Gamma_Distribution.rst
--rw-rw-rw-   0        0        0      284 2021-03-22 08:55:28.000000 reliability-0.8.8/docs/API/Distributions/Gumbel_Distribution.rst
--rw-rw-rw-   0        0        0      299 2021-03-22 08:54:58.000000 reliability-0.8.8/docs/API/Distributions/Loglogistic_Distribution.rst
--rw-rw-rw-   0        0        0      293 2021-03-22 08:47:45.000000 reliability-0.8.8/docs/API/Distributions/Lognormal_Distribution.rst
--rw-rw-rw-   0        0        0      266 2021-03-22 08:57:13.000000 reliability-0.8.8/docs/API/Distributions/Mixture_Model.rst
--rw-rw-rw-   0        0        0      284 2021-03-22 08:55:55.000000 reliability-0.8.8/docs/API/Distributions/Normal_Distribution.rst
--rw-rw-rw-   0        0        0      287 2021-03-22 08:46:48.000000 reliability-0.8.8/docs/API/Distributions/Weibull_Distribution.rst
--rw-rw-rw-   0        0        0      243 2021-03-22 08:59:29.000000 reliability-0.8.8/docs/API/Distributions.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.497036 reliability-0.8.8/docs/API/Fitters/
--rw-rw-rw-   0        0        0      254 2021-03-22 09:22:10.000000 reliability-0.8.8/docs/API/Fitters/Fit_Beta_2P.rst
--rw-rw-rw-   0        0        0      263 2021-03-22 09:23:06.000000 reliability-0.8.8/docs/API/Fitters/Fit_Everything.rst
--rw-rw-rw-   0        0        0      275 2021-03-22 09:15:29.000000 reliability-0.8.8/docs/API/Fitters/Fit_Exponential_1P.rst
--rw-rw-rw-   0        0        0      275 2021-03-22 09:15:56.000000 reliability-0.8.8/docs/API/Fitters/Fit_Exponential_2P.rst
--rw-rw-rw-   0        0        0      257 2021-03-22 09:14:31.000000 reliability-0.8.8/docs/API/Fitters/Fit_Gamma_2P.rst
--rw-rw-rw-   0        0        0      257 2021-03-22 09:14:55.000000 reliability-0.8.8/docs/API/Fitters/Fit_Gamma_3P.rst
--rw-rw-rw-   0        0        0      260 2021-03-22 09:20:42.000000 reliability-0.8.8/docs/API/Fitters/Fit_Gumbel_2P.rst
--rw-rw-rw-   0        0        0      275 2021-03-22 09:21:18.000000 reliability-0.8.8/docs/API/Fitters/Fit_Loglogistic_2P.rst
--rw-rw-rw-   0        0        0      275 2021-03-22 09:21:40.000000 reliability-0.8.8/docs/API/Fitters/Fit_Loglogistic_3P.rst
--rw-rw-rw-   0        0        0      269 2021-03-22 09:23:51.000000 reliability-0.8.8/docs/API/Fitters/Fit_Lognormal_2P.rst
--rw-rw-rw-   0        0        0      269 2021-03-22 09:24:10.000000 reliability-0.8.8/docs/API/Fitters/Fit_Lognormal_3P.rst
--rw-rw-rw-   0        0        0      260 2021-03-22 08:58:51.000000 reliability-0.8.8/docs/API/Fitters/Fit_Normal_2P.rst
--rw-rw-rw-   0        0        0      263 2021-03-22 08:57:59.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_2P.rst
--rw-rw-rw-   0        0        0      287 2021-03-22 09:25:09.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_2P_grouped.rst
--rw-rw-rw-   0        0        0      263 2021-03-22 08:58:26.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_3P.rst
--rw-rw-rw-   0        0        0      263 2021-03-22 09:22:39.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_CR.rst
--rw-rw-rw-   0        0        0      263 2021-07-20 11:39:41.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_DS.rst
--rw-rw-rw-   0        0        0      269 2021-07-21 12:14:43.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_DSZI.rst
--rw-rw-rw-   0        0        0      278 2021-03-22 09:13:46.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_Mixture.rst
--rw-rw-rw-   0        0        0      263 2021-07-20 11:39:58.000000 reliability-0.8.8/docs/API/Fitters/Fit_Weibull_ZI.rst
--rw-rw-rw-   0        0        0      223 2021-03-22 08:59:47.000000 reliability-0.8.8/docs/API/Fitters.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.512659 reliability-0.8.8/docs/API/Nonparametric/
--rw-rw-rw-   0        0        0      260 2021-03-22 09:59:37.000000 reliability-0.8.8/docs/API/Nonparametric/KaplanMeier.rst
--rw-rw-rw-   0        0        0      260 2021-03-22 09:59:43.000000 reliability-0.8.8/docs/API/Nonparametric/NelsonAalen.rst
--rw-rw-rw-   0        0        0      269 2021-03-22 09:59:50.000000 reliability-0.8.8/docs/API/Nonparametric/RankAdjustment.rst
--rw-rw-rw-   0        0        0      241 2021-11-09 03:17:27.000000 reliability-0.8.8/docs/API/Nonparametric.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.559533 reliability-0.8.8/docs/API/Other_functions/
--rw-rw-rw-   0        0        0      259 2021-03-22 21:03:24.000000 reliability-0.8.8/docs/API/Other_functions/crosshairs.rst
--rw-rw-rw-   0        0        0      292 2021-03-22 21:40:33.000000 reliability-0.8.8/docs/API/Other_functions/distribution_explorer.rst
--rw-rw-rw-   0        0        0      256 2021-03-22 21:41:04.000000 reliability-0.8.8/docs/API/Other_functions/histogram.rst
--rw-rw-rw-   0        0        0      268 2021-03-22 21:41:32.000000 reliability-0.8.8/docs/API/Other_functions/make_ALT_data.rst
--rw-rw-rw-   0        0        0      301 2021-03-22 21:42:04.000000 reliability-0.8.8/docs/API/Other_functions/make_right_censored_data.rst
--rw-rw-rw-   0        0        0      292 2021-03-22 21:42:32.000000 reliability-0.8.8/docs/API/Other_functions/similar_distributions.rst
--rw-rw-rw-   0        0        0      274 2021-03-22 21:42:58.000000 reliability-0.8.8/docs/API/Other_functions/stress_strength.rst
--rw-rw-rw-   0        0        0      295 2021-03-22 21:43:22.000000 reliability-0.8.8/docs/API/Other_functions/stress_strength_normal.rst
--rw-rw-rw-   0        0        0      247 2021-11-09 03:17:39.000000 reliability-0.8.8/docs/API/Other_functions.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.606416 reliability-0.8.8/docs/API/PoF/
--rw-rw-rw-   0        0        0      247 2021-03-22 21:44:49.000000 reliability-0.8.8/docs/API/PoF/SN_diagram.rst
--rw-rw-rw-   0        0        0      274 2021-03-22 21:45:16.000000 reliability-0.8.8/docs/API/PoF/acceleration_factor.rst
--rw-rw-rw-   0        0        0      271 2021-03-22 21:45:42.000000 reliability-0.8.8/docs/API/PoF/creep_failure_time.rst
--rw-rw-rw-   0        0        0      277 2021-03-22 21:46:10.000000 reliability-0.8.8/docs/API/PoF/creep_rupture_curves.rst
--rw-rw-rw-   0        0        0      310 2021-03-22 21:46:41.000000 reliability-0.8.8/docs/API/PoF/fracture_mechanics_crack_growth.rst
--rw-rw-rw-   0        0        0      322 2021-03-22 21:47:09.000000 reliability-0.8.8/docs/API/PoF/fracture_mechanics_crack_initiation.rst
--rw-rw-rw-   0        0        0      301 2021-03-22 21:47:45.000000 reliability-0.8.8/docs/API/PoF/palmgren_miner_linear_damage.rst
--rw-rw-rw-   0        0        0      274 2021-03-22 21:48:19.000000 reliability-0.8.8/docs/API/PoF/strain_life_diagram.rst
--rw-rw-rw-   0        0        0      280 2021-03-22 21:48:48.000000 reliability-0.8.8/docs/API/PoF/stress_strain_diagram.rst
--rw-rw-rw-   0        0        0      334 2021-03-22 21:49:33.000000 reliability-0.8.8/docs/API/PoF/stress_strain_life_parameters_from_data.rst
--rw-rw-rw-   0        0        0      211 2021-03-22 21:44:04.000000 reliability-0.8.8/docs/API/PoF.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.685006 reliability-0.8.8/docs/API/Probability_plotting/
--rw-rw-rw-   0        0        0      297 2021-03-22 21:51:05.000000 reliability-0.8.8/docs/API/Probability_plotting/Beta_probability_plot.rst
--rw-rw-rw-   0        0        0      318 2021-03-22 21:51:43.000000 reliability-0.8.8/docs/API/Probability_plotting/Exponential_probability_plot.rst
--rw-rw-rw-   0        0        0      360 2021-03-22 21:52:20.000000 reliability-0.8.8/docs/API/Probability_plotting/Exponential_probability_plot_Weibull_Scale.rst
--rw-rw-rw-   0        0        0      300 2021-03-22 21:52:51.000000 reliability-0.8.8/docs/API/Probability_plotting/Gamma_probability_plot.rst
--rw-rw-rw-   0        0        0      303 2021-03-22 21:53:20.000000 reliability-0.8.8/docs/API/Probability_plotting/Gumbel_probability_plot.rst
--rw-rw-rw-   0        0        0      318 2021-03-22 21:53:55.000000 reliability-0.8.8/docs/API/Probability_plotting/Loglogistic_probability_plot.rst
--rw-rw-rw-   0        0        0      312 2021-03-22 21:54:26.000000 reliability-0.8.8/docs/API/Probability_plotting/Lognormal_probability_plot.rst
--rw-rw-rw-   0        0        0      303 2021-03-22 21:54:56.000000 reliability-0.8.8/docs/API/Probability_plotting/Normal_probability_plot.rst
--rw-rw-rw-   0        0        0      288 2021-03-22 21:55:28.000000 reliability-0.8.8/docs/API/Probability_plotting/PP_plot_parametric.rst
--rw-rw-rw-   0        0        0      300 2021-03-22 21:55:54.000000 reliability-0.8.8/docs/API/Probability_plotting/PP_plot_semiparametric.rst
--rw-rw-rw-   0        0        0      288 2021-03-22 21:56:20.000000 reliability-0.8.8/docs/API/Probability_plotting/QQ_plot_parametric.rst
--rw-rw-rw-   0        0        0      300 2021-03-22 21:56:46.000000 reliability-0.8.8/docs/API/Probability_plotting/QQ_plot_semiparametric.rst
--rw-rw-rw-   0        0        0      306 2021-03-22 21:57:23.000000 reliability-0.8.8/docs/API/Probability_plotting/Weibull_probability_plot.rst
--rw-rw-rw-   0        0        0      267 2021-03-22 21:57:51.000000 reliability-0.8.8/docs/API/Probability_plotting/plot_points.rst
--rw-rw-rw-   0        0        0      288 2021-03-22 21:58:20.000000 reliability-0.8.8/docs/API/Probability_plotting/plotting_positions.rst
--rw-rw-rw-   0        0        0      262 2021-03-22 21:50:14.000000 reliability-0.8.8/docs/API/Probability_plotting.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.731882 reliability-0.8.8/docs/API/Reliability_testing/
--rw-rw-rw-   0        0        0      251 2021-03-22 21:59:33.000000 reliability-0.8.8/docs/API/Reliability_testing/KStest.rst
--rw-rw-rw-   0        0        0      257 2021-03-22 22:04:28.000000 reliability-0.8.8/docs/API/Reliability_testing/chi2test.rst
--rw-rw-rw-   0        0        0      278 2023-01-28 09:44:40.000000 reliability-0.8.8/docs/API/Reliability_testing/likelihood_plot.rst
--rw-rw-rw-   0        0        0      296 2021-03-22 22:05:02.000000 reliability-0.8.8/docs/API/Reliability_testing/one_sample_proportion.rst
--rw-rw-rw-   0        0        0      308 2021-03-22 22:05:31.000000 reliability-0.8.8/docs/API/Reliability_testing/reliability_test_duration.rst
--rw-rw-rw-   0        0        0      305 2021-03-22 22:05:57.000000 reliability-0.8.8/docs/API/Reliability_testing/reliability_test_planner.rst
--rw-rw-rw-   0        0        0      302 2021-03-22 22:06:20.000000 reliability-0.8.8/docs/API/Reliability_testing/sample_size_no_failures.rst
--rw-rw-rw-   0        0        0      308 2021-03-22 22:07:07.000000 reliability-0.8.8/docs/API/Reliability_testing/sequential_sampling_chart.rst
--rw-rw-rw-   0        0        0      290 2021-03-22 22:07:33.000000 reliability-0.8.8/docs/API/Reliability_testing/two_proportion_test.rst
--rw-rw-rw-   0        0        0      259 2021-03-22 22:09:24.000000 reliability-0.8.8/docs/API/Reliability_testing.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:33.763133 reliability-0.8.8/docs/API/Repairable_systems/
--rw-rw-rw-   0        0        0      283 2021-03-22 22:08:37.000000 reliability-0.8.8/docs/API/Repairable_systems/MCF_nonparametric.rst
--rw-rw-rw-   0        0        0      274 2021-03-22 22:10:56.000000 reliability-0.8.8/docs/API/Repairable_systems/MCF_parametric.rst
--rw-rw-rw-   0        0        0      247 2021-03-22 22:11:20.000000 reliability-0.8.8/docs/API/Repairable_systems/ROCOF.rst
--rw-rw-rw-   0        0        0      304 2021-03-22 22:11:45.000000 reliability-0.8.8/docs/API/Repairable_systems/optimal_replacement_time.rst
--rw-rw-rw-   0        0        0      286 2021-03-22 22:13:17.000000 reliability-0.8.8/docs/API/Repairable_systems/reliability_growth.rst
--rw-rw-rw-   0        0        0      256 2021-03-22 22:09:47.000000 reliability-0.8.8/docs/API/Repairable_systems.rst
--rw-rw-rw-   0        0        0      229 2021-03-22 05:05:21.000000 reliability-0.8.8/docs/API/Utils.rst
--rw-rw-rw-   0        0        0      233 2021-03-22 08:39:24.000000 reliability-0.8.8/docs/API reference.rst
--rw-rw-rw-   0        0        0     1821 2022-02-01 11:00:40.000000 reliability-0.8.8/docs/About the author.rst
--rw-rw-rw-   0        0        0     1102 2021-11-11 03:52:41.000000 reliability-0.8.8/docs/Acceleration factor.rst
--rw-rw-rw-   0        0        0    62710 2023-02-21 10:43:29.000000 reliability-0.8.8/docs/Changelog.rst
--rw-rw-rw-   0        0        0     3086 2021-06-24 23:14:07.000000 reliability-0.8.8/docs/Chi-squared test.rst
--rw-rw-rw-   0        0        0     2573 2022-03-23 08:48:37.000000 reliability-0.8.8/docs/Citing reliability in your work.rst
--rw-rw-rw-   0        0        0    13405 2021-11-09 08:11:53.000000 reliability-0.8.8/docs/Competing risk models.rst
--rw-rw-rw-   0        0        0     1258 2021-06-06 10:39:21.000000 reliability-0.8.8/docs/Contributing.rst
--rw-rw-rw-   0        0        0     5561 2021-11-11 04:04:17.000000 reliability-0.8.8/docs/Converting data between different formats.rst
--rw-rw-rw-   0        0        0    10309 2021-06-06 13:02:32.000000 reliability-0.8.8/docs/Copyright information.rst
--rw-rw-rw-   0        0        0     7374 2021-05-16 01:02:05.000000 reliability-0.8.8/docs/Creating and plotting distributions.rst
--rw-rw-rw-   0        0        0     2914 2021-12-02 00:41:15.000000 reliability-0.8.8/docs/Credits to those who helped.rst
--rw-rw-rw-   0        0        0     3679 2021-11-11 03:50:56.000000 reliability-0.8.8/docs/Creep.rst
--rw-rw-rw-   0        0        0     2693 2021-06-19 02:01:11.000000 reliability-0.8.8/docs/Crosshairs.rst
--rw-rw-rw-   0        0        0    16224 2021-07-23 07:02:10.000000 reliability-0.8.8/docs/DSZI models.rst
--rw-rw-rw-   0        0        0     5772 2022-08-01 10:57:27.000000 reliability-0.8.8/docs/Datasets.rst
--rw-rw-rw-   0        0        0     2508 2023-01-27 12:23:32.000000 reliability-0.8.8/docs/Development roadmap.rst
--rw-rw-rw-   0        0        0     1260 2020-10-30 04:11:05.000000 reliability-0.8.8/docs/Distribution explorer.rst
--rw-rw-rw-   0        0        0    10929 2022-05-08 10:05:45.000000 reliability-0.8.8/docs/Equations of ALT models.rst
--rw-rw-rw-   0        0        0    12935 2021-11-09 08:12:28.000000 reliability-0.8.8/docs/Equations of supported distributions.rst
--rw-rw-rw-   0        0        0     9423 2021-11-17 02:00:55.000000 reliability-0.8.8/docs/Fitting a dual stress model to ALT data.rst
--rw-rw-rw-   0        0        0     9617 2021-10-07 04:38:36.000000 reliability-0.8.8/docs/Fitting a single stress model to ALT data.rst
--rw-rw-rw-   0        0        0    21095 2021-12-16 03:27:00.000000 reliability-0.8.8/docs/Fitting a specific distribution to data.rst
--rw-rw-rw-   0        0        0    10011 2021-10-20 22:10:58.000000 reliability-0.8.8/docs/Fitting all available distributions to data.rst
--rw-rw-rw-   0        0        0    10237 2021-10-07 22:43:54.000000 reliability-0.8.8/docs/Fitting all available models to ALT data.rst
--rw-rw-rw-   0        0        0     8977 2021-11-11 03:49:16.000000 reliability-0.8.8/docs/Fracture mechanics.rst
--rw-rw-rw-   0        0        0     2089 2021-02-27 09:34:15.000000 reliability-0.8.8/docs/Getting your ALT data in the right format.rst
--rw-rw-rw-   0        0        0     2032 2021-06-19 01:59:01.000000 reliability-0.8.8/docs/Histogram.rst
--rw-rw-rw-   0        0        0    17340 2021-12-15 04:59:19.000000 reliability-0.8.8/docs/How are the confidence intervals calculated.rst
--rw-rw-rw-   0        0        0     8982 2021-10-14 10:03:51.000000 reliability-0.8.8/docs/How are the plotting positions calculated.rst
--rw-rw-rw-   0        0        0    16689 2021-10-15 10:33:51.000000 reliability-0.8.8/docs/How does Least Squares Estimation work.rst
--rw-rw-rw-   0        0        0    20696 2021-11-23 05:15:53.000000 reliability-0.8.8/docs/How does Maximum Likelihood Estimation work.rst
--rw-rw-rw-   0        0        0     1376 2022-01-18 02:33:13.000000 reliability-0.8.8/docs/How to donate to the project.rst
--rw-rw-rw-   0        0        0     1300 2020-09-08 01:42:19.000000 reliability-0.8.8/docs/How to get help.rst
--rw-rw-rw-   0        0        0     7264 2021-11-11 04:10:50.000000 reliability-0.8.8/docs/Importing data from Excel.rst
--rw-rw-rw-   0        0        0     2443 2021-01-05 09:43:55.000000 reliability-0.8.8/docs/Introduction to the field of reliability engineering.rst
--rw-rw-rw-   0        0        0    11020 2021-05-16 01:04:00.000000 reliability-0.8.8/docs/Kaplan-Meier.rst
--rw-rw-rw-   0        0        0     2750 2021-06-24 23:13:47.000000 reliability-0.8.8/docs/Kolmogorov-Smirnov test.rst
--rw-rw-rw-   0        0        0     2568 2023-01-27 04:41:48.000000 reliability-0.8.8/docs/Likelihood plot.rst
--rw-rw-rw-   0        0        0     2032 2021-01-05 09:05:33.000000 reliability-0.8.8/docs/Logo.rst
--rw-rw-rw-   0        0        0     6451 2021-07-20 11:07:16.000000 reliability-0.8.8/docs/Make ALT data.rst
--rw-rw-rw-   0        0        0     3129 2021-07-19 00:14:55.000000 reliability-0.8.8/docs/Make right censored data.rst
--rw-rw-rw-   0        0        0      634 2021-03-21 21:08:23.000000 reliability-0.8.8/docs/Makefile
--rw-rw-rw-   0        0        0     7932 2021-06-19 02:09:47.000000 reliability-0.8.8/docs/Mean cumulative function.rst
--rw-rw-rw-   0        0        0    10917 2022-05-19 09:57:39.000000 reliability-0.8.8/docs/Mixture models.rst
--rw-rw-rw-   0        0        0     5654 2021-05-16 01:04:56.000000 reliability-0.8.8/docs/Nelson-Aalen.rst
--rw-rw-rw-   0        0        0     1548 2021-06-19 02:05:06.000000 reliability-0.8.8/docs/One sample proportion.rst
--rw-rw-rw-   0        0        0     2622 2021-06-22 10:15:42.000000 reliability-0.8.8/docs/Optimal replacement time.rst
--rw-rw-rw-   0        0        0     5321 2021-10-04 23:34:46.000000 reliability-0.8.8/docs/Optimizers.rst
--rw-rw-rw-   0        0        0     1506 2021-11-11 03:51:57.000000 reliability-0.8.8/docs/Palmgren-Miner linear damage model.rst
--rw-rw-rw-   0        0        0    18798 2021-09-08 00:30:30.000000 reliability-0.8.8/docs/Probability plots.rst
--rw-rw-rw-   0        0        0     5506 2021-06-19 01:50:52.000000 reliability-0.8.8/docs/Probability-Probability plots.rst
--rw-rw-rw-   0        0        0     9214 2021-06-19 01:52:21.000000 reliability-0.8.8/docs/Quantile-Quantile plots.rst
--rw-rw-rw-   0        0        0     3969 2021-01-06 09:45:39.000000 reliability-0.8.8/docs/Quickstart for reliability.rst
--rw-rw-rw-   0        0        0     2159 2021-06-19 02:10:28.000000 reliability-0.8.8/docs/ROCOF.rst
--rw-rw-rw-   0        0        0     5489 2021-05-16 01:06:20.000000 reliability-0.8.8/docs/Rank Adjustment.rst
--rw-rw-rw-   0        0        0    14150 2022-12-01 02:50:54.000000 reliability-0.8.8/docs/Recommended resources.rst
--rw-rw-rw-   0        0        0     9638 2021-12-02 00:47:47.000000 reliability-0.8.8/docs/Reliability growth.rst
--rw-rw-rw-   0        0        0     5847 2021-06-19 02:06:35.000000 reliability-0.8.8/docs/Reliability test duration.rst
--rw-rw-rw-   0        0        0     4846 2021-06-19 02:06:59.000000 reliability-0.8.8/docs/Reliability test planner.rst
--rw-rw-rw-   0        0        0     2931 2021-11-11 03:43:35.000000 reliability-0.8.8/docs/SN diagram.rst
--rw-rw-rw-   0        0        0     2646 2021-06-19 02:07:49.000000 reliability-0.8.8/docs/Sample size required for no failures.rst
--rw-rw-rw-   0        0        0     7473 2021-06-19 02:08:24.000000 reliability-0.8.8/docs/Sequential sampling chart.rst
--rw-rw-rw-   0        0        0     1594 2021-06-19 01:56:58.000000 reliability-0.8.8/docs/Similar Distributions.rst
--rw-rw-rw-   0        0        0     3351 2021-01-04 03:50:01.000000 reliability-0.8.8/docs/Solving simultaneous equations with sympy.rst
--rw-rw-rw-   0        0        0     4015 2021-06-19 01:55:45.000000 reliability-0.8.8/docs/Stress-Strength interference.rst
--rw-rw-rw-   0        0        0    12975 2021-11-11 03:46:32.000000 reliability-0.8.8/docs/Stress-strain and strain-life.rst
--rw-rw-rw-   0        0        0     2097 2021-06-19 02:05:50.000000 reliability-0.8.8/docs/Two proportion test.rst
--rw-rw-rw-   0        0        0     5644 2021-03-01 03:45:40.000000 reliability-0.8.8/docs/What does an ALT probability plot show me.rst
--rw-rw-rw-   0        0        0     7666 2021-03-01 03:45:40.000000 reliability-0.8.8/docs/What is Accelerated Life Testing.rst
--rw-rw-rw-   0        0        0     7847 2022-06-27 11:18:19.000000 reliability-0.8.8/docs/What is censored data.rst
--rw-rw-rw-   0        0        0    10166 2022-08-19 10:00:04.000000 reliability-0.8.8/docs/Working with fitted distributions.rst
--rw-rw-rw-   0        0        0     2460 2021-04-06 03:08:12.000000 reliability-0.8.8/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:34.294675 reliability-0.8.8/docs/images/
--rw-rw-rw-   0        0        0    81434 2021-02-27 09:50:55.000000 reliability-0.8.8/docs/images/ALT_probplot_badfit.png
--rw-rw-rw-   0        0        0   106955 2021-02-27 09:50:28.000000 reliability-0.8.8/docs/images/ALT_probplot_goodfit.png
--rw-rw-rw-   0        0        0    20598 2021-02-22 10:21:56.000000 reliability-0.8.8/docs/images/ALT_stress_profiles.png
--rw-rw-rw-   0        0        0    86820 2020-04-20 03:43:22.000000 reliability-0.8.8/docs/images/CI_diagram.png
--rw-rw-rw-   0        0        0    65825 2021-11-30 01:11:50.000000 reliability-0.8.8/docs/images/CI_example1.png
--rw-rw-rw-   0        0        0    42396 2021-12-15 04:58:17.000000 reliability-0.8.8/docs/images/CI_example2.png
--rw-rw-rw-   0        0        0    48285 2020-09-23 04:42:13.000000 reliability-0.8.8/docs/images/CR_fit_hist1.png
--rw-rw-rw-   0        0        0    58484 2020-09-24 10:53:29.000000 reliability-0.8.8/docs/images/CR_fit_probplot2.png
--rw-rw-rw-   0        0        0    62524 2020-10-30 01:48:50.000000 reliability-0.8.8/docs/images/CR_model_PDF_CDFV2.png
--rw-rw-rw-   0        0        0    87304 2020-10-30 01:47:25.000000 reliability-0.8.8/docs/images/CR_model_plotV2.png
--rw-rw-rw-   0        0        0    66776 2020-09-23 04:35:59.000000 reliability-0.8.8/docs/images/CRprobplot1.png
--rw-rw-rw-   0        0        0    87575 2020-09-23 04:29:52.000000 reliability-0.8.8/docs/images/CRvsMM1.png
--rw-rw-rw-   0        0        0    74229 2020-12-30 02:24:28.000000 reliability-0.8.8/docs/images/CRvsMM_fitV4.png
--rw-rw-rw-   0        0        0    21605 2021-02-22 02:30:11.000000 reliability-0.8.8/docs/images/Complete_data.png
--rw-rw-rw-   0        0        0   104729 2021-07-03 02:57:20.000000 reliability-0.8.8/docs/images/DSZI_combined.png
--rw-rw-rw-   0        0        0    87305 2021-07-17 00:56:20.000000 reliability-0.8.8/docs/images/DSZI_example1.png
--rw-rw-rw-   0        0        0    25414 2021-07-17 00:59:18.000000 reliability-0.8.8/docs/images/DSZI_example2.png
--rw-rw-rw-   0        0        0    64962 2021-07-17 01:06:08.000000 reliability-0.8.8/docs/images/DSZI_example3.png
--rw-rw-rw-   0        0        0    28639 2021-07-17 04:45:06.000000 reliability-0.8.8/docs/images/DSZI_example4.png
--rw-rw-rw-   0        0        0   100185 2021-07-17 05:02:05.000000 reliability-0.8.8/docs/images/DSZI_example5.png
--rw-rw-rw-   0        0        0    66806 2021-07-23 01:26:00.000000 reliability-0.8.8/docs/images/DSZI_example6.png
--rw-rw-rw-   0        0        0    77596 2021-07-03 02:50:38.000000 reliability-0.8.8/docs/images/DSZI_explained.png
--rw-rw-rw-   0        0        0    61331 2021-06-23 06:13:19.000000 reliability-0.8.8/docs/images/Exponential_Eyring_lifestress.png
--rw-rw-rw-   0        0        0   126012 2021-06-23 06:13:32.000000 reliability-0.8.8/docs/images/Exponential_Eyring_probability_plot.png
--rw-rw-rw-   0        0        0    67458 2020-12-31 03:18:32.000000 reliability-0.8.8/docs/images/Exponential_probability_plot_V6.png
--rw-rw-rw-   0        0        0    44088 2019-09-27 14:08:13.000000 reliability-0.8.8/docs/images/Fatigue_1.png
--rw-rw-rw-   0        0        0    50844 2019-09-27 14:14:19.000000 reliability-0.8.8/docs/images/Fatigue_2.png
--rw-rw-rw-   0        0        0    88283 2020-12-30 00:17:21.000000 reliability-0.8.8/docs/images/Fit_Gamma_2P_right_cens_V5.png
--rw-rw-rw-   0        0        0    69432 2020-09-24 10:27:58.000000 reliability-0.8.8/docs/images/Fit_Weibull_2P_V4.png
--rw-rw-rw-   0        0        0    44194 2020-09-22 04:02:02.000000 reliability-0.8.8/docs/images/Fit_Weibull_3P_right_cens_V5.png
--rw-rw-rw-   0        0        0   302066 2021-02-27 03:59:02.000000 reliability-0.8.8/docs/images/Fit_everything_ALT_example1_grid.png
--rw-rw-rw-   0        0        0   111813 2021-02-27 03:59:58.000000 reliability-0.8.8/docs/images/Fit_everything_ALT_example1_single.png
--rw-rw-rw-   0        0        0   414183 2021-02-27 09:08:58.000000 reliability-0.8.8/docs/images/Fit_everything_ALT_example2_grid.png
--rw-rw-rw-   0        0        0   147442 2021-02-27 09:09:10.000000 reliability-0.8.8/docs/images/Fit_everything_ALT_example2_single.png
--rw-rw-rw-   0        0        0    80762 2021-09-07 03:52:59.000000 reliability-0.8.8/docs/images/Fit_everything_PP_plot_V6.png
--rw-rw-rw-   0        0        0   185435 2021-09-07 03:52:21.000000 reliability-0.8.8/docs/images/Fit_everything_histogram_plot_V6.png
--rw-rw-rw-   0        0        0   226169 2021-09-07 03:52:39.000000 reliability-0.8.8/docs/images/Fit_everything_probability_plot_V7.png
--rw-rw-rw-   0        0        0    24606 2021-02-22 02:30:55.000000 reliability-0.8.8/docs/images/Interval_censored_data.png
--rw-rw-rw-   0        0        0    85190 2020-09-29 04:59:48.000000 reliability-0.8.8/docs/images/KM_NA_RA.png
--rw-rw-rw-   0        0        0    71232 2020-12-31 09:22:08.000000 reliability-0.8.8/docs/images/KM_all3functions_V4.png
--rw-rw-rw-   0        0        0    32501 2020-09-29 04:35:39.000000 reliability-0.8.8/docs/images/KMvsNAvsRA.png
--rw-rw-rw-   0        0        0    38391 2020-09-21 23:26:35.000000 reliability-0.8.8/docs/images/KStest.png
--rw-rw-rw-   0        0        0    28870 2020-09-29 09:44:42.000000 reliability-0.8.8/docs/images/KaplanMeier_V3.png
--rw-rw-rw-   0        0        0    31614 2021-11-19 03:03:37.000000 reliability-0.8.8/docs/images/LL_range.png
--rw-rw-rw-   0        0        0    34252 2021-11-21 23:39:18.000000 reliability-0.8.8/docs/images/LL_range2.png
--rw-rw-rw-   0        0        0   142944 2021-11-23 04:00:07.000000 reliability-0.8.8/docs/images/LL_range3.png
--rw-rw-rw-   0        0        0    22739 2021-02-22 02:31:17.000000 reliability-0.8.8/docs/images/Left_censored_data.png
--rw-rw-rw-   0        0        0    88116 2020-09-22 03:28:21.000000 reliability-0.8.8/docs/images/Lognormal_plot2.png
--rw-rw-rw-   0        0        0   243340 2021-11-17 01:43:38.000000 reliability-0.8.8/docs/images/Lognormal_power_exponential_lifestress.png
--rw-rw-rw-   0        0        0   169580 2021-06-23 06:17:16.000000 reliability-0.8.8/docs/images/Lognormal_power_exponential_probplot.png
--rw-rw-rw-   0        0        0     3688 2020-04-08 03:23:13.000000 reliability-0.8.8/docs/images/MCF_data.png
--rw-rw-rw-   0        0        0    26987 2020-04-08 02:24:29.000000 reliability-0.8.8/docs/images/MCF_nonparametric.png
--rw-rw-rw-   0        0        0    43965 2020-04-08 05:14:04.000000 reliability-0.8.8/docs/images/MCF_parametric.png
--rw-rw-rw-   0        0        0    44747 2020-08-14 05:23:09.000000 reliability-0.8.8/docs/images/MCF_parametric_badfit.png
--rw-rw-rw-   0        0        0    69407 2021-06-23 06:14:35.000000 reliability-0.8.8/docs/images/Normal_Exponential_lifestress.png
--rw-rw-rw-   0        0        0   233222 2021-11-17 01:44:35.000000 reliability-0.8.8/docs/images/Normal_dual_exponential_lifestress.png
--rw-rw-rw-   0        0        0    75190 2021-06-23 06:16:19.000000 reliability-0.8.8/docs/images/Normal_dual_exponential_probplot.png
--rw-rw-rw-   0        0        0    87136 2020-10-30 02:06:03.000000 reliability-0.8.8/docs/images/Normal_probability_plotV2.png
--rw-rw-rw-   0        0        0    26814 2020-12-31 04:33:11.000000 reliability-0.8.8/docs/images/PPparametric2.png
--rw-rw-rw-   0        0        0    30192 2020-12-31 04:35:59.000000 reliability-0.8.8/docs/images/PPsemiparametric2.png
--rw-rw-rw-   0        0        0    53815 2020-12-31 04:25:30.000000 reliability-0.8.8/docs/images/PPvsQQparametric2.png
--rw-rw-rw-   0        0        0    57775 2020-12-31 04:26:39.000000 reliability-0.8.8/docs/images/PPvsQQsemiparametric2.png
--rw-rw-rw-   0        0        0    42911 2020-12-31 04:19:58.000000 reliability-0.8.8/docs/images/QQparametric2.png
--rw-rw-rw-   0        0        0    43052 2020-12-31 04:22:23.000000 reliability-0.8.8/docs/images/QQsemiparametric2.png
--rw-rw-rw-   0        0        0    21594 2020-09-29 05:11:19.000000 reliability-0.8.8/docs/images/RAheuristic.png
--rw-rw-rw-   0        0        0    40009 2021-01-03 04:17:29.000000 reliability-0.8.8/docs/images/ROCOF.png
--rw-rw-rw-   0        0        0    22181 2021-02-22 02:30:37.000000 reliability-0.8.8/docs/images/Right_censored_data.png
--rw-rw-rw-   0        0        0    59374 2020-10-30 01:34:00.000000 reliability-0.8.8/docs/images/Weibull_Mixture_V6.png
--rw-rw-rw-   0        0        0    89457 2020-10-30 01:28:31.000000 reliability-0.8.8/docs/images/Weibull_Mixture_distV1.png
--rw-rw-rw-   0        0        0    64464 2020-10-30 01:29:33.000000 reliability-0.8.8/docs/images/Weibull_Mixture_dist_propsV1.png
--rw-rw-rw-   0        0        0    48543 2020-09-23 03:33:11.000000 reliability-0.8.8/docs/images/Weibull_Mixture_histV2.png
--rw-rw-rw-   0        0        0    43202 2020-12-30 02:13:25.000000 reliability-0.8.8/docs/images/Weibull_mixture_vs_Weibull_2P_V5.png
--rw-rw-rw-   0        0        0    49352 2021-06-23 06:12:00.000000 reliability-0.8.8/docs/images/Weibull_power_lifestress.png
--rw-rw-rw-   0        0        0    96360 2021-06-23 06:12:21.000000 reliability-0.8.8/docs/images/Weibull_power_probplot.png
--rw-rw-rw-   0        0        0   158023 2020-09-24 11:11:27.000000 reliability-0.8.8/docs/images/Weibull_probability_plot_multi_V4.png
--rw-rw-rw-   0        0        0    39428 2021-12-15 04:01:18.000000 reliability-0.8.8/docs/images/automotive_bounds.png
--rw-rw-rw-   0        0        0   101158 2020-08-14 04:57:53.000000 reliability-0.8.8/docs/images/autoscale_improvement_v052.png
--rw-rw-rw-   0        0        0    57210 2020-12-30 00:00:10.000000 reliability-0.8.8/docs/images/bathtub_curve2.png
--rw-rw-rw-   0        0        0   110362 2021-01-05 09:43:42.000000 reliability-0.8.8/docs/images/bathtub_not_so_common.png
--rw-rw-rw-   0        0        0    37488 2020-09-21 23:05:50.000000 reliability-0.8.8/docs/images/chi2test.png
--rw-rw-rw-   0        0        0    66045 2022-08-19 09:59:25.000000 reliability-0.8.8/docs/images/confidence_bounds_traceV2.png
--rw-rw-rw-   0        0        0    64157 2019-10-13 19:24:48.000000 reliability-0.8.8/docs/images/creep_rupture_curves.png
--rw-rw-rw-   0        0        0    36621 2020-07-04 04:18:44.000000 reliability-0.8.8/docs/images/crosshairs.png
--rw-rw-rw-   0        0        0    12274 2020-12-24 01:24:27.000000 reliability-0.8.8/docs/images/data_formats.png
--rw-rw-rw-   0        0        0    85362 2020-10-30 03:29:35.000000 reliability-0.8.8/docs/images/distribution_explorerV2.png
--rw-rw-rw-   0        0        0   118748 2021-09-07 05:08:55.000000 reliability-0.8.8/docs/images/downsampling.png
--rw-rw-rw-   0        0        0     3178 2020-12-23 23:53:39.000000 reliability-0.8.8/docs/images/excel_FR.png
--rw-rw-rw-   0        0        0     5858 2020-12-23 23:54:45.000000 reliability-0.8.8/docs/images/excel_XCN_1.png
--rw-rw-rw-   0        0        0     5297 2020-12-24 00:04:59.000000 reliability-0.8.8/docs/images/excel_XCN_special.png
--rw-rw-rw-   0        0        0   154846 2020-12-31 03:52:56.000000 reliability-0.8.8/docs/images/expon_weibull_scale_V5.png
--rw-rw-rw-   0        0        0    80494 2021-09-07 03:53:16.000000 reliability-0.8.8/docs/images/fit_everything_best_dist.png
--rw-rw-rw-   0        0        0    31820 2019-10-12 02:06:10.000000 reliability-0.8.8/docs/images/fracture_mechanics_growth.png
--rw-rw-rw-   0        0        0     8237 2020-04-02 03:19:30.000000 reliability-0.8.8/docs/images/grouped_excel.png
--rw-rw-rw-   0        0        0    39970 2020-07-05 07:51:05.000000 reliability-0.8.8/docs/images/histogram.png
--rw-rw-rw-   0        0        0    68528 2019-10-05 14:20:27.000000 reliability-0.8.8/docs/images/hysteresis_tension_compression.png
--rw-rw-rw-   0        0        0    62815 2021-10-14 03:39:11.000000 reliability-0.8.8/docs/images/least_squares_1.PNG
--rw-rw-rw-   0        0        0    31984 2021-10-14 03:42:41.000000 reliability-0.8.8/docs/images/least_squares_2.png
--rw-rw-rw-   0        0        0    44486 2021-10-14 08:48:54.000000 reliability-0.8.8/docs/images/least_squares_3.png
--rw-rw-rw-   0        0        0    32567 2021-10-14 08:55:06.000000 reliability-0.8.8/docs/images/least_squares_4.png
--rw-rw-rw-   0        0        0    91510 2021-10-15 03:35:05.000000 reliability-0.8.8/docs/images/least_squares_5.png
--rw-rw-rw-   0        0        0     3343 2021-06-06 12:32:17.000000 reliability-0.8.8/docs/images/lgplv3.png
--rw-rw-rw-   0        0        0    47747 2023-01-27 04:40:01.000000 reliability-0.8.8/docs/images/likelihood_plot.png
--rw-rw-rw-   0        0        0    43532 2020-12-30 21:29:42.000000 reliability-0.8.8/docs/images/logo.png
--rw-rw-rw-   0        0        0    58677 2020-09-23 00:47:09.000000 reliability-0.8.8/docs/images/mixture_required1.png
--rw-rw-rw-   0        0        0    74904 2021-03-07 09:25:19.000000 reliability-0.8.8/docs/images/multicolor_probability_plot.png
--rw-rw-rw-   0        0        0    33974 2021-06-23 00:16:32.000000 reliability-0.8.8/docs/images/optimal_replacement_interval.png
--rw-rw-rw-   0        0        0    34664 2021-06-22 10:14:36.000000 reliability-0.8.8/docs/images/optimal_replacement_time.png
--rw-rw-rw-   0        0        0    66641 2021-07-02 02:05:18.000000 reliability-0.8.8/docs/images/optimizer_best.PNG
--rw-rw-rw-   0        0        0    37165 2021-07-02 02:06:07.000000 reliability-0.8.8/docs/images/optimizer_default.PNG
--rw-rw-rw-   0        0        0    32272 2021-07-02 02:07:15.000000 reliability-0.8.8/docs/images/optimizer_specific.PNG
--rw-rw-rw-   0        0        0    46672 2021-09-07 03:28:33.000000 reliability-0.8.8/docs/images/plot_points_V4.png
--rw-rw-rw-   0        0        0    20823 2021-10-12 23:06:22.000000 reliability-0.8.8/docs/images/plotting_positions_1.PNG
--rw-rw-rw-   0        0        0    44724 2021-10-13 08:54:06.000000 reliability-0.8.8/docs/images/plotting_positions_2.png
--rw-rw-rw-   0        0        0    31281 2021-10-13 01:59:57.000000 reliability-0.8.8/docs/images/plotting_positions_3.PNG
--rw-rw-rw-   0        0        0    41329 2021-10-13 02:07:24.000000 reliability-0.8.8/docs/images/plotting_positions_4.png
--rw-rw-rw-   0        0        0    89773 2021-10-13 03:42:05.000000 reliability-0.8.8/docs/images/plotting_positions_5.png
--rw-rw-rw-   0        0        0   131059 2020-09-24 11:22:53.000000 reliability-0.8.8/docs/images/probability_plot_mixture_V3.png
--rw-rw-rw-   0        0        0    89573 2020-12-31 04:01:20.000000 reliability-0.8.8/docs/images/probability_plotting_good_and_bad_V6.png
--rw-rw-rw-   0        0        0    97098 2020-12-29 23:54:21.000000 reliability-0.8.8/docs/images/quickstart3.png
--rw-rw-rw-   0        0        0   162350 2021-12-15 03:22:52.000000 reliability-0.8.8/docs/images/range_of_plots_available.png
--rw-rw-rw-   0        0        0    97779 2021-03-04 05:19:54.000000 reliability-0.8.8/docs/images/readme_image_V3.png
--rw-rw-rw-   0        0        0    31432 2021-12-01 03:20:49.000000 reliability-0.8.8/docs/images/reliability_growth_CrowAMSAA.png
--rw-rw-rw-   0        0        0    27995 2021-12-01 03:22:53.000000 reliability-0.8.8/docs/images/reliability_growth_Duane.png
--rw-rw-rw-   0        0        0    69236 2021-12-01 22:34:54.000000 reliability-0.8.8/docs/images/reliability_growth_both.png
--rw-rw-rw-   0        0        0    39651 2020-08-26 00:36:50.000000 reliability-0.8.8/docs/images/reliability_test_duration.png
--rw-rw-rw-   0        0        0    40653 2019-08-05 23:40:16.000000 reliability-0.8.8/docs/images/sequential_sampling_chart.png
--rw-rw-rw-   0        0        0   110758 2021-01-04 03:49:16.000000 reliability-0.8.8/docs/images/similar_distributions_V5.png
--rw-rw-rw-   0        0        0    69124 2019-10-05 01:54:56.000000 reliability-0.8.8/docs/images/strain_life_diagram1.png
--rw-rw-rw-   0        0        0    48046 2019-10-04 16:40:09.000000 reliability-0.8.8/docs/images/stress_life_diagram_fitting.png
--rw-rw-rw-   0        0        0    30780 2019-10-04 16:39:55.000000 reliability-0.8.8/docs/images/stress_strain_diagram_fitting.png
--rw-rw-rw-   0        0        0    42366 2019-10-05 00:11:08.000000 reliability-0.8.8/docs/images/stress_strain_hysteresis.png
--rw-rw-rw-   0        0        0    36428 2021-01-04 03:19:52.000000 reliability-0.8.8/docs/images/stress_strength_V4.png
--rw-rw-rw-   0        0        0    36610 2019-08-05 14:25:49.000000 reliability-0.8.8/docs/images/stress_strength_convergence.png
--rw-rw-rw-   0        0        0    45107 2021-01-04 03:08:55.000000 reliability-0.8.8/docs/images/stress_strength_normdist_V4.png
--rw-rw-rw-   0        0        0    92194 2020-10-30 03:55:19.000000 reliability-0.8.8/docs/images/weibull_percentiles.png
--rw-rw-rw-   0        0        0    38208 2020-10-05 08:29:54.000000 reliability-0.8.8/docs/images/weibull_plot1.png
--rw-rw-rw-   0        0        0     5870 2023-01-27 04:19:38.000000 reliability-0.8.8/docs/index.rst
--rwxrwxrwx   0        0        0      795 2021-03-21 21:08:23.000000 reliability-0.8.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:34.325926 reliability-0.8.8/reliability/
--rw-rw-rw-   0        0        0   616124 2023-02-21 10:26:15.000000 reliability-0.8.8/reliability/ALT_fitters.py
--rw-rw-rw-   0        0        0    45638 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Convert_data.py
--rw-rw-rw-   0        0        0   129252 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Datasets.py
--rw-rw-rw-   0        0        0   361218 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Distributions.py
--rw-rw-rw-   0        0        0   426210 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Fitters.py
--rw-rw-rw-   0        0        0    42276 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Nonparametric.py
--rw-rw-rw-   0        0        0    72323 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Other_functions.py
--rw-rw-rw-   0        0        0   100049 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/PoF.py
--rw-rw-rw-   0        0        0   117481 2023-02-20 10:00:13.000000 reliability-0.8.8/reliability/Probability_plotting.py
--rw-rw-rw-   0        0        0    61918 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Reliability_testing.py
--rw-rw-rw-   0        0        0    55548 2023-01-28 10:39:27.000000 reliability-0.8.8/reliability/Repairable_systems.py
--rw-rw-rw-   0        0        0   309611 2023-02-21 10:24:12.000000 reliability-0.8.8/reliability/Utils.py
--rw-rw-rw-   0        0        0      898 2023-02-21 10:36:33.000000 reliability-0.8.8/reliability/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:34.357176 reliability-0.8.8/reliability.egg-info/
--rw-rw-rw-   0        0        0     6508 2023-02-21 11:55:31.000000 reliability-0.8.8/reliability.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14098 2023-02-21 11:55:32.000000 reliability-0.8.8/reliability.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 11:55:31.000000 reliability-0.8.8/reliability.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-02-21 11:55:31.000000 reliability-0.8.8/reliability.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-21 11:55:31.000000 reliability-0.8.8/reliability.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      132 2023-02-21 10:40:14.000000 reliability-0.8.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-21 11:55:34.372801 reliability-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     2368 2023-02-21 10:57:46.000000 reliability-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-21 11:55:34.372801 reliability-0.8.8/tests/
--rw-rw-rw-   0        0        0    49109 2023-01-28 09:54:46.000000 reliability-0.8.8/tests/test_ALT_fitters.py
--rw-rw-rw-   0        0        0    18837 2022-05-25 03:20:44.000000 reliability-0.8.8/tests/test_Distributions.py
--rw-rw-rw-   0        0        0    42218 2021-09-07 10:15:30.000000 reliability-0.8.8/tests/test_Fitters.py
--rw-rw-rw-   0        0        0     1633 2020-11-06 03:04:19.000000 reliability-0.8.8/tests/test_Nonparametric.py
--rw-rw-rw-   0        0        0     3411 2021-07-19 00:47:11.000000 reliability-0.8.8/tests/test_Other_functions.py
--rw-rw-rw-   0        0        0     4589 2021-12-01 23:51:53.000000 reliability-0.8.8/tests/test_Repairable_systems.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:58:07.848748 reliability-0.8.9/
+-rw-rw-rw-   0        0        0     7817 2020-04-27 03:35:53.000000 reliability-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0       92 2019-08-04 00:35:42.000000 reliability-0.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6043 2023-04-23 04:58:07.833124 reliability-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4789 2022-08-19 10:00:43.000000 reliability-0.8.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 04:58:07.801900 reliability-0.8.9/reliability/
+-rw-rw-rw-   0        0        0   616124 2023-04-23 03:44:58.000000 reliability-0.8.9/reliability/ALT_fitters.py
+-rw-rw-rw-   0        0        0    45638 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Convert_data.py
+-rw-rw-rw-   0        0        0   129252 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Datasets.py
+-rw-rw-rw-   0        0        0   361610 2023-04-20 12:44:12.000000 reliability-0.8.9/reliability/Distributions.py
+-rw-rw-rw-   0        0        0   426210 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Fitters.py
+-rw-rw-rw-   0        0        0    42276 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Nonparametric.py
+-rw-rw-rw-   0        0        0    72323 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Other_functions.py
+-rw-rw-rw-   0        0        0   100049 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/PoF.py
+-rw-rw-rw-   0        0        0   117481 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Probability_plotting.py
+-rw-rw-rw-   0        0        0    61918 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Reliability_testing.py
+-rw-rw-rw-   0        0        0    55548 2023-04-20 14:10:56.000000 reliability-0.8.9/reliability/Repairable_systems.py
+-rw-rw-rw-   0        0        0   309739 2023-04-23 04:00:53.000000 reliability-0.8.9/reliability/Utils.py
+-rw-rw-rw-   0        0        0      898 2023-04-23 04:27:08.000000 reliability-0.8.9/reliability/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:58:07.817502 reliability-0.8.9/reliability.egg-info/
+-rw-rw-rw-   0        0        0     6043 2023-04-23 04:58:07.000000 reliability-0.8.9/reliability.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-04-23 04:58:07.000000 reliability-0.8.9/reliability.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 04:58:07.000000 reliability-0.8.9/reliability.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-04-23 04:58:07.000000 reliability-0.8.9/reliability.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 04:58:07.000000 reliability-0.8.9/reliability.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 04:58:07.848748 reliability-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     2368 2023-04-23 04:27:20.000000 reliability-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:58:07.833124 reliability-0.8.9/tests/
+-rw-rw-rw-   0        0        0    49109 2023-01-28 09:54:46.000000 reliability-0.8.9/tests/test_ALT_fitters.py
+-rw-rw-rw-   0        0        0    18837 2022-05-25 03:20:44.000000 reliability-0.8.9/tests/test_Distributions.py
+-rw-rw-rw-   0        0        0    42218 2021-09-07 10:15:30.000000 reliability-0.8.9/tests/test_Fitters.py
+-rw-rw-rw-   0        0        0     1633 2020-11-06 03:04:19.000000 reliability-0.8.9/tests/test_Nonparametric.py
+-rw-rw-rw-   0        0        0     3411 2021-07-19 00:47:11.000000 reliability-0.8.9/tests/test_Other_functions.py
+-rw-rw-rw-   0        0        0     4589 2021-12-01 23:51:53.000000 reliability-0.8.9/tests/test_Repairable_systems.py
```

### Comparing `reliability-0.8.8/LICENSE` & `reliability-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/PKG-INFO` & `reliability-0.8.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: reliability
-Version: 0.8.8
+Version: 0.8.9
 Summary: Reliability Engineering toolkit for Python
 Home-page: https://reliability.readthedocs.io/en/latest/
 Author: Matthew Reid
 Author-email: alpha.reliability@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://reliability.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/MatthewReid854/reliability
 Project-URL: Donate, https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html
-Description: ![Logo](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/logo.png)
-        
-        [![PyPI version](https://img.shields.io/pypi/v/reliability?color=brightgreen&logo=Python&logoColor=white&label=PyPI%20package)](https://pypi.org/project/reliability/)
-        [![Documentation Status](https://img.shields.io/readthedocs/reliability/latest.svg?logo=read%20the%20docs&logoColor=white&label=Docs&version=latest)](http://reliability.readthedocs.io/?badge=latest)
-        [![Actions Status](https://github.com/MatthewReid854/reliability/workflows/Build%20and%20Test/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
-        [![Actions Status](https://github.com/MatthewReid854/reliability/workflows/CodeQL/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
-        [![Scc Count Badge](https://sloc.xyz/github/MatthewReid854/reliability/?category=code)](https://github.com/MatthewReid854/reliability/)
-        [![Downloads](https://static.pepy.tech/personalized-badge/reliability?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/reliability)
-        [![LGPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg?logo=GNU&logoColor=white)](https://www.gnu.org/licenses/lgpl-3.0.txt)
-        [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3937999-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.3937999)
-        [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html)
-        [![Survey](https://img.shields.io/badge/Provide%20feedback-gray.svg?logo=Verizon)](https://form.jotform.com/203156856636058)
-        
-        *reliability* is a Python library for [reliability engineering](https://en.wikipedia.org/wiki/Reliability_engineering) and [survival analysis](https://en.wikipedia.org/wiki/Survival_analysis). It significantly extends the functionality of scipy.stats and also includes many specialist tools that are otherwise only available in proprietary software.
-        
-        ![](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/readme_image_V3.png)
-        
-        ## Documentation
-        Detailed documentation and examples are available at [readthedocs](https://reliability.readthedocs.io/en/latest/).
-        
-        ## Key features
-        - Fitting probability distributions to data including right censored data
-        - Fitting Weibull mixture models and Weibull Competing risks models
-        - Fitting Weibull Defective Subpopulation (DS) models, Weibull Zero Inflated (ZI) models, and Weibull Defective Subpopulation Zero Inflated (DSZI) models
-        - Calculating the probability of failure for stress-strength interference between any combination of the supported distributions
-        - Support for Exponential, Weibull, Gamma, Gumbel, Normal, Lognormal, Loglogistic, and Beta probability distributions
-        - Mean residual life, quantiles, descriptive statistics summaries, random sampling from distributions
-        - Plots of probability density function (PDF), cumulative distribution function (CDF), survival function (SF), hazard function (HF), and cumulative hazard function (CHF)
-        - Easy creation of distribution objects. Eg. dist = Weibull_Distribution(alpha=4,beta=2)
-        - Non-parametric estimation of survival function using Kaplan-Meier, Nelson-Aalen, and Rank Adjustment
-        - Goodness of fit tests (AICc, BIC, AD, Log-likelihood)
-        - Probability plots on probability paper for all supported distributions
-        - Quantile-Quantile plots and Probability-Probability plots
-        - Reliability growth, optimal replacement time, sequential sampling charts, similar distributions, reliability test planners
-        - Interactive matplotlib functions including crosshairs and distribution explorer
-        - Physics of Failure (SN diagram, stress-strain, fracture mechanics, creep)
-        - Accelerated Life Testing Models (24) comprising of 4 distributions (Weibull, Exponential, Normal, Lognormal) and 6 life-stress models (Exponential, Eyring, Power, Dual-Exponential, Dual-Power, Power-Exponential).
-        - Mean cumulative function and ROCOF for repairable systems
-        
-        ## Installation and upgrading
-        
-        To install *reliability* for the first time, open your command prompt and type:
-        
-        ```
-        pip install reliability
-        ```
-        
-        To upgrade a previous installation of *reliability* to the most recent version, open your command prompt and type:
-        
-        ```
-        pip install --upgrade reliability
-        ```
-        
-        If you would like to receive an email notification when a new release of *reliability* is uploaded to PyPI, [NewReleases.io](https://newreleases.io/) provides this service for free.
-        
-        ## Contact
-        If you find any errors, have any suggestions, or would like to request that something be added, please email alpha.reliability@gmail.com.
-        
 Keywords: reliability,engineering,RAM,weibull,lognormal,exponential,beta,gamma,normal,loglogistic,gumbel,extreme,value,kaplan meier,kaplan-meier,survival,analysis,censored,data,lifelines,probability,distribution,distributions,fit,fitting,curve,quality,ALT,accelerated,life,testing,MCF,mean,cumulative,CIF,DS,ZI,defective,subpopulation,zero,inflated,DSZI,likelihood
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Logo](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/logo.png)
+
+[![PyPI version](https://img.shields.io/pypi/v/reliability?color=brightgreen&logo=Python&logoColor=white&label=PyPI%20package)](https://pypi.org/project/reliability/)
+[![Documentation Status](https://img.shields.io/readthedocs/reliability/latest.svg?logo=read%20the%20docs&logoColor=white&label=Docs&version=latest)](http://reliability.readthedocs.io/?badge=latest)
+[![Actions Status](https://github.com/MatthewReid854/reliability/workflows/Build%20and%20Test/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
+[![Actions Status](https://github.com/MatthewReid854/reliability/workflows/CodeQL/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
+[![Scc Count Badge](https://sloc.xyz/github/MatthewReid854/reliability/?category=code)](https://github.com/MatthewReid854/reliability/)
+[![Downloads](https://static.pepy.tech/personalized-badge/reliability?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/reliability)
+[![LGPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg?logo=GNU&logoColor=white)](https://www.gnu.org/licenses/lgpl-3.0.txt)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3937999-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.3937999)
+[![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html)
+[![Survey](https://img.shields.io/badge/Provide%20feedback-gray.svg?logo=Verizon)](https://form.jotform.com/203156856636058)
+
+*reliability* is a Python library for [reliability engineering](https://en.wikipedia.org/wiki/Reliability_engineering) and [survival analysis](https://en.wikipedia.org/wiki/Survival_analysis). It significantly extends the functionality of scipy.stats and also includes many specialist tools that are otherwise only available in proprietary software.
+
+![](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/readme_image_V3.png)
+
+## Documentation
+Detailed documentation and examples are available at [readthedocs](https://reliability.readthedocs.io/en/latest/).
+
+## Key features
+- Fitting probability distributions to data including right censored data
+- Fitting Weibull mixture models and Weibull Competing risks models
+- Fitting Weibull Defective Subpopulation (DS) models, Weibull Zero Inflated (ZI) models, and Weibull Defective Subpopulation Zero Inflated (DSZI) models
+- Calculating the probability of failure for stress-strength interference between any combination of the supported distributions
+- Support for Exponential, Weibull, Gamma, Gumbel, Normal, Lognormal, Loglogistic, and Beta probability distributions
+- Mean residual life, quantiles, descriptive statistics summaries, random sampling from distributions
+- Plots of probability density function (PDF), cumulative distribution function (CDF), survival function (SF), hazard function (HF), and cumulative hazard function (CHF)
+- Easy creation of distribution objects. Eg. dist = Weibull_Distribution(alpha=4,beta=2)
+- Non-parametric estimation of survival function using Kaplan-Meier, Nelson-Aalen, and Rank Adjustment
+- Goodness of fit tests (AICc, BIC, AD, Log-likelihood)
+- Probability plots on probability paper for all supported distributions
+- Quantile-Quantile plots and Probability-Probability plots
+- Reliability growth, optimal replacement time, sequential sampling charts, similar distributions, reliability test planners
+- Interactive matplotlib functions including crosshairs and distribution explorer
+- Physics of Failure (SN diagram, stress-strain, fracture mechanics, creep)
+- Accelerated Life Testing Models (24) comprising of 4 distributions (Weibull, Exponential, Normal, Lognormal) and 6 life-stress models (Exponential, Eyring, Power, Dual-Exponential, Dual-Power, Power-Exponential).
+- Mean cumulative function and ROCOF for repairable systems
+
+## Installation and upgrading
+
+To install *reliability* for the first time, open your command prompt and type:
+
+```
+pip install reliability
+```
+
+To upgrade a previous installation of *reliability* to the most recent version, open your command prompt and type:
+
+```
+pip install --upgrade reliability
+```
+
+If you would like to receive an email notification when a new release of *reliability* is uploaded to PyPI, [NewReleases.io](https://newreleases.io/) provides this service for free.
+
+## Contact
+If you find any errors, have any suggestions, or would like to request that something be added, please email alpha.reliability@gmail.com.
```

### Comparing `reliability-0.8.8/README.md` & `reliability-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/ALT_fitters.py` & `reliability-0.8.9/reliability/ALT_fitters.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Convert_data.py` & `reliability-0.8.9/reliability/Convert_data.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Datasets.py` & `reliability-0.8.9/reliability/Datasets.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Distributions.py` & `reliability-0.8.9/reliability/Distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7878,14 +7878,15 @@
         """
         Competing_Risks_Model.__combiner(self, xvals=xvals, xmin=xmin, xmax=xmax)
         plt.figure(figsize=(9, 7))
         text_title = str("Competing Risks Model")
         plt.suptitle(text_title, fontsize=15)
 
         plt.subplot(231)
+        self.__pdf[self.__pdf > 1e100] = 1e100
         plt.plot(self.__xvals, self.__pdf)
         restore_axes_limits(
             [(0, 1), (0, 1), False],
             dist=self,
             func="PDF",
             X=self.__xvals,
             Y=self.__pdf,
@@ -7920,14 +7921,15 @@
             xvals=xvals,
             xmin=xmin,
             xmax=xmax,
         )
         plt.title("Survival Function")
 
         plt.subplot(234)
+        self.__hf[self.__hf > 1e100] = 1e100
         plt.plot(self.__xvals, self.__hf)
         restore_axes_limits(
             [(0, 1), (0, 1), False],
             dist=self,
             func="HF",
             X=self.__xvals,
             Y=self.__hf,
@@ -8046,14 +8048,15 @@
                     else:
                         dist.PDF(xvals=self.__xvals, label=dist.param_title_long)
             if "label" in kwargs:
                 textlabel = kwargs.pop("label")
             else:
                 textlabel = "Competing risks model"
             limits = get_axes_limits()
+            self.__pdf[self.__pdf > 1e100] = 1e100
             plt.plot(self.__xvals, self.__pdf, label=textlabel, **kwargs)
             plt.xlabel("x values")
             plt.ylabel("Probability density")
             text_title = str(
                 "Competing Risks Model\n" + " Probability Density Function"
             )
             plt.title(text_title)
@@ -8300,14 +8303,15 @@
                     else:
                         dist.HF(xvals=self.__xvals, label=dist.param_title_long)
             if "label" in kwargs:
                 textlabel = kwargs.pop("label")
             else:
                 textlabel = "Competing risks model"
             limits = get_axes_limits()
+            self.__hf[self.__hf > 1e100] = 1e100
             plt.plot(self.__xvals, self.__hf, label=textlabel, **kwargs)
             plt.xlabel("x values")
             plt.ylabel("Hazard")
             text_title = str("Competing Risks Model\n" + " Hazard Function")
             plt.title(text_title)
             plt.subplots_adjust(top=0.87)
 
@@ -8865,14 +8869,15 @@
         Mixture_Model.__combiner(self, xvals=xvals, xmin=xmin, xmax=xmax)
 
         plt.figure(figsize=(9, 7))
         text_title = str("Mixture Model")
         plt.suptitle(text_title, fontsize=15)
 
         plt.subplot(231)
+        self.__pdf[self.__pdf > 1e100] = 1e100
         plt.plot(self.__xvals, self.__pdf)
         restore_axes_limits(
             [(0, 1), (0, 1), False],
             dist=self,
             func="PDF",
             X=self.__xvals,
             Y=self.__pdf,
@@ -8907,14 +8912,15 @@
             xvals=xvals,
             xmin=xmin,
             xmax=xmax,
         )
         plt.title("Survival Function")
 
         plt.subplot(234)
+        self.__hf[self.__hf > 1e100] = 1e100
         plt.plot(self.__xvals, self.__hf)
         restore_axes_limits(
             [(0, 1), (0, 1), False],
             dist=self,
             func="HF",
             X=self.__xvals,
             Y=self.__hf,
@@ -9033,14 +9039,15 @@
                         dist.PDF(xvals=self.__xvals, label=dist.param_title_long)
             if "label" in kwargs:
                 textlabel = kwargs.pop("label")
             else:
                 textlabel = "Mixture model"
 
             limits = get_axes_limits()
+            self.__pdf[self.__pdf > 1e100] = 1e100
             plt.plot(self.__xvals, self.__pdf, label=textlabel, **kwargs)
             plt.xlabel("x values")
             plt.ylabel("Probability density")
             text_title = str("Mixture Model\n" + " Probability Density Function")
             plt.title(text_title)
             plt.subplots_adjust(top=0.87)
 
@@ -9282,14 +9289,15 @@
                         dist.HF(xvals=X_positive, label=dist.param_title_long)
                     else:
                         dist.HF(xvals=self.__xvals, label=dist.param_title_long)
             if "label" in kwargs:
                 textlabel = kwargs.pop("label")
             else:
                 textlabel = "Mixture model"
+            self.__hf[self.__hf > 1e100] = 1e100
             plt.plot(self.__xvals, self.__hf, label=textlabel, **kwargs)
             plt.xlabel("x values")
             plt.ylabel("Hazard")
             text_title = str("Mixture Model\n" + " Hazard Function")
             plt.title(text_title)
             plt.subplots_adjust(top=0.87)
```

### Comparing `reliability-0.8.8/reliability/Fitters.py` & `reliability-0.8.9/reliability/Fitters.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Nonparametric.py` & `reliability-0.8.9/reliability/Nonparametric.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Other_functions.py` & `reliability-0.8.9/reliability/Other_functions.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/PoF.py` & `reliability-0.8.9/reliability/PoF.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Probability_plotting.py` & `reliability-0.8.9/reliability/Probability_plotting.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Reliability_testing.py` & `reliability-0.8.9/reliability/Reliability_testing.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Repairable_systems.py` & `reliability-0.8.9/reliability/Repairable_systems.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/reliability/Utils.py` & `reliability-0.8.9/reliability/Utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2174,14 +2174,15 @@
             failure_df_ungrouped = pd.DataFrame(
                 data={"failures": failures, "failure_stress_1": failure_stress_1},
                 columns=["failures", "failure_stress_1"],
             )
             failure_groups = []
             unique_failure_stresses = []
             for key, items in failure_df_ungrouped.groupby(["failure_stress_1"]):
+                key = key[0]
                 values = list(items.iloc[:, 0].values)
                 failure_groups.append(values)
                 unique_failure_stresses.append(key)
             # Check that there are enough failures to fit the model.
             # This does not mean 2 failures at each stress.
             # All we need is as many failures as there are parameters in the model.
             total_unique_failures = 0
@@ -2218,14 +2219,15 @@
                     columns=["right_censored", "right_censored_stress_1"],
                 )
                 right_censored_groups = []
                 unique_right_censored_stresses = []
                 for key, items in right_censored_df_ungrouped.groupby(
                     ["right_censored_stress_1"]
                 ):
+                    key = key[0]
                     values = list(items.iloc[:, 0].values)
                     right_censored_groups.append(values)
                     unique_right_censored_stresses.append(key)
                     if key not in unique_failure_stresses:
                         raise ValueError(
                             str(
                                 "The right censored stress "
@@ -2255,14 +2257,15 @@
                     "failure_stress_pairs": failure_stress_pairs,
                 },
                 columns=["failures", "failure_stress_pairs"],
             )
             failure_groups = []
             unique_failure_stresses_str = []
             for key, items in failure_df_ungrouped.groupby(["failure_stress_pairs"]):
+                key = key[0]
                 values = list(items.iloc[:, 0].values)
                 failure_groups.append(values)
                 unique_failure_stresses_str.append(key)
             # Check that there are enough failures to fit the model.
             # This does not mean 2 failures at each stress.
             # All we need is as many failures as there are parameters in the model.
             total_unique_failures = 0
@@ -2314,14 +2317,15 @@
                     columns=["right_censored", "right_censored_stress_pairs"],
                 )
                 right_censored_groups = []
                 unique_right_censored_stresses_str = []
                 for key, items in right_censored_df_ungrouped.groupby(
                     ["right_censored_stress_pairs"]
                 ):
+                    key = key[0]
                     values = list(items.iloc[:, 0].values)
                     right_censored_groups.append(values)
                     unique_right_censored_stresses_str.append(key)
                     if key not in unique_failure_stresses_str:
                         raise ValueError(
                             str(
                                 "The right censored stress pair "
```

### Comparing `reliability-0.8.8/reliability/__init__.py` & `reliability-0.8.9/reliability/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 from reliability import ALT_fitters
 from reliability import PoF
 from reliability import Utils
 from reliability import Convert_data
 from datetime import date
 
 __title__ = 'reliability'
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 __description__ = 'A Python library for reliability engineering'
 __url__ = 'https://reliability.readthedocs.io/en/latest/index.html'
 __author__ = 'Matthew Reid'
 __author_email__ = 'alpha.reliability@gmail.com'
 __license__ = 'LGPLv3'
 __copyright__ = "Copyright 2019-{}, Matthew Reid".format(date.today().year)
```

### Comparing `reliability-0.8.8/reliability.egg-info/PKG-INFO` & `reliability-0.8.9/reliability.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: reliability
-Version: 0.8.8
+Version: 0.8.9
 Summary: Reliability Engineering toolkit for Python
 Home-page: https://reliability.readthedocs.io/en/latest/
 Author: Matthew Reid
 Author-email: alpha.reliability@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://reliability.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/MatthewReid854/reliability
 Project-URL: Donate, https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html
-Description: ![Logo](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/logo.png)
-        
-        [![PyPI version](https://img.shields.io/pypi/v/reliability?color=brightgreen&logo=Python&logoColor=white&label=PyPI%20package)](https://pypi.org/project/reliability/)
-        [![Documentation Status](https://img.shields.io/readthedocs/reliability/latest.svg?logo=read%20the%20docs&logoColor=white&label=Docs&version=latest)](http://reliability.readthedocs.io/?badge=latest)
-        [![Actions Status](https://github.com/MatthewReid854/reliability/workflows/Build%20and%20Test/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
-        [![Actions Status](https://github.com/MatthewReid854/reliability/workflows/CodeQL/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
-        [![Scc Count Badge](https://sloc.xyz/github/MatthewReid854/reliability/?category=code)](https://github.com/MatthewReid854/reliability/)
-        [![Downloads](https://static.pepy.tech/personalized-badge/reliability?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/reliability)
-        [![LGPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg?logo=GNU&logoColor=white)](https://www.gnu.org/licenses/lgpl-3.0.txt)
-        [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3937999-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.3937999)
-        [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html)
-        [![Survey](https://img.shields.io/badge/Provide%20feedback-gray.svg?logo=Verizon)](https://form.jotform.com/203156856636058)
-        
-        *reliability* is a Python library for [reliability engineering](https://en.wikipedia.org/wiki/Reliability_engineering) and [survival analysis](https://en.wikipedia.org/wiki/Survival_analysis). It significantly extends the functionality of scipy.stats and also includes many specialist tools that are otherwise only available in proprietary software.
-        
-        ![](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/readme_image_V3.png)
-        
-        ## Documentation
-        Detailed documentation and examples are available at [readthedocs](https://reliability.readthedocs.io/en/latest/).
-        
-        ## Key features
-        - Fitting probability distributions to data including right censored data
-        - Fitting Weibull mixture models and Weibull Competing risks models
-        - Fitting Weibull Defective Subpopulation (DS) models, Weibull Zero Inflated (ZI) models, and Weibull Defective Subpopulation Zero Inflated (DSZI) models
-        - Calculating the probability of failure for stress-strength interference between any combination of the supported distributions
-        - Support for Exponential, Weibull, Gamma, Gumbel, Normal, Lognormal, Loglogistic, and Beta probability distributions
-        - Mean residual life, quantiles, descriptive statistics summaries, random sampling from distributions
-        - Plots of probability density function (PDF), cumulative distribution function (CDF), survival function (SF), hazard function (HF), and cumulative hazard function (CHF)
-        - Easy creation of distribution objects. Eg. dist = Weibull_Distribution(alpha=4,beta=2)
-        - Non-parametric estimation of survival function using Kaplan-Meier, Nelson-Aalen, and Rank Adjustment
-        - Goodness of fit tests (AICc, BIC, AD, Log-likelihood)
-        - Probability plots on probability paper for all supported distributions
-        - Quantile-Quantile plots and Probability-Probability plots
-        - Reliability growth, optimal replacement time, sequential sampling charts, similar distributions, reliability test planners
-        - Interactive matplotlib functions including crosshairs and distribution explorer
-        - Physics of Failure (SN diagram, stress-strain, fracture mechanics, creep)
-        - Accelerated Life Testing Models (24) comprising of 4 distributions (Weibull, Exponential, Normal, Lognormal) and 6 life-stress models (Exponential, Eyring, Power, Dual-Exponential, Dual-Power, Power-Exponential).
-        - Mean cumulative function and ROCOF for repairable systems
-        
-        ## Installation and upgrading
-        
-        To install *reliability* for the first time, open your command prompt and type:
-        
-        ```
-        pip install reliability
-        ```
-        
-        To upgrade a previous installation of *reliability* to the most recent version, open your command prompt and type:
-        
-        ```
-        pip install --upgrade reliability
-        ```
-        
-        If you would like to receive an email notification when a new release of *reliability* is uploaded to PyPI, [NewReleases.io](https://newreleases.io/) provides this service for free.
-        
-        ## Contact
-        If you find any errors, have any suggestions, or would like to request that something be added, please email alpha.reliability@gmail.com.
-        
 Keywords: reliability,engineering,RAM,weibull,lognormal,exponential,beta,gamma,normal,loglogistic,gumbel,extreme,value,kaplan meier,kaplan-meier,survival,analysis,censored,data,lifelines,probability,distribution,distributions,fit,fitting,curve,quality,ALT,accelerated,life,testing,MCF,mean,cumulative,CIF,DS,ZI,defective,subpopulation,zero,inflated,DSZI,likelihood
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Logo](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/logo.png)
+
+[![PyPI version](https://img.shields.io/pypi/v/reliability?color=brightgreen&logo=Python&logoColor=white&label=PyPI%20package)](https://pypi.org/project/reliability/)
+[![Documentation Status](https://img.shields.io/readthedocs/reliability/latest.svg?logo=read%20the%20docs&logoColor=white&label=Docs&version=latest)](http://reliability.readthedocs.io/?badge=latest)
+[![Actions Status](https://github.com/MatthewReid854/reliability/workflows/Build%20and%20Test/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
+[![Actions Status](https://github.com/MatthewReid854/reliability/workflows/CodeQL/badge.svg)](https://github.com/MatthewReid854/reliability/actions)
+[![Scc Count Badge](https://sloc.xyz/github/MatthewReid854/reliability/?category=code)](https://github.com/MatthewReid854/reliability/)
+[![Downloads](https://static.pepy.tech/personalized-badge/reliability?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/reliability)
+[![LGPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg?logo=GNU&logoColor=white)](https://www.gnu.org/licenses/lgpl-3.0.txt)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3937999-blue.svg?logo=Buffer&logoColor=white)](https://doi.org/10.5281/zenodo.3937999)
+[![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://reliability.readthedocs.io/en/latest/How%20to%20donate%20to%20the%20project.html)
+[![Survey](https://img.shields.io/badge/Provide%20feedback-gray.svg?logo=Verizon)](https://form.jotform.com/203156856636058)
+
+*reliability* is a Python library for [reliability engineering](https://en.wikipedia.org/wiki/Reliability_engineering) and [survival analysis](https://en.wikipedia.org/wiki/Survival_analysis). It significantly extends the functionality of scipy.stats and also includes many specialist tools that are otherwise only available in proprietary software.
+
+![](https://raw.githubusercontent.com/MatthewReid854/reliability/master/docs/images/readme_image_V3.png)
+
+## Documentation
+Detailed documentation and examples are available at [readthedocs](https://reliability.readthedocs.io/en/latest/).
+
+## Key features
+- Fitting probability distributions to data including right censored data
+- Fitting Weibull mixture models and Weibull Competing risks models
+- Fitting Weibull Defective Subpopulation (DS) models, Weibull Zero Inflated (ZI) models, and Weibull Defective Subpopulation Zero Inflated (DSZI) models
+- Calculating the probability of failure for stress-strength interference between any combination of the supported distributions
+- Support for Exponential, Weibull, Gamma, Gumbel, Normal, Lognormal, Loglogistic, and Beta probability distributions
+- Mean residual life, quantiles, descriptive statistics summaries, random sampling from distributions
+- Plots of probability density function (PDF), cumulative distribution function (CDF), survival function (SF), hazard function (HF), and cumulative hazard function (CHF)
+- Easy creation of distribution objects. Eg. dist = Weibull_Distribution(alpha=4,beta=2)
+- Non-parametric estimation of survival function using Kaplan-Meier, Nelson-Aalen, and Rank Adjustment
+- Goodness of fit tests (AICc, BIC, AD, Log-likelihood)
+- Probability plots on probability paper for all supported distributions
+- Quantile-Quantile plots and Probability-Probability plots
+- Reliability growth, optimal replacement time, sequential sampling charts, similar distributions, reliability test planners
+- Interactive matplotlib functions including crosshairs and distribution explorer
+- Physics of Failure (SN diagram, stress-strain, fracture mechanics, creep)
+- Accelerated Life Testing Models (24) comprising of 4 distributions (Weibull, Exponential, Normal, Lognormal) and 6 life-stress models (Exponential, Eyring, Power, Dual-Exponential, Dual-Power, Power-Exponential).
+- Mean cumulative function and ROCOF for repairable systems
+
+## Installation and upgrading
+
+To install *reliability* for the first time, open your command prompt and type:
+
+```
+pip install reliability
+```
+
+To upgrade a previous installation of *reliability* to the most recent version, open your command prompt and type:
+
+```
+pip install --upgrade reliability
+```
+
+If you would like to receive an email notification when a new release of *reliability* is uploaded to PyPI, [NewReleases.io](https://newreleases.io/) provides this service for free.
+
+## Contact
+If you find any errors, have any suggestions, or would like to request that something be added, please email alpha.reliability@gmail.com.
```

### Comparing `reliability-0.8.8/setup.py` & `reliability-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="reliability",
-    version="0.8.8",
+    version="0.8.9",
     description="Reliability Engineering toolkit for Python",
     author="Matthew Reid",
     author_email="alpha.reliability@gmail.com",
     license="LGPLv3",
     url="https://reliability.readthedocs.io/en/latest/",
     project_urls={
         'Documentation': 'https://reliability.readthedocs.io/en/latest/',
```

### Comparing `reliability-0.8.8/tests/test_ALT_fitters.py` & `reliability-0.8.9/tests/test_ALT_fitters.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/tests/test_Distributions.py` & `reliability-0.8.9/tests/test_Distributions.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/tests/test_Fitters.py` & `reliability-0.8.9/tests/test_Fitters.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/tests/test_Nonparametric.py` & `reliability-0.8.9/tests/test_Nonparametric.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/tests/test_Other_functions.py` & `reliability-0.8.9/tests/test_Other_functions.py`

 * *Files identical despite different names*

### Comparing `reliability-0.8.8/tests/test_Repairable_systems.py` & `reliability-0.8.9/tests/test_Repairable_systems.py`

 * *Files identical despite different names*

