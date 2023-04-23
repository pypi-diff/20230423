# Comparing `tmp/causallib-0.9.2.tar.gz` & `tmp/causallib-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causallib-0.9.2.tar", last modified: Sun Feb 19 11:36:14 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "causallib-0.9.3.tar", last modified: Sun Apr 23 20:38:39 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `causallib-0.9.2.tar` & `causallib-0.9.3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     7906 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4800 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/analysis/
--rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.2/causallib/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/contrib/
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/contrib/adversarial_balancing/
--rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/contrib/adversarial_balancing/adversarial_balancing.py
--rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/contrib/adversarial_balancing/classifier_selection.py
--rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/contrib/adversarial_balancing/__init__.py
--rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/contrib/faissknn.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/contrib/hemm/
--rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/gen_synthetic_data.py
--rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/hemm.py
--rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/hemm_api.py
--rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/hemm_metrics.py
--rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/hemm_outcome_models.py
--rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/hemm_utilities.py
--rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/load_ihdp_data.py
--rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/README.md
--rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/hemm/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.2/causallib/contrib/README.md
--rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/contrib/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/contrib/shared_sparsity_selection/
--rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
--rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/contrib/shared_sparsity_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/contrib/tests/
--rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/contrib/tests/test_adversarial_balancing.py
--rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/tests/test_hemm.py
--rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/contrib/tests/test_shared_sparsity_selection.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.2/causallib/contrib/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.2/causallib/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/datasets/
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/datasets/data/
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/
--rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/x.csv
--rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
--rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
--rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
--rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
--rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
--rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
--rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
--rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
--rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
--rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:47.000000 causallib-0.9.2/causallib/datasets/data/nhefs/
--rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/nhefs/NHEFS.csv
--rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/data/nhefs/NHEFS_codebook.csv
--rw-rw-rw-   0        0        0     9765 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/datasets/data_loader.py
--rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/datasets/README.md
--rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/estimation/
--rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/estimation/base_estimator.py
--rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.2/causallib/estimation/base_weight.py
--rw-rw-rw-   0        0        0    26053 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/estimation/doubly_robust.py
--rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/estimation/ipw.py
--rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.2/causallib/estimation/marginal_outcome.py
--rw-rw-rw-   0        0        0    38742 2023-02-14 13:49:48.000000 causallib-0.9.2/causallib/estimation/matching.py
--rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/estimation/overlap_weights.py
--rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/estimation/README.md
--rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.2/causallib/estimation/rlearner.py
--rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.2/causallib/estimation/standardization.py
--rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/estimation/tmle.py
--rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/estimation/xlearner.py
--rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.2/causallib/estimation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/evaluation/
--rw-rw-rw-   0        0        0     9384 2023-02-14 18:47:52.000000 causallib-0.9.2/causallib/evaluation/evaluator.py
--rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/metrics.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/evaluation/plots/
--rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/plots/curve_data_makers.py
--rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/plots/data_extractors.py
--rw-rw-rw-   0        0        0    14523 2023-02-16 14:54:25.000000 causallib-0.9.2/causallib/evaluation/plots/mixins.py
--rw-rw-rw-   0        0        0    39399 2023-02-16 14:54:25.000000 causallib-0.9.2/causallib/evaluation/plots/plots.py
--rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/plots/__init__.py
--rw-rw-rw-   0        0        0     9034 2023-02-14 18:47:52.000000 causallib-0.9.2/causallib/evaluation/predictions.py
--rw-rw-rw-   0        0        0     8848 2023-02-14 15:26:17.000000 causallib-0.9.2/causallib/evaluation/predictor.py
--rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/README.md
--rw-rw-rw-   0        0        0     7143 2023-02-14 18:47:52.000000 causallib-0.9.2/causallib/evaluation/results.py
--rw-rw-rw-   0        0        0     6566 2023-02-14 18:47:52.000000 causallib-0.9.2/causallib/evaluation/scoring.py
--rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/metrics/
--rw-rw-rw-   0        0        0     3334 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/metrics/outcome_metrics.py
--rw-rw-rw-   0        0        0     6426 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/metrics/propensity_metrics.py
--rw-rw-rw-   0        0        0     5043 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/metrics/scorers.py
--rw-rw-rw-   0        0        0     5076 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/metrics/weight_metrics.py
--rw-rw-rw-   0        0        0      370 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/model_selection/
--rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/model_selection/search.py
--rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/model_selection/split.py
--rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/model_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/preprocessing/
--rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/preprocessing/confounder_selection.py
--rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/preprocessing/filters.py
--rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/preprocessing/README.md
--rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.2/causallib/preprocessing/transformers.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.2/causallib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/simulation/
--rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/simulation/CausalSimulator3.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/survival/
--rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/base_survival.py
--rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/marginal_survival.py
--rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/regression_curve_fitter.py
--rw-rw-rw-   0        0        0     8890 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/survival/standardized_survival.py
--rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/survival_utils.py
--rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/univariate_curve_fitter.py
--rw-rw-rw-   0        0        0     3188 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/survival/weighted_standardized_survival.py
--rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/survival/weighted_survival.py
--rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/survival/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/tests/
--rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.2/causallib/tests/survival_matching.py
--rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.2/causallib/tests/test_base_weight.py
--rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/tests/test_causal_simulator3.py
--rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/tests/test_confounder_selection.py
--rw-rw-rw-   0        0        0     3769 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/tests/test_datasets.py
--rw-rw-rw-   0        0        0    25686 2023-02-14 18:25:48.000000 causallib-0.9.2/causallib/tests/test_doublyrobust.py
--rw-rw-rw-   0        0        0     5694 2023-02-15 08:09:36.000000 causallib-0.9.2/causallib/tests/test_evaluation.py
--rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/tests/test_ipw.py
--rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.2/causallib/tests/test_marginal_outcome.py
--rw-rw-rw-   0        0        0    28672 2023-02-14 13:43:45.000000 causallib-0.9.2/causallib/tests/test_matching.py
--rw-rw-rw-   0        0        0    13540 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/tests/test_metrics.py
--rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/tests/test_overlap_weights.py
--rw-rw-rw-   0        0        0    10277 2023-02-16 14:54:25.000000 causallib-0.9.2/causallib/tests/test_plots.py
--rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.2/causallib/tests/test_rlearner.py
--rw-rw-rw-   0        0        0     7796 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/tests/test_scorers.py
--rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.2/causallib/tests/test_search.py
--rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.2/causallib/tests/test_split.py
--rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.2/causallib/tests/test_standardization.py
--rw-rw-rw-   0        0        0    27138 2023-02-14 18:10:35.000000 causallib-0.9.2/causallib/tests/test_survival.py
--rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/tests/test_tmle.py
--rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.2/causallib/tests/test_transformers.py
--rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/tests/test_utils.py
--rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.2/causallib/tests/test_xlearner.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.2/causallib/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 11:32:48.000000 causallib-0.9.2/causallib/utils/
--rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.2/causallib/utils/crossfit.py
--rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.2/causallib/utils/general_tools.py
--rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.2/causallib/utils/stat_utils.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.2/causallib/utils/__init__.py
--rw-rw-rw-   0        0        0       23 2023-02-19 11:30:07.000000 causallib-0.9.2/causallib/__init__.py
--rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     7906 2023-02-19 11:32:48.000000 causallib-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     6787 2022-12-21 14:00:27.000000 causallib-0.9.2/README.md
--rwxrwxrwx   0        0        0      179 2022-12-21 13:34:47.000000 causallib-0.9.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 11:32:48.000000 causallib-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     2792 2022-12-21 14:06:31.000000 causallib-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     7906 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4800 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/analysis/
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.3/causallib/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/
+-rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/adversarial_balancing.py
+-rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/classifier_selection.py
+-rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/contrib/adversarial_balancing/__init__.py
+-rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/faissknn.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/contrib/hemm/
+-rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/gen_synthetic_data.py
+-rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm.py
+-rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_api.py
+-rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_metrics.py
+-rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_outcome_models.py
+-rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/hemm_utilities.py
+-rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/load_ihdp_data.py
+-rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/README.md
+-rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/hemm/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.3/causallib/contrib/README.md
+-rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/contrib/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/
+-rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/shared_sparsity_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/contrib/tests/
+-rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/contrib/tests/test_adversarial_balancing.py
+-rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/tests/test_hemm.py
+-rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/contrib/tests/test_shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.3/causallib/contrib/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:06.000000 causallib-0.9.3/causallib/datasets/data/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/
+-rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/x.csv
+-rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
+-rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
+-rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
+-rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
+-rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
+-rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
+-rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
+-rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
+-rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
+-rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/datasets/data/nhefs/
+-rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS.csv
+-rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS_codebook.csv
+-rw-rw-rw-   0        0        0     9765 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/datasets/data_loader.py
+-rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/datasets/README.md
+-rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/estimation/
+-rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/estimation/base_estimator.py
+-rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.3/causallib/estimation/base_weight.py
+-rw-rw-rw-   0        0        0    26053 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/estimation/doubly_robust.py
+-rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/ipw.py
+-rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.3/causallib/estimation/marginal_outcome.py
+-rw-rw-rw-   0        0        0    38742 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/estimation/matching.py
+-rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/overlap_weights.py
+-rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/estimation/README.md
+-rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.3/causallib/estimation/rlearner.py
+-rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/estimation/standardization.py
+-rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/tmle.py
+-rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/estimation/xlearner.py
+-rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.3/causallib/estimation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/evaluation/
+-rw-rw-rw-   0        0        0     9384 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/evaluator.py
+-rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/evaluation/plots/
+-rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/curve_data_makers.py
+-rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/data_extractors.py
+-rw-rw-rw-   0        0        0    14523 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/plots/mixins.py
+-rw-rw-rw-   0        0        0    39399 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/plots/plots.py
+-rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/plots/__init__.py
+-rw-rw-rw-   0        0        0     9034 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/predictions.py
+-rw-rw-rw-   0        0        0     8848 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/predictor.py
+-rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/README.md
+-rw-rw-rw-   0        0        0     7143 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/results.py
+-rw-rw-rw-   0        0        0     6566 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/evaluation/scoring.py
+-rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/metrics/
+-rw-rw-rw-   0        0        0     3334 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/outcome_metrics.py
+-rw-rw-rw-   0        0        0     6426 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/propensity_metrics.py
+-rw-rw-rw-   0        0        0     5043 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/scorers.py
+-rw-rw-rw-   0        0        0     5076 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/weight_metrics.py
+-rw-rw-rw-   0        0        0      370 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/model_selection/
+-rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/model_selection/search.py
+-rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/model_selection/split.py
+-rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/model_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/preprocessing/
+-rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/preprocessing/confounder_selection.py
+-rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/preprocessing/filters.py
+-rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/preprocessing/README.md
+-rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.3/causallib/preprocessing/transformers.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/simulation/
+-rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/simulation/CausalSimulator3.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/survival/
+-rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/base_survival.py
+-rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/marginal_survival.py
+-rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/regression_curve_fitter.py
+-rw-rw-rw-   0        0        0     8700 2023-04-23 19:51:30.000000 causallib-0.9.3/causallib/survival/standardized_survival.py
+-rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/survival_utils.py
+-rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/univariate_curve_fitter.py
+-rw-rw-rw-   0        0        0     3188 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/survival/weighted_standardized_survival.py
+-rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/survival/weighted_survival.py
+-rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/survival/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/tests/
+-rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.3/causallib/tests/survival_matching.py
+-rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/tests/test_base_weight.py
+-rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/tests/test_causal_simulator3.py
+-rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_confounder_selection.py
+-rw-rw-rw-   0        0        0     3769 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    25686 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_doublyrobust.py
+-rw-rw-rw-   0        0        0     5694 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_evaluation.py
+-rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_ipw.py
+-rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.3/causallib/tests/test_marginal_outcome.py
+-rw-rw-rw-   0        0        0    28672 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_matching.py
+-rw-rw-rw-   0        0        0    13540 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_overlap_weights.py
+-rw-rw-rw-   0        0        0    10277 2023-03-29 12:20:56.000000 causallib-0.9.3/causallib/tests/test_plots.py
+-rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_rlearner.py
+-rw-rw-rw-   0        0        0     7796 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_scorers.py
+-rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.3/causallib/tests/test_search.py
+-rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.3/causallib/tests/test_split.py
+-rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_standardization.py
+-rw-rw-rw-   0        0        0    30021 2023-04-23 19:58:37.000000 causallib-0.9.3/causallib/tests/test_survival.py
+-rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/tests/test_tmle.py
+-rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.3/causallib/tests/test_transformers.py
+-rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/tests/test_utils.py
+-rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/tests/test_xlearner.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:38:07.000000 causallib-0.9.3/causallib/utils/
+-rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.3/causallib/utils/crossfit.py
+-rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.3/causallib/utils/general_tools.py
+-rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.3/causallib/utils/stat_utils.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.3/causallib/utils/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-23 20:01:11.000000 causallib-0.9.3/causallib/__init__.py
+-rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     7906 2023-04-23 20:38:07.000000 causallib-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6787 2023-03-29 12:38:12.000000 causallib-0.9.3/README.md
+-rwxrwxrwx   0        0        0      179 2023-03-29 12:20:56.000000 causallib-0.9.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:38:07.000000 causallib-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     2792 2023-03-29 12:38:12.000000 causallib-0.9.3/setup.py
```

### Comparing `causallib-0.9.2/causallib.egg-info/PKG-INFO` & `causallib-0.9.3/causallib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.2/causallib.egg-info/SOURCES.txt` & `causallib-0.9.3/causallib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/adversarial_balancing/adversarial_balancing.py` & `causallib-0.9.3/causallib/contrib/adversarial_balancing/adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/adversarial_balancing/classifier_selection.py` & `causallib-0.9.3/causallib/contrib/adversarial_balancing/classifier_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/faissknn.py` & `causallib-0.9.3/causallib/contrib/faissknn.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/gen_synthetic_data.py` & `causallib-0.9.3/causallib/contrib/hemm/gen_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/hemm.py` & `causallib-0.9.3/causallib/contrib/hemm/hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/hemm_api.py` & `causallib-0.9.3/causallib/contrib/hemm/hemm_api.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/hemm_metrics.py` & `causallib-0.9.3/causallib/contrib/hemm/hemm_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/hemm_outcome_models.py` & `causallib-0.9.3/causallib/contrib/hemm/hemm_outcome_models.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/hemm_utilities.py` & `causallib-0.9.3/causallib/contrib/hemm/hemm_utilities.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/load_ihdp_data.py` & `causallib-0.9.3/causallib/contrib/hemm/load_ihdp_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/hemm/README.md` & `causallib-0.9.3/causallib/contrib/hemm/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/README.md` & `causallib-0.9.3/causallib/contrib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py` & `causallib-0.9.3/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/tests/test_adversarial_balancing.py` & `causallib-0.9.3/causallib/contrib/tests/test_adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/tests/test_hemm.py` & `causallib-0.9.3/causallib/contrib/tests/test_hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/contrib/tests/test_shared_sparsity_selection.py` & `causallib-0.9.3/causallib/contrib/tests/test_shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/x.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/x.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_1.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_1.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_10.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_10.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_2.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_2.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_3.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_3.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_4.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_4.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_5.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_5.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_6.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_6.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_7.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_7.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_8.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_8.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/acic_challenge_2016/zymu_9.csv` & `causallib-0.9.3/causallib/datasets/data/acic_challenge_2016/zymu_9.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/nhefs/NHEFS.csv` & `causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data/nhefs/NHEFS_codebook.csv` & `causallib-0.9.3/causallib/datasets/data/nhefs/NHEFS_codebook.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/data_loader.py` & `causallib-0.9.3/causallib/datasets/data_loader.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/datasets/README.md` & `causallib-0.9.3/causallib/datasets/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/base_estimator.py` & `causallib-0.9.3/causallib/estimation/base_estimator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/base_weight.py` & `causallib-0.9.3/causallib/estimation/base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/doubly_robust.py` & `causallib-0.9.3/causallib/estimation/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/ipw.py` & `causallib-0.9.3/causallib/estimation/ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/marginal_outcome.py` & `causallib-0.9.3/causallib/estimation/marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/matching.py` & `causallib-0.9.3/causallib/estimation/matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/overlap_weights.py` & `causallib-0.9.3/causallib/estimation/overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/README.md` & `causallib-0.9.3/causallib/estimation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/rlearner.py` & `causallib-0.9.3/causallib/estimation/rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/standardization.py` & `causallib-0.9.3/causallib/estimation/standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/tmle.py` & `causallib-0.9.3/causallib/estimation/tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/estimation/xlearner.py` & `causallib-0.9.3/causallib/estimation/xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/evaluator.py` & `causallib-0.9.3/causallib/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/metrics.py` & `causallib-0.9.3/causallib/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/plots/curve_data_makers.py` & `causallib-0.9.3/causallib/evaluation/plots/curve_data_makers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/plots/data_extractors.py` & `causallib-0.9.3/causallib/evaluation/plots/data_extractors.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/plots/mixins.py` & `causallib-0.9.3/causallib/evaluation/plots/mixins.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/plots/plots.py` & `causallib-0.9.3/causallib/evaluation/plots/plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/predictions.py` & `causallib-0.9.3/causallib/evaluation/predictions.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/predictor.py` & `causallib-0.9.3/causallib/evaluation/predictor.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/README.md` & `causallib-0.9.3/causallib/evaluation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/results.py` & `causallib-0.9.3/causallib/evaluation/results.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/evaluation/scoring.py` & `causallib-0.9.3/causallib/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/metrics/outcome_metrics.py` & `causallib-0.9.3/causallib/metrics/outcome_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/metrics/propensity_metrics.py` & `causallib-0.9.3/causallib/metrics/propensity_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/metrics/scorers.py` & `causallib-0.9.3/causallib/metrics/scorers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/metrics/weight_metrics.py` & `causallib-0.9.3/causallib/metrics/weight_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/model_selection/search.py` & `causallib-0.9.3/causallib/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/model_selection/split.py` & `causallib-0.9.3/causallib/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/preprocessing/confounder_selection.py` & `causallib-0.9.3/causallib/preprocessing/confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/preprocessing/filters.py` & `causallib-0.9.3/causallib/preprocessing/filters.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/preprocessing/README.md` & `causallib-0.9.3/causallib/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/preprocessing/transformers.py` & `causallib-0.9.3/causallib/preprocessing/transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/README.md` & `causallib-0.9.3/causallib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/simulation/CausalSimulator3.py` & `causallib-0.9.3/causallib/simulation/CausalSimulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/base_survival.py` & `causallib-0.9.3/causallib/survival/base_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/marginal_survival.py` & `causallib-0.9.3/causallib/survival/marginal_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/regression_curve_fitter.py` & `causallib-0.9.3/causallib/survival/regression_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/standardized_survival.py` & `causallib-0.9.3/causallib/survival/standardized_survival.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,28 +107,33 @@
 
         min_time = timeline_start if timeline_start is not None else int(t.min())
         max_time = timeline_end if timeline_end is not None else int(t.max())
         contiguous_times = pd.Series(data=range(min_time, max_time + 1),
                                      name=t.name)  # contiguous time steps for inference
 
         a, _, _, _, X = canonize_dtypes_and_names(a=a, w=None, X=X)
-        unique_treatment_values = a.unique()
-        res = pd.DataFrame()
+        unique_treatment_values = sorted(a.unique())
+        res = {}
         for treatment_value in unique_treatment_values:
             if self.stratify:
-                predict_data = X[a == treatment_value]
-                stratum_curve_fitter = self.stratified_curve_fitters_[treatment_value]
+                predict_data = X
+                model = self.stratified_curve_fitters_[treatment_value]
             else:
-                predict_data, a_name = safe_join(df=X, list_of_series=[a], return_series_names=True)
-                stratum_curve_fitter = self.survival_model
-            stratum_individual_survival_curves = stratum_curve_fitter.predict_survival_function(
+                assignment = pd.Series(treatment_value, index=a.index, name=a.name)
+                predict_data, a_name = safe_join(
+                    df=X, list_of_series=[assignment],
+                    return_series_names=True
+                )
+                model = self.survival_model
+            treatment_individual_survival_curves = model.predict_survival_function(
                 X=predict_data,
                 times=contiguous_times
             )
-            res = pd.concat([res, stratum_individual_survival_curves], axis=1)
+            res[treatment_value] = treatment_individual_survival_curves
+        res = pd.concat(res, axis="columns", names=[a.name])
         return res
 
     def estimate_population_outcome(self,
                                     X: pd.DataFrame,
                                     a: pd.Series,
                                     t: pd.Series,
                                     y: Optional[Any] = None,
@@ -148,22 +153,20 @@
             timeline_end (int): Common end time-step. If provided, will generate survival curves up to 'timeline_end'
                                 for all patients. If None, will predict up to last observed event (t.max()).
 
         Returns:
             pd.DataFrame: with time-step index, treatment values as columns and survival as entries
         """
         a, t, _, _, X = canonize_dtypes_and_names(a=a, t=t,  X=X)
-        unique_treatment_values = a.unique()
-        res = {}
-        for treatment_value in unique_treatment_values:
-            assignment = pd.Series(data=treatment_value, index=X.index, name=a.name)
-            individual_survival_curves = self.estimate_individual_outcome(X=X, a=assignment, t=t,
-                                                                          timeline_start=timeline_start,
-                                                                          timeline_end=timeline_end)
-            res[treatment_value] = individual_survival_curves.mean(axis='columns')
-
-        res = pd.DataFrame(res)
+        individual_survival_curves = self.estimate_individual_outcome(
+            X=X, a=a, t=t,
+            timeline_start=timeline_start,
+            timeline_end=timeline_end,
+        )
+        res = individual_survival_curves.groupby(
+            level=0, axis="columns",
+        ).mean()
 
         # Setting index/column names
         res.index.name = t.name
         res.columns.name = a.name
         return res
```

### Comparing `causallib-0.9.2/causallib/survival/survival_utils.py` & `causallib-0.9.3/causallib/survival/survival_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/univariate_curve_fitter.py` & `causallib-0.9.3/causallib/survival/univariate_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/weighted_standardized_survival.py` & `causallib-0.9.3/causallib/survival/weighted_standardized_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/weighted_survival.py` & `causallib-0.9.3/causallib/survival/weighted_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/survival/__init__.py` & `causallib-0.9.3/causallib/survival/__init__.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/survival_matching.py` & `causallib-0.9.3/causallib/tests/survival_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_base_weight.py` & `causallib-0.9.3/causallib/tests/test_base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_causal_simulator3.py` & `causallib-0.9.3/causallib/tests/test_causal_simulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_confounder_selection.py` & `causallib-0.9.3/causallib/tests/test_confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_datasets.py` & `causallib-0.9.3/causallib/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_doublyrobust.py` & `causallib-0.9.3/causallib/tests/test_doublyrobust.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_evaluation.py` & `causallib-0.9.3/causallib/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_ipw.py` & `causallib-0.9.3/causallib/tests/test_ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_marginal_outcome.py` & `causallib-0.9.3/causallib/tests/test_marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_matching.py` & `causallib-0.9.3/causallib/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_metrics.py` & `causallib-0.9.3/causallib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_overlap_weights.py` & `causallib-0.9.3/causallib/tests/test_overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_plots.py` & `causallib-0.9.3/causallib/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_rlearner.py` & `causallib-0.9.3/causallib/tests/test_rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_scorers.py` & `causallib-0.9.3/causallib/tests/test_scorers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_search.py` & `causallib-0.9.3/causallib/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_split.py` & `causallib-0.9.3/causallib/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_standardization.py` & `causallib-0.9.3/causallib/tests/test_standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_survival.py` & `causallib-0.9.3/causallib/tests/test_survival.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import unittest
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.pipeline import Pipeline
+from sklearn.utils import Bunch
 from causallib.datasets.data_loader import load_nhefs_survival
 from causallib.survival.survival_utils import get_person_time_df, safe_join
 from causallib.estimation.ipw import IPW
 from causallib.estimation import Matching
 from causallib.survival.standardized_survival import StandardizedSurvival
 from causallib.survival.weighted_standardized_survival import WeightedStandardizedSurvival
 from causallib.survival.weighted_survival import WeightedSurvival
@@ -286,34 +287,34 @@
     def setUp(self) -> None:
         np.random.seed(RANDOM_SEED)
         data = load_nhefs_survival()
         self.X, self.a, self.t, self.y = data.X, data.a, data.t, data.y
 
         # Init various multiple models
         self.estimators = {
-            # 'observed_non_parametric': MarginalSurvival(),
-            # 'observed_parametric': MarginalSurvival(survival_model=LogisticRegression(max_iter=2000)),
-            # 'ipw_non_parametric': WeightedSurvival(
-            #     weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
-            #     survival_model=None),
-            # 'ipw_parametric': WeightedSurvival(weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
-            #                                    survival_model=LogisticRegression(max_iter=4000)),
-            # 'ipw_parametric_pipeline': WeightedSurvival(
-            #     weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
-            #     survival_model=Pipeline(
-            #         [('transform', PolynomialFeatures(degree=2)), ('LR', LogisticRegression(max_iter=1000, C=2))])),
+            'observed_non_parametric': MarginalSurvival(),
+            'observed_parametric': MarginalSurvival(survival_model=LogisticRegression(max_iter=2000)),
+            'ipw_non_parametric': WeightedSurvival(
+                weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
+                survival_model=None),
+            'ipw_parametric': WeightedSurvival(weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
+                                               survival_model=LogisticRegression(max_iter=4000)),
+            'ipw_parametric_pipeline': WeightedSurvival(
+                weight_model=IPW(LogisticRegression(max_iter=4000), use_stabilized=True),
+                survival_model=Pipeline(
+                    [('transform', PolynomialFeatures(degree=2)), ('LR', LogisticRegression(max_iter=1000, C=2))])),
             'matching_non_parametric': WeightedSurvival(
                 weight_model=Matching(
                     matching_mode="treatment_to_control",
                 ),
             ),
-            # 'standardization_non_stratified': StandardizedSurvival(survival_model=LogisticRegression(max_iter=4000),
-            #                                                        stratify=False),
-            # 'standardization_stratified': StandardizedSurvival(survival_model=LogisticRegression(max_iter=4000),
-            #                                                    stratify=True),
+            'standardization_non_stratified': StandardizedSurvival(survival_model=LogisticRegression(max_iter=4000),
+                                                                   stratify=False),
+            'standardization_stratified': StandardizedSurvival(survival_model=LogisticRegression(max_iter=4000),
+                                                               stratify=True),
         }
 
     def test_nhefs(self, plot=False):
         EXPECTED_SURVIVAL_DIFFS = {'observed_non_parametric': 6,
                                    'observed_parametric': 6,
                                    'ipw_non_parametric': 1,
                                    'ipw_parametric': 1,
@@ -322,17 +323,18 @@
                                    'standardization_non_stratified': 1,
                                    'standardization_stratified': 1,
                                    }
         TEST_DELTA = 2
 
         res = {}
         for estimator_name, estimator in self.estimators.items():
-            estimator.fit(X=self.X, a=self.a, t=self.t, y=self.y)
-            survival_curves = estimator.estimate_population_outcome(X=self.X, a=self.a, t=self.t, y=self.y)
-            res[estimator_name] = survival_curves
+            with self.subTest(f"Test {estimator_name}"):
+                estimator.fit(X=self.X, a=self.a, t=self.t, y=self.y)
+                survival_curves = estimator.estimate_population_outcome(X=self.X, a=self.a, t=self.t, y=self.y)
+                res[estimator_name] = survival_curves
 
         for estimator_name, survival_curve in res.items():
             surv_non_qsmk = 100.0 * float(survival_curve[0].iloc[-1])
             surv_qsmk = 100.0 * float(survival_curve[1].iloc[-1])
             self.assertAlmostEqual(surv_non_qsmk - surv_qsmk, EXPECTED_SURVIVAL_DIFFS[estimator_name], delta=TEST_DELTA)
 
         # Plots - for debugging purposes
@@ -465,14 +467,67 @@
         model = StandardizedSurvival
         params = {'survival_model': LogisticRegression(max_iter=2000), 'stratify': True}
         adjusted_diff = fit_synthetic_data(model_cls=model, params=params, test_data=test_data)
 
         self.assertAlmostEqual(adjusted_diff, TEST_DATA_DRUG_EFFECTS_B_ORACLE_DIFF,
                                delta=TEST_DATA_DRUG_EFFECTS_DELTA)
 
+    def test_individual_estimation(self):
+        def ensure_individual_estimation(model, data):
+            model.fit(data.X, data.a, data.t, data.y)
+            po = model.estimate_individual_outcome(data.X, data.a, data.t)
+            # Time points are rows:
+            self.assertEqual(po.shape[0], data.t.nunique())
+            # Samples are columns, times two treatments:
+            self.assertEqual(po.shape[1], data.X.shape[0] * 2)
+            # Columns are treatment over samples:
+            self.assertIsInstance(po.columns, pd.MultiIndex)
+            self.assertEqual(po.columns.names, ["a", "subject_id"])
+
+        data = TEST_DATA_TTE_DRUG_EFFECTS['B']
+        data = Bunch(
+            X=data[["x_0", "x_1"]],
+            a=data["a"], t=data["t"],
+            y=data["y"],
+        )
+
+        with self.subTest("Stratified Pooled Logistic Regression"):
+            model = StandardizedSurvival(
+                LogisticRegression(max_iter=2000),
+                stratify=True,
+            )
+            ensure_individual_estimation(model, data)
+
+        with self.subTest("Unstratified Pooled Logistic Regression"):
+            model = StandardizedSurvival(
+                LogisticRegression(max_iter=2000),
+                stratify=False,
+            )
+            ensure_individual_estimation(model, data)
+
+    def test_unnamed_input(self):
+        test_data = TEST_DATA_TTE_DRUG_EFFECTS['A']
+        X = test_data[['x_0', 'x_1']]
+        a = test_data['a']
+        y = test_data['y']
+        t = test_data['t']
+
+        X.index.name = None
+        a.name = None
+        y.name = None
+        t.name = None
+        std = StandardizedSurvival(survival_model=LogisticRegression())
+        std.fit(X, a, t, y)
+        outcomes = std.estimate_population_outcome(X=X, a=a, t=t, y=y)
+
+        self.assertEqual(outcomes.index.name, "t")  # Default time name when canonizing names
+        self.assertEqual(outcomes.columns.name, "a")  # Default time name when canonizing names
+
+
+class TestWeightedStandardizedSurvival(unittest.TestCase):
     def test_weighted_standardization_stratified(self):
         test_data = TEST_DATA_TTE_DRUG_EFFECTS['A']
         model = WeightedStandardizedSurvival
         params = {'weight_model': IPW(LogisticRegression(max_iter=1000), use_stabilized=True),
                   'survival_model': LogisticRegression(max_iter=1000),
                   'stratify': True}
         adjusted_diff = fit_synthetic_data(model_cls=model, params=params, test_data=test_data)
@@ -487,32 +542,14 @@
                   'survival_model': LogisticRegression(max_iter=4000, C=5),
                   'stratify': False}
         adjusted_diff = fit_synthetic_data(model_cls=model, params=params, test_data=test_data)
 
         self.assertAlmostEqual(adjusted_diff, TEST_DATA_DRUG_EFFECTS_A_ORACLE_DIFF,
                                delta=TEST_DATA_DRUG_EFFECTS_DELTA)
 
-    def test_unnamed_input(self):
-        test_data = TEST_DATA_TTE_DRUG_EFFECTS['A']
-        X = test_data[['x_0', 'x_1']]
-        a = test_data['a']
-        y = test_data['y']
-        t = test_data['t']
-
-        X.index.name = None
-        a.name = None
-        y.name = None
-        t.name = None
-        std = StandardizedSurvival(survival_model=LogisticRegression())
-        std.fit(X, a, t, y)
-        outcomes = std.estimate_population_outcome(X=X, a=a, t=t, y=y)
-
-        self.assertEqual(outcomes.index.name, "t")  # Default time name when canonizing names
-        self.assertEqual(outcomes.columns.name, "a")  # Default time name when canonizing names
-
 
 @unittest.skipUnless(LIFELINES_FOUND, 'lifelines not found')
 class TestLifelines(unittest.TestCase):
     """
     Test integration with 'lifelines' Python package.
     """
     def setUp(self) -> None:
@@ -576,14 +613,48 @@
             weighted_standardized_survival.fit(self.X, self.a, self.t, self.y)
 
         # With fit_kwargs - should not raise StatisticalWarning (might raise other warnings, though)
         with self.assertRaises(AssertionError):  # negation workaround since there's no assertNotWarns
             with self.assertWarns(lifelines.exceptions.StatisticalWarning):
                 weighted_standardized_survival.fit(self.X, self.a, self.t, self.y, fit_kwargs={'robust': True})
 
+    def test_individual_estimation(self):
+        def ensure_individual_estimation(model, data):
+            model.fit(data.X, data.a, data.t, data.y)
+            po = model.estimate_individual_outcome(data.X, data.a, data.t)
+            # Time points are rows:
+            self.assertEqual(po.shape[0], data.t.nunique())
+            # Samples are columns, times two treatments:
+            self.assertEqual(po.shape[1], data.X.shape[0] * 2)
+            # Columns are treatment over samples:
+            self.assertIsInstance(po.columns, pd.MultiIndex)
+            # Cox regression does not save X.index name:
+            self.assertEqual(po.columns.names, ["a", None])
+
+        data = TEST_DATA_TTE_DRUG_EFFECTS['B']
+        data = Bunch(
+            X=data[["x_0", "x_1"]],
+            a=data["a"], t=data["t"],
+            y=data["y"],
+        )
+
+        with self.subTest("Stratified Cox Regression"):
+            model = StandardizedSurvival(
+                lifelines.CoxPHFitter(penalizer=10),
+                stratify=True,
+            )
+            ensure_individual_estimation(model, data)
+
+        with self.subTest("Unstratified Cox Regression"):
+            model = StandardizedSurvival(
+                lifelines.CoxPHFitter(penalizer=10),
+                stratify=False,
+            )
+            ensure_individual_estimation(model, data)
+
 
 class TestFeatureTransform(unittest.TestCase):
     """
     Test scikit-learn Pipeline/transform as a base learner for standardized survival curves.
     """
     def setUp(self) -> None:
         test_data = TEST_DATA_TTE_DRUG_EFFECTS['A']
```

### Comparing `causallib-0.9.2/causallib/tests/test_tmle.py` & `causallib-0.9.3/causallib/tests/test_tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_transformers.py` & `causallib-0.9.3/causallib/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_utils.py` & `causallib-0.9.3/causallib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/tests/test_xlearner.py` & `causallib-0.9.3/causallib/tests/test_xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/utils/crossfit.py` & `causallib-0.9.3/causallib/utils/crossfit.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/utils/general_tools.py` & `causallib-0.9.3/causallib/utils/general_tools.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/causallib/utils/stat_utils.py` & `causallib-0.9.3/causallib/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/LICENSE` & `causallib-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/PKG-INFO` & `causallib-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.2/README.md` & `causallib-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.2/setup.py` & `causallib-0.9.3/setup.py`

 * *Files identical despite different names*

