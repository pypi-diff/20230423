# Comparing `tmp/jupyterlab_ui_profiler-0.1.8.tar.gz` & `tmp/jupyterlab_ui_profiler-0.2.0.tar.gz`

## Comparing `jupyterlab_ui_profiler-0.1.8.tar` & `jupyterlab_ui_profiler-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.eslintignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.eslintrc.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.stylelintrc
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/babel.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jest.config.js
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/package.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/readthedocs.yml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/setup.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/tsconfig.json
--rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/yarn.lock
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/make.bat
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/source/changelog.rst
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/source/conf.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/source/index.rst
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyter-config/nb-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyter-config/server-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/_version.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/package.json
--rw-r--r--   0        0        0    64637 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/103.fef9f7b84e7801e31ec3.js
--rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
--rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/remoteEntry.01dddfb6079d8140a904.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/style.js
--rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/benchmark.ts
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/css.ts
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/dramaturg.ts
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/index.ts
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/jsBenchmarks.ts
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/lumino.tsx
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/profiler.d.ts
--rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/scenarios.ts
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/statistics.ts
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/styleBenchmarks.tsx
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/table.ts
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/templates.tsx
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/tokens.ts
--rw-r--r--   0        0        0    41126 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/ui.tsx
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/utils.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/__tests__/jupyterlab-ui-profiler.spec.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/__tests__/statistics.spec.ts
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-base.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-execution.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-profile.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-rule-group.json
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-rule-usage.json
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-rule.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-base.json
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-completer.json
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-debugger.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-menu-open.json
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-scroll.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-sidebars.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/schema/scenario-tabs.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-base.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-execution.ts
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-profile.ts
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-rule-group.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-rule-usage.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-rule.ts
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-base.ts
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-completer.ts
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-debugger.ts
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-menu-open.ts
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-scroll.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-sidebars.ts
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/src/types/_scenario-tabs.ts
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/package.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
--rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
--rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
--rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
--rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
--rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
--rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
--rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.eslintignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.eslintrc.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.stylelintrc
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/babel.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jest.config.js
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/package.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/readthedocs.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/setup.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/yarn.lock
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyter-config/nb-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyter-config/server-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/_version.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/package.json
+-rw-r--r--   0        0        0    65688 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/148.d0923e85cee15af0e9d9.js
+-rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/remoteEntry.2c015c9bba0ac87e826d.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/style.js
+-rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/benchmark.ts
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/browserProfiler.d.ts
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/css.ts
+-rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/dramaturg.ts
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/index.ts
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/jsBenchmarks.ts
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/lumino.tsx
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/profiler.ts
+-rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/scenarios.ts
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/statistics.ts
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/styleBenchmarks.tsx
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/table.ts
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/templates.tsx
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/tokens.ts
+-rw-r--r--   0        0        0    40154 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/ui.tsx
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/utils.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/__tests__/jupyterlab-ui-profiler.spec.ts
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/__tests__/statistics.spec.ts
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-base.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-execution.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-profile.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-group.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-usage.json
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-base.json
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-completer.json
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-debugger.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-menu-open.json
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-scroll.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-sidebars.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-tabs.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-base.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-execution.ts
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-profile.ts
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-group.ts
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-usage.ts
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule.ts
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-base.ts
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-completer.ts
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-debugger.ts
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-menu-open.ts
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-scroll.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-sidebars.ts
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-tabs.ts
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/package.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
+-rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
+-rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
+-rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
+-rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
+-rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
+-rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
+-rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_ui_profiler-0.1.8/.eslintrc.js` & `jupyterlab_ui_profiler-0.2.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/CHANGELOG.md` & `jupyterlab_ui_profiler-0.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.0
+
+([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.8...3c4d2c8f2f80ba5e81c16b1dea2b77d76c209766))
+
+### Enhancements made
+
+- Separate profiler out of the user interface [#46](https://github.com/jupyterlab/ui-profiler/pull/46) ([@krassowski](https://github.com/krassowski))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-04-02&to=2023-04-23&type=c))
+
+[@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-04-02..2023-04-23&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.8
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.7...528461f6f554e6656475aa2054c3ec12240f65e5))
 
 ### Bugs fixed
 
 - Use `_version.py` auto-generated by Hatchling [#44](https://github.com/jupyterlab/ui-profiler/pull/44) ([@krassowski](https://github.com/krassowski))
@@ -24,16 +40,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-02-11&to=2023-04-02&type=c))
 
 [@CommanderPho](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3ACommanderPho+updated%3A2023-02-11..2023-04-02&type=Issues) | [@dependabot](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Adependabot+updated%3A2023-02-11..2023-04-02&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Agithub-actions+updated%3A2023-02-11..2023-04-02&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-02-11..2023-04-02&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Awelcome+updated%3A2023-02-11..2023-04-02&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.7
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.6...eac70e739f420197f6ae0049d93602ce6ac8a1eb))
 
 ### Enhancements made
 
 - Allow to add scenarios programmatically [#31](https://github.com/jupyterlab/ui-profiler/pull/31) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyterlab_ui_profiler-0.1.8/RELEASE.md` & `jupyterlab_ui_profiler-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/jest.config.js` & `jupyterlab_ui_profiler-0.2.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/package.json` & `jupyterlab_ui_profiler-0.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.8"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_ui_profiler-0.1.8/tsconfig.json` & `jupyterlab_ui_profiler-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/yarn.lock` & `jupyterlab_ui_profiler-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/docs/Makefile` & `jupyterlab_ui_profiler-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/docs/make.bat` & `jupyterlab_ui_profiler-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/docs/source/conf.py` & `jupyterlab_ui_profiler-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/docs/source/_static/logo-icon.png` & `jupyterlab_ui_profiler-0.2.0/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/__init__.py` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/package.json` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2c015c9bba0ac87e826d.js'}}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -47,15 +47,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jupyterlab/ui-profiler",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.01dddfb6079d8140a904.js",
+            "load": "static/remoteEntry.2c015c9bba0ac87e826d.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_ui_profiler/labextension",
         "sharedPackages": {
             "@lumino/datagrid": {
                 "bundled": false,
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.8"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/103.fef9f7b84e7801e31ec3.js` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/148.d0923e85cee15af0e9d9.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,67 +1,67 @@
 "use strict";
 (self.webpackChunk_jupyterlab_ui_profiler = self.webpackChunk_jupyterlab_ui_profiler || []).push([
-    [103], {
-        103: (e, t, n) => {
+    [148], {
+        8148: (e, t, n) => {
             n.r(t), n.d(t, {
-                IUIProfiler: () => ye,
-                default: () => We
+                IUIProfiler: () => we,
+                default: () => ze
             });
             var s = n(5687),
                 i = n(3033),
-                r = n(8142),
-                o = n(7986),
-                a = n(7280),
-                l = n(1467),
-                c = n(3169),
-                u = n(2502),
-                d = n(3443),
-                p = n(6271),
-                m = n.n(p),
-                h = n(8820),
-                f = n(2583),
-                g = n(1526),
+                r = n(7986),
+                o = n(7280),
+                a = n(1467),
+                l = n(3169),
+                c = n(2502),
+                u = n(3443),
+                d = n(6271),
+                p = n.n(d),
+                m = n(8820),
+                h = n(2583),
+                f = n(1526),
+                g = n(8142),
                 w = n(1840),
                 y = n(1641);
 
             function b() {
                 const e = document.querySelectorAll("*"),
                     t = {};
                 for (const n of e.values()) {
                     const e = n.tagName.toLocaleLowerCase();
                     Object.prototype.hasOwnProperty.call(t, e) ? t[e] += 1 : t[e] = 1
                 }
                 return t
             }
 
-            function v(e) {
+            function k(e) {
                 if (isNaN(e)) return "-";
                 const t = e / 1e3,
                     n = Math.floor(t / 60);
                 let s = Math.round(t - 60 * n) + " seconds";
                 if (n < 1) return s;
                 const i = Math.floor(n / 60);
                 return s = Math.round(n - 60 * i) + " minutes " + s, i < 1 || (s = Math.round(i) + " hours " + s), s
             }
 
-            function* k(e) {
-                for (const t of e.childNodes) yield t, yield* k(t)
+            function* v(e) {
+                for (const t of e.childNodes) yield t, yield* v(t)
             }
 
             function* S(e) {
                 for (const t of e) {
                     yield t.target;
                     for (const e of t.addedNodes)
                         if (e !== document.body) {
                             yield e;
-                            for (const t of k(e)) yield t
+                            for (const t of v(e)) yield t
                         } for (const e of t.removedNodes)
                         if (e !== document.body) {
                             yield e;
-                            for (const t of k(e)) yield t
+                            for (const t of v(e)) yield t
                         }
                 }
             }
             const E = 1 / (2 * Math.PI) ** .5;
             var x;
             ! function(e) {
                 function t(e) {
@@ -134,15 +134,15 @@
                 constructor(e) {
                     this.element = e
                 }
                 $(e) {
                     return A(e, this.element)
                 }
                 click() {
-                    return _(this.element)
+                    return R(this.element)
                 }
                 async focus() {
                     return this.element.focus()
                 }
                 press(e, t = {
                     delay: 0
                 }) {
@@ -225,33 +225,33 @@
                 }
                 const s = t.timeout || 5e3;
                 return Promise.race([n, new Promise(((n, i) => {
                     setTimeout((() => i(`Selector ${e} not found in ${t.state} state in ${s/1e3}s`)), s)
                 }))])
             }
             const I = (0, j.Vc)(),
-                T = I._codes,
-                R = Object.fromEntries(Object.entries(T).map((e => e.reverse())));
+                _ = I._codes,
+                T = Object.fromEntries(Object.entries(_).map((e => e.reverse())));
             async function B(e, t = {
                 delay: 0
             }, n = null) {
                 n || (n = document.activeElement || document.body);
                 const s = e.split("+"),
                     i = s.filter((e => I.isModifierKey(e))),
                     r = s.filter((e => !I.isModifierKey(e)))[0],
                     o = {
-                        keyCode: R[r],
+                        keyCode: T[r],
                         shiftKey: i.includes("Shift"),
                         ctrlKey: i.includes("Ctrl"),
                         metaKey: i.includes("Meta"),
                         key: r
                     };
                 n.dispatchEvent(new KeyboardEvent("keydown", o)), n.dispatchEvent(new KeyboardEvent("keypress", o)), t.delay && await new Promise((e => setTimeout(e, t.delay))), n.dispatchEvent(new KeyboardEvent("keyup", o))
             }
-            async function _(e) {
+            async function R(e) {
                 const t = e.getBoundingClientRect(),
                     n = {
                         clientX: t.x + t.width / 2,
                         clientY: t.x + t.height / 2,
                         bubbles: !0
                     };
                 e.dispatchEvent(new MouseEvent("mousedown", n)), e.dispatchEvent(new MouseEvent("mouseup", n)), e.click()
@@ -268,15 +268,15 @@
                     delay: 0
                 }) => (await O(e, {
                     state: "visible"
                 })).type(t, n),
                 click: async e => {
                     await O(e, {
                         state: "attached"
-                    }), _((await O(e, {
+                    }), R((await O(e, {
                         state: "visible"
                     })).element)
                 },
                 focus: async e => {
                     (await O(e, {
                         state: "visible"
                     })).element.focus()
@@ -343,88 +343,88 @@
                             r = i - s,
                             o = Math.min(s + 1.5 * r, t),
                             a = Math.max(i - 1.5 * r, n),
                             l = 200 / 3,
                             c = e => e / t * 750,
                             u = e.times.map((t => x.kernelDensityEstimate(e.times, t))),
                             d = Math.max(...u),
-                            p = Math.round(375),
+                            m = Math.round(375),
                             h = t,
-                            f = Math.ceil((h - 0) / p),
-                            g = Array.from(Array(p), (() => [])),
+                            f = Math.ceil((h - 0) / m),
+                            g = Array.from(Array(m), (() => [])),
                             w = new Array(e.times.length);
                         for (let t = 0; t < e.times.length; t++) {
                             const n = e.times[t],
                                 s = Math.floor(n / f);
                             g[s].push(t), w[t] = s
                         }
                         const y = e.times.map(((e, t) => {
                                 const n = w[t],
                                     s = g[n],
                                     i = (s.indexOf(t) / s.length - .5) * u[t] / d * l;
-                                return m().createElement("g", null, m().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), m().createElement("circle", {
+                                return p().createElement("g", null, p().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), p().createElement("circle", {
                                     cx: c(e),
                                     cy: 100 + i,
                                     r: 2,
                                     className: "point"
                                 }))
                             })),
                             b = [1, 2, 3].map((t => {
                                 const n = x.quartile(e.times, t),
                                     s = c(n),
                                     i = 100 - l / 2;
-                                return m().createElement("g", null, m().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), m().createElement("line", {
+                                return p().createElement("g", null, p().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), p().createElement("line", {
                                     x1: s,
                                     y1: i,
                                     x2: s,
                                     y2: i + l,
                                     className: "box-line"
                                 }))
                             }));
-                        return m().createElement("svg", {
+                        return p().createElement("svg", {
                             viewBox: "0 0 755 200",
                             className: "up-BoxPlot"
-                        }, y, m().createElement("g", null, m().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), m().createElement("line", {
+                        }, y, p().createElement("g", null, p().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), p().createElement("line", {
                             x1: c(a),
                             y1: 100,
                             x2: c(s),
                             y2: 100,
                             className: "whisker"
-                        })), m().createElement("g", null, m().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), m().createElement("line", {
+                        })), p().createElement("g", null, p().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), p().createElement("line", {
                             x1: c(i),
                             y1: 100,
                             x2: c(o),
                             y2: 100,
                             className: "whisker"
-                        })), m().createElement("rect", {
+                        })), p().createElement("rect", {
                             x: c(s),
                             y: 100 - l / 2,
                             width: c(i - s),
                             height: l,
                             className: "box"
-                        }), b, m().createElement("line", {
+                        }), b, p().createElement("line", {
                             x1: "0",
                             x2: 750,
                             y1: 185,
                             y2: 185,
                             className: "timeline"
-                        }), m().createElement("text", {
+                        }), p().createElement("text", {
                             x: "0",
                             y: 200,
                             className: "tickLabel"
-                        }, "0ms"), m().createElement("text", {
+                        }, "0ms"), p().createElement("text", {
                             x: 750,
                             y: 200,
                             style: {
                                 textAnchor: "end"
                             },
                             className: "tickLabel"
                         }, Math.round(t), "ms"))
                     }));
-                    return m().createElement(m().Fragment, null, t)
+                    return p().createElement(p().Fragment, null, t)
                 }
             };
 
             function* q(e) {
                 let t = new Map;
                 for (const n of e.samples) {
                     const s = n.timestamp;
@@ -537,16 +537,16 @@
                             totalTime: Date.now() - a,
                             type: "profile",
                             interrupted: i
                         }
                     },
                     isAvailable: () => void 0 !== window.Profiler,
                     render: function(e) {
-                        const t = m().useRef(null),
-                            [n, s] = m().useState(0);
+                        const t = p().useRef(null),
+                            [n, s] = p().useState(0);
                         if (null === t.current || t.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const t of e.outcome.results)
                                 for (const e of t.traces)
                                     for (const t of L(e)) {
                                         const e = [t.name, t.resource, t.column, t.line].join("-");
                                         if (e in n) n[e].times.push(t.time), n[e].totalTime += t.time, n[e].calls += 1;
@@ -571,82 +571,82 @@
                             0 !== s.length ? t.current = new G({
                                 measurements: s,
                                 stateSource: e.outcome,
                                 sortColumn: "totalTime",
                                 lowerIsBetter: !0
                             }) : t.current = null
                         }
-                        return n > e.outcome.results[0].traces.length ? (s(0), m().createElement(m().Fragment, null)) : m().createElement(m().Fragment, null, m().createElement("select", {
+                        return n > e.outcome.results[0].traces.length ? (s(0), p().createElement(p().Fragment, null)) : p().createElement(p().Fragment, null, p().createElement("select", {
                             value: n,
                             onChange: e => {
                                 s(Number(e.target.value))
                             },
                             className: "up-trace-selector"
-                        }, e.outcome.results[0].traces.map(((e, t) => m().createElement("option", {
+                        }, e.outcome.results[0].traces.map(((e, t) => p().createElement("option", {
                             value: t,
                             key: "trace-" + t
-                        }, "Trace ", t, " (", e.samples.length, " samples)")))), m().createElement(Y, {
+                        }, "Trace ", t, " (", e.samples.length, " samples)")))), p().createElement(Y, {
                             trace: e.outcome.results[0].traces[n],
                             itemHeight: 20
-                        }), t.current ? m().createElement(K, {
+                        }), t.current ? p().createElement(K, {
                             widget: t.current
                         }) : "No results available. Reduce sampling interval, use macro mode, and/or increase the number of repeats.")
                     }
                 },
                 W = e => {
                     const t = e.load("jupyterlab"),
-                        n = e => m().createElement("div", {
+                        n = e => p().createElement("div", {
                             className: e.className
-                        }, m().createElement(e.TitleField, {
+                        }, p().createElement(e.TitleField, {
                             title: e.title,
                             required: e.required,
                             id: `${e.idSchema.$id}-title`
-                        }), m().createElement(e.DescriptionField, {
+                        }), p().createElement(e.DescriptionField, {
                             id: `${e.idSchema.$id}-description`,
                             description: e.schema.description ?? ""
-                        }), e.items.map((e => m().createElement("div", {
+                        }), e.items.map((e => p().createElement("div", {
                             key: e.key,
                             className: e.className
-                        }, e.children, m().createElement("div", {
+                        }, e.children, p().createElement("div", {
                             className: "jp-ArrayOperations"
-                        }, m().createElement("button", {
+                        }, p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index - 1),
                             disabled: !e.hasMoveUp
-                        }, t.__("Move Up")), m().createElement("button", {
+                        }, t.__("Move Up")), p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index + 1),
                             disabled: !e.hasMoveDown
-                        }, t.__("Move Down")), m().createElement("button", {
+                        }, t.__("Move Down")), p().createElement("button", {
                             className: "jp-mod-styled jp-mod-warn",
                             onClick: e.onDropIndexClick(e.index),
                             disabled: !e.hasRemove
-                        }, t.__("Remove")))))), e.canAdd && m().createElement("button", {
+                        }, t.__("Remove")))))), e.canAdd && p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onAddClick
                         }, t.__("Add")));
                     return n.displayName = "JupyterLabArrayTemplate", n
                 },
                 z = e => {
                     const t = e.load("jupyterlab"),
                         n = e => {
                             const {
                                 TitleField: n,
                                 DescriptionField: s
                             } = e;
-                            return m().createElement("fieldset", {
+                            return p().createElement("fieldset", {
                                 id: e.idSchema.$id
-                            }, (e.uiSchema["ui:title"] || e.title) && m().createElement(n, {
+                            }, (e.uiSchema["ui:title"] || e.title) && p().createElement(n, {
                                 id: `${e.idSchema.$id}__title`,
                                 title: e.title || e.uiSchema["ui:title"],
                                 required: e.required
-                            }), e.description && m().createElement(s, {
+                            }), e.description && p().createElement(s, {
                                 id: `${e.idSchema.$id}__description`,
                                 description: e.description
-                            }), e.properties.map((e => e.content)), d.P6.canExpand(e.schema, e.uiSchema, e.formData) && m().createElement("button", {
+                            }), e.properties.map((e => e.content)), u.P6.canExpand(e.schema, e.uiSchema, e.formData) && p().createElement("button", {
                                 className: "jp-mod-styled jp-mod-reject",
                                 onClick: e.onAddClick(e.schema),
                                 disabled: e.disabled || e.readonly
                             }, t.__("Add")))
                         };
                     return n.displayName = "JupyterLabObjectTemplate", n
                 },
@@ -658,41 +658,41 @@
                                 label: s,
                                 displayLabel: i,
                                 id: r,
                                 errors: o,
                                 rawErrors: a,
                                 children: l,
                                 onKeyChange: c,
-                                onDropPropertyClick: u
-                            } = e, p = r.split("_");
-                            p.shift();
-                            const h = "" === p.join("."),
+                                onDropPropertyClick: d
+                            } = e, m = r.split("_");
+                            m.shift();
+                            const h = "" === m.join("."),
                                 f = !h && "object" !== n.type,
-                                g = Object.prototype.hasOwnProperty.call(n, d.P6.ADDITIONAL_PROPERTY_FLAG);
-                            return m().createElement("div", {
+                                g = Object.prototype.hasOwnProperty.call(n, u.P6.ADDITIONAL_PROPERTY_FLAG);
+                            return p().createElement("div", {
                                 className: "form-group " + (i || "boolean" === n.type ? "small-field" : "")
-                            }, a && m().createElement("div", {
+                            }, a && p().createElement("div", {
                                 className: "jp-modifiedIndicator jp-errorIndicator"
-                            }), m().createElement("div", {
+                            }), p().createElement("div", {
                                 className: "jp-FormGroup-content"
-                            }, i && !h && s && !g && m().createElement("h3", {
+                            }, i && !h && s && !g && p().createElement("h3", {
                                 className: "jp-FormGroup-fieldLabel jp-FormGroup-contentItem"
-                            }, s), g && m().createElement("input", {
+                            }, s), g && p().createElement("input", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled",
                                 type: "text",
                                 onBlur: e => c(e.target.value),
                                 defaultValue: s
-                            }), m().createElement("div", {
+                            }), p().createElement("div", {
                                 className: h ? "jp-root" : "object" === n.type ? "jp-objectFieldWrapper" : "jp-inputFieldWrapper jp-FormGroup-contentItem"
-                            }, l), g && m().createElement("button", {
+                            }, l), g && p().createElement("button", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled jp-mod-warn jp-FormGroup-removeButton",
-                                onClick: u(s)
-                            }, t.__("Remove")), n.description && f && m().createElement("div", {
+                                onClick: d(s)
+                            }, t.__("Remove")), n.description && f && p().createElement("div", {
                                 className: "jp-FormGroup-description"
-                            }, n.description), m().createElement("div", {
+                            }, n.description), p().createElement("div", {
                                 className: "validationErrors"
                             }, o)))
                         };
                     return n.displayName = "JupyterLabFieldTemplate", n
                 };
             var U = n(5414);
             class J extends U.BasicMouseHandler {
@@ -826,43 +826,43 @@
                         const t = this.dataModel.data(e.region, e.row, e.column);
                         t === this.sortColumn ? this.sortOrder = "ascending" === this.sortOrder ? "descending" : "ascending" : this.sortColumn = t, this._setupDataModel(!0), this.update()
                     }
                 }
             }
             var V = n(8832);
             const K = e => {
-                const t = m().useRef(null);
-                return m().useEffect((() => {
+                const t = p().useRef(null);
+                return p().useEffect((() => {
                     const n = e.widget;
                     V.Widget.attach(n, t.current);
                     const s = new ResizeObserver((t => {
                         e.widget.fit()
                     }));
                     return s.observe(t.current), () => {
                         V.Widget.detach(n), s.disconnect()
                     }
-                }), [e.widget]), m().createElement("div", {
+                }), [e.widget]), p().createElement("div", {
                     className: "up-LuminoWidgetWrapper",
                     ref: t
                 })
             };
-            class Y extends m().Component {
+            class Y extends p().Component {
                 constructor(e) {
                     super(e), this.deepest = 0, this.contentWidth = 100, this.contentHeight = 100, this.initialWidth = 100, this.state = {
                         scale: {
                             x: 1,
                             y: 1
                         },
                         position: {
                             x: 0,
                             y: 0
                         },
                         dimensions: null,
                         inDrag: !1
-                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = m().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
+                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = p().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
                 }
                 componentDidMount() {
                     const e = this.props.trace,
                         t = e.samples[0].timestamp,
                         n = Math.max(...e.samples.map((e => e.timestamp - t))),
                         s = {
                             width: this.container.current.offsetWidth,
@@ -920,25 +920,25 @@
                     }), document.addEventListener("mousemove", this.handleMouseMove), document.addEventListener("mouseup", this.handleMouseUp)
                 }
                 renderContent() {
                     const {
                         trace: e,
                         itemHeight: t
                     } = this.props;
-                    if (!e.samples) return m().createElement("div", null, "No samples in trace");
+                    if (!e.samples) return p().createElement("div", null, "No samples in trace");
                     const n = e.samples[0].timestamp,
                         s = [...q(e)];
                     this.deepest = Math.max(...s.map((e => e.stackDepth)));
                     const i = this.state.scale,
                         r = e.samples.map(((t, s) => {
                             const r = {
                                 width: (e.samples[s + 1]?.timestamp - t.timestamp) * i.x,
                                 left: (t.timestamp - n) * i.x
                             };
-                            return m().createElement("div", {
+                            return p().createElement("div", {
                                 className: "up-ProfileTrace-sample",
                                 key: "sample-" + s,
                                 style: r
                             })
                         }));
                     let o = 0;
                     const a = s.map(((s, r) => {
@@ -948,94 +948,97 @@
                         o = Math.max(o, l + c);
                         const u = {
                             width: c,
                             top: (s.stackDepth - 1) * t * i.y,
                             left: l,
                             height: t
                         };
-                        return m().createElement("div", {
+                        return p().createElement("div", {
                             className: "up-ProfileTrace-frame " + (void 0 === a.resourceId ? "up-ProfileTrace-frame-native" : ""),
                             key: "frame-" + r,
                             style: u,
                             title: [a.name, x.round(s.duration, 1) + "ms"].join("\n")
                         }, a.name)
                     }));
-                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, m().createElement("div", {
+                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, p().createElement("div", {
                         className: "up-ProfileTrace-content",
                         style: {
                             transform: `translate(${this.state.position.x}px, ${this.state.position.y}px)`,
                             width: o + "px",
                             height: this.contentHeight + "px"
                         }
                     }, a, r)
                 }
                 render() {
-                    return m().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-ProfileTrace",
                         onWheel: this.handleWheel,
                         onMouseDown: this.handleMouseDown,
                         ref: this.container
                     }, this.state.dimensions ? this.renderContent() : "Loading")
                 }
             }
 
             function X(e) {
                 const t = e % 10;
                 return t > 3 || e % 100 > 3 || 0 === t ? e + "th" : e + ["st", "nd", "rd"][t - 1]
             }
             class Z extends i.ReactWidget {
                 constructor(e) {
-                    super(), this.props = e, this.result = null, this.progress = new w.Signal(this), this.handleResult = this.handleResult.bind(this), this.loadResult = this.loadResult.bind(this), this.upload = this.upload.bind(this), this.manager = new h.ServiceManager, this.resultAdded = new w.Signal(this), this.ensureResultsDirectory()
+                    super(), this.props = e, this.result = null, this.progress = new w.Signal(this), this.handleResult = this.handleResult.bind(this), this.loadResult = this.loadResult.bind(this), this.upload = this.upload.bind(this), this.manager = new m.ServiceManager, this.resultAdded = new w.Signal(this), this.ensureResultsDirectory(), this.props.profiler.progress.connect(((e, t) => {
+                        this.progress.emit(t)
+                    })), this.props.profiler.scenarioAdded.connect((() => {
+                        this.update()
+                    }))
                 }
                 async ensureResultsDirectory() {
                     return this.manager.contents.save(this.props.resultLocation, {
                         type: "directory"
                     }).catch((e => {
                         (0, i.showErrorMessage)("filesystem error", "ui-profiler could not create results directory; see console for details"), console.error("directory creation failure reason:", e)
                     }))
                 }
                 handleResult(e) {
                     this.result = e, this.update(), this.resultAdded.emit(e)
                 }
                 async loadResult(e) {
-                    e = await this.manager.contents.get(e.path), this.handleResult(JSON.parse(e.content))
-                }
-                addScenario(e) {
-                    this.props.scenarios.push(e), this.update()
+                    e = await this.manager.contents.get(e.path);
+                    const t = JSON.parse(e.content);
+                    t.result && (t.outcome = t.result), this.handleResult(t)
                 }
                 async upload(e) {
                     return await this.ensureResultsDirectory(), this.props.upload(e)
                 }
                 render() {
-                    return m().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-UIProfiler"
-                    }, m().createElement(oe, Object.assign({
+                    }, p().createElement(re, Object.assign({
                         onResult: this.handleResult,
                         progress: this.progress
                     }, this.props, {
                         upload: this.upload
-                    })), m().createElement(ee, Object.assign({
+                    })), p().createElement(ee, Object.assign({
                         resultAdded: this.resultAdded,
                         manager: this.manager,
                         onSelect: this.loadResult
-                    }, this.props)), m().createElement(te, {
+                    }, this.props)), p().createElement(te, {
                         result: this.result,
-                        scenarios: this.props.scenarios,
-                        benchmarks: this.props.benchmarks.filter((e => e.id === this.result?.benchmark))
+                        scenarios: this.props.profiler.scenarios,
+                        benchmarks: this.props.profiler.benchmarks.filter((e => e.id === this.result?.benchmark))
                     }))
                 }
             }
-            class ee extends m().Component {
+            class ee extends p().Component {
                 constructor(e) {
                     super(e), this._handle = null, this.state = {
                         files: [],
                         current: null
                     }, this.update(), this.update = this.update.bind(this), this.props.resultAdded.connect((async (e, t) => {
                         await this.update(), this.setState({
-                            current: ie(t)
+                            current: se(t)
                         })
                     }))
                 }
                 async update() {
                     const e = (await this.props.manager.contents.get(this.props.resultLocation)).content.filter((e => e.path.endsWith(".profile.json")));
                     e.sort(((e, t) => new Date(t.created).getTime() - new Date(e.created).getTime())), this.setState({
                         files: e
@@ -1044,112 +1047,112 @@
                 componentDidMount() {
                     this._handle = window.setInterval(this.update, 2e3)
                 }
                 componentWillUnmount() {
                     null !== this._handle && window.clearInterval(this._handle)
                 }
                 render() {
-                    let e = this.state.files.map((e => m().createElement("li", {
+                    let e = this.state.files.map((e => p().createElement("li", {
                         className: this.state.current === e.name ? "up-BenchmarkHistory-file up-BenchmarkHistory-file-active" : "up-BenchmarkHistory-file",
                         key: e.name,
                         onClick: () => {
                             this.props.onSelect(e), this.setState({
                                 current: e.path
                             })
                         }
                     }, e.name.replace(".profile.json", ""))));
-                    return this.state.files.length || (e = [m().createElement("li", {
+                    return this.state.files.length || (e = [p().createElement("li", {
                         className: "up-BenchmarkHistory-entry"
-                    }, "(No previous results found)")]), m().createElement("div", {
+                    }, "(No previous results found)")]), p().createElement("div", {
                         className: "up-BenchmarkHistory"
-                    }, m().createElement("h3", {
+                    }, p().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "History"), m().createElement("ul", {
+                    }, "History"), p().createElement("ul", {
                         className: "up-BenchmarkHistory-files"
                     }, e))
                 }
             }
-            class te extends m().Component {
+            class te extends p().Component {
                 constructor() {
                     super(...arguments), this._table = null, this._previousResult = null
                 }
                 render() {
                     const {
                         result: e,
                         benchmarks: t,
                         scenarios: n
-                    } = this.props, s = e => m().createElement("div", {
+                    } = this.props, s = e => p().createElement("div", {
                         className: "up-BenchmarkResult"
                     }, e);
-                    if (!e) return s(m().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
+                    if (!e) return s(p().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
                     const i = n.find((t => t.id === e.scenario)),
                         r = t.find((t => t.id === e.benchmark));
-                    if (!i) return s(m().createElement("div", null, "Unknown scenario: ", e.scenario));
-                    if (!r) return s(m().createElement("div", null, "Unknown benchmark: ", e.benchmark));
-                    r.render || this._previousResult === e.id || ("time" === e.result.type ? this._table = new G({
-                        measurements: e.result.results,
-                        reference: e.result.reference,
+                    if (!i) return s(p().createElement("div", null, "Unknown scenario: ", e.scenario));
+                    if (!r) return s(p().createElement("div", null, "Unknown benchmark: ", e.benchmark));
+                    r.render || this._previousResult === e.id || ("time" === e.outcome.type ? this._table = new G({
+                        measurements: e.outcome.results,
+                        reference: e.outcome.reference,
                         sortColumn: r.sortColumn,
                         stateSource: null,
                         lowerIsBetter: !1
                     }) : this._table = null);
-                    const o = [...Object.entries(e.result.tags)].map((([e, t]) => `${e}:  ${t}`)).join("\n"),
-                        a = x.sum([...Object.values(e.result.tags)]);
-                    return s(m().createElement(m().Fragment, null, m().createElement("div", {
+                    const o = [...Object.entries(e.outcome.tags)].map((([e, t]) => `${e}:  ${t}`)).join("\n"),
+                        a = x.sum([...Object.values(e.outcome.tags)]);
+                    return s(p().createElement(p().Fragment, null, p().createElement("div", {
                         className: "up-BenchmarkResult-summary"
-                    }, m().createElement("div", {
+                    }, p().createElement("div", {
                         className: "up-BenchmarkResult-benchmarkInfo"
-                    }, m().createElement("div", null, r.name, " ", i.name), "time" === e.result.type ? (l = e.result, m().createElement(m().Fragment, null, m().createElement("div", {
+                    }, p().createElement("div", null, r.name, " ", i.name), "time" === e.outcome.type ? (l = e.outcome, p().createElement(p().Fragment, null, p().createElement("div", {
                         title: [...l.reference].sort().map(x.round).join(" ms\n") + " ms"
-                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), m().createElement("div", null, "Total time: ", v(l.totalTime)))) : function(e) {
+                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), p().createElement("div", null, "Total time: ", k(l.totalTime)))) : function(e) {
                         const t = e.results[0];
-                        return m().createElement(m().Fragment, null, m().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", m().createElement("span", {
+                        return p().createElement(p().Fragment, null, p().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", p().createElement("span", {
                             title: "Average recorderd: " + x.round(t.averageSampleInterval, 1)
-                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), m().createElement("div", null, "Total time: ", v(e.totalTime)))
-                    }(e.result)), m().createElement("div", {
+                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), p().createElement("div", null, "Total time: ", k(e.totalTime)))
+                    }(e.outcome)), p().createElement("div", {
                         className: "up-BenchmarkResult-environmentInfo"
-                    }, m().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), m().createElement("div", null, m().createElement("span", {
+                    }, p().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), p().createElement("div", null, p().createElement("span", {
                         title: e.userAgent
                     }, "Browser: ", function(e) {
                         const t = [/Firefox\/\d+/, /OPR\/\d+/, /Edg\/\d+/, /Mobile\/.* Safari\/\d+/, /Chrome\/\d+/];
                         for (const n of t) {
                             const t = e.match(n);
                             if (t) return t[0]
                         }
                         return "Unknown browser"
-                    }(e.userAgent)), ", ", m().createElement("span", {
+                    }(e.userAgent)), ", ", p().createElement("span", {
                         title: o
-                    }, "DOM Elements: ", a)), m().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), m().createElement("div", {
+                    }, "DOM Elements: ", a)), p().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), p().createElement("div", {
                         className: "up-BenchmarkResult-options"
-                    }, m().createElement("details", null, m().createElement("summary", null, "Options"), m().createElement("div", {
+                    }, p().createElement("details", null, p().createElement("summary", null, "Options"), p().createElement("div", {
                         className: "up-BenchmarkResult-options-benchmark"
-                    }, m().createElement("b", null, "Benchmark"), m().createElement(y.w, {
+                    }, p().createElement("b", null, "Benchmark"), p().createElement(y.w, {
                         data: e.options.benchmark
-                    })), m().createElement("div", {
+                    })), p().createElement("div", {
                         className: "up-BenchmarkResult-options-scenario"
-                    }, m().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? m().createElement("div", null, "No options") : m().createElement(y.w, {
+                    }, p().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? p().createElement("div", null, "No options") : p().createElement(y.w, {
                         data: e.options.scenario
-                    })))), m().createElement("div", {
+                    })))), p().createElement("div", {
                         className: "up-BenchmarkResult-details"
-                    }, r.interpretation ? m().createElement("details", null, m().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? m().createElement(r.render, {
-                        outcome: e.result
-                    }) : this._table ? m().createElement(K, {
+                    }, r.interpretation ? p().createElement("details", null, p().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? p().createElement(r.render, {
+                        outcome: e.outcome
+                    }) : this._table ? p().createElement(K, {
                         widget: this._table
                     }) : null)));
                     var l
                 }
             }
-            class ne extends m().Component {
+            class ne extends p().Component {
                 constructor() {
                     super(...arguments), this.start = null, this.end = null
                 }
                 render() {
-                    return m().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-BenchmarkMonitor"
-                    }, m().createElement(i.UseSignal, {
+                    }, p().createElement(i.UseSignal, {
                         signal: this.props.progress,
                         initialArgs: {
                             percentage: -1
                         }
                     }, ((e, t) => {
                         t || (t = {
                             percentage: -1
@@ -1157,125 +1160,104 @@
                         let n = NaN,
                             s = NaN,
                             i = "up-mod-waiting";
                         if (t.interrupted && (i = "up-mod-interrupted"), t.errored && (i += " up-mod-errored"), this.start) {
                             const e = (100 === t.percentage || t.interrupted || t.errored) && this.end ? this.end : new Date;
                             this.end = e, n = e.getTime() - this.start.getTime(), t.interrupted || t.errored || (s = (100 - t.percentage) * n / t.percentage, i = 100 === t.percentage ? "up-mod-completed" : "")
                         }
-                        return m().createElement("div", {
+                        return p().createElement("div", {
                             className: i + " up-BenchmarkMonitor-content"
-                        }, m().createElement("div", null, "Elapsed: ", v(n), ". Remaining:", " ", v(s)), m().createElement(f.ProgressBar, {
+                        }, p().createElement("div", null, "Elapsed: ", k(n), ". Remaining:", " ", k(s)), p().createElement(h.ProgressBar, {
                             percentage: t.percentage
                         }))
                     })))
                 }
             }
 
             function se(e) {
-                return [e.benchmark, e.scenario, e.completed.toISOString()].join("_")
-            }
-
-            function ie(e) {
                 return e.id + ".profile.json"
             }
 
-            function re(e) {
-                return m().createElement("div", {
+            function ie(e) {
+                return p().createElement("div", {
                     className: "rjsf"
-                }, m().createElement("div", {
+                }, p().createElement("div", {
                     className: "jp-root"
-                }, m().createElement("fieldset", null, m().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
+                }, p().createElement("fieldset", null, p().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
             }
-            class oe extends m().Component {
+            class re extends p().Component {
                 constructor(e) {
                     super(e), this._config = {
                         scenarios: {},
                         benchmarks: {}
-                    }, this._stop = new w.Signal(this), this.state = {
-                        benchmarks: 0 !== e.benchmarks.length ? [e.benchmarks[0]] : [],
-                        scenarios: 0 !== e.scenarios.length ? [e.scenarios[0]] : [],
+                    }, this._stop = new w.Signal(this);
+                    const {
+                        profiler: t
+                    } = e;
+                    this.state = {
+                        benchmarks: 0 !== t.benchmarks.length ? [t.benchmarks[0]] : [],
+                        scenarios: 0 !== t.scenarios.length ? [t.scenarios[0]] : [],
                         fieldTemplate: H(this.props.translator),
                         arrayFieldTemplate: W(this.props.translator),
                         objectFieldTemplate: z(this.props.translator),
                         isRunning: !1
                     }, this.runSelected = this.runSelected.bind(this), this.stopCurrent = this.stopCurrent.bind(this)
                 }
                 async runBenchmark(e, t, n) {
-                    const s = g.JSONExt.deepCopy({
-                        scenario: n.scenarios[e.id],
-                        benchmark: n.benchmarks[t.id]
-                    });
-                    e.setOptions && e.setOptions(s.scenario), this.props.progress.emit({
-                        percentage: 0
-                    });
-                    const i = await t.run(e, s.benchmark, this.props.progress, this._stop);
-                    i.interrupted ? this.props.progress.emit({
-                        percentage: NaN,
-                        interrupted: !0
-                    }) : this.props.progress.emit({
-                        percentage: 100
-                    });
-                    const r = {
-                        result: i,
-                        options: s,
-                        benchmark: t.id,
-                        scenario: e.id,
-                        userAgent: window.navigator.userAgent,
-                        hardwareConcurrency: window.navigator.hardwareConcurrency,
-                        completed: new Date,
-                        windowSize: {
-                            width: window.innerWidth,
-                            height: window.innerHeight
-                        },
-                        jupyter: this.props.getJupyterState()
-                    };
-                    return {
-                        ...r,
-                        id: se(r)
-                    }
+                    return this.props.profiler.runBenchmark({
+                        id: e.id,
+                        options: f.JSONExt.deepCopy(n.scenarios[e.id])
+                    }, {
+                        id: t.id,
+                        options: f.JSONExt.deepCopy(n.benchmarks[t.id])
+                    })
                 }
                 onBenchmarkChanged(e) {
-                    const t = this.props.benchmarks.find((t => t.id === e.target.value));
-                    if (!t) throw Error(`Benchmark not matched ${e.target.value}`);
-                    let n = [...this.state.benchmarks];
-                    e.target.checked ? n.push(t) : n = n.filter((e => e.id !== t.id));
-                    const s = this.props.benchmarks.map((e => e.id));
-                    n.sort(((e, t) => s.indexOf(e.id) - s.indexOf(t.id))), this.setState({
-                        benchmarks: n
+                    const {
+                        profiler: t
+                    } = this.props, n = t.benchmarks.find((t => t.id === e.target.value));
+                    if (!n) throw Error(`Benchmark not matched ${e.target.value}`);
+                    let s = [...this.state.benchmarks];
+                    e.target.checked ? s.push(n) : s = s.filter((e => e.id !== n.id));
+                    const i = t.benchmarks.map((e => e.id));
+                    s.sort(((e, t) => i.indexOf(e.id) - i.indexOf(t.id))), this.setState({
+                        benchmarks: s
                     })
                 }
                 onScenarioChanged(e) {
-                    const t = this.props.scenarios.find((t => t.id === e.target.value));
-                    if (!t) throw Error(`Scenario not matched ${e.target.value}`);
-                    let n = [...this.state.scenarios];
-                    e.target.checked ? n.push(t) : n = n.filter((e => e.id !== t.id));
-                    const s = this.props.scenarios.map((e => e.id));
-                    n.sort(((e, t) => s.indexOf(e.id) - s.indexOf(t.id))), this.setState({
-                        scenarios: n
+                    const {
+                        profiler: t
+                    } = this.props, n = t.scenarios.find((t => t.id === e.target.value));
+                    if (!n) throw Error(`Scenario not matched ${e.target.value}`);
+                    let s = [...this.state.scenarios];
+                    e.target.checked ? s.push(n) : s = s.filter((e => e.id !== n.id));
+                    const i = t.scenarios.map((e => e.id));
+                    s.sort(((e, t) => i.indexOf(e.id) - i.indexOf(t.id))), this.setState({
+                        scenarios: s
                     })
                 }
                 async runSelected() {
                     this.setState({
                         isRunning: !0
                     });
                     let e = !1;
                     const t = () => {
                         e = !0
                     };
                     this._stop.connect(t);
                     try {
                         const t = [...this.state.benchmarks],
                             n = [...this.state.scenarios],
-                            s = g.JSONExt.deepCopy(this._config);
+                            s = f.JSONExt.deepCopy(this._config);
                         for (const i of t)
                             for (const t of n) {
                                 if (e) break;
                                 const n = await this.runBenchmark(t, i, s),
-                                    o = ie(n);
-                                await this.props.upload(new File(JSON.stringify(n).split("\n"), r.PathExt.join(this.props.resultLocation, o), {
+                                    r = se(n);
+                                await this.props.upload(new File(JSON.stringify(n).split("\n"), g.PathExt.join(this.props.resultLocation, r), {
                                     type: "application/json"
                                 })), this.props.onResult(n)
                             }
                     } catch (t) {
                         e ? this.props.progress.emit({
                             percentage: NaN,
                             interrupted: !0
@@ -1285,134 +1267,135 @@
                         }), (0, i.showErrorMessage)("Benchmark failed", t))
                     }
                     this._stop.disconnect(t), this.setState({
                         isRunning: !1
                     })
                 }
                 stopCurrent() {
-                    this._stop.emit()
+                    this._stop.emit(), this.props.profiler.abortBenchmark()
                 }
                 render() {
-                    const e = this.props.benchmarks.map((e => {
-                            const t = !!e.isAvailable && !e.isAvailable();
-                            return m().createElement("label", {
-                                key: e.id,
-                                className: t ? "up-label-disabled" : "",
-                                title: t ? "This benchmark is not available on this browser" : ""
-                            }, m().createElement("input", {
-                                type: "checkbox",
-                                defaultChecked: this.state.benchmarks.includes(e),
-                                className: "up-BenchmarkLauncher-choice-input",
-                                disabled: t,
-                                value: e.id
-                            }), e.name)
-                        })),
-                        t = this.props.scenarios.map((e => m().createElement("label", {
-                            key: e.id
-                        }, m().createElement("input", {
+                    const {
+                        profiler: e
+                    } = this.props, t = e.benchmarks.map((e => {
+                        const t = !!e.isAvailable && !e.isAvailable();
+                        return p().createElement("label", {
+                            key: e.id,
+                            className: t ? "up-label-disabled" : "",
+                            title: t ? "This benchmark is not available on this browser" : ""
+                        }, p().createElement("input", {
                             type: "checkbox",
-                            defaultChecked: this.state.scenarios.includes(e),
+                            defaultChecked: this.state.benchmarks.includes(e),
                             className: "up-BenchmarkLauncher-choice-input",
+                            disabled: t,
                             value: e.id
-                        }), e.name)));
-                    return m().createElement("div", {
+                        }), e.name)
+                    })), n = e.scenarios.map((e => p().createElement("label", {
+                        key: e.id
+                    }, p().createElement("input", {
+                        type: "checkbox",
+                        defaultChecked: this.state.scenarios.includes(e),
+                        className: "up-BenchmarkLauncher-choice-input",
+                        value: e.id
+                    }), e.name)));
+                    return p().createElement("div", {
                         className: "up-BenchmarkLauncher",
                         style: {
                             height: "450px"
                         }
-                    }, m().createElement("h3", {
+                    }, p().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "Launch"), m().createElement("div", {
+                    }, "Launch"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-cards"
-                    }, m().createElement("div", {
+                    }, p().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, m().createElement("h4", {
+                    }, p().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Benchmark"), m().createElement("div", {
+                    }, "Benchmark"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onBenchmarkChanged.bind(this)
-                    }, e), m().createElement("div", {
+                    }, t), p().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.benchmarks.map((e => {
                         const t = e.configSchema.properties;
-                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", m().createElement(d.ZP, {
+                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
                             key: "up-profiler-benchmark-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-benchmark",
                             onChange: t => {
                                 this._config.benchmarks[e.id] = t.formData
                             },
                             formData: this._config.benchmarks[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : m().createElement(re, {
+                        })) : p().createElement(ie, {
                             name: e.name
                         })
-                    })))), m().createElement("div", {
+                    })))), p().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, m().createElement("h4", {
+                    }, p().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Scenario"), m().createElement("div", {
+                    }, "Scenario"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onScenarioChanged.bind(this)
-                    }, t), m().createElement("div", {
+                    }, n), p().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.scenarios.map((e => {
                         const t = e.configSchema?.properties;
-                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", m().createElement(d.ZP, {
+                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
                             key: "up-profiler-scenario-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-scenario-" + e.id,
                             onChange: t => {
                                 this._config.scenarios[e.id] = t.formData
                             },
                             formData: this._config.scenarios[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : m().createElement(re, {
+                        })) : p().createElement(ie, {
                             name: e.name
                         })
-                    }))))), m().createElement("div", {
+                    }))))), p().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar"
-                    }, m().createElement(ne, Object.assign({}, this.props)), m().createElement("div", {
+                    }, p().createElement(ne, Object.assign({}, this.props)), p().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar-buttons"
-                    }, m().createElement("button", {
+                    }, p().createElement("button", {
                         onClick: this.runSelected,
                         className: "jp-mod-styled jp-mod-accept" + (this.state.isRunning ? " jp-mod-hidden" : ""),
                         disabled: 0 === this.state.scenarios.length || 0 === this.state.benchmarks.length || this.state.isRunning
-                    }, "Start"), m().createElement("button", {
+                    }, "Start"), p().createElement("button", {
                         onClick: this.stopCurrent,
                         className: "jp-mod-styled jp-mod-warn" + (this.state.isRunning ? "" : " jp-mod-hidden"),
                         disabled: !this.state.isRunning
                     }, "Stop"))))
                 }
             }
-            async function ae(e) {
+            async function oe(e) {
                 if (!e) return null;
                 const t = e.matchAll(new RegExp("# sourceMappingURL=(.*)\\s*\\*/", "g"));
                 if (!t) return null;
                 let n = "";
                 for (const e of t) {
                     const t = e[1].split("data:application/json;base64,");
                     if (t.length > 1) return JSON.parse(atob(t[1]));
                     n = e[1]
                 }
                 return "" === n ? null : (await fetch(n)).json()
             }
-            async function le(e, t) {
+            async function ae(e, t) {
                 let n = 0;
                 const s = [];
                 for (const i of e) {
                     const e = i.sheet;
                     if (!e) continue;
-                    const r = await ae(i.textContent),
+                    const r = await oe(i.textContent),
                         o = r ? r.sources[0] : null;
                     n++;
                     const a = e.rules;
                     for (let i = 0; i < a.length; i++) {
                         const r = a[i];
                         r instanceof CSSStyleRule && (t.skipPattern && null != r.selectorText.match(t.skipPattern) || s.push({
                             rule: r,
@@ -1422,34 +1405,34 @@
                             ruleIndex: i,
                             stylesheetIndex: n
                         }))
                     }
                 }
                 return s
             }
-            const ce = JSON.parse('{"title":"Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5}}}'),
-                ue = JSON.parse('{"title":"Style Rule Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":3},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"}}}'),
-                de = JSON.parse('{"title":"Style Rule Group Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"minBlocks":{"title":"Block size to start with","type":"integer","minimum":1,"default":3},"maxBlocks":{"title":"Maximal block size","type":"integer","minimum":1,"default":5},"sheetRandomizations":{"title":"Number of sheet randomizations","type":"integer","minimum":0,"default":5}}}'),
-                pe = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"}}}');
-            class me extends Map {
+            const le = JSON.parse('{"title":"Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5}}}'),
+                ce = JSON.parse('{"title":"Style Rule Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":3},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"}}}'),
+                ue = JSON.parse('{"title":"Style Rule Group Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"minBlocks":{"title":"Block size to start with","type":"integer","minimum":1,"default":3},"maxBlocks":{"title":"Maximal block size","type":"integer","minimum":1,"default":5},"sheetRandomizations":{"title":"Number of sheet randomizations","type":"integer","minimum":0,"default":5}}}'),
+                de = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"}}}');
+            class pe extends Map {
                 add(e, t) {
                     let n = this.get(e);
                     n || (n = new Set, this.set(e, n)), n.add(t)
                 }
                 countRulesUsage() {
                     const e = new Map;
                     for (const t of this.values())
                         for (const n of t.values()) e.set(n, (e.get(n) || 0) + 1);
                     return e
                 }
             }
-            const he = {
+            const me = {
                     id: "rule-usage",
                     name: "Style Rule Usage",
-                    configSchema: pe,
+                    configSchema: de,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
@@ -1472,20 +1455,20 @@
                         await M(), h.observe(document.body, d), await D(e, o, !0), await M(), m(h.takeRecords()), h.disconnect();
                         const f = [...p].filter((e => e instanceof Element)).filter((e => "body" !== e.tagName.toLocaleLowerCase()));
                         console.log("Relevant nodes:", p);
                         const g = new Set([...f.map((e => [...e.classList.values()])).flat().filter((e => !c || !e.match(c)))]),
                             w = f.filter((e => e.id)).map((e => e.id));
                         console.log("Relevant class names:", g), console.log("Relevant IDs:", w);
                         const y = [],
-                            v = [...document.querySelectorAll("style")],
-                            k = await le(v, {
+                            k = [...document.querySelectorAll("style")],
+                            v = await ae(k, {
                                 skipPattern: l
                             }),
                             E = new Set;
-                        for (const e of k) {
+                        for (const e of v) {
                             for (const t of g)
                                 if (e.selector.includes("." + t)) {
                                     E.add(e);
                                     break
                                 } for (const t of w)
                                 if (e.selector.includes("#" + t)) {
                                     E.add(e);
@@ -1493,63 +1476,63 @@
                                 }
                         }
                         const x = [...E];
                         n?.emit({
                             percentage: 50 / x.length
                         });
                         const j = new Map,
-                            N = new me,
-                            C = new me,
+                            N = new pe,
+                            C = new pe,
                             O = e => {
                                 const t = new Set;
                                 for (const n of S(e)) t.add(n);
                                 for (const e of t)
                                     if (e instanceof Element)
                                         for (const t of E) e.matches(t.selector) && (j.set(t.selector, (j.get(t.selector) || 0) + 1), C.add(e, t.selector));
                                 for (const e of E)
                                     for (const t of document.querySelectorAll(e.selector)) N.add(t, e.selector)
                             },
                             I = new MutationObserver(O);
                         I.observe(document.body, d), await D(e, o, !0), await M(), O(I.takeRecords()), I.disconnect();
-                        const T = C.countRulesUsage(),
-                            R = N.countRulesUsage();
+                        const _ = C.countRulesUsage(),
+                            T = N.countRulesUsage();
                         for (let t = 0; t < x.length && !i; t++) {
                             n?.emit({
                                 percentage: 100 * (t + .5) / x.length
                             });
                             const s = x[t];
                             s.sheet.deleteRule(s.ruleIndex), await M();
                             const i = await D(e, o, !0);
                             y.push({
                                 ...i,
                                 selector: s.selector,
                                 source: s.source,
                                 ruleIndex: s.ruleIndex,
                                 stylesheetIndex: s.stylesheetIndex,
                                 touchCount: j.get(s.selector) || 0,
-                                elementsTouched: T.get(s.selector) || 0,
-                                elementsSeen: R.get(s.selector) || 0
+                                elementsTouched: _.get(s.selector) || 0,
+                                elementsSeen: T.get(s.selector) || 0
                             }), s.sheet.insertRule(s.rule.cssText, s.ruleIndex), await M()
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
                             results: y,
                             reference: u.times,
                             tags: b(),
                             totalTime: Date.now() - a,
                             type: "time",
                             interrupted: i
                         }
                     },
                     sortColumn: "elementsSeen",
-                    interpretation: m().createElement(m().Fragment, null, m().createElement("ul", null, m().createElement("li", null, m().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), m().createElement("li", null, m().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), m().createElement("li", null, m().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), m().createElement("div", null, "Low number of ", m().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", m().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), p().createElement("div", null, "Low number of ", p().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
-                fe = {
+                he = {
                     id: "style-sheet",
                     name: "Style Sheets",
-                    configSchema: ce,
+                    configSchema: le,
                     run: async (e, t = {}, n, s) => {
                         const i = t.repeats || 3,
                             r = Date.now();
                         let o = !1;
                         const a = () => {
                             o = !0
                         };
@@ -1567,15 +1550,15 @@
                             const s = t.sheet;
                             if (p++, !s) continue;
                             n?.emit({
                                 percentage: 100 * d / m.length
                             }), d++, s.disabled = !0, await M();
                             const r = await D(e, i, !0);
                             await M(), s.disabled = !1;
-                            const a = await ae(t.textContent);
+                            const a = await oe(t.textContent);
                             u.push({
                                 ...r,
                                 content: t.textContent,
                                 source: null != a ? a.sources[0] : null,
                                 stylesheetIndex: p
                             })
                         }
@@ -1585,33 +1568,33 @@
                             tags: b(),
                             totalTime: Date.now() - r,
                             type: "time",
                             interrupted: o
                         }
                     }
                 },
-                ge = {
+                fe = {
                     id: "style-rule",
                     name: "Style Rules",
-                    configSchema: ue,
+                    configSchema: ce,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
                             l = Date.now();
                         e.setupSuite && await e.setupSuite();
                         const c = [...document.querySelectorAll("style")],
                             u = await D(e, 2 * o, !0);
                         console.log("Reference for", e.name, "is:", u);
                         const d = [],
-                            p = await le(c, {
+                            p = await ae(c, {
                                 skipPattern: a
                             });
                         for (let t = 0; t < p.length && !i; t++) {
                             n?.emit({
                                 percentage: 100 * t / p.length
                             });
                             const s = p[t];
@@ -1631,20 +1614,20 @@
                             reference: u.times,
                             tags: b(),
                             totalTime: Date.now() - l,
                             type: "time",
                             interrupted: i
                         }
                     },
-                    interpretation: m().createElement(m().Fragment, null, m().createElement("ul", null, m().createElement("li", null, m().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), m().createElement("div", null, "Negative ", m().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), p().createElement("div", null, "Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
-                we = {
+                ge = {
                     id: "style-rule-group",
                     name: "Style Rule Groups",
-                    configSchema: de,
+                    configSchema: ue,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
@@ -1663,15 +1646,15 @@
                         for (let t = 0; t < h + 1 && !i; t++) {
                             0 !== t && (d = d.map((e => ({
                                 value: e,
                                 sort: Math.random()
                             }))).sort(((e, t) => e.sort - t.sort)).map((({
                                 value: e
                             }) => e)));
-                            const s = await le(d, {
+                            const s = await ae(d, {
                                 skipPattern: a
                             });
                             console.log(`Collected ${s.length} rules, randomization: ${t}`);
                             for (let r = c; r <= l && !i; r++) {
                                 f += 1, n?.emit({
                                     percentage: 100 * f / g
                                 });
@@ -1707,23 +1690,23 @@
                             totalTime: Date.now() - u,
                             type: "time",
                             interrupted: i
                         }
                     },
                     render: function(e) {
                         const t = e.outcome.results,
-                            [n, s] = m().useState("block"),
-                            i = m().useRef(null);
+                            [n, s] = p().useState("block"),
+                            i = p().useRef(null);
                         null !== i.current && i.current.stateSource === e.outcome || (i.current = new G({
                             measurements: t,
                             reference: e.outcome.reference,
                             stateSource: e.outcome,
                             lowerIsBetter: !1
                         }));
-                        const r = m().useRef(null);
+                        const r = p().useRef(null);
                         if (null === r.current || r.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const e of t)
                                 for (const t of e.rulesInBlock)
                                     if (t.selector in n) n[t.selector].times.push(...e.times);
                                     else {
                                         const s = {
@@ -1735,80 +1718,153 @@
                                     } r.current = new G({
                                 measurements: [...Object.values(n)],
                                 reference: e.outcome.reference,
                                 stateSource: e.outcome,
                                 lowerIsBetter: !1
                             })
                         }
-                        return m().createElement(m().Fragment, null, m().createElement("div", {
+                        return p().createElement(p().Fragment, null, p().createElement("div", {
                             onChange: e => {
                                 s(e.target.value)
                             }
-                        }, m().createElement("label", null, m().createElement("input", {
+                        }, p().createElement("label", null, p().createElement("input", {
                             type: "radio",
                             checked: "block" === n,
                             value: "block"
-                        }), "Blocks"), m().createElement("label", null, m().createElement("input", {
+                        }), "Blocks"), p().createElement("label", null, p().createElement("input", {
                             type: "radio",
                             checked: "rule" === n,
                             value: "rule"
-                        }), "Rules")), "block" === n ? m().createElement(K, {
+                        }), "Rules")), "block" === n ? p().createElement(K, {
                             widget: i.current
-                        }) : m().createElement(K, {
+                        }) : p().createElement(K, {
                             widget: r.current
                         }))
                     }
                 },
-                ye = new g.Token("@jupyterlab/ui-profiler:plugin"),
-                be = JSON.parse('{"title":"Scenario Options","type":"object","properties":{}}'),
+                we = new f.Token("@jupyterlab/ui-profiler:plugin");
+
+            function ye(e) {
+                return [e.benchmark, e.scenario, e.completed.toISOString()].join("_")
+            }
+            class be {
+                constructor(e) {
+                    this.options = e, this._scenarios = [], this._scenarioAdded = new w.Signal(this), this._abortBenchmark = new w.Signal(this), this._progress = new w.Signal(this)
+                }
+                get scenarioAdded() {
+                    return this._scenarioAdded
+                }
+                get progress() {
+                    return this._progress
+                }
+                get benchmarks() {
+                    return this.options.benchmarks
+                }
+                get scenarios() {
+                    return this._scenarios
+                }
+                addScenario(e) {
+                    this._scenarios.push(e), this._scenarioAdded.emit(e)
+                }
+                async runBenchmark(e, t) {
+                    const n = this.options.benchmarks.find((e => e.id === t.id));
+                    if (!n) throw Error(`Benchmark with id ${t} not found`);
+                    const s = this._scenarios.find((t => t.id === e.id));
+                    if (!s) throw Error(`Scenario with id ${e} not found`);
+                    s.setOptions && s.setOptions(e.options), this._progress.emit({
+                        percentage: 0
+                    });
+                    const i = await n.run(s, t.options, this._progress, this._abortBenchmark);
+                    i.interrupted ? this._progress.emit({
+                        percentage: NaN,
+                        interrupted: !0
+                    }) : this._progress.emit({
+                        percentage: 100
+                    });
+                    const r = {
+                        outcome: i,
+                        options: {
+                            benchmark: t.options,
+                            scenario: e.options
+                        },
+                        benchmark: t.id,
+                        scenario: e.id,
+                        userAgent: window.navigator.userAgent,
+                        hardwareConcurrency: window.navigator.hardwareConcurrency,
+                        completed: new Date,
+                        windowSize: {
+                            width: window.innerWidth,
+                            height: window.innerHeight
+                        },
+                        jupyter: this.getJupyterState()
+                    };
+                    return {
+                        ...r,
+                        id: ye(r)
+                    }
+                }
+                abortBenchmark() {
+                    this._abortBenchmark.emit()
+                }
+                getJupyterState() {
+                    const e = this.options.app;
+                    return {
+                        client: e.name,
+                        version: e.version,
+                        devMode: "true" === (g.PageConfig.getOption("devMode") || "").toLowerCase(),
+                        mode: g.PageConfig.getOption("mode")
+                    }
+                }
+            }
+            const ke = JSON.parse('{"title":"Scenario Options","type":"object","properties":{}}'),
                 ve = JSON.parse('{"title":"Menu Open Scenario Options","type":"object","properties":{"menu":{"title":"The menu to open","type":"string","default":"file","enum":["file","edit","view","run","kernel","settings","help"]}},"required":["menu"]}'),
-                ke = JSON.parse('{"title":"Tab Scenario Options","type":"object","definitions":{"tab":{"description":"Tab to open","type":"object","properties":{"path":{"title":"Path","description":"Location of file/notebook to open. If empty opens a new launcher.","type":"string"}},"default":{"path":""}}},"properties":{"tabs":{"title":"List of tabs to use in scenario","description":"Series of two or more tabs","type":"array","items":{"$ref":"#/definitions/tab"},"default":[{"path":""},{"path":""}]}},"required":["tabs"]}'),
-                Se = JSON.parse('{"title":"Completer Scenario Options","type":"object","properties":{"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"File Editor"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"setup":{"title":"Editor setup for completion","description":"How should the editor be populated?","default":{"tokenCount":1000,"tokenSize":50},"anyOf":[{"type":"object","title":"Auto-generate tokens to complete","properties":{"tokenCount":{"title":"Token count","description":"The number of completion items to generate","type":"number","minimum":1,"default":1000},"tokenSize":{"title":"Token size","description":"The number characters in each token","type":"number","minimum":1,"default":50}},"required":["tokenCount","tokenSize"]},{"type":"object","title":"I will provide a custom text","properties":{"setupText":{"title":"Trigger code","description":"Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.","type":"string","default":"np."},"setupCell":{"title":"Code to run (notebook only)","description":"Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.","type":"string","default":"import numpy as np"}},"required":["setupText","triggerCell"]}]}},"required":["editor","setup"],"additionalProperties":false}'),
-                Ee = JSON.parse('{"title":"Debugger Scenario Options","type":"object","properties":{"codeCells":{"title":"Code to execute","description":"Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`","type":"array","items":{"type":"string"},"default":["[globals().__setitem__(f\'x{i}\', \'y\') for i in range(1000)];","z = 1"]},"expectedNumberOfVariables":{"title":"Expected number of variables","description":"The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.","type":"array","items":{"type":"integer","min":0},"default":[1000,1001]}},"required":["codeCells","expectedNumberOfVariables"],"additionalProperties":false}'),
-                xe = JSON.parse('{"title":"Sidebars Scenario Options","type":"object","properties":{"sidebars":{"title":"The sidebars to open","type":"array","default":["table-of-contents","jp-debugger-sidebar","jp-property-inspector","filebrowser","extensionmanager.main-view","jp-running-sessions"],"items":{"type":"string"}}},"required":["sidebars"]}'),
-                je = JSON.parse('{"title":"Scroll Scenario Options","type":"object","properties":{"scrollTop":{"title":"Scroll from top","description":"Number of pixes to scroll by","type":"number","minimum":0,"default":10000},"scrollBehavior":{"title":"Scroll behaviour","description":"Behavior of scroll, either \'smooth\' for smooth scrolling, or \'auto\' for instant scrolling.","type":"string","enum":["smooth","auto"],"default":"smooth"},"cellByCell":{"title":"Traverse cell-by-cell","description":"Instead of scrolling, traverse notebook cell-by-cell (which also combines stepwise scrolling and cell activation/deactivation). Small number of cells (50-100) is recommended for benchmarking such scenario. \'scrollTop\' and \'scrollBehavior\' have no effect if this variant is enabled. Has no effect in file editor.","type":"boolean","default":false},"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"Notebook"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"cells":{"title":"Number of cells/blocks to append","description":"If using a notebook, how many cell should be created? For file editor, how many lines?","type":"number","minimum":0,"default":1000},"editorContent":{"title":"Editor/cell content","description":"Text to populate editors/cells with.","type":"string","default":"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."}},"required":["editor","cells","scrollTop","scrollBehavior"],"additionalProperties":false}');
-            async function Ne(e, t = "file") {
+                Se = JSON.parse('{"title":"Tab Scenario Options","type":"object","definitions":{"tab":{"description":"Tab to open","type":"object","properties":{"path":{"title":"Path","description":"Location of file/notebook to open. If empty opens a new launcher.","type":"string"}},"default":{"path":""}}},"properties":{"tabs":{"title":"List of tabs to use in scenario","description":"Series of two or more tabs","type":"array","items":{"$ref":"#/definitions/tab"},"default":[{"path":""},{"path":""}]}},"required":["tabs"]}'),
+                Ee = JSON.parse('{"title":"Completer Scenario Options","type":"object","properties":{"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"File Editor"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"setup":{"title":"Editor setup for completion","description":"How should the editor be populated?","default":{"tokenCount":1000,"tokenSize":50},"anyOf":[{"type":"object","title":"Auto-generate tokens to complete","properties":{"tokenCount":{"title":"Token count","description":"The number of completion items to generate","type":"number","minimum":1,"default":1000},"tokenSize":{"title":"Token size","description":"The number characters in each token","type":"number","minimum":1,"default":50}},"required":["tokenCount","tokenSize"]},{"type":"object","title":"I will provide a custom text","properties":{"setupText":{"title":"Trigger code","description":"Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.","type":"string","default":"np."},"setupCell":{"title":"Code to run (notebook only)","description":"Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.","type":"string","default":"import numpy as np"}},"required":["setupText","triggerCell"]}]}},"required":["editor","setup"],"additionalProperties":false}'),
+                xe = JSON.parse('{"title":"Debugger Scenario Options","type":"object","properties":{"codeCells":{"title":"Code to execute","description":"Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`","type":"array","items":{"type":"string"},"default":["[globals().__setitem__(f\'x{i}\', \'y\') for i in range(1000)];","z = 1"]},"expectedNumberOfVariables":{"title":"Expected number of variables","description":"The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.","type":"array","items":{"type":"integer","min":0},"default":[1000,1001]}},"required":["codeCells","expectedNumberOfVariables"],"additionalProperties":false}'),
+                je = JSON.parse('{"title":"Sidebars Scenario Options","type":"object","properties":{"sidebars":{"title":"The sidebars to open","type":"array","default":["table-of-contents","jp-debugger-sidebar","jp-property-inspector","filebrowser","extensionmanager.main-view","jp-running-sessions"],"items":{"type":"string"}}},"required":["sidebars"]}'),
+                Ne = JSON.parse('{"title":"Scroll Scenario Options","type":"object","properties":{"scrollTop":{"title":"Scroll from top","description":"Number of pixes to scroll by","type":"number","minimum":0,"default":10000},"scrollBehavior":{"title":"Scroll behaviour","description":"Behavior of scroll, either \'smooth\' for smooth scrolling, or \'auto\' for instant scrolling.","type":"string","enum":["smooth","auto"],"default":"smooth"},"cellByCell":{"title":"Traverse cell-by-cell","description":"Instead of scrolling, traverse notebook cell-by-cell (which also combines stepwise scrolling and cell activation/deactivation). Small number of cells (50-100) is recommended for benchmarking such scenario. \'scrollTop\' and \'scrollBehavior\' have no effect if this variant is enabled. Has no effect in file editor.","type":"boolean","default":false},"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"Notebook"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"cells":{"title":"Number of cells/blocks to append","description":"If using a notebook, how many cell should be created? For file editor, how many lines?","type":"number","minimum":0,"default":1000},"editorContent":{"title":"Editor/cell content","description":"Text to populate editors/cells with.","type":"string","default":"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."}},"required":["editor","cells","scrollTop","scrollBehavior"],"additionalProperties":false}');
+            async function Me(e, t = "file") {
                 await e.commands.execute(`${t}menu:open`), await P.waitForSelector(`#jp-mainmenu-${t}`, {
                     state: "attached"
                 }), await M()
             }
-            async function Me() {
+            async function Ce() {
                 await P.waitForSelector(".lm-Menu", {
                     state: "attached"
                 }), await P.press("Escape"), await P.waitForSelector(".lm-Menu", {
                     state: "detached"
                 }), await M()
             }
-            class Ce {
+            class Oe {
                 constructor(e) {
-                    this.jupyterApp = e, this.cleanup = Me, this.id = "menuSwitch", this.name = "Switch Menu", this.configSchema = be
+                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuSwitch", this.name = "Switch Menu", this.configSchema = ke
                 }
                 async setup() {
-                    return Ne(this.jupyterApp)
+                    return Me(this.jupyterApp)
                 }
                 async run() {
                     return async function(e) {
-                        for (const t of ["edit", "view", "run", "kernel", "settings", "help"]) await Ne(e, t)
+                        for (const t of ["edit", "view", "run", "kernel", "settings", "help"]) await Me(e, t)
                     }(this.jupyterApp)
                 }
             }
-            class Oe {
+            class Ie {
                 constructor(e) {
-                    this.jupyterApp = e, this.cleanup = Me, this.id = "menuOpen", this.name = "Open Menu", this.configSchema = ve, this._menu = "file"
+                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuOpen", this.name = "Open Menu", this.configSchema = ve, this._menu = "file"
                 }
                 setOptions(e) {
                     this._menu = e.menu
                 }
                 async run() {
-                    return Ne(this.jupyterApp, this._menu)
+                    return Me(this.jupyterApp, this._menu)
                 }
             }
-            class Ie {
+            class _e {
                 constructor(e) {
-                    this.jupyterApp = e, this.id = "sidebarOpen", this.name = "Open Sidebar", this.configSchema = xe, this._sidebars = ["filebrowser"]
+                    this.jupyterApp = e, this.id = "sidebarOpen", this.name = "Open Sidebar", this.configSchema = je, this._sidebars = ["filebrowser"]
                 }
                 setOptions(e) {
                     this._sidebars = e.sidebars
                 }
                 async setup() {
                     return async function(e) {
                         for (const t of ["left", "right"]) {
@@ -1830,15 +1886,15 @@
                 return e.commands.execute("apputils:run-first-enabled", {
                     commands: ["notebook:replace-selection", "console:replace-selection", "fileeditor:replace-selection"],
                     args: {
                         text: t
                     }
                 })
             }
-            class Re {
+            class Be {
                 constructor(e) {
                     this.jupyterApp = e, this.editor = null, this.path = null, this.options = null, this.useNotebook = !0, this.widget = null
                 }
                 setOptions(e) {
                     this.options = e, this.useNotebook = "Notebook" === this.options.editor
                 }
                 async setupSuite() {
@@ -1857,40 +1913,40 @@
                     }
                     const e = await this.jupyterApp.commands.execute("docmanager:open", {
                         path: this.path,
                         factory: this.useNotebook ? "Notebook" : "Editor"
                     });
                     this.widget = e, this.jupyterApp.shell.add(this.widget, "main", {
                         mode: "split-right"
-                    }), await Pe(this.jupyterApp, e), await M(), this.useNotebook && await P.click(".jp-Dialog-button.jp-mod-accept");
+                    }), await De(this.jupyterApp, e), await M(), this.useNotebook && await P.click(".jp-Dialog-button.jp-mod-accept");
                     const t = new C(this.widget.node);
                     await t.waitForSelector(".jp-Editor", {
                         state: "attached"
                     }), await M(), await t.waitForSelector(".jp-Editor", {
                         state: "visible"
                     }), await M(), this.editor = this.useNotebook ? this.widget.node.querySelector(".jp-Notebook") : this.widget.node.querySelector(".jp-FileEditorCodeWrapper")
                 }
                 async cleanupSuite() {
                     this.widget && (await this.jupyterApp.commands.execute("docmanager:save"), this.widget.close())
                 }
             }
-            class Be extends Re {
+            class Re extends Be {
                 constructor() {
-                    super(...arguments), this.id = "completer", this.name = "Completer", this.configSchema = Se
+                    super(...arguments), this.id = "completer", this.name = "Completer", this.configSchema = Ee
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     let e;
                     if (void 0 !== this.options.setup?.setupText) e = this.options.setup.setupText;
                     else {
                         const t = [];
                         for (let e = 0; e < this.options.setup.tokenCount; e++) t.push(("t" + e).padEnd(this.options.setup.tokenSize, "x") + " = " + e);
                         t.push("t"), e = t.join("\n")
                     }
-                    this.useNotebook && this.options.setup.setupCell ? (await Te(this.jupyterApp, this.options.setup.setupCell), await Ae(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await Te(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
+                    this.useNotebook && this.options.setup.setupCell ? (await Te(this.jupyterApp, this.options.setup.setupCell), await Pe(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await Te(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
                         top: 20 * this.options.setup.tokenCount,
                         left: 0,
                         behavior: "smooth"
                     });
                     try {
                         await this.run()
                     } catch (e) {}
@@ -1912,17 +1968,17 @@
                 }
                 async cleanup() {
                     await P.press("Escape"), await M(), await P.waitForSelector(".jp-Completer[style]", {
                         state: "hidden"
                     }), await M()
                 }
             }
-            class _e extends Re {
+            class Ae extends Be {
                 constructor() {
-                    super(...arguments), this.id = "debugger", this.name = "Debugger", this.configSchema = Ee
+                    super(...arguments), this.id = "debugger", this.name = "Debugger", this.configSchema = xe
                 }
                 setOptions(e) {
                     super.setOptions({
                         ...e,
                         editor: "Notebook",
                         path: null
                     })
@@ -1930,15 +1986,15 @@
                 async _goToTop() {
                     if (!this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length + 1; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-up")
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     for (const e of this.options.codeCells) await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:insert-cell-below"), await M(), await M(), await this.jupyterApp.commands.execute("notebook:enter-edit-mode"), await M(), await M();
-                    await Te(this.jupyterApp, "%reset -f"), await this._goToTop(), await Ae(this.widget.node, "idle");
+                    await Te(this.jupyterApp, "%reset -f"), await this._goToTop(), await Pe(this.widget.node, "idle");
                     const e = new C(this.widget.node),
                         t = await e.waitForSelector('button[aria-disabled="false"][title="Enable Debugger"]', {
                             state: "attached"
                         });
                     await t.click(), await P.waitForSelector(`#${CSS.escape("jp-debugger-sidebar")}`, {
                         state: "visible"
                     }), await e.waitForSelector('button[aria-disabled="false"][title="Disable Debugger"]', {
@@ -1948,48 +2004,48 @@
                     }), await P.waitForSelector(".jp-DebuggerVariables-body", {
                         state: "visible"
                     })
                 }
                 async run() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length; e++) {
-                        await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Ae(this.widget.node, "idle");
+                        await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Pe(this.widget.node, "idle");
                         const t = this.options.expectedNumberOfVariables[e];
                         void 0 !== t && await P.waitForSelector(`.jp-DebuggerVariables-body li:nth-child(${t+2})`, {
                             state: "attached"
                         }), await M()
                     }
                 }
                 async cleanup() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     await M();
                     const e = Math.min(...this.options.expectedNumberOfVariables);
-                    await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Ae(this.widget.node, "idle"), await async function(e) {
+                    await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Pe(this.widget.node, "idle"), await async function(e) {
                         return new Promise(((t, n) => {
                             let s = 0;
                             const i = setInterval((() => document.querySelector(e) ? s > 5e3 ? (clearInterval(i), n(`${e} did not disappear in 5000ms`)) : void(s += 50) : (clearInterval(i), t())), 50)
                         }))
                     }(`.jp-DebuggerVariables-body li:nth-child(${e})`), await this._goToTop(), await M()
                 }
             }
-            async function Ae(e, t) {
+            async function Pe(e, t) {
                 await new C(e).waitForSelector(`.jp-Notebook-ExecutionIndicator[data-status="${t}"]`, {
                     state: "attached"
                 })
             }
-            async function Pe(e, t) {
+            async function De(e, t) {
                 await e.commands.execute("tabsmenu:activate-by-id", {
                     id: t.id
                 }), await M(), await P.waitForSelector(`li.lm-mod-current[data-id="${t.id}"]`, {
                     state: "attached"
                 }), await M()
             }
-            class De extends Re {
+            class Fe extends Be {
                 constructor() {
-                    super(...arguments), this.id = "scroll", this.name = "Scroll", this.configSchema = je
+                    super(...arguments), this.id = "scroll", this.name = "Scroll", this.configSchema = Ne
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     const e = this.options.cells < 100 ? 20 : 50;
                     for (let t = 0; t < this.options.cells; t++) this.useNotebook && await this.jupyterApp.commands.execute("notebook:insert-cell-below"), this.options.editorContent && await Te(this.jupyterApp, this.useNotebook ? this.options.editorContent : this.options.editorContent + "\n"), (t < 5 || t % e == 0) && await M();
                     this.editor.scrollTop = 0, await M()
                 }
@@ -2017,17 +2073,17 @@
                     if (!this.widget || !this.options) throw new Error("Scrol scenario setup failure");
                     if (this.options.cellByCell && this.useNotebook) {
                         for (let e = 0; e < this.options.cells; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-up");
                         await M()
                     } else this.editor.scrollTop = 0, await M()
                 }
             }
-            class Fe {
+            class qe {
                 constructor(e) {
-                    this.jupyterApp = e, this.id = "tabSwitch", this.name = "Switch Tabs", this.split = "first", this.configSchema = ke, this._tabs = [], this._widgets = []
+                    this.jupyterApp = e, this.id = "tabSwitch", this.name = "Switch Tabs", this.split = "first", this.configSchema = Se, this._tabs = [], this._widgets = []
                 }
                 setOptions(e) {
                     const {
                         tabs: t
                     } = e;
                     if (!t || !t.length) throw new Error("At least one tab specification must be provided");
                     this._tabs = t, this._widgets = []
@@ -2038,96 +2094,91 @@
                         let t;
                         t = e.path ? await this.jupyterApp.commands.execute("docmanager:open", {
                             path: e.path
                         }) : await this.jupyterApp.commands.execute("launcher:create"), await P.waitForSelector("#" + t.id, {
                             state: "attached"
                         }), ("first" === this.split && 0 === this._widgets.length || "all" === this.split) && this.jupyterApp.shell.add(t, "main", {
                             mode: "split-right"
-                        }), await Pe(this.jupyterApp, t), this._widgets.push(t)
+                        }), await De(this.jupyterApp, t), this._widgets.push(t)
                     }
                 }
                 async cleanupSuite() {
                     for (const e of this._widgets) e.close(), await P.waitForSelector(`.lm-Widget[data-id="${e.id}"]`, {
                         state: "detached"
                     })
                 }
                 async run() {
                     if (!this._widgets.length) throw new Error("Suite not set up");
-                    for (const e of this._widgets) await Pe(this.jupyterApp, e)
+                    for (const e of this._widgets) await De(this.jupyterApp, e)
                 }
             }
-            class qe extends Fe {
+            class Le extends qe {
                 constructor() {
                     super(...arguments), this.id = "tabSwitchFocus", this.name = "Switch Tab Focus", this.split = "all"
                 }
             }
-            const Le = {
+            const $e = {
                 id: "@jupyterlab/ui-profiler:default-scenarios",
                 autoStart: !0,
-                requires: [ye],
+                requires: [we],
                 activate: (e, t) => {
-                    [new Oe(e), new Ce(e), new Fe(e), new qe(e), new Ie(e), new Be(e), new De(e), new _e(e)].map((e => t.addScenario(e)))
+                    [new Ie(e), new Oe(e), new qe(e), new Le(e), new _e(e), new Re(e), new Fe(e), new Ae(e)].map((e => t.addScenario(e)))
                 }
             };
-            var $e;
+            var We;
             ! function(e) {
                 e.openProfiler = "ui-profiler:open"
-            }($e || ($e = {}));
-            const We = [{
+            }(We || (We = {}));
+            const ze = [{
                 id: "@jupyterlab/ui-profiler:plugin",
                 autoStart: !0,
-                requires: [o.IDocumentManager],
-                optional: [l.ILauncher, s.ILayoutRestorer],
-                provides: ye,
-                activate: (e, t, n, s) => {
-                    const o = new a.FileBrowserModel({
-                            manager: t
+                provides: we,
+                activate: e => new be({
+                    app: e,
+                    benchmarks: [F, he, fe, ge, me, $]
+                })
+            }, $e, {
+                id: "@jupyterlab/ui-profiler:user-interface",
+                autoStart: !0,
+                requires: [we, r.IDocumentManager],
+                optional: [a.ILauncher, s.ILayoutRestorer],
+                activate: (e, t, n, s, r) => {
+                    const a = new o.FileBrowserModel({
+                            manager: n
                         }),
-                        l = [],
-                        d = {
-                            benchmarks: [F, fe, ge, we, he, $],
-                            scenarios: l,
-                            translator: c.nullTranslator,
-                            upload: e => o.upload(e),
-                            getJupyterState: () => ({
-                                client: e.name,
-                                version: e.version,
-                                devMode: "true" === (r.PageConfig.getOption("devMode") || "").toLowerCase(),
-                                mode: r.PageConfig.getOption("mode")
-                            }),
+                        u = {
+                            translator: l.nullTranslator,
+                            profiler: t,
+                            upload: e => a.upload(e),
                             resultLocation: "/ui-profiler-results/"
                         };
-                    let p = null;
-                    const m = new i.WidgetTracker({
+                    let d = null;
+                    const p = new i.WidgetTracker({
                         namespace: "ui-profiler"
                     });
-                    return e.commands.addCommand($e.openProfiler, {
+                    e.commands.addCommand(We.openProfiler, {
                         execute: async () => {
                             let t;
-                            t = !p || p.isDisposed ? (() => {
-                                const e = new Z(d),
+                            t = !d || d.isDisposed ? (() => {
+                                const e = new Z(u),
                                     t = new i.MainAreaWidget({
                                         content: e
                                     });
-                                return t.id = "ui-profiler-centre", t.title.label = "UI Profiler", t.title.closable = !0, t.title.icon = u.offlineBoltIcon, t
-                            })() : p, p = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), m.add(t)
+                                return t.id = "ui-profiler-centre", t.title.label = "UI Profiler", t.title.closable = !0, t.title.icon = c.offlineBoltIcon, t
+                            })() : d, d = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), p.add(t)
                         },
                         label: "UI Profiler",
-                        icon: u.offlineBoltIcon,
+                        icon: c.offlineBoltIcon,
                         caption: "Open JupyterLab UI Profiler"
-                    }), s && s.restore(m, {
-                        command: $e.openProfiler,
+                    }), r && r.restore(p, {
+                        command: We.openProfiler,
                         name: e => e.title.label
-                    }), n && n.add({
-                        command: $e.openProfiler,
+                    }), s && s.add({
+                        command: We.openProfiler,
                         category: "Other",
                         rank: 1
-                    }), {
-                        addScenario: e => {
-                            l.push(e), p && p.content.addScenario(e)
-                        }
-                    }
+                    })
                 }
-            }, Le]
+            }]
         }
     }
 ]);
```

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/remoteEntry.01dddfb6079d8140a904.js` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/remoteEntry.2c015c9bba0ac87e826d.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v = {
+    var e, r, t, n, a, o, i, l, u, f, s, d, p, c, h, v = {
             4299: (e, r, t) => {
-                var a = {
-                        "./index": () => Promise.all([t.e(511), t.e(103)]).then((() => () => t(103))),
-                        "./extension": () => Promise.all([t.e(511), t.e(103)]).then((() => () => t(103))),
+                var n = {
+                        "./index": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
+                        "./extension": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var a = "default",
-                                n = t.S[a];
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[a] = e, t.I(a, r)
+                            var n = "default",
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => n,
+                    get: () => a,
                     init: () => o
                 })
             }
         },
         b = {};
 
     function m(e) {
@@ -44,80 +44,80 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        103: "fef9f7b84e7801e31ec3",
+        148: "d0923e85cee15af0e9d9",
         511: "91d18779f0d0a64a6570",
         747: "cddb110f7b8c43b31d07"
     } [e] + ".js?v=" + {
-        103: "fef9f7b84e7801e31ec3",
+        148: "d0923e85cee15af0e9d9",
         511: "91d18779f0d0a64a6570",
         747: "cddb110f7b8c43b31d07"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/ui-profiler:", m.l = (t, a, n, o) => {
-        if (e[t]) e[t].push(a);
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/ui-profiler:", m.l = (t, n, a, o) => {
+        if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== n)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var d = u[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var n = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, m.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         m.S = {};
         var e = {},
             r = {};
-        m.I = (t, a) => {
-            a || (a = []);
-            var n = r[t];
-            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
-                if (a.push(n), e[t]) return e[t];
+        m.I = (t, n) => {
+            n || (n = []);
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 m.o(m.S, t) || (m.S[t] = {});
                 var o = m.S[t],
                     i = "@jupyterlab/ui-profiler",
                     l = [];
-                return "default" === t && ((e, r, t, a) => {
-                    var n = o[e] = o[e] || {},
-                        l = n[r];
-                    (!l || !l.loaded && (1 != !l.eager ? a : i > l.from)) && (n[r] = {
-                        get: () => Promise.all([m.e(511), m.e(103)]).then((() => () => m(103))),
+                return "default" === t && ((e, r, t, n) => {
+                    var a = o[e] = o[e] || {},
+                        l = a[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
+                        get: () => Promise.all([m.e(511), m.e(148)]).then((() => () => m(8148))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab/ui-profiler", "0.1.8"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@jupyterlab/ui-profiler", "0.2.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -125,74 +125,74 @@
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            a = t[1] ? r(t[1]) : [];
-        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
-    }, a = (e, r) => {
+            n = t[1] ? r(t[1]) : [];
+        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
+    }, n = (e, r) => {
         e = t(e), r = t(r);
-        for (var a = 0;;) {
-            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
-            var n = e[a],
-                o = (typeof n)[0];
-            if (a >= r.length) return "u" == o;
-            var i = r[a],
+        for (var n = 0;;) {
+            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
+            var i = r[n],
                 l = (typeof i)[0];
             if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && n != i) return n < i;
-            a++
+            if ("o" != o && "u" != o && a != i) return a < i;
+            n++
         }
-    }, n = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var a = e[0],
-                n = a < 0;
-            n && (a = -a - 1);
+            var n = e[0],
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!u || "u" != s) return !1
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
+                if ("u" == s) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == d)
-                        if (l <= a) {
+                    if (d == s)
+                        if (l <= n) {
                             if (f != e[l]) return !1
                         } else {
-                            if (n ? f > e[l] : f < e[l]) return !1;
+                            if (a ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (n || l <= a) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || d < s != n) return !1;
+                    if (l <= n || s < d != a) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -200,89 +200,89 @@
         return !!c()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
-        var n = l(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), d(e[t][n])
-    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, a, n) {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), s(e[t][a])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
         var o = m.I(r);
-        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, a, n)) : e(r, m.S[r], t, a)
-    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), p = {}, c = {
-        1467: () => s("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
-        1526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        1840: () => s("default", "@lumino/signaling", [1, 1, 10, 0]),
-        2502: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        2583: () => s("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
-        3033: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        3169: () => s("default", "@jupyterlab/translation", [1, 3, 6, 3]),
-        5414: () => s("default", "@lumino/datagrid", [2, 0, 36, 4]),
-        5687: () => s("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        6271: () => s("default", "react", [1, 17, 0, 1]),
-        7280: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
-        7986: () => s("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
-        8142: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        8820: () => s("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        8832: () => s("default", "@lumino/widgets", [1, 1, 37, 2])
+        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
+        1467: () => d("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        1526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        1840: () => d("default", "@lumino/signaling", [1, 1, 10, 0]),
+        2502: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        2583: () => d("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
+        3033: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        3169: () => d("default", "@jupyterlab/translation", [1, 3, 6, 3]),
+        5414: () => d("default", "@lumino/datagrid", [2, 0, 36, 4]),
+        5687: () => d("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        6271: () => d("default", "react", [1, 17, 0, 1]),
+        7280: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        7986: () => d("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        8820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
     }, h = {
-        103: [1467, 1526, 1840, 2502, 2583, 3033, 3169, 5414, 5687, 6271, 7280, 7986, 8142, 8820, 8832]
+        148: [1467, 1526, 1840, 2502, 2583, 3033, 3169, 5414, 5687, 6271, 7280, 7986, 8142, 8820, 8832]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
             if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
-                a = r => {
+                n = r => {
                     delete p[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
-                var n = c[e]();
-                n.then ? r.push(p[e] = n.then(t).catch(a)) : t(n)
+                var a = c[e]();
+                a.then ? r.push(p[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
-                a(e)
+                n(e)
             }
         }))
     }, (() => {
         var e = {
             770: 0
         };
         m.f.j = (r, t) => {
-            var a = m.o(e, r) ? e[r] : void 0;
-            if (0 !== a)
-                if (a) t.push(a[2]);
+            var n = m.o(e, r) ? e[r] : void 0;
+            if (0 !== n)
+                if (n) t.push(n[2]);
                 else {
-                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
-                    t.push(a[2] = n);
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
                     var o = m.p + m.u(r),
                         i = new Error;
                     m.l(o, (t => {
-                        if (m.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
-                            var n = t && ("load" === t.type ? "missing" : t.type),
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var a, n, [o, i, l] = t,
+                var n, a, [o, i, l] = t,
                     u = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (a in i) m.o(i, a) && (m.m[a] = i[a]);
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
                     l && l(m)
                 }
-                for (r && r(t); u < o.length; u++) n = o[u], m.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); u < o.length; u++) a = o[u], m.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyterlab_ui_profiler = self.webpackChunk_jupyterlab_ui_profiler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
     var g = m(4299);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/ui-profiler"] = g
 })();
```

### Comparing `jupyterlab_ui_profiler-0.1.8/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json` & `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/css.ts` & `jupyterlab_ui_profiler-0.2.0/src/css.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/dramaturg.ts` & `jupyterlab_ui_profiler-0.2.0/src/dramaturg.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/index.ts` & `jupyterlab_ui_profiler-0.2.0/src/index.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,101 @@
 import {
   ILayoutRestorer,
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { MainAreaWidget, WidgetTracker } from '@jupyterlab/apputils';
-import { PageConfig } from '@jupyterlab/coreutils';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { FileBrowserModel } from '@jupyterlab/filebrowser';
 import { ILauncher } from '@jupyterlab/launcher';
 import { nullTranslator } from '@jupyterlab/translation';
 import { offlineBoltIcon } from '@jupyterlab/ui-components';
-import type { DockPanel } from '@lumino/widgets';
-import { UIProfiler } from './ui';
+import { UIProfilerWidget, ConstrainedUIProfiler } from './ui';
 import {
   styleSheetsBenchmark,
   styleRuleBenchmark,
   styleRuleGroupBenchmark,
   styleRuleUsageBenchmark
 } from './styleBenchmarks';
 import { selfProfileBenchmark } from './jsBenchmarks';
-import {
-  executionTimeBenchmark,
-  IBenchmark,
-  ITimingOutcome,
-  IProfilingOutcome
-} from './benchmark';
-import { IJupyterState } from './utils';
-import { IScenario, IUIProfiler } from './tokens';
+import { executionTimeBenchmark } from './benchmark';
+import { IBenchmark, IUIProfiler } from './tokens';
+import { UIProfiler } from './profiler';
 import { plugin as scenariosPlugin } from './scenarios';
 
 namespace CommandIDs {
   // export const findUnusedStyles = 'ui-profiler:find-unused-styles';
   export const openProfiler = 'ui-profiler:open';
 }
 
 /**
  * Initialization data for the @jupyterlab/ui-profiler extension.
  */
 const plugin: JupyterFrontEndPlugin<IUIProfiler> = {
   id: '@jupyterlab/ui-profiler:plugin',
   autoStart: true,
-  requires: [IDocumentManager],
-  optional: [ILauncher, ILayoutRestorer],
   provides: IUIProfiler,
+  activate: (app: JupyterFrontEnd) => {
+    return new UIProfiler({
+      app,
+      benchmarks: [
+        executionTimeBenchmark,
+        styleSheetsBenchmark,
+        styleRuleBenchmark,
+        styleRuleGroupBenchmark,
+        styleRuleUsageBenchmark,
+        selfProfileBenchmark
+      ] as IBenchmark<any>[]
+    });
+  }
+};
+
+const interfacePlugin: JupyterFrontEndPlugin<void> = {
+  id: '@jupyterlab/ui-profiler:user-interface',
+  autoStart: true,
+  requires: [IUIProfiler, IDocumentManager],
+  optional: [ILauncher, ILayoutRestorer],
   activate: (
     app: JupyterFrontEnd,
+    profiler: IUIProfiler,
     docManager: IDocumentManager,
     launcher: ILauncher | null,
     restorer: ILayoutRestorer | null
   ) => {
     const fileBrowserModel = new FileBrowserModel({
       manager: docManager
     });
-    const scenarios: IScenario[] = [];
     const options = {
-      benchmarks: [
-        executionTimeBenchmark,
-        styleSheetsBenchmark,
-        styleRuleBenchmark,
-        styleRuleGroupBenchmark,
-        styleRuleUsageBenchmark,
-        selfProfileBenchmark
-      ] as (IBenchmark<ITimingOutcome<any>> | IBenchmark<IProfilingOutcome>)[],
-      scenarios: scenarios,
       translator: nullTranslator,
+      profiler: profiler as unknown as ConstrainedUIProfiler,
       upload: (file: File) => {
         // https://github.com/jupyterlab/jupyterlab/issues/11416
         return fileBrowserModel.upload(file);
       },
-      getJupyterState: () => {
-        const state: IJupyterState = {
-          client: app.name,
-          version: app.version,
-          devMode:
-            (PageConfig.getOption('devMode') || '').toLowerCase() === 'true',
-          mode: PageConfig.getOption('mode') as DockPanel.Mode
-        };
-        return state;
-      },
       resultLocation: '/ui-profiler-results/'
     };
-    let lastWidget: MainAreaWidget<UIProfiler> | null = null;
+    let lastWidget: MainAreaWidget<UIProfilerWidget> | null = null;
 
     const createWidget = () => {
-      const content = new UIProfiler(options);
+      const content = new UIProfilerWidget(options);
       const widget = new MainAreaWidget({ content });
       widget.id = 'ui-profiler-centre';
       widget.title.label = 'UI Profiler';
       widget.title.closable = true;
       widget.title.icon = offlineBoltIcon;
       return widget;
     };
 
-    const tracker = new WidgetTracker<MainAreaWidget<UIProfiler>>({
+    const tracker = new WidgetTracker<MainAreaWidget<UIProfilerWidget>>({
       namespace: 'ui-profiler'
     });
 
     app.commands.addCommand(CommandIDs.openProfiler, {
       execute: async () => {
-        let widget: MainAreaWidget<UIProfiler>;
+        let widget: MainAreaWidget<UIProfilerWidget>;
         if (!lastWidget || lastWidget.isDisposed) {
           widget = createWidget();
         } else {
           widget = lastWidget;
         }
         lastWidget = widget;
 
@@ -137,22 +130,13 @@
     if (launcher) {
       launcher.add({
         command: CommandIDs.openProfiler,
         category: 'Other',
         rank: 1
       });
     }
-
-    return {
-      addScenario: (scenario: IScenario) => {
-        scenarios.push(scenario);
-        if (lastWidget) {
-          lastWidget.content.addScenario(scenario);
-        }
-      }
-    };
   }
 };
 
 export * from './tokens';
 
-export default [plugin, scenariosPlugin];
+export default [plugin, scenariosPlugin, interfacePlugin];
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/jsBenchmarks.ts` & `jupyterlab_ui_profiler-0.2.0/src/jsBenchmarks.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import { JSONSchema7 } from 'json-schema';
 
-import {
-  IProfilingOutcome,
-  IBenchmark,
-  IProfileMeasurement,
-  profile
-} from './benchmark';
+import { profile } from './benchmark';
+import { IProfilingOutcome, IProfileMeasurement } from './tokens';
 import { reportTagCounts } from './utils';
 import { layoutReady } from './dramaturg';
 import { renderProfile } from './ui';
-import { IScenario } from './tokens';
+import { IBenchmark, IScenario } from './tokens';
 
 import benchmarkProfileOptionsSchema from './schema/benchmark-profile.json';
 import type { ProfileBenchmarkOptions } from './types/_benchmark-profile';
 
 interface IFunctionTiming {
   time: number;
   readonly name: string;
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/lumino.tsx` & `jupyterlab_ui_profiler-0.2.0/src/lumino.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/profiler.d.ts` & `jupyterlab_ui_profiler-0.2.0/src/browserProfiler.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/scenarios.ts` & `jupyterlab_ui_profiler-0.2.0/src/scenarios.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/statistics.ts` & `jupyterlab_ui_profiler-0.2.0/src/statistics.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/styleBenchmarks.tsx` & `jupyterlab_ui_profiler-0.2.0/src/styleBenchmarks.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import { JSONSchema7 } from 'json-schema';
 import React from 'react';
 
-import {
-  ITimeMeasurement,
-  ITimingOutcome,
-  IBenchmark,
-  benchmark
-} from './benchmark';
+import { benchmark } from './benchmark';
+import { ITimeMeasurement, ITimingOutcome } from './tokens';
 import { reportTagCounts, shuffled, iterateAffectedNodes } from './utils';
 import { layoutReady } from './dramaturg';
 import {
   IRuleData,
   IRuleDescription,
   extractSourceMap,
   collectRules
 } from './css';
 import { renderBlockResult } from './ui';
-import { IScenario } from './tokens';
+import { IBenchmark, IScenario } from './tokens';
 
 import benchmarkOptionsSchema from './schema/benchmark-base.json';
 import benchmarkRuleOptionsSchema from './schema/benchmark-rule.json';
 import benchmarkRuleGroupOptionsSchema from './schema/benchmark-rule-group.json';
 import benchmarkRuleUsageOptionsSchema from './schema/benchmark-rule-usage.json';
 
 import type { BenchmarkOptions } from './types/_benchmark-base';
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/table.ts` & `jupyterlab_ui_profiler-0.2.0/src/table.ts`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,17 @@
   DataGrid,
   JSONModel,
   BasicKeyHandler,
   BasicMouseHandler,
   BasicSelectionModel,
   SelectionModel
 } from '@lumino/datagrid';
-import { ITimeMeasurement } from './benchmark';
 import { IRuleDescription } from './css';
-
 import { Statistic } from './statistics';
+import { ITimeMeasurement } from './tokens';
 
 class MouseHandler extends BasicMouseHandler {
   get clicked(): ISignal<this, DataGrid.HitTestResult> {
     return this._clicked;
   }
 
   onMouseDown(grid: DataGrid, event: MouseEvent): void {
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/templates.tsx` & `jupyterlab_ui_profiler-0.2.0/src/templates.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/ui.tsx` & `jupyterlab_ui_profiler-0.2.0/src/ui.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -4,45 +4,49 @@
 import { Contents, ServiceManager } from '@jupyterlab/services';
 import { ProgressBar } from '@jupyterlab/statusbar';
 import { ITranslator } from '@jupyterlab/translation';
 import { JSONExt, JSONObject } from '@lumino/coreutils';
 import { PathExt } from '@jupyterlab/coreutils';
 import { Signal, ISignal } from '@lumino/signaling';
 import { Component as JSONComponent } from '@jupyterlab/json-extension/lib/component';
-import {
-  IBenchmark,
-  IOutcome,
-  ITimeMeasurement,
-  IProgress,
-  ITimingOutcome,
-  IProfilingOutcome
-} from './benchmark';
-import { formatTime, IJupyterState, extractBrowserVersion } from './utils';
+import { formatTime, extractBrowserVersion } from './utils';
 import { IRuleBlockResult } from './styleBenchmarks';
 import { extractTimes, iterateFrames } from './jsBenchmarks';
 import {
   CustomTemplateFactory,
   CustomArrayTemplateFactory,
   CustomObjectTemplateFactory
 } from './templates';
 import { Statistic } from './statistics';
 import { TimingTable, ResultTable } from './table';
 import { LuminoWidget } from './lumino';
-import { IScenario, IUIProfiler } from './tokens';
+import {
+  IOutcome,
+  ITimeMeasurement,
+  ITimingOutcome,
+  IProfilingOutcome,
+  IBenchmarkResult,
+  IScenario,
+  IUIProfiler,
+  IProgress,
+  IBenchmark
+} from './tokens';
 
-interface IProfilerProps {
+export type ConstrainedUIProfiler = Omit<IUIProfiler, 'benchmarks'> & {
   benchmarks: (IBenchmark<ITimingOutcome> | IBenchmark<IProfilingOutcome>)[];
-  scenarios: IScenario[];
+};
+
+interface IProfilerProps {
+  profiler: ConstrainedUIProfiler;
   /**
    * Translator object
    */
   translator: ITranslator;
   upload: (file: File) => Promise<Contents.IModel>;
   resultLocation: string;
-  getJupyterState: () => IJupyterState;
 }
 
 interface ILauncherProps extends IProfilerProps {
   progress: Signal<any, IProgress>;
   onResult: (result: IBenchmarkResult) => void;
   resultLocation: string;
 }
@@ -600,24 +604,30 @@
       ) : (
         <LuminoWidget widget={rulesWidget.current} />
       )}
     </>
   );
 }
 
-export class UIProfiler extends ReactWidget implements IUIProfiler {
+export class UIProfilerWidget extends ReactWidget {
   constructor(private props: IProfilerProps) {
     super();
     this.progress = new Signal(this);
     this.handleResult = this.handleResult.bind(this);
     this.loadResult = this.loadResult.bind(this);
     this.upload = this.upload.bind(this);
     this.manager = new ServiceManager();
     this.resultAdded = new Signal(this);
     this.ensureResultsDirectory();
+    this.props.profiler.progress.connect((_, progress) => {
+      this.progress.emit(progress);
+    });
+    this.props.profiler.scenarioAdded.connect(() => {
+      this.update();
+    });
   }
 
   async ensureResultsDirectory() {
     return this.manager.contents
       .save(this.props.resultLocation, {
         type: 'directory'
       })
@@ -634,20 +644,20 @@
     this.result = result;
     this.update();
     this.resultAdded.emit(result);
   }
 
   async loadResult(file: Contents.IModel): Promise<void> {
     file = await this.manager.contents.get(file.path);
-    this.handleResult(JSON.parse(file.content));
-  }
-
-  addScenario(scenario: IScenario) {
-    this.props.scenarios.push(scenario);
-    this.update();
+    const result = JSON.parse(file.content);
+    if (result.result) {
+      // handle the old format which used "result" instead of "outcome"
+      result.outcome = result.result;
+    }
+    this.handleResult(result);
   }
 
   async upload(file: File): Promise<Contents.IModel> {
     await this.ensureResultsDirectory();
     return this.props.upload(file);
   }
 
@@ -663,18 +673,18 @@
         <BenchmarkHistory
           resultAdded={this.resultAdded}
           manager={this.manager}
           onSelect={this.loadResult}
           {...this.props}
         />
         <BenchmarkResult<T>
-          result={this.result as IBenchmarkResultBase<T>}
-          scenarios={this.props.scenarios}
+          result={this.result as IBenchmarkResult<T>}
+          scenarios={this.props.profiler.scenarios}
           benchmarks={
-            this.props.benchmarks.filter(
+            this.props.profiler.benchmarks.filter(
               b => b.id === this.result?.benchmark
             ) as unknown as IBenchmark<T>[]
           }
         />
       </div>
     );
   }
@@ -777,15 +787,15 @@
     );
   }
 
   private _handle: number | null = null;
 }
 
 interface IResultProps<T extends IOutcome> {
-  result: IBenchmarkResultBase<T> | null;
+  result: IBenchmarkResult<T> | null;
   benchmarks: IBenchmark<T>[];
   scenarios: IScenario[];
 }
 
 function timingSummary(timing: ITimingOutcome): JSX.Element {
   return (
     <>
@@ -859,41 +869,41 @@
     if (!scenario) {
       return wrap(<div>Unknown scenario: {result.scenario}</div>);
     }
     if (!benchmark) {
       return wrap(<div>Unknown benchmark: {result.benchmark}</div>);
     }
     if (!benchmark.render && this._previousResult !== result.id) {
-      if (result.result.type === 'time') {
+      if (result.outcome.type === 'time') {
         this._table = new TimingTable({
-          measurements: (result.result as ITimingOutcome).results,
-          reference: (result.result as ITimingOutcome).reference,
+          measurements: (result.outcome as ITimingOutcome).results,
+          reference: (result.outcome as ITimingOutcome).reference,
           sortColumn: benchmark.sortColumn,
           stateSource: null,
           lowerIsBetter: false
         });
       } else {
         // should there be a default ProfileTable?
         this._table = null;
       }
     }
-    const tagsSummary = [...Object.entries(result.result.tags)]
+    const tagsSummary = [...Object.entries(result.outcome.tags)]
       .map(([tag, count]) => `${tag}:  ${count}`)
       .join('\n');
-    const totalTags = Statistic.sum([...Object.values(result.result.tags)]);
+    const totalTags = Statistic.sum([...Object.values(result.outcome.tags)]);
     return wrap(
       <>
         <div className="up-BenchmarkResult-summary">
           <div className="up-BenchmarkResult-benchmarkInfo">
             <div>
               {benchmark.name} {scenario.name}
             </div>
-            {result.result.type === 'time'
-              ? timingSummary(result.result as ITimingOutcome)
-              : profilingSummary(result.result as IProfilingOutcome)}
+            {result.outcome.type === 'time'
+              ? timingSummary(result.outcome as ITimingOutcome)
+              : profilingSummary(result.outcome as IProfilingOutcome)}
           </div>
           <div className="up-BenchmarkResult-environmentInfo">
             <div>
               Application: {result.jupyter.client} {result.jupyter.version}{' '}
               {result.jupyter.devMode ? 'dev mode' : null} {result.jupyter.mode}
             </div>
             <div>
@@ -926,15 +936,15 @@
           {benchmark.interpretation ? (
             <details>
               <summary>Interpretation</summary>
               {benchmark.interpretation}
             </details>
           ) : null}
           {benchmark.render ? (
-            <benchmark.render outcome={result.result as any} />
+            <benchmark.render outcome={result.outcome as any} />
           ) : this._table ? (
             <LuminoWidget widget={this._table} />
           ) : null}
         </div>
       </>
     );
   }
@@ -1002,47 +1012,15 @@
       </div>
     );
   }
   start: Date | null = null;
   end: Date | null = null;
 }
 
-interface IBenchmarkData {
-  options: {
-    scenario: JSONObject;
-    benchmark: JSONObject;
-  };
-  benchmark: string;
-  scenario: string;
-  userAgent: string;
-  hardwareConcurrency: number;
-  completed: Date;
-  windowSize: {
-    width: number;
-    height: number;
-  };
-  id: string;
-  jupyter: IJupyterState;
-}
-
-interface IBenchmarkResultBase<T extends IOutcome> extends IBenchmarkData {
-  result: T;
-}
-
-type IBenchmarkResult<T extends IOutcome = ITimingOutcome | IProfilingOutcome> =
-  IBenchmarkResultBase<T>;
-
-function benchmarkId(result: Omit<IBenchmarkData, 'id'>): string {
-  return [
-    result.benchmark,
-    result.scenario,
-    result.completed.toISOString()
-  ].join('_');
-}
-function benchmarkFilename(result: IBenchmarkData): string {
+function benchmarkFilename(result: IBenchmarkResult): string {
   return result.id + '.profile.json';
 }
 
 function OptionsStub(props: { name: string }): JSX.Element {
   return (
     <div className="rjsf">
       <div className="jp-root">
@@ -1058,107 +1036,84 @@
 export class BenchmarkLauncher extends React.Component<
   ILauncherProps,
   IProfilerState
 > {
   constructor(props: ILauncherProps) {
     super(props);
     this._stop = new Signal(this);
+    const { profiler } = props;
     this.state = {
-      benchmarks: props.benchmarks.length !== 0 ? [props.benchmarks[0]] : [],
-      scenarios: props.scenarios.length !== 0 ? [props.scenarios[0]] : [],
+      benchmarks:
+        profiler.benchmarks.length !== 0 ? [profiler.benchmarks[0]] : [],
+      scenarios: profiler.scenarios.length !== 0 ? [profiler.scenarios[0]] : [],
       fieldTemplate: CustomTemplateFactory(this.props.translator),
       arrayFieldTemplate: CustomArrayTemplateFactory(this.props.translator),
       objectFieldTemplate: CustomObjectTemplateFactory(this.props.translator),
       isRunning: false
     };
     this.runSelected = this.runSelected.bind(this);
     this.stopCurrent = this.stopCurrent.bind(this);
   }
   state: IProfilerState;
 
   async runBenchmark<T extends IOutcome = ITimingOutcome | IProfilingOutcome>(
     scenario: IScenario,
     benchmark: IBenchmark<ITimingOutcome> | IBenchmark<IProfilingOutcome>,
     config: IConfigValue
-  ): Promise<IBenchmarkResultBase<T>> {
-    const options = JSONExt.deepCopy({
-      scenario: config.scenarios[scenario.id],
-      benchmark: config.benchmarks[benchmark.id]
-    } as any);
-    if (scenario.setOptions) {
-      scenario.setOptions(options.scenario);
-    }
-    this.props.progress.emit({ percentage: 0 });
-    const result = (await benchmark.run(
-      scenario,
-      options.benchmark,
-      this.props.progress,
-      this._stop
-    )) as T;
-    if (result.interrupted) {
-      this.props.progress.emit({ percentage: NaN, interrupted: true });
-    } else {
-      this.props.progress.emit({ percentage: 100 });
-    }
-    const data: Omit<IBenchmarkResultBase<T>, 'id'> = {
-      result: result,
-      options: options,
-      benchmark: benchmark.id,
-      scenario: scenario.id,
-      userAgent: window.navigator.userAgent,
-      hardwareConcurrency: window.navigator.hardwareConcurrency,
-      completed: new Date(),
-      windowSize: {
-        width: window.innerWidth,
-        height: window.innerHeight
+  ): Promise<IBenchmarkResult<T>> {
+    return this.props.profiler.runBenchmark<T>(
+      {
+        id: scenario.id,
+        options: JSONExt.deepCopy(config.scenarios[scenario.id])
       },
-      jupyter: this.props.getJupyterState()
-    };
-    return {
-      ...data,
-      id: benchmarkId(data)
-    };
+      {
+        id: benchmark.id,
+        options: JSONExt.deepCopy(config.benchmarks[benchmark.id])
+      }
+    );
   }
 
   onBenchmarkChanged(event: React.ChangeEvent<HTMLInputElement>): void {
-    const matched = this.props.benchmarks.find(
+    const { profiler } = this.props;
+    const matched = profiler.benchmarks.find(
       benchmark => benchmark.id === event.target.value
     );
     if (!matched) {
       throw Error(`Benchmark not matched ${event.target.value}`);
     }
     let activeBenchmarks = [...this.state.benchmarks];
     if (event.target.checked) {
       activeBenchmarks.push(matched);
     } else {
       activeBenchmarks = activeBenchmarks.filter(b => b.id !== matched.id);
     }
-    const referenceOrder = this.props.benchmarks.map(s => s.id);
+    const referenceOrder = profiler.benchmarks.map(s => s.id);
     activeBenchmarks.sort(
       (a, b) => referenceOrder.indexOf(a.id) - referenceOrder.indexOf(b.id)
     );
     this.setState({
       benchmarks: activeBenchmarks
     });
   }
 
   onScenarioChanged(event: React.ChangeEvent<HTMLInputElement>): void {
-    const matched = this.props.scenarios.find(
+    const { profiler } = this.props;
+    const matched = profiler.scenarios.find(
       scenario => scenario.id === event.target.value
     );
     if (!matched) {
       throw Error(`Scenario not matched ${event.target.value}`);
     }
     let activeScenarios = [...this.state.scenarios];
     if (event.target.checked) {
       activeScenarios.push(matched);
     } else {
       activeScenarios = activeScenarios.filter(s => s.id !== matched.id);
     }
-    const referenceOrder = this.props.scenarios.map(s => s.id);
+    const referenceOrder = profiler.scenarios.map(s => s.id);
     activeScenarios.sort(
       (a, b) => referenceOrder.indexOf(a.id) - referenceOrder.indexOf(b.id)
     );
     this.setState({
       scenarios: activeScenarios
     });
   }
@@ -1207,19 +1162,23 @@
     this._stop.disconnect(stopListener);
     this.setState({
       isRunning: false
     });
   }
 
   stopCurrent(): void {
+    // interruped scheduling
     this._stop.emit();
+    // interrupt currently running benchmark if any
+    this.props.profiler.abortBenchmark();
   }
 
   render(): JSX.Element {
-    const benchmarks = this.props.benchmarks.map(benchmark => {
+    const { profiler } = this.props;
+    const benchmarks = profiler.benchmarks.map(benchmark => {
       const disabled = benchmark.isAvailable ? !benchmark.isAvailable() : false;
       return (
         <label
           key={benchmark.id}
           className={disabled ? 'up-label-disabled' : ''}
           title={
             disabled ? 'This benchmark is not available on this browser' : ''
@@ -1232,15 +1191,15 @@
             disabled={disabled}
             value={benchmark.id}
           />
           {benchmark.name}
         </label>
       );
     });
-    const scenarios = this.props.scenarios.map(scenario => {
+    const scenarios = profiler.scenarios.map(scenario => {
       return (
         <label key={scenario.id}>
           <input
             type="checkbox"
             defaultChecked={this.state.scenarios.includes(scenario)}
             className="up-BenchmarkLauncher-choice-input"
             value={scenario.id}
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/utils.ts` & `jupyterlab_ui_profiler-0.2.0/src/utils.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import type { DockPanel } from '@lumino/widgets';
-
 export function shuffled<T = any>(array: T[]): T[] {
   return array
     .map(value => ({ value, sort: Math.random() }))
     .sort((a, b) => a.sort - b.sort)
     .map(({ value }) => value);
 }
 
@@ -36,21 +34,14 @@
   if (hours < 1) {
     return formatted;
   }
   formatted = Math.round(hours) + ' hours ' + formatted;
   return formatted;
 }
 
-export interface IJupyterState {
-  version: string;
-  client: string;
-  devMode: boolean;
-  mode: DockPanel.Mode;
-}
-
 /**
  * Simplistic extraction of major browsers data, based on
  * https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent
  */
 export function extractBrowserVersion(userAgent: string): string {
   // order matters!
   const expressions = [
```

### Comparing `jupyterlab_ui_profiler-0.1.8/src/__tests__/statistics.spec.ts` & `jupyterlab_ui_profiler-0.2.0/src/__tests__/statistics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-profile.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-profile.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-rule-group.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-group.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/benchmark-rule-usage.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-usage.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/scenario-completer.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-completer.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/scenario-debugger.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-debugger.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/scenario-scroll.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-scroll.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/schema/scenario-tabs.json` & `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-tabs.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-profile.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-profile.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-rule-group.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-group.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_benchmark-rule-usage.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-usage.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_scenario-completer.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-completer.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_scenario-debugger.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-debugger.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_scenario-scroll.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-scroll.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/src/types/_scenario-tabs.ts` & `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-tabs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/style/base.css` & `jupyterlab_ui_profiler-0.2.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/README.md` & `jupyterlab_ui_profiler-0.2.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/jupyter_server_test_config.py` & `jupyterlab_ui_profiler-0.2.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/yarn.lock` & `jupyterlab_ui_profiler-0.2.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/.gitignore` & `jupyterlab_ui_profiler-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/LICENSE` & `jupyterlab_ui_profiler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/README.md` & `jupyterlab_ui_profiler-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/pyproject.toml` & `jupyterlab_ui_profiler-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.1.8/PKG-INFO` & `jupyterlab_ui_profiler-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-ui-profiler
-Version: 0.1.8
+Version: 0.2.0
 Summary: JupyterLab extension for profiling UI performance
 Project-URL: Homepage, https://github.com/jupyterlab/ui-profiler
 Project-URL: Bug Tracker, https://github.com/jupyterlab/ui-profiler/issues
 Project-URL: Repository, https://github.com/jupyterlab/ui-profiler.git
 Author: Project Jupyter Contributors
 License: BSD 3-Clause License
```

